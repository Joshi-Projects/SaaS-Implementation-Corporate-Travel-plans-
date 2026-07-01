# UAT Testing Checklist 🧪

## Purpose

This checklist outlines User Acceptance Testing requirements for ABC GmbH’s corporate travel booking SaaS implementation.

The goal is to confirm that user access, travel policy rules, approval workflows, reporting requirements, and key onboarding scenarios work as expected before go-live.

## What UAT Means

User Acceptance Testing helps confirm that the platform setup meets the client’s business requirements before launch.

In this project, UAT focuses on whether ABC GmbH’s employees, managers, Finance users, and admins can complete their expected tasks correctly.

## UAT Scope

The following areas are included in testing:

* User login and role access
* Travel booking flow
* Travel policy rules
* Approval workflow
* Cost center and reporting fields
* Employee data accuracy
* Finance reporting output
* Training and support readiness

## Test Scenarios

| Test ID | Test Scenario                            | Expected Result                                  | Owner                  | Status  |
| ------- | ---------------------------------------- | ------------------------------------------------ | ---------------------- | ------- |
| UAT-001 | Employee logs in successfully            | Employee can access platform                     | IT Contact             | Planned |
| UAT-002 | Manager logs in successfully             | Manager can access approval view                 | IT Contact             | Planned |
| UAT-003 | Finance user logs in successfully        | Finance can access reporting view                | IT Contact             | Planned |
| UAT-004 | Employee books hotel under Germany limit | Booking is auto-approved                         | Implementation Manager | Planned |
| UAT-005 | Employee books hotel above Germany limit | Booking is routed to manager approval            | Implementation Manager | Planned |
| UAT-006 | Employee books flight under €500         | Booking is auto-approved                         | Implementation Manager | Planned |
| UAT-007 | Employee books flight above €500         | Booking is routed to manager approval            | Implementation Manager | Planned |
| UAT-008 | Business class booking request           | Booking requires senior leadership approval      | Implementation Manager | Planned |
| UAT-009 | Booking includes cost center             | Cost center is captured successfully             | Finance Manager        | Planned |
| UAT-010 | Monthly travel spend report generated    | Report shows spend by department and cost center | Finance Manager        | Planned |
| UAT-011 | Approval reminder after delay            | Pending approval reminder is triggered           | Operations Lead        | Planned |
| UAT-012 | Out-of-policy warning shown              | Employee sees policy warning before submission   | Implementation Manager | Planned |

## Acceptance Criteria

UAT is considered successful when:

* Employees can access the platform
* Managers can review approval requests
* Finance can access required reporting fields
* Travel policy rules behave as expected
* Out-of-policy bookings trigger approval
* Cost center data is captured correctly
* Critical issues are resolved before go-live
* Client stakeholders confirm readiness

## Issue Handling During UAT

If a test fails:

1. Log the issue in the issue log.
2. Assign an owner.
3. Define priority.
4. Document expected vs. actual result.
5. Track next action.
6. Retest after resolution.

## UAT Sign-Off Requirements

Before go-live, the following stakeholders should confirm readiness:

* Implementation Manager
* Project Sponsor
* Finance Manager
* HR Manager
* IT Contact
* Operations Lead

## Implementation Value

A structured UAT checklist helps reduce go-live risk, improve customer confidence, and ensure the platform setup reflects the client’s agreed requirements.
