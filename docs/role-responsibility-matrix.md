# OctoAcme Role Responsibility Matrix (RACI)

## Purpose
This matrix clarifies who is **R**esponsible, **A**ccountable, **C**onsulted, and **I**nformed for common project activities. Use it to resolve ambiguity, onboard new team members, and reduce hand-off gaps.

See also: [Roles & Personas](./octoacme-roles-and-personas.md) | [Onboarding Checklist Template](./templates/role-onboarding-checklist.md)

---

## RACI Key

| Code | Meaning |
|------|---------|
| **R** | **Responsible** — does the work |
| **A** | **Accountable** — owns the outcome; approves the result (only one per row) |
| **C** | **Consulted** — provides input before or during the activity |
| **I** | **Informed** — notified of outcome or status |

---

## RACI Matrix

| Activity | PM | PdM | Developer | Scrum Master | UX/UI Designer | SME | QA Lead | DevOps Engineer | Support Lead | Release Manager | Data Analyst | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **Project Charter** | A | C | I | I | I | C | I | I | I | I | I | C |
| **Backlog Prioritization** | C | A | C | C | C | C | C | I | C | I | C | I |
| **Sprint Planning** | I | C | R | A | C | C | C | C | I | I | I | I |
| **Acceptance Criteria Definition** | C | A | C | I | C | C | R | I | I | I | C | C |
| **UX/UI Design Review** | I | C | C | I | A | C | C | I | I | I | I | I |
| **Code Review** | I | I | A | I | I | I | C | C | I | I | I | I |
| **QA Sign-off** | C | I | C | I | I | C | A | C | I | C | I | I |
| **Release Approval (Go/No-Go)** | C | C | I | I | I | I | C | C | C | A | I | I |
| **Deployment** | I | I | C | I | I | I | I | A | I | C | I | I |
| **Incident Response** | C | I | R | I | I | I | I | A | C | C | I | I |
| **Stakeholder Communication** | A | C | I | I | I | I | I | I | C | C | I | I |
| **Retrospective Facilitation** | C | C | C | A | I | I | C | C | I | I | I | I |
| **Risk Register Maintenance** | A | C | C | C | I | C | C | C | C | C | I | I |
| **Success Metrics Definition** | C | A | C | I | C | C | C | I | I | I | R | C |

---

## How to Use This Matrix

1. **Reference before project kick-off** — confirm every activity has exactly one Accountable (A) owner. If a cell is blank, assign explicitly.
2. **Review at each phase transition** — roles may change between Initiation, Execution, and Release. Update the matrix accordingly.
3. **Use during onboarding** — share this matrix with new team members so they understand their responsibilities from day one (see [Onboarding Checklist Template](./templates/role-onboarding-checklist.md)).
4. **Resolve conflicts with RACI** — when responsibility is disputed, the Accountable owner makes the final call after consulting relevant parties.

## How to Maintain This Matrix

- The **Project Manager (PM)** owns and maintains this document.
- Review and update at the start of each major project or quarterly (whichever comes first).
- When roles change (new hires, re-orgs), update assignments and communicate via the weekly status update.
- Track significant changes in [CHANGELOG.md](./CHANGELOG.md).

---

## Abbreviations

| Abbreviation | Full Role |
|---|---|
| PM | Project Manager |
| PdM | Product Manager |
| SM | Scrum Master |
| QA | QA Lead |
| DevOps | DevOps Engineer |
| RM | Release Manager |
| DA | Data Analyst |
| SME | Subject Matter Expert |
