---
name: project
description: Project
allowed-tools: Read
---

# Project

Get project recommendations, implementation guidance, code reviews, and portfolio-building strategies for 70+ hands-on projects aligned with your learning path.

## Usage

```
/project suggest <skill>        # Find projects for your skill level
/project <project-name>         # Get guidance for specific project
/project guide <project>        # Step-by-step implementation help
/project review <repo-url>      # Get code review feedback
/project portfolio              # Build portfolio strategy
```

## Examples

```
/project suggest react
# Find React projects at your skill level

/project weather-app
# Get detailed guidance for Weather Web App project

/project guide personal-portfolio
# Step-by-step instructions for building portfolio site

/project review https://github.com/user/my-project
# Get AI code review and improvement suggestions

/project portfolio
# Develop 5-project portfolio strategy for job interviews
```

## 70+ Projects Available

### Frontend Projects (24)
- **Beginner**: CV, Portfolio, Components (buttons, tabs, dropdowns)
- **Intermediate**: Task Tracker, Weather App, GitHub Client, Quiz App
- **Advanced**: Instagram Stories Clone

### Backend Projects (23)
- **Beginner**: CLI tools, APIs (weather, todo, expense tracker)
- **Intermediate**: URL Shortener, Chat Server, Image Processor
- **Advanced**: E-Commerce Platform, Microservices

### DevOps Projects (23)
- **Beginner**: Deployment, Monitoring basics
- **Intermediate**: Docker Compose, Terraform, Ansible
- **Advanced**: Kubernetes, Blue-Green Deployment

## Project Matching

The plugin suggests projects based on:

**Your Skill Level**
- Beginner: Foundational projects
- Intermediate: Feature-rich applications
- Advanced: Complex architectures

**Your Learning Goals**
- Frontend: Visual applications
- Backend: APIs and systems
- Full Stack: Complete applications
- DevOps: Infrastructure automation

**Time Investment**
- Quick: 4-8 hours (learning projects)
- Medium: 12-20 hours (portfolio quality)
- Substantial: 24-40+ hours (showpiece projects)

**Technology Stack**
- JavaScript/React focused
- Python/Django focused
- Multi-stack comprehensive

## Detailed Project Guidance

For each project, you get:

```
PROJECT OVERVIEW:
├─ Description and objectives
├─ Learning outcomes
├─ Technology stack required
├─ Difficulty level
├─ Time estimate
├─ Portfolio value
└─ Prerequisite skills

REQUIREMENTS:
├─ Functional requirements (features)
├─ Non-functional (performance, scalability)
├─ UI/UX considerations
├─ Testing expectations
└─ Documentation needs

IMPLEMENTATION PHASES:
├─ Phase 1: Setup & Basics
├─ Phase 2: Core Features
├─ Phase 3: Advanced Features
├─ Phase 4: Polish & Optimization
└─ Phase 5: Deployment & Sharing

RESOURCES FOR PROJECT:
├─ Tutorials & guides
├─ Library documentation
├─ Code examples
├─ Best practices
└─ Common pitfalls

TESTING & QA:
├─ Test scenarios
├─ Edge cases
├─ Performance benchmarks
└─ Accessibility checks

DEPLOYMENT OPTIONS:
├─ Frontend: Vercel, Netlify, GitHub Pages
├─ Backend: Render, Railway, Heroku
├─ Full Stack: Fly.io, AWS, DigitalOcean
└─ DevOps: Docker Hub, Kubernetes

PORTFOLIO PRESENTATION:
├─ Demo video tips
├─ Blog post outline
├─ GitHub README template
└─ Portfolio description
```

## Code Review Process

```
STEP 1: Submit your project
/project review <github-repo-url>

STEP 2: AI analyzes your code
├─ Architecture & design
├─ Code quality
├─ Testing coverage
├─ Performance optimization
├─ Best practices adherence
├─ Security considerations
└─ Documentation quality

STEP 3: Receive detailed feedback
├─ Strengths (what you did well)
├─ Areas for improvement (specific)
├─ Refactoring suggestions
├─ Performance optimization tips
├─ Best practices recommendations
├─ Interview talking points
└─ Overall quality rating

STEP 4: Implement improvements
├─ Address high-priority issues
├─ Apply suggested improvements
├─ Retest and validate
└─ Commit improvements

STEP 5: Re-review if needed
/project review <updated-repo-url>
```

