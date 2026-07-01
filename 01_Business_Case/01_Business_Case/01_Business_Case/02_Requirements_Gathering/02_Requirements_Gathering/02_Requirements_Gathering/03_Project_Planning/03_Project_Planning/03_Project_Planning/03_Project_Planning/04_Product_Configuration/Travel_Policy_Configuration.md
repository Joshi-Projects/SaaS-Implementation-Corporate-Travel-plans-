# Travel Policy Configuration ⚙️

## Purpose

This document outlines the travel policy configuration requirements for ABC GmbH’s corporate travel booking SaaS platform.

The goal is to translate ABC GmbH’s business travel rules into clear platform configuration requirements that support policy compliance, cost control, approval visibility, and consistent employee booking behavior.

## Configuration Context

ABC GmbH wants employees to book business travel through one centralized platform. The platform should guide users toward compliant booking options and trigger approvals when bookings exceed defined policy limits.

## Hotel Policy Rules

| Rule ID | Policy Rule                         | Configuration Requirement                  | Approval Logic            |
| ------- | ----------------------------------- | ------------------------------------------ | ------------------------- |
| H-001   | Germany hotel limit: €400 per night | Flag hotel bookings above €400             | Manager approval required |
| H-002   | Spain hotel limit: €350 per night   | Flag hotel bookings above €350             | Manager approval required |
| H-003   | Out-of-policy hotel booking         | Display policy warning before confirmation | Route to manager approval |
| H-004   | Hotel booking under country limit   | Allow booking without additional approval  | Auto-approved             |

## Flight Policy Rules

| Rule ID | Policy Rule           | Configuration Requirement                          | Approval Logic                      |
| ------- | --------------------- | -------------------------------------------------- | ----------------------------------- |
| F-001   | Flights up to €500    | Allow booking within policy                        | Auto-approved                       |
| F-002   | Flights above €500    | Flag as out-of-policy                              | Manager approval required           |
| F-003   | Economy class travel  | Economy class enabled as default booking option    | Auto-approved if within price limit |
| F-004   | Business class travel | Business class requires senior leadership approval | Senior leadership approval required |

## Rental Car Policy Rules

| Rule ID | Policy Rule                                      | Configuration Requirement                    | Approval Logic                   |
| ------- | ------------------------------------------------ | -------------------------------------------- | -------------------------------- |
| R-001   | Rental cars allowed for approved business travel | Enable rental car booking for business trips | Manager approval may be required |
| R-002   | Economy or compact category preferred            | Display preferred rental category guidance   | Auto-approved if within policy   |
| R-003   | Premium rental category                          | Flag premium rental option                   | Manager approval required        |

## Cost Center Requirements

Every booking should include:

* Employee name
* Department
* Cost center
* Country
* Manager
* Travel purpose
* Booking type
* Booking value

## User Experience Requirements

The platform should:

* Clearly show whether a booking is within policy
* Display warnings for out-of-policy bookings
* Route bookings for approval when required
* Allow employees to understand why approval is needed
* Support managers in reviewing approval requests quickly
* Provide Finance with reliable cost center data

## Business Value

This configuration supports ABC GmbH by:

* Reducing manual approval follow-up
* Improving travel policy compliance
* Supporting cost control
* Increasing visibility for Finance
* Creating a more consistent employee booking experience
* Improving reporting quality by department and cost center

## Implementation Notes

* All high-priority policy rules must be confirmed before configuration.
* Out-of-policy booking logic should be tested during UAT.
* Finance and Operations stakeholders should validate approval rules before go-live.
* Any late policy changes should be documented as a configuration change.
