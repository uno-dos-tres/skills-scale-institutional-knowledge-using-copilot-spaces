# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared
- Release readiness reviewed by Project Manager, Product Manager, QA Lead, and Delivery Lead

## Release Readiness Gates
- Acceptance criteria complete and tested
- Dependencies validated and resolved
- Deployment plan confirmed with Ops or environment owner
- Communication plan for impacted teams and stakeholders approved
- Rollback plan and success criteria agreed

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support
- [ ] Confirm monitoring and alerting are active for release metrics

## Post-release Review
- Conduct a short launch review with the team
- Confirm release objectives and success metrics
- Capture issues and improvement opportunities
- Update release notes with any follow-up actions
- Share post-release summary with stakeholders

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
