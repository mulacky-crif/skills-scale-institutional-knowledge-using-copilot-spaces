# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

The **Risk Champion** is responsible for maintaining the risk register and ensuring it stays current. For detailed escalation procedures, see [Risk Escalation Paths Template](template-risk-escalation-paths.md).

## Risk Lifecycle
- Identify: during planning and ongoing execution (facilitated by Risk Champion)
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status (tracked by Risk Champion)
- Escalate: follow defined escalation paths when risks require senior attention

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
Clear escalation paths ensure timely decision-making and risk mitigation:

- **Level 1 (Team-level)**: Risk Champion raises in standup → Team collaborates on mitigation
- **Level 2 (Project-level)**: Risk Champion escalates to PM → PM facilitates mitigation with team
- **Level 3 (Program-level)**: PM escalates to Product Lead → Convene risk review meeting
- **Level 4 (Security/Compliance)**: Immediate notification to Security on-call → Follow security incident runbook

For detailed escalation procedures, decision templates, and examples, see [Risk Escalation Paths Template](template-risk-escalation-paths.md).
