# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises. For a simplified view of how roles interact across the project lifecycle, see the [RACI-Lite Template](octoacme-raci-lite-template.md).

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

## QA / Testing

### Role Summary
QA/Testing specialists validate that delivered features meet acceptance criteria and quality standards. They own the test strategy and provide an independent quality signal before release.

### Responsibilities
- Define and maintain the test strategy (unit, integration, end-to-end)
- Write and execute test cases against acceptance criteria
- Log, track, and verify defects
- Participate in sprint reviews to validate completed work
- Collaborate on the Definition of Done

### Goals
- Prevent defect leakage to production
- Shorten feedback loops between development and quality validation
- Continuously improve test coverage and automation

### Typical Communication
- Sprint ceremonies (planning, review, retro)
- Bug reports and test result summaries
- Close collaboration with Developers on test plans and environment parity

### Interactions with Other Roles
- **Developers**: pair on testability requirements; verify fixes
- **Product Manager**: confirm acceptance criteria are testable
- **Project Manager**: surface quality risks and testing blockers early
- **DevOps Engineer**: align on test environments and CI/CD pipeline gates

---

## Stakeholders

### Role Summary
Stakeholders are internal or external parties with a vested interest in project outcomes. They provide direction, approvals, and feedback without being day-to-day delivery contributors.

### Responsibilities
- Provide strategic requirements and business context
- Review and approve project charters, roadmaps, and releases
- Escalate priorities and resolve cross-team blockers
- Offer feedback during demos and milestone reviews

### Goals
- Ensure the project delivers measurable business value
- Stay informed without being in the weeds of delivery
- Align delivery teams to organizational priorities

### Typical Communication
- Monthly stakeholder updates
- Ad-hoc milestone reviews and demos
- Escalation via the Project Manager

### Interactions with Other Roles
- **Project Manager**: primary point of contact for status, risks, and decisions
- **Product Manager**: aligns business requirements and priorities
- **Developers/QA**: occasionally consulted on technical feasibility and quality risk

---

## Scrum Master

### Role Summary
The Scrum Master facilitates agile ceremonies, removes team impediments, and coaches the team on process adherence and continuous improvement. This role focuses on team health, velocity, and process rather than content.

### Responsibilities
- Facilitate sprint ceremonies: planning, daily standup, review, and retrospective
- Identify and actively resolve blockers and impediments
- Shield the team from unplanned interruptions during a sprint
- Coach the team on agile principles and practices
- Track and share team metrics (velocity, cycle time, escaped defects)
- Partner with the Project Manager on delivery health reporting

### Goals
- Improve team flow and reduce friction in the delivery process
- Foster a culture of continuous improvement and psychological safety
- Keep ceremonies efficient and outcome-focused

### Typical Communication
- Daily standups and sprint ceremonies
- Impediment log and team health dashboards
- Regular 1:1s or check-ins with team members

### Interactions with Other Roles
- **Project Manager**: align on delivery risks, schedule, and team capacity; the Scrum Master focuses on team process while the PM owns external commitments and stakeholder communication
- **Developers**: remove technical blockers; protect sprint scope
- **Product Manager**: coordinate backlog readiness and acceptance criteria clarity before sprint planning
- **QA/Testing**: ensure testing tasks are included in sprint planning and Definition of Done

---

## UX Designer / Researcher

### Role Summary
UX Designers/Researchers lead discovery, design, and usability validation to ensure features meet user needs. They translate user research into intuitive, accessible experiences.

### Responsibilities
- Conduct user research (interviews, usability testing, surveys)
- Create wireframes, prototypes, and design specifications
- Define and maintain design systems and accessibility standards
- Collaborate with Product Managers to shape feature requirements
- Validate designs with real users before and after implementation
- Participate in sprint reviews to evaluate shipped UI/UX quality

### Goals
- Deliver experiences that are intuitive, accessible, and aligned with user mental models
- Reduce redesign cycles by validating assumptions early
- Champion the user perspective throughout the product lifecycle

### Typical Communication
- Design reviews and prototype walkthroughs with Product and Engineering
- User research readouts for the broader team
- Design specifications and annotated mockups in project tooling

### Interactions with Other Roles
- **Product Manager**: co-define problem statements, validate that designs meet business goals, and inform prioritization with user insights
- **Developers**: provide design specs and answer implementation questions; review final implementation for fidelity
- **Project Manager**: flag design discovery tasks as dependencies in the project plan
- **Stakeholders**: present research findings and design rationale at milestone reviews

---

## DevOps Engineer

### Role Summary
DevOps Engineers establish and maintain CI/CD pipelines, manage infrastructure-as-code, monitor deployment health, and lead incident response practices. They bridge the gap between development velocity and operational reliability.

