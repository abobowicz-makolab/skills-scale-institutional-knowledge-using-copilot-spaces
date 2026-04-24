# OctoAcme — Release Readiness Checklist

Use this checklist before every production release to confirm all gates are cleared. The **Release Manager** owns the checklist and collects sign-offs from each role listed below.

> For role definitions, see [Roles and Personas](octoacme-roles-and-personas.md).
> For deployment steps, see [Release & Deployment Guide](octoacme-release-and-deployment.md).

---

## Scope & Quality

- [ ] All acceptance criteria met and verified by QA/Testing
- [ ] All planned PRs merged to the release branch; no open blocking PRs
- [ ] No unresolved High/Critical bugs in scope for this release
- [ ] Regression suite passed (unit, integration, and smoke tests)
- [ ] UX Designer reviewed final implementation against design specifications (for UI changes)
- [ ] Business Analyst confirmed deliverables meet documented requirements

## Security

- [ ] Security Touchpoints Checklist completed — see [Security Touchpoints Checklist](octoacme-security-touchpoints.md)
- [ ] Security Champion has provided written sign-off (comment in release ticket or PR)
- [ ] All High/Critical SAST/SCA findings resolved or formally accepted

## Release Artifacts

- [ ] Release notes drafted and reviewed by Release Manager and Product Manager
- [ ] Deployment runbook or steps documented (or reference to CI/CD pipeline)
- [ ] Rollback plan documented and tested (where applicable)
- [ ] Environment-specific configuration changes identified and staged

## Communication & Coordination

- [ ] Deployment window confirmed with all affected teams
- [ ] Stakeholders notified of upcoming release and expected downtime (if any)
- [ ] Support / on-call team briefed on changes and potential issues
- [ ] Go/no-go meeting held with PM, PdM, Release Manager, and Security Champion

## Post-Release

- [ ] Smoke tests executed in production immediately after deployment
- [ ] Success metrics and dashboards reviewed within 24 hours of release
- [ ] Release announcement sent to stakeholders and support channels
- [ ] Retrospective scheduled if the release involved significant complexity or issues

---

## Go / No-Go Sign-Offs

| Role | Owner | Status |
|---|---|---|
| Project Manager | | ☐ Approved / ☐ Blocked |
| Product Manager | | ☐ Approved / ☐ Blocked |
| Release Manager | | ☐ Approved / ☐ Blocked |
| Security Champion | | ☐ Approved / ☐ Blocked |
| QA Lead / Testing | | ☐ Approved / ☐ Blocked |

> A single **Blocked** status halts the release until the issue is resolved or formally accepted by the accountable parties.

---

*See also: [Security Touchpoints Checklist](octoacme-security-touchpoints.md) · [RACI Matrix](octoacme-raci-matrix.md) · [Risk Management & Communication](octoacme-risks-and-communication.md)*
