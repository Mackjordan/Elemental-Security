# Account Types Overview
| Account type |         Description                                          |
|--------------|--------------------------------------------------------------|
| Default | Accounts that are created by the operating system or application. |
| Privileged | Accounts that have powerful rights and permissions (”keys to the kingdom”) |
| User / Group | Accounts designed to be used for normal tasks. |
| Guest | Account with very limited resource access. |
| Service | Accounts used by services and applications. |
| Shared / Generic | Accounts used by multiple users or services. |

### Default Accounts
Three types of default accounts:
* Predefined accounts are users and group installed with the OS or application (e.g. Administrator, Guest).
* Built-in accounts are special use accounts (e.g. LocalSystem).
* Implicit accounts are created implicitly when network resources are accessed. These are also known as special identities (e.g. Everyone, Authenticated User). Default accounts can be modified but rarely can they be deleted.
* Consideration should be given to renaming and/or disabling predefined accounts (e.g. Administrator)

### Privileged Accounts
Privileged accounts are those which powerful rights and permissions have been granted (e.g. Admin, Root).
* Security policy should dictate who can authorize the assignment of privileged accounts.
* Privileged accounts should not be shared.
* Privileged accounts should be used only for required functions.
* Privileged account activity should be monitored.
* In Windows, the three built-in highest privileged groups are: ( Enterprise Admins, Domain Admins & Administrators. )
* Privileged account names should not reflect their level of access (e.g. Admin-John).

### User / Group Accounts
User accounts (also known as standard accounts) are accounts used for normal everyday tasks.
* User accounts can be unique and assigned to a specific individual (e.g. John).
* User accounts can be shared and used by multiple users. (No-accountability).
* User accounts can be generic and used for a specific task for example, Teller (No-accountability).

Group accounts are designed to streamline and simplify account administration.
* User accounts can be members of multiple groups.

### Windows User Account Control (UAC)
Windows UAC can be configured so that apps and tasks always run in the security context of a non—administrator account, unless an administrator specifically authorizes administrator-level access to the system.

### Guest User
Guest accounts are used for limited resource access (e.g. web browsing).
* The guest account is disabled by default in Windows. If the account is required, it should be renamed.
* MAC OS X, Ubuntu, and Chrome automatically delete guest user files upon log out.

### Service Account
A service account is a type of user account that is created explicitly to provide a security context for a service or application.
##### Service accounts should be unique.
* Reduces the impact in case of a incident with a service. (compartmentalization)
* Easier to track down associated resources.

Default service account should ALWAYS be renamed unless hard coded in the application/utility.
