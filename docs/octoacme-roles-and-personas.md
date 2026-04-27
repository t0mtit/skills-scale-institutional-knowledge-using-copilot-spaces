# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

See also:
- [Role Responsibility Matrix (RACI)](./role-responsibility-matrix.md)
- [Role Onboarding Checklist Template](./templates/role-onboarding-checklist.md)
- [Acceptance Criteria Template](./templates/acceptance-criteria-template.md)

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
- Collaborate with QA Lead on testability and test coverage
- Support DevOps Engineer on deployment readiness and monitoring hooks

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

### Interacts With
- **Scrum Master** — surface blockers during standups; partner on sprint health
- **QA Lead** — clarify acceptance criteria; coordinate on bug triage and test coverage
- **DevOps Engineer** — align on CI/CD requirements, environment needs, and deployment steps
- **UX/UI Designer** — review designs before implementation; raise feasibility concerns early
- **Product Manager (PdM)** — clarify requirements and acceptance criteria; flag scope risks

### Escalation Points
- Escalate unresolved technical blockers to Scrum Master (sprint level) or PM (cross-team dependencies)
- Escalate unresolvable quality issues to QA Lead before release

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics
- Author and review acceptance criteria (see [Acceptance Criteria Template](./templates/acceptance-criteria-template.md))
- Engage SMEs to validate domain assumptions in requirements

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

### Interacts With
- **Project Manager (PM)** — align on scope, timeline, and risk; resolve prioritization conflicts
- **UX/UI Designer** — co-author user flows; review wireframes and prototypes
- **SME** — validate domain feasibility; incorporate expert constraints into backlog
- **Data Analyst** — review success metrics; use data to inform prioritization
- **Scrum Master** — surface backlog refinement needs; ensure sprint goals are value-focused

### Escalation Points
- Escalate priority conflicts or scope creep to Product Lead or Sponsor
- Escalate unvalidated requirements to SME before sprint commitment

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
- Maintain the [Role Responsibility Matrix](./role-responsibility-matrix.md) and ensure RACI clarity
- Drive onboarding of new team members using the [Onboarding Checklist Template](./templates/role-onboarding-checklist.md)

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

### Interacts With
- **Scrum Master** — remove cross-team impediments; align sprint health with overall project timeline
- **Release Manager** — coordinate release windows, change freeze, and go/no-go decisions
- **Support Lead** — ensure runbooks and support readiness ahead of releases
- **Product Manager (PdM)** — manage scope and prioritization trade-offs

### Escalation Points
- Escalate resource conflicts or missed milestones to Program Lead or Sponsor
- Escalate repeated team-level blockers unresolved by Scrum Master to Product Lead

---

## Scrum Master

### Role Summary
The Scrum Master facilitates agile ceremonies, protects the team from interruptions, and coaches continuous improvement. They serve as the team's process guardian.

### Responsibilities
- Facilitate daily standups, sprint planning, reviews, and retrospectives
- Identify and remove team-level impediments
- Shield the team from unplanned interruptions during a sprint
- Coach the team on agile practices and continuous improvement
- Track sprint velocity and health metrics
- Escalate cross-team blockers to the Project Manager

### Goals
- Sustain a predictable, healthy delivery cadence
- Foster psychological safety and high team morale
- Improve team practices sprint over sprint

### Interacts With
- **Project Manager (PM)** — escalate impediments that require cross-team action; align sprint goals with project milestones
- **Product Manager (PdM)** — coordinate backlog refinement sessions; ensure stories are ready for sprint commitment
- **Developers** — facilitate technical retrospectives; surface and address technical debt signals
- **QA Lead** — ensure QA is embedded in sprint ceremonies; track quality gates

### Escalation Points
- Escalate unresolved impediments to PM after two consecutive standups without progress
- Escalate process violations (scope creep mid-sprint, missing acceptance criteria) to PdM and PM

### Artifacts Owned or Influenced
- Sprint velocity and burndown charts
- Retrospective action items log
- Impediment backlog

---

## UX/UI Designer

### Role Summary
UX/UI Designers own the usability, accessibility, and visual design of product deliverables. They ensure that solutions are intuitive and meet user needs before and during development.

### Responsibilities
- Create wireframes, mockups, and interactive prototypes
- Conduct or coordinate user research and usability testing
- Define interaction patterns, component guidelines, and accessibility standards
- Collaborate with Developers to ensure design fidelity in implementation
- Review implemented features against design specifications
- Contribute acceptance criteria related to UX and accessibility (see [Acceptance Criteria Template](./templates/acceptance-criteria-template.md))

