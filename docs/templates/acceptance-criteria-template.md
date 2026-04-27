# Acceptance Criteria Template

Use this template when writing acceptance criteria for a user story or feature. Acceptance criteria must be agreed upon by the Product Manager (PdM) and QA Lead before a story enters a sprint.

See also: [Roles & Personas](../octoacme-roles-and-personas.md) | [RACI Matrix](../role-responsibility-matrix.md)

---

## Story Reference

| Field | Value |
|---|---|
| **Story / Issue** | _(link to GitHub issue or backlog item)_ |
| **Feature / Epic** | _(feature or epic name)_ |
| **Author** | _(Product Manager name)_ |
| **Reviewed by** | _(QA Lead name, SME name if applicable)_ |
| **Sprint / Milestone** | _(sprint name or milestone)_ |

---

## User Story

> **As a** _(role / user type)_,  
> **I want to** _(action / capability)_,  
> **So that** _(benefit / outcome)_.

**Example:**
> As a **project manager**, I want to view a consolidated risk register dashboard, so that I can quickly identify high-priority risks and take action without reading multiple documents.

---

## Acceptance Criteria

Write each criterion in **Given / When / Then** format, or as a clear bullet condition. All criteria must be verifiable and testable.

### Format A: Given / When / Then (recommended for user-facing behavior)

```
Given <some initial context or precondition>,
When <an action is taken>,
Then <an expected outcome is observable>.
```

**Example 1:**
```
Given I am logged in as a Project Manager,
When I navigate to the Risk Register dashboard,
Then I see a list of all open risks sorted by priority (High → Medium → Low).
```

**Example 2:**
```
Given a risk item has a status of "High",
When I view the risk register,
Then the risk row is highlighted in red and displays the assigned owner name.
```

**Example 3:**
```
Given I am on the Risk Register dashboard,
When I click "Export",
Then a CSV file is downloaded containing all visible risk rows with columns: ID, Title, Status, Priority, Owner, Last Updated.
```

### Format B: Bullet Conditions (for non-behavioral or constraint-based criteria)

- [ ] The feature is accessible to users with the `project-manager` role only.
- [ ] The dashboard loads within 2 seconds on a standard broadband connection.
- [ ] The feature is accessible (WCAG 2.1 AA compliant).
- [ ] All API responses return appropriate HTTP status codes (200, 400, 404, 500).
- [ ] No Personally Identifiable Information (PII) is logged.

---

## Edge Cases & Negative Scenarios

Document how the system should behave when things go wrong or inputs are unexpected.

| Scenario | Expected Behavior |
|---|---|
| _(e.g., Risk register is empty)_ | _(e.g., Display "No risks found. Add a risk to get started." message)_ |
| _(e.g., User does not have the required role)_ | _(e.g., Redirect to 403 error page with a "Request Access" link)_ |
| _(e.g., Export fails due to server error)_ | _(e.g., Display error toast; do not partially download the file)_ |

---

## Definition of Done (DoD) Checklist

All items below must be completed before a story is considered **Done**. The QA Lead confirms DoD compliance before marking the story closed.

### Code Quality
- [ ] Code is reviewed and approved by at least one Developer peer
- [ ] All automated tests pass in CI (unit, integration, e2e as applicable)
- [ ] No new linting or static analysis errors introduced
- [ ] Code is merged to the main branch

### Testing
- [ ] Acceptance criteria verified by QA Lead against the test plan
- [ ] Happy-path scenarios tested and passing
- [ ] Edge cases and negative scenarios tested
- [ ] Regression tests updated or added as needed
- [ ] Accessibility checks completed (if UI is involved)

### Documentation
- [ ] PR description references the issue and summarizes the change
- [ ] Inline code comments added for complex logic
- [ ] Any new user-facing behavior documented in release notes or user guides
- [ ] Runbook updated if operational behavior changed (relevant for DevOps / Support)

### Design & UX (if applicable)
- [ ] Implementation reviewed against design specs by UX/UI Designer
- [ ] Any approved design deviations documented

### Domain Sign-Off (if applicable)
- [ ] SME has reviewed domain-specific logic for correctness

### Release Readiness
- [ ] Feature flag or rollout strategy confirmed (if applicable)
- [ ] Monitoring / alerting configured for new behavior
- [ ] Support team notified and runbook updated (if applicable)

---

## Approvals

| Role | Name | Approved | Date |
|---|---|---|---|
| Product Manager | _(name)_ | ☐ | _(date)_ |
| QA Lead | _(name)_ | ☐ | _(date)_ |
| SME (if applicable) | _(name)_ | ☐ | _(date)_ |
