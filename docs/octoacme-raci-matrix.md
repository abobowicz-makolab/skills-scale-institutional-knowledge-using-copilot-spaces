# OctoAcme — RACI Matrix

Quick-reference guide showing who is **R**esponsible, **A**ccountable, **C**onsulted, or **I**nformed for key activities across the project lifecycle.

> **Key:** R = Responsible (does the work) · A = Accountable (owns outcome) · C = Consulted (input required) · I = Informed (kept up to date)

---

## Project Initiation

| Activity | PM | PdM | Dev | Scrum Master | BA | UX | Release Mgr | Security Champion |
|---|---|---|---|---|---|---|---|---|
| Define problem statement & goals | C | A/R | I | I | R | C | I | I |
| Stakeholder identification & alignment | A/R | C | I | I | C | I | I | I |
| Project One-pager creation | A/R | C | I | I | R | C | I | I |
| Initial risk assessment | A/R | C | C | I | C | I | I | R |
| Team roles & resource planning | A/R | C | I | C | I | I | C | I |

---

## Planning

| Activity | PM | PdM | Dev | Scrum Master | BA | UX | Release Mgr | Security Champion |
|---|---|---|---|---|---|---|---|---|
| Backlog creation & prioritization | C | A/R | C | C | R | C | I | I |
| Acceptance criteria definition | C | C | C | I | A/R | C | I | I |
| Release schedule & milestones | A/R | C | I | C | I | I | R | I |
| Definition of Done | C | C | A/R | R | C | I | I | I |
| Security requirements capture | C | C | C | I | C | I | I | A/R |
| UX research & design planning | I | C | I | I | C | A/R | I | I |

---

## Execution & Tracking

| Activity | PM | PdM | Dev | Scrum Master | BA | UX | Release Mgr | Security Champion |
|---|---|---|---|---|---|---|---|---|
| Daily standups & impediment removal | I | I | R | A/R | I | I | I | I |
| Sprint planning & commitment | C | C | R | A/R | C | C | I | I |
| Feature implementation | I | I | A/R | I | I | I | I | I |
| Design implementation review | I | I | R | I | I | A/R | I | I |
| Security review (PRs / designs) | I | I | C | I | I | I | I | A/R |
| Blocker escalation | A/R | I | I | R | I | I | I | I |
| Status reporting | A/R | C | I | I | I | I | I | I |
| Risk register updates | A/R | I | C | I | I | I | I | C |

---

## Release

| Activity | PM | PdM | Dev | Scrum Master | BA | UX | Release Mgr | Security Champion |
|---|---|---|---|---|---|---|---|---|
| Release readiness sign-off | C | C | C | I | I | I | A/R | C |
| Go/no-go decision | A | A | I | I | I | I | R | C |
| Deployment execution | I | I | R | I | I | I | A/R | I |
| Release notes & announcement | C | C | I | I | I | I | A/R | I |
| Security clearance pre-release | I | I | I | I | I | I | C | A/R |
| Smoke tests & post-deploy verification | I | I | R | I | I | I | C | I |
| Rollback decision & execution | C | C | R | I | I | I | A/R | I |

---

## Communication & Risk

| Activity | PM | PdM | Dev | Scrum Master | BA | UX | Release Mgr | Security Champion |
|---|---|---|---|---|---|---|---|---|
| Stakeholder updates | A/R | C | I | I | I | I | C | I |
| Risk register maintenance | A/R | I | C | C | I | I | C | C |
| Security incident response | C | I | C | I | I | I | I | A/R |
| Retrospective facilitation | C | I | R | A/R | I | I | I | I |
| Continuous improvement tracking | A/R | I | C | R | I | I | I | I |

---

## Handoff / Interaction Map

Key handoffs between roles during a typical project:

1. **PdM → BA:** Product vision and high-level requirements passed to BA for detailed elaboration.
2. **BA → Dev + UX:** Refined user stories with acceptance criteria handed to Developers and UX Designer for design and implementation.
3. **UX → Dev:** Design specifications and prototypes handed off to Developers; UX reviews implementation for fidelity.
4. **Dev → QA/Testing:** Completed features handed off for acceptance and regression testing.
5. **Security Champion → Dev:** Security review findings passed back to Developers before merge; cleared before release.
6. **Scrum Master → PM:** Sprint metrics, velocity, and blocker summary handed to PM for timeline and stakeholder reporting.
7. **PM + PdM + Security Champion → Release Manager:** Go/no-go inputs consolidated by Release Manager before deployment.
8. **Release Manager → Stakeholders:** Release notes and announcements distributed post-deployment.

---

*For role definitions and full responsibilities, see [Roles and Personas](octoacme-roles-and-personas.md).*
