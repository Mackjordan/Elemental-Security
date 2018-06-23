# Troubleshooting Security Issues
As a security practitioners, it is important to be aware of ”common security issues," how to identify the issue, how to
troubleshoot the issue, and the path to resolution.
* A root cause analysis (RCA) is a method of problem solving used for identifying the root causes of faults or problems.


### Root Cause Analysis (5 Whys)
Often most security issues can be diagnosed by asking why and digging into the issue deeper. Figuring out why something happened, then asking why that happened and so on 5 layers deep should help to unmask the underline issue that allowed the issue to happen.

### 12 Common Security Issues
| # | Issues |
|---|--------|  
| 1. | Unencrypted credentials/ clear text |
| 2. | Log and event anomalies |
| 3. | Permissions issues |
| 4. | Access violations |
| 5. | Data exfiltration |
| 6. | Misconfigured devices (e.g. firewall, content filter, access points) |
| 7. | Weak security configurations |
| 8. | Unauthorized software |
| 9. | Baseline deviations |
| 10. | License compliance violation |
| 11. | Asset management |
| 12. | Authentication issues |

### Unencrypted Credentials
Issue:
* Unencrypted credentials / clear text

Impact:
* Captured credentials = unauthorized access

Cause(s):  
* Insecure protocols being used (e.g. FTP instead of SFTP)
* Passwords are being stored insecurely (local spreadsheet, application)
* Passwords are being included in unencrypted communications

Troubleshooting:
* Talk to the user/application owner
* Sniff traffic
* Review logs and DLP alerts (if applicable)
* Review configuration settings
* Configuration and compliance scanning

### Log and Event Anomalies

Issues:
* issue Log and event anomalies

Impact:
* Variable depending upon the issue

Cause(s):
* Variable depending upon the issue

Troubleshooting:
* Log analysis (manual, SIEM, outsourced)
* Tracing issue back to the source (importance of accountability)
* Ensure that log settings are correct and eliminate false positives


### Permissions Violations
Issue:
* Unauthorized access

Impact:
* Violation of confidentiality
* Potential Violation of integrity is unauthorized changes were made.

Cause(s):
* Access control misconfiguration
* User error
* User malicious intent
* Authorizations creep: Users move to a different role and keep the same permissions.

Troubleshooting:
* Talk to the user/talk to the owner
* Review access reports
* Review access control lists
* Review group membership
* Review logs and SIEM reports


### Data Exfiltration

Issue:
* Inadvertent or intentional data ex-filtration.

Impact:
* Authorization disclosure
* Regulatory and/or policy compliance Violation

Cause(s):
* Incorrect labeling or classification
* User error (didn’t know not to share)
* Malicious activity
* Accidental (e.g. included in documents, code, etc.)

Troubleshooting:
* Log analysis
* Packet analysis
* DLP alerts
* Review data classification controls
* Talk to the user


### Misconfigured Devices
Issue:
* Misconfigured devices including firewalls, content filters, and access points

Impact:
* Unauthorized access, denial of service, device integrity (administration)

Cause(s):
* Default setting
* No change control
* Lack of standards/ guidance

Troubleshooting:
* Talk to the custodian
* Port scanning / Vulnerability scanning
* Configuration and compliance scanning

### Weak Security Configuration
Issue:
* Weak security configuration

Impact:
* Unauthorized access, denial of service, device integrity (administration)

Cause(s):
* Default setting
* No change control
* Lack of standards/guidance

Troubleshooting:
* Discuss with internal personnel
* Port scanning
* Vulnerability scanning
* Configuration and compliance scanning


### Unauthorized Software
Issue:
* Installed software that has not been approved or authorized

Impact:
* Introduction of malware
* Bandwidth utilization
* Compatibility issues
* Maintenance issues (vulnerability management)
* License violations

Cause(s):
* Lack of centralized control
* Local administrative privileges
* Lack of standards / guidance

Troubleshooting:
* Port scanning
* Vulnerability scanning
* Asset inventory (audit)

### Baseline Deviation
Issue:
* Non-standard configuration settings

Impact:
* Incompatibility
* Security settings not enforced
* Unauthorized access, denial of service, device integrity (administration)

Cause(s):
* Poor configuration management
* Lack of standards
* No technical enforcement

Troubleshooting:
* Discuss with internal personnel
* Port scanning
* Vulnerability scanning
* Configuration and compliance scanning
* Audit

### License compliance Violations
Issue:
* Unlicensed software

Impact:
* Availability
* Fines and penalties
* Reputation damage

Cause(s):
* Lack of asset management
* Server/desktop sprawl
* Willful Violation
* Piracy

Troubleshooting:
* Software audit www.bsa.org


### Asset management
Issue:
* Unmanaged assets

Impact:  
* Loss, theft, no lifecycle management, introduction of vulnerable devices

Cause(s):
* Insufficient asset management

Troubleshooting:
* Network mapping
* Asset inventory (Requires coordination between departments e.g. physical security, IT, HR and accounting)

Authentication Issues
Issue:
* Users can’t log in.

Impact:
* Denial of service

Cause(s):
* Disabled accounts
* Expired passwords
* User error
* Revoked or expired tokens or cards
* Biometric false positives

Troubleshooting:
* Ensure the user is providing the correct credentials
* Ensure that multi-factor components are working correctly
* Review account settings
* Review logs

### 5 Common Personnel Security Issues
1. Policy Violation
2. Insider threat
3. Social engineering
4. Social media
5. Personal email

### Policy Violation
Issue:
* Policy violation

Impact:
* Depends upon the violation

Cause(s):
* Lack of awareness and/or understanding
* Accidental/ inadvertent
* Policy impediment

Response:
* Talk to the user
* Training
* Technical controls or configuration adjustment
* Sanctions

### Insider Threat
Issue:
* Insider threat (employee, trusted partner, imposter)

Impact:
* Significant

Casue(s):
* Anger / disconnect
* Financial pressure
* Extortion
* Sabotage
* Malicious intent

Response:
* Organizational awareness (”trust but verify”)
* Incident reporting encouragement
* Defense in depth preventive, deterrent, and detective controls

### Social Engineering
Issue:
* Vulnerable to a social engineering attack

Impact:
* Significant

Cause(s):
* Lack of awareness or understanding susceptibility

Response:
* Training and awareness programs
* Social engineering vulnerability assessments
* Defense in depth preventive, deterrent and detective controls

### Social Media
* Unauthorized or damaging social media posts
* Use of social media from inside the network

Impact
* Confidentiality violations
* Reputational damage
* Malware distribution

Cause(s):
* Lack of awareness or understanding
* Not having a social media policy
* Allowing access to social media sites

Response:
* Social media policy
* User training and awareness
* Technical controls restricting access
* Or if allowed, enhanced malware controls (perhaps sandboxing)

### Personal Email

Issue
* Use of personal email

Impact:
* Confidentiality violation
* Malware distribution
* Evades archiving
* SPAM

Cause(s):
* Lack of awareness or understanding
* Not having an email policy
* Allowing access to personal email sites (e.g. Gmail)

Response:

* Or if allowed, extending email-related controls to approved sites.
* Personal email policy (component of Acceptable Use)
* Technical controls restricting access.
* User training and awareness
