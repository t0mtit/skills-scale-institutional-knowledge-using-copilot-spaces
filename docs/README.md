# OctoAcme Project Management Docs

This folder is the single source of truth for OctoAcme's project management processes, designed to give every team member — and our Copilot Space — fast, consistent answers about how we plan, build, and ship.

## Quick Links

- [Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risks & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)

## Team Rhythm

| Cadence | Format | Goal |
|---------|--------|------|
| Daily standup (15 min) | Delivery team | Share progress, surface blockers, flag dependencies |
| Weekly sync | PM + PdM | Review priorities, risks, and upcoming milestones |
| Sprint demo / review | End of sprint or milestone | Demonstrate working software, gather feedback |
| Monthly stakeholder update | Written or meeting | Communicate status and decisions to sponsors and stakeholders |

## Workflows & PR Expectations

- **Project board columns:** Backlog → Ready → In Progress → In Review → QA → Done
- **Small PRs:** keep pull requests to ≤ 400 lines when possible to speed up review
- **Link issues:** include the related issue number and acceptance criteria in every PR description
- **CI gates:** automated tests and linting must pass before requesting review
- **Approval policy:** at least one approval required before merging (or per team-defined policy)
- **Branching:** follow the repo's documented branching conventions

## Key Artifacts & Roles

**Artifacts**

- **Project One-pager** — problem statement, goal, success metrics, and initial timeline
- **Backlog** — prioritized list of work items with acceptance criteria and estimates
- **Risk Register** — tracks risks by ID, impact, likelihood, owner, and mitigation status
- **Release Notes** — summarizes changes, migration steps, and known issues for each release

**Core Roles**

- **Project Manager (PM)** — coordinates delivery, timelines, risks, and cross-team communication
- **Product Manager (PdM)** — defines outcomes, owns the backlog, and measures product success
- **Developers** — implement features, write tests, and participate in design and code reviews
- **QA / Testing** — validates acceptance criteria, runs smoke tests, and flags quality issues

## How to Use These Docs & Contribution Process

All process documentation lives in this `docs/` folder so that it is version-controlled and available as context for the OctoAcme Copilot Space.

**To propose an update or a new document:**

1. Open a new issue using the [Add / Update Content to Process Docs](./../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) template.
2. Fill in the affected document, a summary of the change, and the rationale.
3. Create a pull request that adds or modifies only files in `docs/`, referencing the issue in the PR description.
4. Request a review from the relevant team lead before merging.

> **Copilot Space tip:** Add this folder as a repository source in your Copilot Space so Copilot can answer questions about OctoAcme processes using these docs as grounded context.