### Goals
- Deliver intuitive, accessible, and consistent user experiences
- Reduce re-work by aligning designs with engineering constraints early
- Ensure usability testing validates key user journeys

### Interacts With
- **Product Manager (PdM)** — align on user stories and problem framing; incorporate UX research findings into backlog
- **Developers** — hand off design specs; clarify UI behavior edge cases; review implementations
- **QA Lead** — define acceptance criteria for visual and interaction correctness
- **SME** — validate domain-specific UI conventions and terminology

### Escalation Points
- Escalate design-feasibility disagreements to PdM and PM for trade-off decision
- Escalate accessibility compliance blockers to PM and Release Manager before release

### Artifacts Owned or Influenced
- Wireframes and high-fidelity mockups
- Design system / component library
- Usability testing reports

---

## Subject Matter Expert (SME)

### Role Summary
Subject Matter Experts provide deep domain knowledge to validate requirements, assess feasibility, and ensure that the solution correctly addresses business or technical constraints.

### Responsibilities
- Review and validate business requirements and acceptance criteria for domain correctness
- Identify domain-specific risks, constraints, and edge cases
- Participate in backlog refinement to advise on scope and complexity
- Provide input on test scenarios that reflect real-world usage
- Review deliverables for accuracy before QA sign-off

### Goals
- Ensure the product correctly solves real-world domain problems
- Reduce rework caused by misunderstood domain constraints
- Serve as an on-call resource for domain questions during development

### Interacts With
- **Product Manager (PdM)** — validate problem framing and acceptance criteria; flag domain gaps in requirements
- **Developers** — clarify domain rules and edge cases; review complex logic implementations
- **QA Lead** — provide domain-accurate test scenarios and expected outcomes
- **UX/UI Designer** — validate domain terminology and workflow conventions in UI

### Escalation Points
- Escalate unresolvable domain conflicts (competing standards, regulatory ambiguity) to PdM and Sponsor
- Flag risks discovered late in development immediately to PM for impact assessment

### Artifacts Owned or Influenced
- Domain knowledge base / FAQ
- Validated acceptance criteria (domain sign-off)
- Test scenario inputs

---

## QA Lead

### Role Summary
The QA Lead owns the overall test strategy, coordinates manual and automated test efforts, and serves as the quality gate before release.

### Responsibilities
- Define and maintain the test strategy (unit, integration, e2e, exploratory)
- Review and contribute to acceptance criteria for testability (see [Acceptance Criteria Template](./templates/acceptance-criteria-template.md))
- Coordinate manual and automated testing execution
- Manage bug triage, severity classification, and resolution tracking
- Provide QA sign-off as part of the release process
- Escalate unresolved critical defects to PM and Release Manager

### Goals
- Achieve and maintain agreed quality gates before every release
- Shift testing left by embedding QA in sprint ceremonies
- Reduce production defect rate and mean-time-to-detect

### Interacts With
- **Developers** — co-define acceptance criteria; collaborate on testability and test automation
- **Project Manager (PM)** — report quality status; flag release-blocking defects
- **Release Manager** — confirm QA sign-off before go/no-go decision
- **SME** — obtain domain-accurate test scenarios and expected results
- **Scrum Master** — track QA capacity and blockers in sprint ceremonies

### Escalation Points
- Escalate release-blocking defects to PM and Release Manager immediately
- Escalate recurring quality issues to PdM for backlog prioritization

### Artifacts Owned or Influenced
- Test plan and test strategy document
- Bug/defect tracker
- QA sign-off checklist

---

## DevOps Engineer

### Role Summary
DevOps Engineers manage CI/CD pipelines, infrastructure, deployment automation, and production observability. They enable fast, safe, and repeatable delivery.

### Responsibilities
- Design, maintain, and improve CI/CD pipelines
- Manage infrastructure as code and environment configurations
- Monitor production systems and respond to infrastructure incidents
- Coordinate deployment windows and rollback procedures with Release Manager
- Integrate security scanning and quality gates into pipelines
- Support developers with build and deployment troubleshooting

### Goals
- Achieve high deployment frequency with low change failure rate
- Minimize mean time to recovery (MTTR) from incidents
- Ensure environment parity from dev to production

### Interacts With
- **Developers** — provide pipeline tooling; unblock build/deployment issues; advise on testability and observability
- **Release Manager** — coordinate release deployments; define rollback criteria
- **QA Lead** — integrate automated test execution in CI; provide environment support for QA
- **Project Manager (PM)** — report CI/CD health; flag infrastructure risks

