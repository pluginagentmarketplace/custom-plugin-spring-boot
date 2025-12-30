---
name: spring-data-jpa
description: Master Spring Data JPA - repositories, queries, relationships, transactions, and performance
sasmp_version: "1.3.0"
bonded_agent: 03-spring-data
bond_type: PRIMARY_BOND
version: "2.0.0"
updated: "2024-12-30"
---

# Spring Data JPA Skill

Comprehensive guide to data access with Spring Data JPA including repository patterns, custom queries, and performance optimization.

## Overview

This skill covers everything needed for production-ready database access with Spring Data JPA.

## Parameters

| Name | Type | Required | Default | Validation |
|------|------|----------|---------|------------|
| `database` | enum | ✗ | postgresql | postgresql \| mysql \| h2 |
| `migration_tool` | enum | ✗ | flyway | flyway \| liquibase \| none |
| `fetch_strategy` | enum | ✗ | lazy | lazy \| eager |

## Topics Covered

### Core (Must Know)
- **Entities**: `@Entity`, `@Table`, `@Id`, relationships
- **Repositories**: `JpaRepository`, derived queries
- **Transactions**: `@Transactional`, propagation

### Intermediate
- **Custom Queries**: `@Query` with JPQL and native SQL
- **Projections**: Interface-based, class-based
- **Auditing**: `@CreatedDate`, `@LastModifiedDate`

### Advanced
- **Specifications**: Dynamic query building
- **Entity Graphs**: Fetch optimization
- **N+1 Prevention**: JOIN FETCH strategies

## Code Examples

### Entity with Relationships
```java
@Entity
@Table(name = "orders")
@EntityListeners(AuditingEntityListener.class)
public class Order {

    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    @Column(unique = true, nullable = false)
    private String orderNumber;

    @ManyToOne(fetch = FetchType.LAZY)
    @JoinColumn(name = "customer_id", nullable = false)
    private Customer customer;

    @OneToMany(mappedBy = "order", cascade = CascadeType.ALL, orphanRemoval = true)
    private List<OrderItem> items = new ArrayList<>();

    @CreatedDate
    private LocalDateTime createdAt;

    @Version
    private Long version;

    public void addItem(OrderItem item) {
        items.add(item);
        item.setOrder(this);
    }
}
```

### Repository with Custom Queries
```java
public interface OrderRepository extends JpaRepository<Order, Long>,
                                         JpaSpecificationExecutor<Order> {

    Optional<Order> findByOrderNumber(String orderNumber);

    @Query("SELECT o FROM Order o JOIN FETCH o.items WHERE o.customer.id = :customerId")
    List<Order> findByCustomerWithItems(@Param("customerId") Long customerId);

    @EntityGraph(attributePaths = {"items", "customer"})
    Optional<Order> findWithDetailsById(Long id);

    @Modifying
    @Query("UPDATE Order o SET o.status = :status WHERE o.id = :id")
    int updateStatus(@Param("id") Long id, @Param("status") OrderStatus status);
}
```

### Specification Pattern
```java
public class OrderSpecifications {

    public static Specification<Order> hasStatus(OrderStatus status) {
        return (root, query, cb) ->
            status == null ? null : cb.equal(root.get("status"), status);
    }

    public static Specification<Order> createdAfter(LocalDateTime date) {
        return (root, query, cb) ->
            date == null ? null : cb.greaterThan(root.get("createdAt"), date);
    }
}

// Usage
Specification<Order> spec = Specification
    .where(OrderSpecifications.hasStatus(status))
    .and(OrderSpecifications.createdAfter(since));
Page<Order> orders = orderRepository.findAll(spec, pageable);
```

## Troubleshooting

### Failure Modes

| Issue | Diagnosis | Fix |
|-------|-----------|-----|
| N+1 queries | Multiple SELECTs | Use `@EntityGraph` or `JOIN FETCH` |
| LazyInitializationException | Access outside session | Use `@Transactional` or DTO |
| Data not saved | Missing `@Transactional` | Add to service method |

### Debug Checklist

```
□ Enable SQL logging: spring.jpa.show-sql=true
□ Check for N+1 with hibernate.generate_statistics
□ Verify @Transactional on write operations
□ Review fetch types (LAZY vs EAGER)
```

## Unit Test Template

```java
@DataJpaTest
@Testcontainers
class OrderRepositoryTest {

    @Container
    @ServiceConnection
    static PostgreSQLContainer<?> postgres = new PostgreSQLContainer<>("postgres:15");

    @Autowired
    private OrderRepository orderRepository;

    @Test
    void shouldFindByOrderNumber() {
        Order order = new Order();
        order.setOrderNumber("ORD-001");
        orderRepository.save(order);

        Optional<Order> found = orderRepository.findByOrderNumber("ORD-001");
        assertThat(found).isPresent();
    }
}
```

## Usage

```
Skill("spring-data-jpa")
```

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 2.0.0 | 2024-12-30 | Specifications, auditing, performance patterns |
| 1.0.0 | 2024-01-01 | Initial release |
