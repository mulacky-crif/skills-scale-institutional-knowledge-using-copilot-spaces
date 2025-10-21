# Release Coordination Checklist

Use this checklist to ensure all pre-release, deployment, and post-deployment activities are completed. Assign a Release Coordinator for each release to own this process.

## Pre-Release Readiness (T-minus 3 days)

- [ ] **All PRs merged** - Confirm all planned features are merged to release branch
- [ ] **CI/CD passing** - All automated tests, linting, and security scans pass
- [ ] **Acceptance criteria validated** - QA Lead confirms all acceptance criteria met
- [ ] **Release notes drafted** - Document notable changes, migration steps, known issues
- [ ] **Deployment plan reviewed** - Deployment steps, timing, and rollback procedures documented
- [ ] **Smoke tests prepared** - Critical flow tests ready for staging and production
- [ ] **Backup/snapshot taken** - Database or system backup completed (if applicable)
- [ ] **Stakeholder notification sent** - Inform stakeholders of planned release window

## Staging Deployment (T-minus 1 day)

- [ ] **Deploy to staging** - Execute deployment to staging environment
- [ ] **Run smoke tests** - Validate critical flows in staging
- [ ] **QA sign-off obtained** - QA Lead approves staging deployment
- [ ] **Performance verified** - Check latency, error rates, resource usage
- [ ] **Security scan reviewed** - No new high-severity vulnerabilities introduced
- [ ] **Rollback plan tested** - Verify rollback procedure works in staging (if needed)

## Go/No-Go Decision (T-minus 4 hours)

Meeting attendees: Release Coordinator, Project Manager, QA Lead, Risk Champion (optional)

- [ ] **Review deployment readiness** - All pre-release and staging checks passed
- [ ] **Assess risks** - Risk Champion confirms no critical blockers
- [ ] **Confirm on-call coverage** - Engineering on-call is aware and available
- [ ] **Communication plan ready** - Support team and stakeholders briefed on release
- [ ] **Decision made** - Document GO or NO-GO decision with rationale

If NO-GO: Document reasons, create action items, and reschedule release.

## Production Deployment

- [ ] **Deployment window started** - Begin deployment during scheduled window
- [ ] **Deployment executed** - Follow documented deployment steps
- [ ] **Initial health checks pass** - Verify application starts and responds
- [ ] **Run smoke tests** - Execute critical flow tests in production
- [ ] **Monitor metrics** - Watch error rates, latency, traffic patterns for 15-30 minutes
- [ ] **Verify key features** - Spot-check new features work as expected

## Post-Deployment (Within 2 hours)

- [ ] **Release announced** - Notify stakeholders and support teams via agreed channels
- [ ] **Documentation updated** - Update wikis, changelogs, or knowledge bases as needed
- [ ] **Monitor for issues** - Continue monitoring metrics and support channels
- [ ] **Close release ticket** - Update project tracking with release completion

## Rollback Procedure (If needed)

If critical issues detected post-deployment:

1. **Trigger incident response** - Notify on-call and Project Manager immediately
2. **Assess severity** - Determine if rollback is necessary or if hotfix is feasible
3. **Execute rollback** - Follow documented rollback procedure
4. **Verify rollback success** - Confirm system returns to stable state
5. **Communicate status** - Update stakeholders on rollback and next steps
6. **Schedule post-incident review** - Capture learnings and prevent recurrence

## Roles and Responsibilities

- **Release Coordinator**: Owns this checklist, coordinates activities, makes go/no-go call
- **QA Lead**: Provides quality sign-off, executes smoke tests
- **Project Manager**: Participates in go/no-go decision, manages stakeholder communication
- **Developers**: Available during deployment window for troubleshooting
- **Risk Champion**: Provides risk assessment for go/no-go decision
- **On-call Engineer**: Available to respond to production issues post-deployment

---

*Last updated: October 2025*