## Portfolio Building Strategy

### The "5-Project Portfolio"

Build these 5 projects strategically:

```
PROJECT 1: Personal Website (Frontend Showcase)
├─ Time: 12-16 hours
├─ Impact: First impression, portfolio hub
├─ Skills: HTML, CSS, responsive design
├─ Visitors: Hundreds monthly
└─ Purpose: Demonstrates design and polish

PROJECT 2: API Integration (Practical Skills)
├─ Time: 16-20 hours
├─ Impact: Shows API knowledge
├─ Skills: Async code, error handling, data transformation
├─ Complexity: Medium-High
└─ Purpose: Demonstrates practical capability

PROJECT 3: Full App (Complete System)
├─ Time: 24-32 hours
├─ Impact: Professional-level work
├─ Skills: Architecture, state management, testing
├─ Complexity: High
└─ Purpose: Shows ability to complete complex projects

PROJECT 4: Backend API (Server-Side Skills)
├─ Time: 20-28 hours
├─ Impact: Full-stack understanding
├─ Skills: Database, security, API design
├─ Complexity: High
└─ Purpose: Backend expertise

PROJECT 5: Specialty Project (Differentiation)
├─ Time: 32-40 hours
├─ Impact: Stands out from other candidates
├─ Skills: Cutting-edge tech or unique domain
├─ Complexity: Very High
└─ Purpose: Shows innovation and depth

TOTAL TIME: 120-160 hours (~4-6 months)
JOB IMPACT: Transformative - many offers
```

### Portfolio Presentation

For each project, create:

```
✅ LIVE DEMO
   - Always working version
   - Polished UX
   - Responsive design
   - 2-3 min demo video

✅ GITHUB REPOSITORY
   - Clean commits
   - Professional README
   - Well-commented code
   - MIT license

✅ BLOG POST
   - Problem & solution
   - Technical decisions
   - Challenges faced
   - Lessons learned

✅ PORTFOLIO WEBSITE
   - Featured prominently
   - Live links
   - Screenshots
   - Brief descriptions

✅ INTERVIEW TALKING POINTS
   - Why you built it
   - Technical challenges
   - Design decisions
   - What you'd improve
```

## Project Selection Tips

1. **Skill Progression**: Build simple → medium → complex
2. **Balanced Stack**: Don't focus only on frontend or backend
3. **Real-World Value**: Build things people want
4. **Portfolio Quality**: 5 amazing > 15 mediocre
5. **Timely Execution**: Finish fast, iterate based on feedback
6. **Documentation**: Great code + great docs = hiring interest

## Integration with Other Commands

```
/roadmap        # See projects aligned with current phase
/assess         # Validate skills after completing project
/resources      # Find tutorials for project technologies
/progress       # Track project completion milestones
/career         # Discuss how projects help job readiness
```

## Sample Project Sequences

### Frontend Track
1. Personal Portfolio (showcase)
2. Weather App (API integration)
3. Todo App + React (framework)
4. GitHub Client (complex state)
5. E-Commerce Demo (advanced)

### Backend Track
1. Task Tracker CLI (basics)
2. Weather API (HTTP server)
3. Blogging Platform (full CRUD)
4. E-Commerce API (complexity)
5. Real-time System (advanced)

### Full Stack Track
1. Personal Portfolio (frontend)
2. Task Tracker (full stack)
3. Note App (complete system)
4. E-Commerce Demo (advanced)
5. Specialty Project (unique)

## Next Steps

1. Run `/project suggest <skill>`
2. Pick a project that excites you
3. Run `/project guide <project-name>`
4. Follow step-by-step instructions
5. Build and deploy your project
6. Run `/project review` for feedback
7. Improve based on recommendations
8. Share your project widely
9. Move to next project
10. Build your 5-project portfolio
