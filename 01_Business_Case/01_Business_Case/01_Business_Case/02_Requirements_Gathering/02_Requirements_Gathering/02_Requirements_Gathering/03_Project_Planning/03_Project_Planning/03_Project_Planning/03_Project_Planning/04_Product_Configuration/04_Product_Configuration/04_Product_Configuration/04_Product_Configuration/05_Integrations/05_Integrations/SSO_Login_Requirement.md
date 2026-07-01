# SSO Login Requirement 🔐

## Purpose

This document defines the Single Sign-On login requirement for ABC GmbH’s corporate travel booking SaaS platform.

The goal is to allow employees to access the travel platform using their existing company login, reducing password-related issues and improving the user experience during onboarding and after go-live.

## Business Requirement

ABC GmbH wants employees to log in to the travel platform using their company Microsoft account instead of creating a separate username and password.

## What SSO Means

Single Sign-On allows employees to use one company login to access multiple business applications.

For this implementation, the expected user experience is:

Employee opens the travel platform → Employee selects company login → Employee signs in with Microsoft account → Platform grants access based on assigned user role.

## Business Value

SSO supports ABC GmbH by:

* Reducing password-related support tickets
* Improving employee login experience
* Supporting secure access management
* Making onboarding smoother for 500 employees
* Reducing manual account administration
* Helping users access the platform faster after go-live

## User Groups in Scope

| User Group            | SSO Required    | Notes                          |
| --------------------- | --------------- | ------------------------------ |
| Employees             | Yes             | Standard travel booking access |
| Department Managers   | Yes             | Approval access required       |
| Finance Users         | Yes             | Reporting access required      |
| HR Users              | Yes             | User data support access       |
| Travel Administrators | Yes             | Admin access required          |
| External contractors  | To be confirmed | Scope still open               |

## Key Data Needed

To support SSO readiness, the following information should be confirmed:

* Identity provider, such as Microsoft Entra ID / Azure AD
* User email domain
* User role mapping
* Employee access scope
* Admin users
* Fallback login process
* Client-side IT contact
* Testing timeline

## Open Questions

* Which Microsoft identity setup does ABC GmbH use?
* Are all 500 employees included in SSO at go-live?
* Are external contractors included?
* Who approves SSO configuration from the client side?
* What is the fallback plan if SSO testing is delayed?
* Should access be restricted by country, department, or role?
* Who will test SSO before go-live?

## Testing Scenarios

SSO should be tested for:

* Standard employee login
* Manager login
* Finance user login
* Admin user login
* Incorrect access attempt
* Deactivated employee access
* Role-based access after login

## Risks

| Risk                        | Impact                            | Mitigation                               |
| --------------------------- | --------------------------------- | ---------------------------------------- |
| SSO setup delayed           | Go-live may be delayed            | Schedule technical review early          |
| Incorrect user role mapping | Users may receive wrong access    | Validate role mapping before testing     |
| Employee data mismatch      | Login may fail for some users     | Validate email and HR data before import |
| No fallback process         | Users may be blocked if SSO fails | Define temporary access process          |

## Implementation Manager Responsibilities

The Implementation Manager is responsible for:

* Capturing the SSO requirement from the client
* Documenting business needs and open questions
* Coordinating with client-side IT and internal technical teams
* Tracking SSO-related risks and blockers
* Ensuring SSO testing is included in UAT
* Confirming readiness before go-live

## Important Note

This document captures the business and implementation requirement for SSO. Technical configuration, security validation, and final setup should be handled by the relevant technical team.
