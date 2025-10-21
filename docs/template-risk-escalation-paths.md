# Risk Escalation Paths

This template defines clear escalation paths for different types of risks to ensure timely decision-making and risk mitigation. Use this as a reference when managing the risk register.

## Escalation Principles

1. **Escalate early** - Surface risks before they become critical issues
2. **Be specific** - Include impact, likelihood, and suggested mitigation
3. **Follow the chain** - Respect escalation levels unless urgent
4. **Document outcomes** - Record decisions and action items in risk register
5. **Close the loop** - Update stakeholders when risks are resolved

## Escalation Levels

### Level 1: Team-Level Risk (Low Impact or Likelihood)

**When to use**: Minor technical challenges, small delays, manageable dependency issues

**Escalation path**:
- **Risk Champion** raises in daily standup or team sync
- **Developers/Team members** collaborate on mitigation
- **Project Manager** (optional) provides guidance if needed

**Response time**: Within 24-48 hours

**Example risks**:
- Test flakiness causing minor CI delays
- Small scope clarification needed from Product Manager
- Non-critical third-party service intermittent issues

---

### Level 2: Project-Level Risk (Medium Impact or High Likelihood)

**When to use**: Risks that could affect project timeline, scope, or quality but are still manageable within the team

**Escalation path**:
- **Risk Champion** alerts **Project Manager** immediately
- **Project Manager** facilitates mitigation planning with team
- **Project Manager** updates stakeholders on status and plan
- Document in risk register with mitigation actions

**Response time**: Within 4-8 hours

**Example risks**:
- Key team member unavailable for 1-2 weeks
- Critical dependency delayed by another team
- Integration complexity higher than estimated
- Security vulnerability requires refactoring
- Test coverage gap identified late in sprint

**Mitigation strategies**:
- Adjust sprint scope or timeline
- Reallocate resources or priorities
- Engage cross-team collaboration
- Create contingency plan

---

### Level 3: Program-Level Risk (High Impact and High Likelihood)

**When to use**: Risks that threaten project delivery, budget, or strategic objectives

**Escalation path**:
- **Risk Champion** or **Project Manager** escalates to **Product Lead** immediately
- **Product Lead** evaluates impact on roadmap and priorities
- **Product Lead** may escalate to **Sponsor/Executive** if business-critical
- Convene risk review meeting within 24 hours with:
  - Project Manager
  - Product Manager
  - Product Lead
  - Risk Champion
  - Relevant stakeholders

**Response time**: Within 2-4 hours (same business day)

**Example risks**:
- Major architectural change required mid-project
- Compliance or legal blocker discovered
- Resource constraints threaten project cancellation
- Critical production incident affecting customer trust
- Major partner or vendor failure

**Mitigation strategies**:
- Rescope or phase deliverables
- Secure additional resources or budget
- Shift timelines or reprioritize roadmap
- Escalate to executive leadership for decision

---

### Level 4: Security or Compliance Incident (Critical)

**When to use**: Security vulnerabilities, data breaches, or compliance violations

**Escalation path**:
- **Immediate notification** to Security on-call (via PagerDuty or incident system)
- **Risk Champion** or **Project Manager** notifies **Product Lead** and **Sponsor** immediately
- Follow security incident runbook (see security policy docs)
- Convene incident response team:
  - Security Lead
  - On-call Engineer
  - Project Manager
  - Legal/Compliance (if needed)

**Response time**: Immediate (within 15-30 minutes)

**Example incidents**:
- Active security vulnerability discovered in production
- Potential data exposure or breach
- Critical dependency with known CVE affecting production
- Compliance violation (GDPR, SOC2, etc.)

**Post-incident actions**:
- Conduct blameless post-mortem within 48 hours
- Update risk register with root cause and preventions
- Update escalation procedures if needed

---

## Risk Escalation Template

Use this format when escalating risks:

```
**Risk ID**: [From risk register, e.g., RISK-123]
**Risk Title**: [Short description]
**Impact**: [High/Medium/Low] - [Describe business/project impact]
**Likelihood**: [High/Medium/Low] - [Describe probability]
**Current Status**: [Active/Monitoring/Escalating]
**Owner**: [Person responsible for mitigation]
**Escalation Reason**: [Why this needs escalation now]
**Suggested Actions**: [Proposed mitigation steps]
**Timeline**: [When decision/action is needed]
```

### Example Escalation

```
**Risk ID**: RISK-042
**Risk Title**: Payment gateway integration delayed by 2 weeks
**Impact**: High - Blocks Q4 launch, affects revenue projections
**Likelihood**: High - Partner confirmed delay yesterday
**Current Status**: Escalating to Product Lead
**Owner**: Alex Chen (Project Manager)
**Escalation Reason**: Delay puts us past launch window, need roadmap adjustment
**Suggested Actions**: 
  1. Phase release: Ship without payment gateway in v1.0
  2. Evaluate alternative payment providers
  3. Adjust roadmap to move gateway to v1.1
**Timeline**: Decision needed by EOD tomorrow to adjust sprint plan
```

---

## Decision Documentation

When a risk escalation results in a decision, document the outcome:

- **Decision Made**: [What was decided]
- **Decision Maker**: [Who made the call]
- **Rationale**: [Why this decision was made]
- **Action Items**: [Who does what by when]
- **Communication Plan**: [Who needs to be informed]

Update the risk register status to reflect the decision and track action items to completion.

---

## Roles in Risk Escalation

- **Risk Champion**: Monitors risks, triggers escalations, maintains risk register
- **Project Manager**: Facilitates Level 2 escalations, coordinates mitigation within project team
- **Product Manager**: Provides input on impact to product goals and user experience
- **Product Lead**: Makes decisions for Level 3 escalations, adjusts roadmap priorities
- **Sponsor/Executive**: Approves major scope, budget, or timeline changes
- **Security Team**: Leads Level 4 security/compliance incidents
- **Developers**: Provide technical input on feasibility and mitigation options
- **QA Lead**: Assesses quality and testing implications of risk mitigations

---

*Last updated: October 2025*
