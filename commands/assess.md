# Assess

Evaluate your current skill levels across technical competencies using multiple assessment methods: conversational AI, code analysis, adaptive quizzes, and project reviews.

## Usage

```
/assess status              # Check overall skill levels
/assess test <skill>        # Take adaptive skill test
/assess gaps                # Identify skill gaps
/assess <role>              # Compare to job requirements
/assess progress            # Track improvements over time
```

## Examples

```
/assess status
# Shows dashboard with all your skills and proficiency levels

/assess test react
# Takes an adaptive 10-15 question quiz to evaluate React proficiency

/assess gaps
# Shows which skills you need to improve for your goal role

/assess senior-frontend-developer
# Compares your skills to "Senior Frontend Developer" requirements

/assess progress
# Shows your progress over time and retention metrics
```

## Assessment Methods

### Conversational Assessment
You describe your experience, Claude evaluates:
- Practical hands-on experience
- Conceptual understanding
- Real-world application ability
- Knowledge depth and breadth

### Code Analysis
Share your GitHub profile, Claude analyzes:
- Code quality and architecture
- Design patterns used
- Testing practices
- Performance optimization
- Best practices adherence

### Adaptive Skill Tests
Take difficulty-adjusted quizzes:
- 10-15 questions per test
- Difficulty adjusts based on answers
- Covers theory and practical concepts
- Results in proficiency level

### Project Code Review
Submit your project work:
- Functional correctness
- Code quality assessment
- Testing coverage evaluation
- Performance analysis
- Security review

## Proficiency Scale

```
Level 1: UNAWARE (0-20%)
- Never encountered technology
- No hands-on experience
- Need introductory course

Level 2: AWARE (21-40%)
- Know basic concepts
- Familiar with syntax
- Can follow tutorials with guidance

Level 3: NOVICE (41-60%)
- Use with documentation
- Build simple projects
- Understand core patterns

Level 4: COMPETENT (61-85%)
- Use independently
- Build production code
- Design reasonable solutions

Level 5: EXPERT (86-100%)
- Deep understanding
- Mentor others
- Contribute to open-source
```

## Skill Gap Analysis

Claude will:
1. Identify skills for your target role
2. Assess your current proficiency
3. Calculate gaps (high priority to low priority)
4. Estimate learning time per gap
5. Recommend learning resources
6. Create action plan

## Assessment Calibration

After testing, Claude compares:
- Your self-reported confidence
- Actual test/project performance
- Identifies overconfidence or underconfidence
- Helps calibrate future self-assessments

## Using Results

**Identified Gaps?**
- Run `/roadmap` to find learning paths
- Run `/resources` to find materials
- Run `/project` for project practice
- Run `/progress` to track improvement

**Ready for Advancement?**
- Run `/career fit <job_url>` to check job fit
- Run `/career market <skill>` to check demand
- Start new skill learning

**Strong Performance?**
- Celebrate your progress!
- Take on bigger challenges
- Help others learn
- Contribute to open-source

## Tips for Accurate Assessment

1. **Be Honest**: Self-assessment is most accurate
2. **Be Specific**: Describe concrete examples
3. **Show Evidence**: Share projects and code
4. **Test Regularly**: Assess every 4-8 weeks
5. **Track Progress**: Monitor improvements over time

## Next Steps

1. Run `/assess status` for initial evaluation
2. Choose a skill that's unclear
3. Take `/assess test <skill>`
4. Review gaps with `/assess gaps`
5. Create learning plan to close gaps
6. Re-assess in 4-8 weeks
