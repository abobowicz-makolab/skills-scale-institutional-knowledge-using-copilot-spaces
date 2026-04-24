# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Business Analyst

### Role Summary
Business Analysts bridge the gap between stakeholder needs and the delivery team. They gather, clarify, and document requirements, ensuring that what gets built solves the right problem and meets business expectations.

### Responsibilities
- Elicit and document requirements through stakeholder interviews and workshops
- Translate business needs into clear user stories and acceptance criteria
- Validate deliverables against business requirements throughout the project lifecycle
- Facilitate requirement reviews and sign-offs with stakeholders
- Maintain a requirements traceability matrix to link work items back to business goals

### Goals
- Ensure the team is solving the right problem before writing a line of code
- Reduce rework caused by unclear or misunderstood requirements
- Accelerate decision-making by providing clear, well-documented options and trade-offs

### Typical Communication
- Requirement workshops and stakeholder interviews during initiation and planning
- User story reviews with Product Manager and Developers
- Acceptance-criteria check-ins before sprint commitments
- Sign-off meetings with stakeholders before major releases

### Interactions with Existing Roles
- **Product Managers:** Co-own the backlog; BA provides detailed requirements that PdM uses to prioritize.
- **Project Managers:** Surface scope risks early; escalate unclear requirements that could affect timeline.
- **Developers:** Clarify acceptance criteria, answer questions during implementation, and validate delivered stories.
- **Stakeholders:** Primary liaison for capturing business needs and communicating progress against requirements.

---

## Release Manager

### Role Summary
Release Managers plan, coordinate, and oversee the release process to ensure software reaches production safely and on schedule. They serve as the single point of accountability for release readiness and deployment execution.

### Responsibilities
- Own the release schedule and communicate it to all stakeholders
- Gate releases against the [Release Readiness Checklist](octoacme-release-readiness-checklist.md)
- Coordinate go/no-go decisions with PM, PdM, QA, and Security Champion
- Manage deployment windows, change requests, and rollback procedures
- Draft and distribute release notes and announcements

### Goals
- Ship reliably with minimal production incidents
- Keep release process predictable and repeatable
- Reduce time-to-recovery when releases require rollback

### Typical Communication
- Release schedule updates to all affected teams
- Go/no-go calls with PM, QA, and Security Champion before each release
- Post-release announcements and incident retrospectives

### Interactions with Existing Roles
- **Project Managers:** Align on milestones, deployment windows, and risk exposure before each release.
- **Product Managers:** Confirm scope is correct and release notes reflect intended changes.
- **Developers:** Coordinate branching strategy, deployment artifacts, and smoke-test execution.
- **QA/Testing:** Verify all acceptance criteria and regression tests pass before go/no-go sign-off.
- **Security Champion:** Confirm security touchpoints (see [Security Touchpoints Checklist](octoacme-security-touchpoints.md)) are cleared before release.

---

## Scrum Master

### Role Summary
Scrum Masters facilitate the team's agile ceremonies, remove impediments, and protect the team's focus. They coach the team on process and help continuously improve how work gets done.

### Responsibilities
- Facilitate daily standups, sprint planning, reviews, and retrospectives
- Identify and remove blockers or escalate them promptly
- Shield the team from scope creep and unplanned interruptions during a sprint
- Coach team members on agile principles and practices
- Track velocity and sprint health metrics; surface trends to the Project Manager

### Goals
- Keep the team focused and productive within each sprint
- Reduce waste and inefficiency in the delivery process
- Foster a culture of continuous improvement and psychological safety

### Typical Communication
- Daily standups and sprint ceremonies
- Blocker and impediment logs shared with PM for escalation
- Sprint metrics summary (velocity, burndown) at the end of each sprint

### Interactions with Existing Roles
- **Project Managers:** Collaborate on escalations, risk flags, and capacity planning; Scrum Master focuses on sprint-level flow while PM manages broader timeline and stakeholder coordination.
- **Product Managers:** Ensure backlog items are ready for sprint commitment; flag unclear or missing acceptance criteria before planning.
- **Developers:** Day-to-day facilitation of ceremonies; acts as first responder for team-level impediments.
- **Stakeholders:** May represent team progress in demos; manages stakeholder expectations during sprint reviews.

---

## Security Champion

### Role Summary
Security Champions advocate for security best practices within the delivery team. They act as the first line of defense for identifying risks during design and implementation, and serve as the point of contact for security incidents.

### Responsibilities
- Review designs and significant PRs for security risks
- Ensure security requirements are captured in the backlog and acceptance criteria
- Maintain and follow the [Security Touchpoints Checklist](octoacme-security-touchpoints.md)
- Act as the team's primary contact during a security incident
- Stay current on relevant security advisories and communicate impacts to the team

### Goals
- Embed security early ("shift-left") to avoid costly late-stage fixes
- Reduce the risk of production security incidents
- Ensure the team meets compliance and audit requirements

### Typical Communication
- Security review sessions during planning and pre-release gates
- Async comments on design docs and PRs flagged for security review
- Incident communication following the escalation path in the [Risk Management & Communication](octoacme-risks-and-communication.md) doc

### Interactions with Existing Roles
- **Project Managers:** Surface security risks as project-level risks in the risk register; coordinate timeline adjustments when security issues are found.
- **Product Managers:** Advise on security implications of product decisions and prioritize security-related backlog items.
- **Developers:** Pair on secure-coding practices; review high-risk code changes before merge.
- **Release Manager:** Provide security sign-off as part of the go/no-go process before each release.
- **Stakeholders:** Communicate security posture and any material incidents that affect customers or compliance.

---

## UX Designer

### Role Summary
UX Designers research user needs, design intuitive interfaces and interaction flows, and ensure that what gets built is usable and accessible. They translate product requirements into design specifications that developers can implement.

### Responsibilities
- Conduct user research (interviews, usability tests, analytics review) to inform design decisions
- Create wireframes, mockups, and interactive prototypes
- Define interaction patterns, visual hierarchy, and accessibility standards
- Work with Product Manager to turn user insights into prioritized design requirements
- Collaborate with Developers to ensure designs are implemented as intended

### Goals
- Deliver experiences that are intuitive, accessible, and aligned with user needs
- Reduce usability issues discovered late in QA or post-release
- Build a shared design system that speeds up implementation and ensures consistency

### Typical Communication
- Design reviews with Product Manager and Developers during planning and early implementation
- Prototype walkthroughs with stakeholders to validate concepts before build
- Async handoffs via annotated design files or specifications shared in the project repo

### Interactions with Existing Roles
- **Product Managers:** Collaborate on defining user problems, prioritizing design work, and validating prototypes with users.
- **Project Managers:** Surface design dependencies and timeline needs (e.g., research phases, design sign-off gates).
- **Developers:** Provide detailed specs and be available for implementation questions; review builds against design intent.
- **QA/Testing:** Share acceptance criteria related to usability and accessibility; participate in exploratory testing of UI flows.
- **Stakeholders:** Present design concepts and gather feedback to ensure alignment before full implementation.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See the [RACI Matrix](octoacme-raci-matrix.md) for a quick-reference overview of who owns what across the project lifecycle.

