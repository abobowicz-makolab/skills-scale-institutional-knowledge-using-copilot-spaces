# OctoAcme — Security Touchpoints Checklist

Lightweight checklist of security activities to complete at each phase of the project lifecycle. The **Security Champion** owns this checklist and works with the team to complete each item.

> For the Security Champion role definition, see [Roles and Personas](octoacme-roles-and-personas.md).
> For security incident escalation, see [Risk Management & Communication](octoacme-risks-and-communication.md).

---

## Planning Phase

- [ ] Security requirements identified and added to the backlog (e.g., auth, data protection, audit logging)
- [ ] Threat model or lightweight risk review completed for significant new features
- [ ] Sensitive data types catalogued (PII, credentials, payment data) and handling requirements documented
- [ ] Dependency vulnerability scan scheduled as part of CI pipeline
- [ ] Compliance or regulatory constraints identified and noted in the project One-pager

---

## Implementation Phase

- [ ] Secure-coding guidelines shared with Developers (input validation, output encoding, least privilege)
- [ ] High-risk PRs (auth, permissions, data access) flagged for Security Champion review before merge
- [ ] Secrets and credentials managed via environment variables or a secrets manager (never committed to source)
- [ ] Security scanning (SAST/SCA) running in CI and results reviewed each sprint
- [ ] New dependencies checked for known vulnerabilities before adoption

---

## Pre-Release Phase

- [ ] Security scan results reviewed; all High/Critical findings resolved or formally accepted with a mitigation plan
- [ ] Authentication and authorization flows tested end-to-end
- [ ] Release notes include any security-relevant changes or advisories
- [ ] Security Champion provides sign-off to Release Manager for the go/no-go decision
- [ ] Rollback / incident response plan reviewed and ready if a security issue is discovered post-release

---

## Post-Release / Ongoing

- [ ] Monitor for new CVEs affecting shipped dependencies; patch within SLA
- [ ] Security-related production incidents trigger a blameless retrospective within 48 hours
- [ ] Lessons learned from incidents fed back into this checklist and the planning phase for the next cycle

---

*See also: [Release Readiness Checklist](octoacme-release-readiness-checklist.md) · [RACI Matrix](octoacme-raci-matrix.md)*
