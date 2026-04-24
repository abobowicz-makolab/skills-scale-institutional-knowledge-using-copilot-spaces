# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (see [Security Touchpoints Checklist](octoacme-security-touchpoints.md))
- Release notes drafted by **Release Manager** and reviewed by Product Manager
- Rollback / mitigation plan documented
- Smoke tests prepared
- **Release Manager** completes the [Release Readiness Checklist](octoacme-release-readiness-checklist.md) and collects go/no-go sign-offs

## Deployment Checklist
- [ ] **Release Manager** confirms all go/no-go sign-offs collected (see [Release Readiness Checklist](octoacme-release-readiness-checklist.md))
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

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
