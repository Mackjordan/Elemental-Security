### Network Access Control
Network Access Control (NAC) is an agent or agentless approach
to network security that attempts to unify endpoint security
technology, user or system authentication, and network security
enforcement.
* An agent is a piece of code that performs a function on behalf
of an application.


### Inside the Perimeter
| Acronym | Name | Synopsis |
|---------|------|----------|
| NAC | Network Access Control | Network Access Governs connections to the network based on Control configuration requirements (e.g. patch level, AV) |
| DLP | Data Loss Prevention | Data Loss Prevention Inspects content with the objective of preventing data exfiltration (inadvertent or intended) |
| SEG | Secure Mail Gateway | Secure Mail Gateway Antivirus, antimalware, antiphishing, and antispam features plus DLP and encryption enforcement |


| Type | Description |
|------|-------------|
| Persistent or Permanent | Installed on a device and runs continuously |
| Dissolvable or Portal-based | Downloads and runs when required (one time authentication) and then disappears |
| Agentless | Integrates with a directory services (e.g. Active Directory)

### NAC Policies
NAC pre-admission policies determines if a device is allowed on
the network and if so, what segment based on host health.
* Antivirus application level
* OS and application patch level
* Firewall and host intrusion prevention software status
* Configuration settings
NAC post-admission polices regulate and restrict access once the
connection is allowed.

### NAC Remediation
Two common strategies for remediation are quarantine
networks and captive portals.
* A quarantine network is a restricted IP network that provides
users with routed access only to certain hosts and applications
that can provide the appropriate updates.
* A captive portal redirects users to a web application that
provides instructions and tools for updating their computer.
