# Vulnerability
A vulnerability is defined as a hardware or software weakness that can be exploited.
Common examples of vulnerabilities include:
* Unpatched operating systems and applications
* Broken versions.
* Weak Ciphers
* Improper input/output handling
* Poor coding.

### Exposure
An exposure is a system or software configuration issue or lack of a control that could contribute to a successful exploit or compromise:
Common examples of exposures include:
* Default Settings
* Running unnecessary services that are common attack points (HTTP, FTP, SMTP)
* Weak Passwords
* End of life applications and devices.
* System Sprawl (Too many devices that have become unmanaged. )

### Common Vulnerabilities & Exposures
The Common Vulnerabilities and Exposures (CVE) list is a database of information security vulnerabilities and exposures.
* The CVE Provides a standardized identifier for a given vulnerability or exposure.
* https://cve.mitre.org

### CVE Identifier
| Component | Description | Example |
|-----------|-------------|---------|
| Number | CVE identifier number with four or more digits in the sequence number portion of the ID. | CVE-2017-3074 |
| Description | Brief description of the security vulnerability or exposures | Adobe Flash PLayer versions 25.0.0.148 and earlier have an exploitable memory corruption vulnerability in the Graphics class. Successful exploitation could lead to arbitrary code execution.|
| References | Any pertinent references (i.e vulnerability reports and advisories. | Confirm: https://helpx.adobe.com/security/products/flash-player/apsb17-15.html |

### Vulnerability Research

Identification of code flaws in protocols, operating systems, utilities, applications, and firmware is an ongoing process conducted by software publishers, researchers, gray hats and black hats.

### Bug Bounty Programs

A bug bounty program is an incentive offered by many websites and software developers by which individuals can receive recognition and compensation for reporting “bugs”, especially those pertaining to exploits and vulnerabilities.
* Bug bounties are now offered by hundreds of companies including Google, Microsoft, United Airlines, PayPal, Uber, and a variety of government agencies.

Here are examples of various bug bounty program:
* https://www.google.com/about/appsecurity/reward-program/
* https://technet.microsoft.com/en-us/library/dn425036.aspx
* https://www.united.com/ual/en/us/fly/contact/bugbounty.html
* https://www.paypal.com/bugbounty
* https://www.uber.com/newsroom/bug-bounty-program/


### Business Process Vulnerabilities
Security doesn’t operate in a vacuum nor is it solely an IT issue. Weak or insecure business processes can have a devastating impact on an organization.
Consequences can include:
* Unnecessary risk
* Financial Loss
* Reputational damage
* Inefficient operations
* Low morale
* Regulatory non-compliance

### Configuration vulnerabilities
Configuration vulnerabilities are often a reflection of weak or non-existent business processes including configuration, change, and vulnerability management.
Consequences can include:
* Exposure (Opportunistic)
* Theft and loss
* Interruption of service / downtime
* Resource exhaustion
* Compromise.

### Asset-related Vulnerabilities

| Issue | Description | Impact |
|-------|-------------|--------|
| System Sprawl | Unplanned / Unmanaged growth Inconsistent platforms. Multiple vendors | Support buden, Decentralized management, Inability to enforce standards|
| Architecture / Design Weakness | Implementation of inherently insecure systems or network segments | Exposure to Attack |
| Documented Assets | Assets not inventoried, documented, or tracked. | Excluded from vulnerability, change, and , configuration management process. Not included in testing scope. Loss of ownership control. |

### Vendor-related Vulnerabilities
| Issue | Description | Impact |
|-------|-------------|--------|
| End of Life System | Devices, operating systems, or applications that are not longer supported by vendor. | Vulnerabilities not addressed. No vendor support and guidance. |
| Lack of vendor Support | Absence of support or maintenance contracts
Deficient warranty. Unresponsive Vendors | Vulnerabilities not addressed, Problems unresolved, Downtime.|

### Personnal-related Vulnerabilities
| Issue | Description | Impact |
|-------|-------------|--------|
| Untrained Users | Users who are not aware of and/or do not understand their role in protecting information and information systems. | Inadvertent participation in exploits,  Bypassing controls Inability to recognize and report potential incidents. |
| Improperly Configured Accounts | Accounts that have incorrect rights and/permission (explicit or group) Accounts that are stale. | Inadvertent participation in exploits Ability to make adverse changes (e.g. disable AV) Confidentiality violations. |

### Configuration-related Vulnerabilities  
| Issue | Description | Impact |
|-------|-------------|--------|
| Default Configuration | Using the “Out-of-the-box” settings which generally favor convenience over security. | Diminished attack workfactor as default settings are publicly known |
| Misconfiguration | Configuration parameters either incorrect and/or not in accordance with best practices | Could be significant - depending upon what the misconfiguration is. |
| Resource Exhaustion | Resources required to execute an action entirely expended | Denial of service. |
| Embedded systems | Proprietary configurations “Old software” inability to update. | Unknown exposure, Vulnerabilities not addressed|

### Cryptographic-related Vulnerabilities
| Issue | Description | Impact |
|-------|-------------|--------|
| Weak Ciphers | Implementing ciphers that are either broken, deprecated (weak), or not on par with the level of protection required | Unexpected exposure and confidentiality violations |
| Improper Certificate and Key Management | Not properly protecting private keys, Not properly managing certificate ownership.| Unauthorized access, Impersonation, Reputational damage |

### Source Code Vulnerability

Source code vulnerability is an error, failure, or fault in a computer or program that causes it to produce an incorrect or unexpected result or unintentional behavior and / or response.
* Source code flaws can affect functionality, performance, and security.
* Improper Input handling.

| Vulnerability | Description | Impact |
|---------------|-------------|--------|
| Injection | Tricking an application into including unintended commands in the  data sent to an interpreter (OS, LDAP, SQL) | Can result in database, schema, account, and/or operating system access.|
| Cross-Site Scripting | Injection of malicious code into a vulnerable web application or back-end database that will execute scripts in a victims browser.| Can result in user session hijack, redirect to malware distribution site, or bypassing access controls. |
| Cross-Site Request Forgery (CSRF / XSRF) | Tricking a web browser into executing a malicious  action on a trusted site for  which the user is currently authenticated. CSRF exploits the trust that a site has in a user’s browser.  | Can result in data theft, unauthorized funds transfers, credential modifications, or stolen session cookies. |

### Improper Error Handling.
| Vulnerability | Description | Impact |
|---------------|-------------|--------|
| Error Messages | Generation of error messages are reveal implementation or debugging details. | Disclosure Recon “Clues” |
| Default Messages | Divulge system information such as “Invalid user name” | Disclosure Recon “Clues” |

### Memory / Buffer Vulnerabilities
| Vulnerability | Description | Impact |
|---------------|-------------|--------|
| Buffer Overflow | Overrunning the memory allocated (buffer) for data input and writing the excess data into non-allocated system memory | The excess data can contain instructions that the processor will execute.|
| Memory Leak | Failure of an OS or Program to free up dynamically requested memory. | Slow response time (Sluggishness) Denial of service.|
| Integer Overflow | Trying to place into computer memory an integer ( Whole number ) that is too large for the integer data type in given system. | Incorrect results |  | | Pointer Dereference | Memory point = Null | Application crash |
| DLL injection | Running code in the address space of another process by forcing it to load a DLL. | Unintended behavior. |

### Race Conditions
| Vulnerability | Description | Impact |
|---------------|-------------|--------|
| Race Condition. | A race condition is a flaw that produces an unexpected result when the timing of actions impact other actions. An example may be seen on a multi-threaded application where actions are being performed on the same data. | Unauthorized Access, Unexpected Results. |  

### Security Code Review
Security code review is the process of auditing the source code for an application to verify that the proper security controls are present and work as intended.
* Static code analysis is the examination of non-running code (static) for vulnerabilities.
* White box tests internal structure of an application with explicit knowledge.
* Penetration testing evaluates security by attempting to exploit vulnerabilities (Code, Configuration or functionality.
