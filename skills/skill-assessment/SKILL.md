---
name: skill-assessment
description: Conduct multi-dimensional skill assessments using conversational AI, code analysis, adaptive quizzes, and project evaluation. Use for proficiency evaluation, gap identification, and progress tracking.
sasmp_version: "1.3.0"
bonded_agent: 01-roadmap-navigator
bond_type: PRIMARY_BOND
---

# Skill Assessment Skill

Master self-assessment and validation using multiple methods to accurately measure technical proficiency and identify growth opportunities.

## Quick Start

```
/assess status              # Check your skill levels
/assess test <skill>        # Take adaptive skill test
/assess gaps                # Identify skill gaps
/assess progress            # Track improvement over time
```

## Core Concepts

### Proficiency Scale (1-5)

```
LEVEL 1 - UNAWARE (0-20%):
├─ Never encountered technology
├─ Cannot recognize concepts
├─ No hands-on experience
└─ Action: Start introductory course

LEVEL 2 - AWARE (21-40%):
├─ Know basic concepts
├─ Familiar with syntax
├─ Can follow tutorials
└─ Action: Build simple projects

LEVEL 3 - NOVICE (41-60%):
├─ Use with documentation
├─ Build simple projects
├─ Understand core patterns
└─ Action: Practice with projects

LEVEL 4 - COMPETENT (61-85%):
├─ Use independently
├─ Build production code
├─ Design reasonable solutions
└─ Action: Learn advanced topics

LEVEL 5 - EXPERT (86-100%):
├─ Deep understanding
├─ Mentor others
├─ Contribute open-source
└─ Action: Share knowledge
```

### Assessment Methods

**Method 1: Conversational Assessment**
```
Questions:
- Describe a recent project using React
- How would you handle state management?
- Explain the virtual DOM
- When would you use hooks vs classes?

Evaluates:
- Practical experience
- Conceptual understanding
- Real-world application
- Knowledge depth
```

**Method 2: Code Analysis**
```
Analyzes:
- Architecture & design patterns
- Code organization
- Testing practices
- Performance awareness
- Best practices adherence
- Technology stack knowledge
```

**Method 3: Adaptive Quiz**
```
Process:
1. Start at medium difficulty
2. Correct answer → Increase difficulty
3. Incorrect answer → Decrease difficulty
4. Convergent difficulty = Proficiency level
```

**Method 4: Project Review**
```
Evaluates:
- Functional correctness
- Code quality
- Testing coverage (>70% ideal)
- Performance optimization
- Security practices
- Documentation
```

## Assessment Framework

### Step 1: Self-Reflection

Ask yourself:
```
□ How long have I used this skill?
□ Can I explain it to others?
□ Have I built projects with it?
□ Have I solved problems independently?
□ What areas feel weak?
```

### Step 2: Evidence Gathering

Collect proof of proficiency:
```
□ Quiz scores (% correct)
□ Project portfolio (working examples)
□ Code samples (GitHub repositories)
□ Mentoring experience (helping others)
□ Open-source contributions
□ Technical articles written
□ Teaching experience
```

### Step 3: Assessment

Choose methods:
```
Select 2-3 of:
□ Conversational discussion
□ Code analysis of your projects
□ Adaptive skill test (10-15 questions)
□ Project code review
□ Teaching/mentoring assessment
```

### Step 4: Calibration

Compare results:
```
Self-reported confidence vs actual performance:
├─ Accurate: Self-assessment matches measured ability
├─ Overconfident: Self-reported > measured ability
└─ Underconfident: Self-reported < measured ability

Adjust future learning based on calibration.
```

## Common Proficiency Profiles

### Profile 1: The Confident Expert
```
Self-reported: 90/100
Measured: 85/100
Calibration: Accurate ✅

Assessment shows:
- Strong conceptual understanding
- Excellent practical experience
- Minor gaps in edge cases
- Ready for expert roles
```

### Profile 2: The Uncertain Competent
```
Self-reported: 50/100
Measured: 78/100
Calibration: Underconfident ⚠️

Assessment shows:
- Actually quite proficient
- Imposter syndrome likely
- Should take on more challenging work
- Ready for senior roles despite doubts
```

### Profile 3: The Overconfident Beginner
```
Self-reported: 75/100
Measured: 40/100
Calibration: Overconfident ⚠️

Assessment shows:
- Strong fundamentals
- Doesn't know what they don't know
- Needs deeper learning
- Ready for intermediate practice
```

## Skill Gap Analysis

### Process

```
STEP 1: Identify Target
├─ Target job role
├─ Desired expertise level
├─ Timeline constraints
└─ Market demands

STEP 2: Assess Current State
├─ Current proficiency per skill
├─ Confidence level per skill
├─ Experience evidence
└─ Time investment made

STEP 3: Calculate Gaps
├─ Required level - Current level = Gap
├─ Gap size (small/medium/large/critical)
├─ Estimated learning time
└─ Dependency analysis

STEP 4: Prioritize
├─ Critical gaps (blocking advancement)
├─ Important gaps (accelerate progress)
├─ Beneficial gaps (optimize career)
└─ Optional gaps (nice-to-have)

STEP 5: Create Action Plan
├─ Resource recommendations
├─ Timeline to close gap
├─ Project recommendations
└─ Success metrics
```

