# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability. The **Release Coordinator** owns the end-to-end release process, ensuring smooth coordination across teams.

For a comprehensive release coordination checklist, see [Release Coordination Checklist Template](template-release-coordination-checklist.md).

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted (by Release Coordinator)
- Rollback / mitigation plan documented
- Smoke tests prepared (coordinated with QA Lead)
- QA Lead sign-off obtained

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) - coordinated by Release Coordinator
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests - validated by QA Lead
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support - managed by Release Coordinator

For a detailed pre-release, deployment, and post-deployment checklist, see [Release Coordination Checklist Template](template-release-coordination-checklist.md).

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (Release Coordinator coordinates)
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items (Risk Champion tracks)
  - Conduct post-incident blameless retrospective

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
