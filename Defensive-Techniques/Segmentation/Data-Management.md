# Data Management
Data management is defined as the planning and execution of policies and practices that protect data throughout its lifecycle.

### Key U.S. Data Protection Regulations
| Regulation / Law  | Focus  |
|-------------------|--------|
| GLBA(U.S.) | Financial records |
| HIPAA (U.S.) | Medical records |
| FERPA (U.S.) | Student educational records |
| MA 201 CMR 17 | Standards for the Protection of Personal Information of Residents of the Commonwealth (2010) |
| State | 31 states and Puerto Rico have enacted laws that require entities upon end of life to destroy, dispose, or otherwise make personal information unreadable or undecipherable. |
| State | 47 states, the District of Columbia, Guam, Puerto Rico and the Virgin Islands have enacted data breach notification laws. |

### Data Management Ecosystem
Level 1
>    | Data Users

Level 2
>    || Data Custodians

Level 3
>    ||| Data Owners

Level 4
>    |||| Directors & Executive Management


### Roles and Responsibilities

| Role  |  Responsibility  |
|-------|------------------|
| Directors & Executive management | Responsible for governance and oversight. From a legal and regulatory perspective, they are ultimately responsible for the actions (or inaction) of the organization. |
| Privacy Officer | Responsible for identification of and ensuring compliance with applicable organizational, regulatory, and contractual requirements.|
| Data Owners, Data Stewards | Responsible for decisions related to classification, access control, and protection. |
| Data Custodians | Responsible for implementing, managing, and monitoring controls. |
| Data Users | Responsible for treating data and interacting with information systems in accordance with organizational policy and standards. |

### Information Classification Policy
A Data Classification Policy codifies the requirements for classifying and protecting an organizations data. The policy should also define the classification framework.
* Handling standards inform custodians and users how to treat the information they use and systems they interact with.
* Data should be labeled so that users recognize the classification and can apply the appropriate handling standard.

### Classification Frameworks
* Government / Military (Subject to variation) - Based on disclosure.

| Classification    | Description       |
|-------------------|-------------------|
| Top Secret (TS) | Cause exceptionally grave danger to national security. |
| Secret (S) | Cause serious damage to national security. |
| Confidential | Cause damage to national security. |
| Unclassified | No threat to national security |

### Classification Frameworks
* Private Sector (Examples only - subject to Variation.)

| Classification    | Description       |
|-------------------|-------------------|
| Protected | Protection required by regulation or contractual obligation (e.g. PI, PHI) |
| Proprietary | Intellectual property or process; significant impact if disclosed. |
| Public | Available for distribution.  |

### Handling Standards Example
| Standard | Protected | Proprietary | Confidential | Public |
|----------|-----------|-----------|-------------|--------------|--------|
| Data Storage Mobile Devices | Not allowed | Allowed Encryption required | Allowed Encryption highly recommend | Allowed in plain text |
| External File Transfer | Must be pre-authorized by a SVP Encryption required. | Must be pre-authorized by a SVP Encryption required. | Allowed Encryption highly recommended | Allowed in plain text |
| Electronic Disposal / Destruction | Must be irrevocably destroyed. Destruction certification required. | Must be irrevocably destroyed. | Recommended irrevocable destruction. | Overwritten |

# Data Retention & Destruction

### Information Life cycle
1. Collection
2. Use or Retention Archiving
3. Deletion Destruction or possible legal hold.

### Retention and Archiving
* Retention is a protocol (set of rules) within an organization that dictates types of unaltered data that must be kept and for how long.
* Legal and regulatory requirement must be considered.
* Archiving is the process of securely storing unaltered data for later potential retrieval.
* Backup and replication is the process of making copies of data to ensure recoverability. They are distinct processes.

### Legal Hold
A legal hold is the requirement for a organization to preserve all forms of relevant information when litigation, audit, or government investigation is reasonably anticipated. The objective is to avoid evidence spoliation.
* A legal hold supersedes organizational retention policies.

### Data Deletion Warning
Operating system data deletion doesn’t actually remove a file. When a file is deleted, the corresponding entry in the Master File Table (MFT) is cleared and the MFT entry is marked as ready to be re-used.
* The original file remains intact until the space is used and the original file is overwritten.
* Potentially all or part of the deleted file and/or MFT entry can be recovered (data remanence).

### Data Remanence
Data remanence is the residual representation of digital data that remains even after attempts have been made to remove or erase the data. Techniques to counter data remanence include:
* Clearing which is the removal of data is such a way that data cannot be recovered using normal system functions or recovery utilities.
* Purging/sanitizing which is the removal of data that cannot be reconstructed by any known technique.
* Destruction which is the physical act of destroying media in such as way that it cannot be reconstructed.

### Anti-Remanence Techniques
| Technique | Description                    | Result                             |  
|-----------|--------------------------------|------------------------------------|
| Wiping | Overwrites all addressable storage and indexing locations multiple times | Clearing |
| Degaussing | Using a electromagnetic field to destroy all magnetically recorded data | Purging |
| Crypto-shredding | Encrypting remaining data | Purging |
| Shredding | Physically breaking media into pieces | Destruction |
| Pulverizing | Reducing media to dust | Destruction |
| Pulping | Chemical altering media | Destruction |
| Burning | Incinerating media  | Destruction |
