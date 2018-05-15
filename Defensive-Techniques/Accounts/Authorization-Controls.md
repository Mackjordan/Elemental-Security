### Authorization & Access Control
Authorization is the process of granting users and systems (subjects) access to resources (objects). An Access Control Model is a framework that dictates how subjects access objects or how objects access objects.
* Access control models are built-in to operating systems and some applications.

##### Access control models and techniques include:
###### Subject-based
* Mandatory access control (MAC)
* Discretionary access control (DAC)
* Role-based access control (RBAC)

###### Object—based
* Rule-based access controls
* Content—based access controls
* Context—based access control
* Constrained interfaces

### Subject-based Access
| Technique | Description | Enforcement |
|-----------|-------------|-------------|
| Mandatory Access Control (MAC) | Access is based on the relationship between subject clearance and need to know and the object classification level. | Security Labels |
| Discretionary Access Control (DAC) | Data owners decide subject access | Access Control Lists, Capabilities Tables |
| Role—Based Access Control (RBAC) [Non-discretionary] | Access is based on the subject’s assigned roles, Many-many relationships allowed | Capabilities Tables, Access Control Lists, Security Policy |

### Simple MAC Security Label Matrix
Access is based on the relationship between subject clearance and need to know and the object classification level.

| Object | Object Classification | Subject Clearance | Need-to-Know |
|--------|-----------------------|-------------------|--------------|
| File A | Top Secret | Top Secret | TBD |
| File B | Secret | Top Secret or Secret | TBD |   
| File C | Confidential | Top Secret, Secret or Confidential | TBD |   

### Simple DAC ACL Matrix
As owner, Bob has full control by default and can assign permissions.
| Assignment | File A Permission | File B Permission | File C Permission |
|------------|-------------------|-------------------|-------------------|
| Bob (Owner) | Full Control | Full Control | Full Control |
| Alica | Read, Write | Read Only | No Permissions |

### DAC Access Permissions
DAC file system permissions:
* User permissions are assigned to a user account
* Group permissions are assigned to each member of the group.
* Inherited permissions refer to permissions that flow from parent to child directories and files.
* Cumulative permissions are combination of all user and group assigned and inherited permissions.
* The exception is the explicit deny permission which overrules all other assigned permissions.

### Simple DAC ACL Matrix
| Assignment | File A Permission | File B Permission | File C Permission |
|------------|-------------------|-------------------|-------------------|
| Bob (Owner) | Full Control | Full Control | Full Control |
| Alica | Read, Write | Read Only | No Assignment |
| Accounting | Read Only | Read, Write, Delete | explicit Deny |

* If Bob and Alica are members of the group Accounting then cumulative permissions are:

| Cumulative | File A Permission | File B Permission | File C Permission |
|------------|-------------------|-------------------|-------------------|
| Bob (Owner) | Full Control | Full Control | Explicit Deny |
| Alica | Read, Write | Read, Write, Delete | Explicit Deny |

### Simple DAC ACL Matrix
| Role | File A Permission | File B Permission | File C Permission |
|------------|-------------------|-------------------|-------------------|
| Accounting Clerk | Read | Read, Write | No Assignment |
| Accountant | Read, Write | Read, Write | Read |
| CFO | Read, Write, Delete | Read | Full Control |

* If Bob is assigned both the accountant and CFO role then cumulative permissions are:

| Cumulative | File A Permission | File B Permission | File C Permission |
|------------|-------------------|-------------------|-------------------|
| Bob | Read, Write, Delete | Read, Write | Full Control |


### Object-based Access Controls
| Technique | Description | Enforcement |
|-----------|-------------|-------------|
| Rule-based | Access based on situational if-then statements | Rules |
| Content Dependent | Filter based on the data being acted upon | Keywords, Categories |  
| Context Dependent | Access based on a collection or sequence of actions. | Rules, Security Policy. |
| Constrained Interface. Menus and shells, Database views | Access restricted by functionality | Design, Configuration |

### ABAC (emerging)
Attribute-based access control (ABAC) is a logical access control model that controls access to objects by evaluating rules against the attributes of entities (both subject and object), operations, and the environment relevant to a request.
* ABAC supports a complex Boolean rule set that can evaluate many different attributes.
* The policies that can be implemented in an ABAC model are limited only to the degree imposed by the computational language and the richness of the available attributes.
* An example of an access control framework that is consistent with ABAC is the Extensible Access Control Markup Language (XACML).
