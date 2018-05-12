# Activity and Error Reporting

### Output and Reporting
Security devices generate reports applicable to their function.
* Understanding content is important for identifying predictors and
indicators of compromise ( POC / IOC ), performance and resource
utilization, and post-incident forensics.
* Access to reports may be dependent upon system privileges.

### Host Security Technologies
| Tool | Purpose | Output |
|------|---------|--------|
| HIDS/HIPS | Host intrusion detection and prevention. | Local suspicious activity, Response taken (if HIPS) |
| Antivirus | Block malicious code, Scan for signatures | Malicious file-identified Blocked, quarantined, deleted files. |
| File Integrity Check | Identify changes in files or file Structures. | File changes including time, date and file size. |
| Firewall | Control ingress and egress traffic | Allowed and denied traffic (including Attacks) |
| DEP Data Execution Prevention | Monitors program memory use | Denied / blocked executables. |

### Enterprise Security Technologies
| Tools | Purpose | Output |
|-------|---------|--------|
| Application whitelisting | Explicitly specify allowed Application | Application access (Allowed and Denied) |
| RMC Removable Media Control | Control access to and use of Removable Media access (USB ,  CD / DVD ) | Media Access (Allowed and Denied) |
| Advanced Malware Tools | Identify malicious code that could evade or subvert anti—virus software | Suspicious or malicious files, Suspicious or malicious endpoint activity, Suspicious or malicious traffic. |
| Patch Management Tools | Inventory patches, Identify missing patches, Manage deployment. |  Patch inventory, Missing Patches, Patch deployment schedule, Patching errors. |

### Border Security Technologies
| Tools | Purpose | Output |
|-------|---------|--------|
| Unified Threat Management (UTM) | Multiple (network firewalling, network intrusion, detection/prevention (IDS/IPS), Gateway antivirus (AV), etc..)  | Depends upon what the device is being used for. |
| Data Loss Prevention (DLP) | Prevent malicious and accidental, date exfiltration. | Allowed and denied activity, Quarantined activity (queued) |
| Web Application Firewall (WAP) | Filters, monitors, inspects blocks HTTP traffic to and from web application. | Suspicious traffic and requests including SQL injection and XSS.| 
