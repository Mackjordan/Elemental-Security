# Incident Response Plan and Playbook
An incident response plan includes roles and responsibilities, strategies and procedures for preparing for, responding to, and managing incidents.

* A incident playbook is a set of instructions for responding to a specific type of event, attack or scenario. Generally playbooks are developed for high risk events (measured in terms of likelihood and impact). For example, malware, DDOS attacks, ransomware extortion and payment card compromise.

### Security Incident
An security incident is an event or action that endangers the confidentiality, integrity, or availability of information or information systems.
* A data breach is when data is ex-filtrated or extracted or there is a loss of control. A data breach may trigger reporting and notification requirements.

### IRP Components
| Component | Description  |
|-----------|--------------|
| Incident types and Categorization | Based on severity and used to determine response times, resource assignments, and preparation requirements. |
| Roles and responsibilities | Assignments including first responders, incident handlers, and designated spokespersons. |
| Reporting requirements | How incidents are internally reported, documented, and reviewed as well as when notification requirements are triggered. |
| Escalation requirements | Definitions for escalation thresholds. |
| Incident Response Team | Membership, preparation, skill requirements, external resources.|
| Exercise requirements | Training and exercise requirements and reporting. |

### IRT Membership and Resources
Membership of the incident response team (IRT) is generally composed of internal personnel and adjunct (as needed) external resources.
* Internal personnel should represent a cross-section of the organization including operations, information security, information technology, risk management, marketing, legal and compliance, and executive management.
* External resources include forensic experts, legal counsel,
insurance representatives, public relations, and law enforcement.

### Incident Response Training
Incident response training should be included in organization-wide SETA programs.
* All personnel should be aware of potential incident scenarios and reporting procedures.
* First responders and CIRT team members/should receive training related to their assigned tasks.
* Executives should be educated on incident-relate organizational risks.  

### Incident Response Testing
Incident response exercises should be conducted on a periodic basis to assure readiness.
* Exercises include tabletop and simulations.
* Participants should include the CIRT team, external resources, and as applicable, executive management.

### Incident Response (IR) Process
1. preparation
2. Identification Detection & Analysis
3. Containment
4. Eradication
5. Recovery
6. Lessons Learned

http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf

### Incident Response Phases
| Phase | Objective(s) |
|-------|--------------|
| Preparation | Establish response capability. Prevent incidents from occurring. |
| Detection | Identify and analyze predictors of compromise (POC) and indicators of compromise (IOC). Examples include IDS, SIEM, AV, File integrity checking, logs, network, flows, threat intelligence, people. |
| Containment | Minimize the damage. Examples include shutting down a system, disconnecting it from a network, disabling certain functions. |
| Eradication | Eliminate components of the incident. Examples include deleting malware, disabling breached accounts, mitigating associated vulnerabilities. |
| Recovery | Restore systems to normal operations. |

### Preparation
In preparation of incident, an organizations would:
* Ensure that appropriate preventive, deterrent, and detection controls are in place. (Defense-in-Depth).
* Set response criteria based on scope and severity'(from single infected device through entire infected network).  
* Have trained responders.
* Have documented procedures.
* Know how to handle (not destroy) evidence.
* Have internal capability or an established relationship with a forensics firm.

### Identification
Early identification can help an organization minimize the number of infected systems, which will lessen the magnitude of the recovery effort and the amount of damage the organization sustains.
* Monitor alerts (anti-malware software, IDS/IPS, log analysis).
* Monitor advisories and industry bulletins for news of new malware strains, trends, and activity.
* Encourage users to report unusual or suspicious activity, and monitor and follow up on reports.

### Containment
Malware containment has two major components:
1. Identifying and understanding the malware.
   * Responders should be trained in how to handle evidence
   * Malware files submitted for analysis.
2. Stopping the spread of the malware and preventing further damage.
   * Organizations should be prepared (with management approval) to block or shut down services and/or devices.
   * All external connections should be evaluated for command and control (C2) channels.

### Eradication
Eradication ranges from simple to complex depending upon the veracity of the malware. Containment methods should remain in place until management authorizes lifting the measures.
* Quarantine and delete
* Remove files and/or registry settings
* Remove drive

### Recover
Recovery is closely linked to the eradication method. The more invasive the eradication; the more significant the recovery.
* Rebuild/reimage/restore.

### Lessons Learned
Post-incident lessons learned should be evaluated and integrated into organizational processes and controls.
* Exactly what happened, and at what times?
* How well did staff and management perform in dealing with the incident?
* What would the staff and management do differently the next time a similar incident occurs?
* What corrective actions can prevent similar incidents in the future?
* What precursors or indicators should be watched for in the future to detect similar incidents?
* What additional tools or resources are needed to detect, analyze, and mitigate future incidents?