### Escalation Points
- Escalate infrastructure-level incidents to Release Manager and PM immediately
- Escalate recurring pipeline instability to PM for capacity/prioritization decision

### Artifacts Owned or Influenced
- CI/CD pipeline configurations
- Infrastructure as code (IaC) repository
- Deployment runbooks and rollback procedures
- Production monitoring dashboards

---

## Support Lead

### Role Summary
The Support Lead owns the customer-facing support function, manages escalations from users, and ensures the team is prepared to support each release.

### Responsibilities
- Maintain support runbooks and knowledge base for new features
- Coordinate with Release Manager on support readiness before go-live
- Triage and escalate customer-reported issues to the appropriate team
- Track and report on support ticket volume and trends
- Participate in post-incident reviews to improve support processes

### Goals
- Reduce time-to-resolution for customer issues
- Ensure zero support surprises at release by driving readiness reviews
- Improve self-service and deflection through documentation

### Interacts With
- **Release Manager** — confirm support readiness (runbooks, escalation paths) before each release
- **Project Manager (PM)** — report on support impact of upcoming releases; flag readiness gaps
- **Developers** — escalate reproducible bugs; request hotfix prioritization
- **QA Lead** — share customer-reported defect patterns; align on regression coverage

### Escalation Points
- Escalate Severity-1 customer issues to PM and DevOps Engineer immediately
- Escalate knowledge gaps in upcoming releases to PM and Release Manager for remediation before go-live

### Artifacts Owned or Influenced
- Support runbooks
- Known issues and workarounds log
- Support readiness checklist

---

## Release Manager

### Role Summary
The Release Manager owns the end-to-end release process: change management, scheduling, go/no-go decisions, and post-release verification.

### Responsibilities
- Define and maintain the release calendar and change freeze windows
- Coordinate the go/no-go decision with PM, QA Lead, DevOps, and Support Lead
- Manage release notes and stakeholder communication for each release
- Ensure rollback plans are documented and tested
- Conduct post-release reviews and capture lessons learned

### Goals
- Execute releases with zero unplanned downtime
- Maintain a reliable, predictable release cadence
- Ensure all stakeholders are informed and prepared before every release

### Interacts With
- **Project Manager (PM)** — align release windows with project milestones; manage scope freeze
- **DevOps Engineer** — coordinate deployment steps, environment readiness, and rollback triggers
- **QA Lead** — receive QA sign-off; confirm release criteria are met
- **Support Lead** — verify support readiness and runbook availability
- **Stakeholders** — communicate release timelines, changes, and any post-release actions

### Escalation Points
- Escalate failed go/no-go criteria to PM and Sponsor for a hold or scope reduction decision
- Escalate production incidents post-release to DevOps Engineer and PM immediately

### Artifacts Owned or Influenced
- Release calendar and change log
- Release notes and announcements
- Go/no-go checklist
- Post-release review report

---

## Data Analyst

### Role Summary
Data Analysts measure product and process outcomes, surface insights from data, and support evidence-based decision-making across the team.

### Responsibilities
- Define and instrument success metrics aligned with product goals
- Build and maintain dashboards for key product and operational signals
- Conduct ad-hoc analyses to answer business questions
- Contribute data-driven insights to backlog prioritization and retrospectives
- Validate that data collection (instrumentation) is correctly implemented by Developers

### Goals
- Ensure every feature has measurable success criteria before launch
- Enable the team to make faster, more confident decisions using data
- Reduce time to insight for product and operational questions

### Interacts With
- **Product Manager (PdM)** — define success metrics for features; present findings to inform roadmap decisions
- **Developers** — review instrumentation requirements; validate that events are captured correctly
- **Project Manager (PM)** — provide metrics for status reports and retrospectives
- **QA Lead** — validate data pipeline correctness as part of QA scope

### Escalation Points
- Escalate missing or broken instrumentation to PM for prioritization as a release blocker
- Escalate conflicting or misleading data findings to PdM for interpretation and decision

### Artifacts Owned or Influenced
- Analytics dashboards
- Metrics definitions and data dictionary
- Ad-hoc analysis reports

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Cross-reference the [RACI Matrix](./role-responsibility-matrix.md) to understand accountability for each activity.
- Use the [Onboarding Checklist Template](./templates/role-onboarding-checklist.md) when a new person joins in any of these roles.