### Responsibilities
- Design, build, and maintain CI/CD pipelines and deployment automation
- Manage cloud infrastructure, environments, and configuration as code
- Monitor system health; own alerting, on-call rotations, and incident response
- Define environment parity standards (dev, staging, production)
- Collaborate with Developers on release-readiness and rollback strategies
- Maintain platform documentation and runbooks

### Goals
- Reduce deployment lead time and increase release frequency
- Improve system reliability and minimize mean time to recovery (MTTR)
- Make infrastructure observable, reproducible, and auditable

### Typical Communication
- Deployment readiness checks before release windows
- Incident post-mortems and action item tracking
- Infrastructure change proposals via pull requests or RFCs

### Interactions with Other Roles
- **Developers**: advise on build tooling, container strategy, and local/staging environment setup
- **Project Manager**: provide deployment schedule inputs and escalate environment risks
- **QA/Testing**: ensure test environments match production configuration
- **Security Champion**: implement security controls in the pipeline (secret scanning, image scanning, SAST)
- **Stakeholders**: communicate planned maintenance windows and SLA/SLO status

---

## Support Lead

### Role Summary
The Support Lead coordinates support operations, triages escalated issues, ensures timely resolution, and collects product feedback from users. They act as the bridge between end users and the delivery team.

### Responsibilities
- Manage the support queue and set triage priorities and SLAs
- Escalate critical bugs and incidents to the engineering team
- Track user-reported defects and ensure they are logged in the backlog
- Synthesize support trends and surface them as product improvement inputs
- Maintain support runbooks and knowledge base articles
- Coordinate user communications for incidents and service updates

### Goals
- Resolve user issues quickly and within SLA
- Reduce repeat incidents through root-cause-driven fixes
- Close the feedback loop between users and the product team

### Typical Communication
- Support queue management and escalation pings
- Weekly support summary shared with Product Manager and Project Manager
- Incident communication to affected users

### Interactions with Other Roles
- **Project Manager**: escalate critical incidents that affect delivery commitments or require engineering priority changes
- **Product Manager**: share support trends and user feedback to inform backlog prioritization
- **Developers**: hand off escalated bugs with reproduction steps and impact context
- **DevOps Engineer**: collaborate on incident response and post-incident reviews
- **Stakeholders**: provide support metrics and SLA reports at milestone reviews

---

## Security Champion

### Role Summary
The Security Champion advocates for security best practices, reviews risk registers for security entries, and helps the team integrate security early in the development lifecycle (shift-left security).

### Responsibilities
- Promote secure coding practices and awareness across the team
- Review design docs and pull requests for security implications
- Contribute security risk entries to the Risk Register
- Coordinate with DevOps on pipeline security controls (secret scanning, dependency audits, SAST/DAST)
- Assist with threat modeling for new features or significant changes
- Triage and track security vulnerabilities through remediation

### Goals
- Reduce security vulnerabilities before they reach production
- Build a security-aware culture without slowing delivery
- Ensure compliance requirements are understood and met

### Typical Communication
- Security review checkpoints at design and pre-release stages
- Vulnerability reports and remediation status updates
- Periodic security awareness sessions or brown-bags

### Interactions with Other Roles
- **Project Manager**: surface security risks early so they can be planned and prioritized
- **Developers**: provide guidance on secure coding, review PRs, and validate fixes
- **DevOps Engineer**: define and enforce security gates in CI/CD pipelines
- **Product Manager**: help frame security requirements as user-facing value (e.g., data privacy)
- **Stakeholders**: report on security posture and compliance status at key milestones

---

## Role Interaction Mapping (RACI-Lite)

The table below summarizes which roles are **Responsible (R)**, **Accountable (A)**, **Consulted (C)**, or **Informed (I)** for key project phases.

> For a reusable blank template, see [RACI-Lite Template](octoacme-raci-lite-template.md).

| Phase / Activity | Project Manager | Product Manager | Scrum Master | Developers | QA/Testing | UX Designer | DevOps Engineer | Support Lead | Security Champion | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|---|
| **Initiation** (charter, goals) | A | R | C | C | I | C | I | I | C | C |
| **Planning** (scope, milestones) | A | R | C | C | C | C | C | I | C | I |
| **Sprint Ceremonies** | C | C | A/R | R | R | R | C | I | I | I |
| **Execution** (build, test) | I | C | C | R | R | C | C | I | C | I |
| **Release / Deployment** | A | C | I | R | R | I | R | C | C | I |
| **Incident Response** | A | I | I | R | C | I | R | R | C | I |
| **Retrospective** | A | C | R | R | R | R | C | C | C | I |
| **Stakeholder Reporting** | R | C | I | I | I | I | I | C | C | A |

**Key:** R = Responsible · A = Accountable · C = Consulted · I = Informed

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Refer to the [RACI-Lite Template](octoacme-raci-lite-template.md) to map role ownership for a specific project or workstream.

