# User Roles and Access 👤🔐

## Purpose

This document defines the user roles and access requirements for ABC GmbH’s corporate travel booking SaaS platform.

The goal is to ensure that each user group has the correct access level, responsibilities, and visibility within the platform before go-live.

## User Role Overview

| User Role            | Main Purpose                                         | Access Level                       |
| -------------------- | ---------------------------------------------------- | ---------------------------------- |
| Employee             | Book business travel within company policy           | Standard user access               |
| Department Manager   | Review and approve out-of-policy bookings            | Approval access                    |
| Travel Administrator | Manage travel settings and support users             | Admin access                       |
| Finance User         | Review travel spend, cost centers, and reporting     | Reporting access                   |
| HR User              | Support employee data and user access updates        | User data access                   |
| Senior Leader        | Approve exceptional bookings such as business class  | Senior approval access             |
| Account Manager      | Manage long-term customer relationship after go-live | Post-implementation access/context |
| Customer Support     | Support user issues after launch                     | Support access/context             |

## Employee Access

Employees should be able to:

* Search and book flights, hotels, and rental cars
* View company travel policy rules
* Submit bookings for approval when required
* Add travel purpose and cost center information
* Receive booking and approval status updates
* Access user guidance or FAQ material

## Department Manager Access

Department Managers should be able to:

* View approval requests from team members
* Approve or reject out-of-policy bookings
* See booking value and policy limit comparison
* Review travel purpose and cost center
* Receive reminders for pending approval requests

## Travel Administrator Access

Travel Administrators should be able to:

* Support user questions
* Review basic platform settings
* Support employee access issues
* Coordinate with Account Management or Support after go-live
* Escalate configuration or policy questions when needed

## Finance User Access

Finance users should be able to:

* View travel spend by department
* Review cost center data
* Access monthly travel reports
* Check booking value and travel policy compliance
* Support invoice and reporting follow-up

## HR User Access

HR users should be able to:

* Provide employee data for user setup
* Confirm manager relationships
* Confirm departments and cost centers
* Support employee changes after go-live

## Senior Leader Access

Senior Leaders should be able to:

* Review exceptional booking requests
* Approve business class or high-value travel exceptions
* Receive escalation notifications when required

## Access Requirements

Each user profile should include:

* Full name
* Company email
* Country
* Department
* Cost center
* Manager
* User role
* Access status

## Access Control Considerations

* Employees should only see their own bookings.
* Managers should only approve bookings for their assigned teams.
* Finance users should access reporting data but not change travel policies without approval.
* Travel administrators should support operational platform use but should not approve financial policy changes independently.
* Senior approval access should be limited to selected leadership roles.

## Business Value

Clear user roles and access support ABC GmbH by:

* Reducing access-related confusion
* Improving approval routing accuracy
* Supporting secure platform use
* Improving reporting reliability
* Helping employees understand what they can do in the system
* Supporting a smoother go-live process

## Implementation Notes

* User roles should be confirmed before access setup.
* HR should validate employee data before user upload.
* Finance should validate cost center mapping before go-live.
* Approval routing should be tested during UAT.
* Final user role assumptions should be included in the handover document.
