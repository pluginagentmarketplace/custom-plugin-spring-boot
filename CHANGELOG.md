# Changelog

All notable changes to this project are documented in this file.

Format: [Keep a Changelog](https://keepachangelog.com/)
Versioning: [Semantic Versioning](https://semver.org/)

## [Unreleased]

### Added
- Upcoming features

## [2.0.0] - 2024-12-30

### Changed - Production-Grade Upgrade

#### Agents (7 agents completely rewritten)
- **01-spring-boot-fundamentals**: Auto-configuration, ConfigurationProperties, profiles, actuator patterns
- **02-spring-mvc**: REST controllers, validation, RFC 7807 ProblemDetail, CORS configuration
- **03-spring-data**: JPA entities, repositories, Specifications, Entity Graphs, N+1 prevention
- **04-spring-security**: JWT SecurityFilterChain (Spring Boot 3.x), OAuth2, method security
- **05-spring-cloud**: Eureka, Spring Cloud Gateway, Resilience4j, distributed tracing
- **06-spring-testing**: MockMvc, TestContainers, WireMock, test slices, integration tests
- **07-spring-reactive**: WebFlux, Mono/Flux, R2DBC, SSE, WebSocket patterns

#### Skills (7 skills completely rewritten)
- **spring-boot-basics**: Parameters table, configuration examples, troubleshooting guide
- **spring-rest-api**: DTO patterns, GlobalExceptionHandler, validation examples
- **spring-data-jpa**: Entity relationships, Specification pattern, pagination
- **spring-security**: JWT implementation, SecurityConfig with lambda DSL
- **spring-microservices**: Gateway routes, circuit breaker, tracing configuration
- **spring-testing**: Test pyramid, TestContainers integration, WireMock examples
- **spring-reactive**: Reactive operators, backpressure, WebTestClient patterns

#### All Files Now Include
- Role & Responsibility boundaries
- Input/Output schemas with validation
- Error handling tables with diagnosis/fix
- Fallback strategies
- Token optimization guidelines
- Troubleshooting sections (failure modes, debug checklists)
- Code examples with Spring Boot 3.x patterns
- Unit test templates
- Version history

### Added
- Comprehensive code examples for each topic
- Debug checklists for common issues
- Failure mode tables with solutions
- Operator quick references for reactive programming
- Test configuration templates

### Fixed
- Updated all patterns to Spring Boot 3.x (SecurityFilterChain lambda DSL)
- Corrected deprecated API usage (WebSecurityConfigurerAdapter → SecurityFilterChain)
- Fixed RFC 7807 ProblemDetail integration patterns

### Security
- JWT implementation with proper secret key handling
- Method-level security with @PreAuthorize patterns
- CORS configuration best practices

## [1.0.0] - 2025-12-29

### Added
- Initial release
- SASMP v1.3.0 compliance
- Golden Format skills
- Protective LICENSE

---

**Maintained by:** Dr. Umit Kacar & Muhsin Elcicek
