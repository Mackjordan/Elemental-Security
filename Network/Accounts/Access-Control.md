# Access control

The objective of access control is to protect information and information systems from unauthorized access (confidentiality),
modification (Integrity), and disruption (availability).

### Access Control Concepts
| Term   | Definition                                                          |
|--------|---------------------------------------------------------------------|
| Rights | Ability of a subject to take an action (e.g. install software).
| Permissions | Functions that a subject can perform on a object, file, or folder (e.g. read). |
| Privilege | Overriding capabilities; trumps rights and permissions (e.g. Root). |
| Need to know | Demonstrated reason for requiring access. |
| Least privilege | Assigning the minimal rights and permissions needed to accomplish a task. |
| Default deny | Any access or action not explicitly allowed — is forbidden. |
| Default allow | Any access or action not explicitly denied — is allowed. |
| Time / Location Restrictions | Restrictions that are based upon time of day or physical/logical location. |
| Dual control | Requiring more than one subject or key to complete a task. |
| Separation of duties | Breaking a task into segments so that no one subject is in complete control. |

### Rights
Rights generally refer to the ability of a subject to take an action; for example, the right to log on remotely, install software, and create user accounts.
* Rights can be assigned to user accounts, group accounts, or profiles depending upon the system or device.
* For example, in the MS Windows environment, local security polices and group policies are used to assign rights.

### Permissions
Permissions are functions that a subject can perform on an object, a file or a folder; for example, read, write, modify, and delete.
* Access control lists are generally used to assign permissions.
* Permissions can be assigned to user accounts, group accounts, or profiles depending upon the system or device.
* Permissions are generally cumulative.
* Permissions can be explicit or inherited.
* Permissions should be audited on a regular basis.

### Privilege
Privilege relates to overriding capabilities.
* Administrative, root, and super user.
* Privilege trumps rights and permissions.

Privileged credential theft and privileged escalation are two of
the most serious attacks.
* Pass-the-Hash is a technique in which an attacker captures hashed account credentials on one computer and reuses the credentials to authenticate to another computer.

### Need-to-Know & Least Privilege
Need-to-know means that the subject has a demonstrated and approved reason for being granted access.

Least privilege means assigning subjects only the rights and permissions needed to complete their assignment.
* Once need-to-know has been established, least privilege should be enforced.

### Default Allow and Default Deny
* Default allow means any access or action not explicitly forbidden
is allowed.
* Default deny means any access or action not explicitly allowed is
forbidden.

### Time / Location Restrictions
Time and location restrictions are generally used for control rights or access to a resource (as opposed to specific permissions).
* Time of day restrictions are used to deny/allow access as well as terminate a session.
* Location restrictions are used to deny/allow access from a specific location (e.g. IP address) or a specific device (host/NetBIOS name).

### Dual Control & Separation of Duties
* Dual control is the practice of having more than one subject or key required to complete a specific task.
* Separation of duties is the breaking down of a process into tasks that are assigned to different subjects so that no one subject is in complete control.
