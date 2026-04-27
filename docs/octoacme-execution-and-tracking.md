# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

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

## Day-to-Day Activity Ownership

The table below maps recurring day-to-day activities to the role responsible for running or owning them. For full accountability detail see the [RACI Matrix](./role-responsibility-matrix.md).

| Activity | Primary Owner | Supporting Roles |
|---|---|---|
| Daily standup facilitation | Scrum Master | PM (notified of blockers) |
| Sprint planning facilitation | Scrum Master | PM, PdM, Developers, QA Lead |
| Backlog grooming / refinement | Product Manager (PdM) | Scrum Master, Developers, SME |
| CI/CD pipeline health | DevOps Engineer | Developers |
| Risk register updates | Project Manager (PM) | All roles (flag new risks) |
| Acceptance criteria authoring | Product Manager (PdM) | QA Lead, SME, UX/UI Designer |
| Code review | Developers (peers) | QA Lead (testability review) |
| QA test execution | QA Lead | Developers (test support) |
| Release scheduling & go/no-go | Release Manager | PM, QA Lead, DevOps Engineer, Support Lead |
| Stakeholder status updates | Project Manager (PM) | PdM, Release Manager |
| Post-incident review | DevOps Engineer | PM, QA Lead, Support Lead |
| Success metrics review | Data Analyst | PdM, PM |
| Retrospective facilitation | Scrum Master | PM, PdM |

## Blocker Escalation

| Level | Trigger | Owner | Action |
|---|---|---|---|
| **Level 1** | Blocker raised but expected to resolve within the sprint | Scrum Master | Triage in daily standup; track in impediment backlog |
| **Level 2** | Blocker unresolved for 2+ standups, requires cross-team action | Project Manager (PM) | Escalate to Product Lead and dependent teams; update risk register |
| **Level 3** | Business-impacting blocker (missed milestone, production incident, regulatory) | PM + Sponsor | Sponsor-level escalation; activate incident/crisis process |

**Escalation ownership by type:**
- **Technical blocker** (build, deployment, environment) → DevOps Engineer → PM (Level 2) → Sponsor (Level 3)
- **Requirement / scope conflict** → PdM → PM → Sponsor (Level 3)
- **Quality / release-blocking defect** → QA Lead → Release Manager → PM → Sponsor (Level 3)
- **Support / customer-facing incident** → Support Lead → DevOps Engineer + PM → Sponsor (Level 3)

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
