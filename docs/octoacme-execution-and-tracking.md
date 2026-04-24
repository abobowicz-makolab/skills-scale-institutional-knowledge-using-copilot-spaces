# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — facilitated by the **Scrum Master**; focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Sprint planning — **Scrum Master** ensures backlog items are ready and team capacity is respected
- Demo/Review at the end of each sprint or milestone
- Sprint retrospective — **Scrum Master** facilitates; output feeds the [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) process

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: **Scrum Master** triages in daily standup; removes or escalates impediments same day
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues
- Security blockers: **Security Champion** is looped in for any security-related impediment; follow the escalation path in [Risk Management & Communication](octoacme-risks-and-communication.md)

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
