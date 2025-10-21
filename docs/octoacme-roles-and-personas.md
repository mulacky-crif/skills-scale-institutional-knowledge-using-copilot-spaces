# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Release Coordinator

### Role Summary
Release Coordinators orchestrate the end-to-end release process, ensuring that features move smoothly from development through staging to production. They coordinate timing, communications, and verification activities across teams.

### Responsibilities
- Schedule and manage release windows and deployment activities
- Coordinate pre-release readiness checks (CI passes, security scans, smoke tests)
- Facilitate release go/no-go decisions with Project Managers and stakeholders
- Execute deployment procedures and post-deployment verification
- Manage release notes and communicate releases to stakeholders and support teams
- Maintain rollback procedures and coordinate incident response during releases

### Goals
- Minimize deployment risk and downtime
- Ensure predictable, repeatable release processes
- Maintain clear communication about release status and impacts
- Enable rapid rollback when issues arise

### Typical Communication
- Pre-release status updates and readiness reviews
- Release announcements to stakeholders and support teams
- Post-deployment verification reports
- Coordination with Developers, QA Lead, and Project Managers

### Interactions with Other Roles
- **With Developers**: Reviews deployment readiness, coordinates merge timing, validates smoke test results
- **With QA Lead**: Confirms acceptance criteria are met, coordinates final testing in staging
- **With Project Managers**: Aligns on release schedules, reports on deployment risks and status
- **With Risk Champion**: Escalates deployment issues and coordinates mitigation plans

---

## Risk Champion

### Role Summary
Risk Champions proactively identify, assess, and monitor project risks throughout the lifecycle. They facilitate risk discussions, maintain the risk register, and ensure timely escalation when risks materialize or require senior attention.

### Responsibilities
- Facilitate risk identification sessions during planning and execution
- Maintain and update the risk register with impact, likelihood, and mitigation plans
- Monitor risk status and trigger escalations following defined paths
- Conduct risk reviews in weekly syncs and milestone meetings
- Track risk mitigation actions and ensure owners follow through
- Escalate high-impact risks to Project Managers and stakeholders

### Goals
- Surface risks early before they become critical issues
- Ensure every significant risk has a clear owner and mitigation plan
- Maintain transparency about project health and risk exposure
- Enable data-driven risk decisions

### Typical Communication
- Weekly risk status updates in team syncs
- Escalation notifications to Project Managers and Product Leads
- Risk assessment summaries for stakeholders
- Post-incident risk analysis and lessons learned

### Interactions with Other Roles
- **With Project Managers**: Reports on risk status, escalates critical risks, coordinates mitigation strategies
- **With Developers**: Gathers technical risk inputs, validates feasibility of mitigation approaches
- **With Product Managers**: Discusses impact of risks on roadmap and prioritization decisions
- **With Release Coordinator**: Identifies deployment risks, coordinates go/no-go decisions

---

## QA Lead

### Role Summary
QA Leads define and oversee the quality assurance strategy for projects, ensuring that features meet acceptance criteria and quality standards before release. They coordinate testing activities, define test plans, and validate that Definition of Done is satisfied.

### Responsibilities
- Define test strategy and acceptance criteria with Product Managers
- Create and maintain test plans for features and releases
- Coordinate testing activities across unit, integration, and end-to-end levels
- Review test coverage and results before release approval
- Facilitate manual QA sessions for complex or UI-heavy features
- Track quality metrics and identify testing gaps or improvements

### Goals
- Ensure features meet quality standards and acceptance criteria
- Prevent defects from reaching production
- Maintain comprehensive test coverage for critical flows
- Enable fast, confident releases through automation

### Typical Communication
- Test plan reviews with Product Managers and Developers
- Daily testing status updates during active sprints
- Pre-release quality assessments for Release Coordinators
- Bug triage and prioritization discussions

### Interactions with Other Roles
- **With Developers**: Reviews test coverage, pairs on complex test scenarios, clarifies acceptance criteria
- **With Product Managers**: Validates acceptance criteria, confirms feature behavior matches requirements
- **With Release Coordinator**: Provides quality sign-off for releases, coordinates final testing in staging
- **With Project Managers**: Reports on quality metrics, flags testing-related risks or delays

---

## Onboarding Facilitator

### Role Summary
Onboarding Facilitators ensure that new team members can quickly understand their role, access necessary resources, and contribute effectively to projects. They manage the onboarding process, maintain knowledge transfer materials, and reduce single-person dependency risks.

### Responsibilities
- Create and maintain onboarding checklists and documentation
- Coordinate new team member orientation sessions
- Pair new hires with mentors or buddies for their first weeks
- Ensure access to repositories, tools, and communication channels
- Gather feedback on onboarding effectiveness and iterate improvements
- Identify documentation gaps that slow down onboarding

### Goals
- Accelerate time-to-productivity for new team members
- Reduce single-person knowledge dependencies
- Create a welcoming, supportive onboarding experience
- Build and maintain comprehensive knowledge transfer materials

### Typical Communication
- Onboarding kickoff meetings with new team members
- Check-ins during first 30-60-90 days
- Feedback sessions to improve onboarding materials
- Coordination with Project Managers on team ramp-up plans

### Interactions with Other Roles
- **With Project Managers**: Plans onboarding timelines, identifies knowledge gaps in team capacity
- **With Developers**: Coordinates code reviews and pairing sessions for new developers
- **With Product Managers**: Facilitates product knowledge transfer for new team members
- **With all roles**: Gathers documentation feedback to improve knowledge base

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

## Persona Interaction Matrix

The following matrix summarizes key interactions between personas:

| From / To | Developers | Product Managers | Project Managers | Release Coordinator | Risk Champion | QA Lead | Onboarding Facilitator |
|-----------|-----------|------------------|------------------|---------------------|---------------|---------|----------------------|
| **Developers** | Peer reviews | Clarify requirements | Report progress | Deployment readiness | Technical risks | Test coverage | Mentor new devs |
| **Product Managers** | Define features | Strategic alignment | Backlog priority | Release planning | Impact assessment | Acceptance criteria | Product knowledge |
| **Project Managers** | Remove blockers | Roadmap sync | Cross-team coord | Schedule releases | Risk escalation | Quality status | Onboarding plans |
| **Release Coordinator** | Merge timing | Release approval | Deployment status | - | Deployment risks | Quality sign-off | Deploy process docs |
| **Risk Champion** | Technical input | Impact analysis | Risk reports | Deployment risk | - | Quality risks | Knowledge gaps |
| **QA Lead** | Test support | Validate behavior | Quality metrics | Pre-release testing | Testing risks | - | Testing practices |
| **Onboarding Facilitator** | Pairing sessions | Product training | Ramp-up plans | Deploy training | Risk awareness | QA training | - |

