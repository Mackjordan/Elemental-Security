# Auditing Concepts
| Term | Determination |
|------|---------------|
| Account Auditing | Is this a valid account? |
| Membership Auditing | Are membership assignments correct? |
| Permissions Auditing | Are the explicit/inherited permissions appropriate? |
| Usage Auditing | Is user activity and resource utilization within normal boundaries?
| Authorization Creep | Authorization creep is the accumulation of access rights, permissions, and privileges over time. Promotions, lateral moves, cross-training, and temporary coverage may contribute to authorization creep. |
| Recertification | Management validates that rights and permission assignment are correct and that they adhere to internal policies and compliance requirements. Also referred to as access attestation or entitlements review. |

### User Account Management
User account management required vigilance. The following should be audited:
* Privileged accounts
* Service accounts
* User (standard) accounts and access permissions
* Group membership and permissions
* User and administrator access

### Privileged Accounts
Privileged accounts should be audited frequently for the following:
* Are any of the accounts stale?
* Should any of the account be disabled (disablement)?
* Are the assignments appropriate?
* Correct number of privileged account (too many, too few)?
* Are any of the accounts being shared?
* Is all activity being logged and monitored?

### Service Accounts
Service accounts should be audited periodically for the following:
* Is the account still required?
* Are the rights and permissions correct?

### User Accounts
User accounts should be audited periodically for the following:
* What is the last login date?
* Are any of the internal accounts stale?
* Are external accounts still required?
* Are the account settings correct?
* Should any of the accounts be disabled (disablement)?
* Are expiration dates correct?
* Is group membership correct?

### Group Accounts
Group accounts should be audited periodically following:
* Are the members appropriate?
* Are the rights and permissions correct?

### User Access & Usage
A user access review is a process that an organization implements to actively monitor and verify the appropriateness of a user’s access to applications and permissions.
* Access reviews are generally performed by the business unit.

### Ongoing Monitoring of User Activity
In the Windows environment, built-in security audit logs can be configured to capture and report on failed and successful user activity such as:
* Account login / logout
* Account lockouts
* Invalid passwords
* Password changes
* Login restriction violation
* Invalid accounts

### Ongoing Monitoring of Admin Activity
In addition to logging and monitoring user activity Administrative accounts should also be monitoring following:
* Interactive server (console) logins.
* User management activity.
* Group management activity.
* Computer management activity.
