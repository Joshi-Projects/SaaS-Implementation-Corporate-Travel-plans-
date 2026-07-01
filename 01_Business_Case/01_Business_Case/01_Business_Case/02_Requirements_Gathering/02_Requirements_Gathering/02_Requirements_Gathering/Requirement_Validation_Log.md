# Requirement Validation Log 🔍

## Purpose

This log tracks how client requirements are reviewed, validated, and confirmed before product configuration begins.

The goal is to reduce misunderstandings, avoid rework, and ensure that each requirement has a clear owner, decision status, and next step.

## Validation Log

| Requirement ID | Requirement                                                | Validated By                 | Status    | Notes / Decision                                                |
| -------------- | ---------------------------------------------------------- | ---------------------------- | --------- | --------------------------------------------------------------- |
| REQ-001        | Platform access for 500 employees across Germany and Spain | HR Manager                   | Confirmed | Initial rollout includes all active employees in both countries |
| REQ-002        | Employee, manager, admin, and Finance user roles           | HR Manager / Finance Manager | Confirmed | Role-based access required before go-live                       |
| REQ-003        | Hotel limit of €400 per night for Germany                  | Finance Manager              | Confirmed | Bookings above limit require manager approval                   |
| REQ-004        | Hotel limit of €350 per night for Spain                    | Finance Manager              | Confirmed | Country-specific rule required                                  |
| REQ-005        | Flights above €500 require manager approval                | Finance Manager              | Confirmed | Approval workflow required                                      |
| REQ-006        | Business class requires senior leadership approval         | Finance Manager              | Confirmed | Applies to all employees unless exception is approved           |
| REQ-007        | Department managers approve out-of-policy bookings         | Operations Lead              | Confirmed | Approval routing depends on employee department                 |
| REQ-008        | Delayed approvals escalated after 48 hours                 | Operations Lead              | Open      | Escalation owner still needs confirmation                       |
| REQ-009        | Every booking must include department and cost center      | Finance Manager              | Confirmed | Required for monthly reporting                                  |
| REQ-010        | Monthly travel spend report by department                  | Finance Manager              | Confirmed | Required after go-live                                          |
| REQ-011        | Monthly travel spend report by country                     | Finance Manager              | Open      | Reporting format still needs confirmation                       |
| REQ-012        | SSO login using company Microsoft account                  | IT Contact                   | In Review | Technical feasibility review required                           |
| REQ-013        | HR employee data import                                    | HR Manager / IT Contact      | In Review | Required fields need technical validation                       |
| REQ-014        | Finance reporting export                                   | Finance Manager              | Open      | Export format and frequency still need confirmation             |
| REQ-015        | Admin, manager, and employee training                      | Implementation Manager       | Planned   | Training plan to be prepared before UAT                         |
| REQ-016        | Go-live checklist                                          | Implementation Manager       | Planned   | Required before launch approval                                 |
| REQ-017        | Handover document for Account Manager                      | Implementation Manager       | Planned   | Prepared after go-live readiness review                         |

## Validation Rules

* No high-priority requirement should move to configuration until the responsible stakeholder has confirmed it.
* Open requirements must be reviewed during weekly implementation status meetings.
* Any change to confirmed requirements should be documented as a scope or configuration change.
* Technical requirements should be reviewed with the technical or integration team before testing.

## Implementation Notes

This validation log helps the Implementation Manager keep client expectations, project scope, and configuration requirements aligned throughout the onboarding lifecycle.