### Example Gap Analysis

```
TARGET: Senior React Developer

REQUIRED SKILLS:
React        Your: Level 4 (Competent) ✅ READY
TypeScript   Your: Level 2 (Aware) ❌ GAP
Testing      Your: Level 2 (Aware) ❌ GAP
Perf Opt     Your: Level 2 (Aware) ❌ GAP
System Design Your: Level 2 (Aware) ❌ GAP

GAPS IDENTIFIED:
1. TypeScript (Critical)
   Current: Level 2
   Target: Level 4
   Gap: 2 levels
   Est. Time: 6-8 weeks
   Resources: Official handbook, advanced course

2. Testing (Important)
   Current: Level 2
   Target: Level 4
   Gap: 2 levels
   Est. Time: 4-6 weeks
   Resources: Jest advanced, testing library

3. Performance (Important)
   Current: Level 2
   Target: Level 4
   Gap: 2 levels
   Est. Time: 4-6 weeks
   Resources: Web Vitals, optimization course

4. System Design (Important)
   Current: Level 2
   Target: Level 4
   Gap: 2 levels
   Est. Time: 6-8 weeks
   Resources: System design interview prep

TOTAL TIME TO READY: 20-28 weeks (5-7 months)
```

## Progress Tracking

### Retention Tracking

```
Timeline    Retention Rate    Action
─────────────────────────────────────
Week 1      90%              ✅ Fresh learning
Week 2      75%              ⚠️ Review needed
Week 3      65%              ⚠️ Practice needed
Week 4      60%              ❌ Spaced repetition
Week 8      50%              ❌ Active review
Week 12     60%              ✅ Consolidating
Week 16     75%              ✅ Well retained
Month 6+    78%              ✅ Long-term memory
```

### Confidence Calibration

```
After each assessment, compare:
Self-Reported: What you think (0-100)
Measured: Quiz/project score (0-100)
Delta: Difference

Patterns:
Consistent gap → Adjust future self-assessments
Large overconfidence → Careful assessment before advancement
Underconfidence → Take on bigger challenges

Track changes over time to improve calibration.
```

## Assessment Tools

### Quick Self-Assessment Questionnaire

```
Rate yourself 1-5 (1=Never, 5=Expert):

For JavaScript:
□ I understand closures and scope
□ I can write async code correctly
□ I know event loop mechanics
□ I can optimize performance
□ I could teach others
□ I contribute to JS projects

Sum score: ____/30 (÷6 = avg level)
```

### Project-Based Assessment

```
Submit a project for evaluation:
□ Repo link on GitHub
□ Live demo URL
□ Brief description
□ Technology choices

Evaluator reviews:
✓ Code quality (architecture, patterns)
✓ Functionality (requirements met)
✓ Testing (coverage, types)
✓ Performance (metrics)
✓ Documentation (clarity)

Results in proficiency level + recommendations
```

### Adaptive Skill Test

```
10-15 questions with adaptive difficulty:

Question 1 (Medium): Basic concept
→ Correct: Next = Hard
→ Incorrect: Next = Medium

Question 10 (varies): Convergent on level
→ Final score + proficiency level + weak areas
```

## Gap Closing Strategy

### Immediate Gaps (1-2 weeks)
```
Learning approach:
- Intensive focused course
- Daily practice (1-2 hours)
- Build small projects
- Daily assessment

Example:
├─ Day 1-2: Course videos
├─ Day 3-5: Hands-on labs
├─ Day 6-10: Build project
└─ Day 11-14: Deep understanding
```

### Medium Gaps (4-8 weeks)
```
Learning approach:
- Comprehensive course
- 4-5 projects
- Code reviews
- Weekly assessment

Example:
├─ Week 1: Foundations
├─ Week 2-3: Core concepts
├─ Week 4-5: Projects
├─ Week 6-7: Advanced topics
└─ Week 8: Assessment
```

### Large Gaps (12+ weeks)
```
Learning approach:
- Full learning path
- 10+ projects
- Reading, videos, courses
- Mentorship
- Monthly assessments

Example:
├─ Months 1-2: Fundamentals
├─ Months 3-4: Core concepts + projects
├─ Months 5-8: Advanced topics + portfolio
├─ Months 9-12: Specialization + contribution
└─ Monthly: Progress assessment
```

## Next Steps

1. Choose a skill to assess
2. Answer self-reflection questions
3. Take adaptive skill test
4. Get code analysis
5. Compare results
6. Identify gaps
7. Create learning plan
8. Track progress over time
