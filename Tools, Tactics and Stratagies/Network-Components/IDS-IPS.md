### IDS /|PS
An intrusion is any activity or event that attempts to undermine
or compromise the confidentiality, integrity or availability of
resources.
* Intrusion Detection is the process of monitoring for an intrusion.
* Intrusion Detection System (IDS) monitors and reports on
intrusion attempts.
* Intrusion Prevention System (IPS) monitors, reports on, and
responds to intrusion attempts.
* IPS/IDS can be network-based or host-based.


### Network-based IDS/IPS
A network-based IDS (NIDS) analyzes and reports on network
traffic. A network-based IPS (NIPS) can take responsive action.

### Placement
A NIDS/NIPS can be situated out-of-band or in-band.
*  Out-of—band placement utilizes a passive tap that receives a
copy of the network traffic and can process samples. Generally,
NIDS will be out-of-band.
*  In—band (inline) placement is directly in the flow of traffic and
must process (inspect) every packet. Generally, NIPS will be in-
band.

### Host—based IDS/IPS

A host-based IDS (HIDS) is software designed to run on a host
computer system and monitors system events, application
interactions and machine logs. A host-based IPS (HIPS) can take
responsive action.


### IDS Detection Approach

| Approach | Description |
|----------|-------------|
| Signature-based | Pattern-matching decisions are based on established known signatures. Signatures must be updated frequently. |
| Ruled-based | Analyzes behavior for violation of preconfigured rules.|
| Behavior-based | Behavior-based anomaly decisions rely on predicted norms and deviations. Can be learned over time and/or start with a set of assumptions and adapt to local conditions. Requires fine tuning.|
| Heuristic | Continually trains on network behavior and can continually alter detection. Capabilities based on learned knowledge.|

### Decision States
| State | Description |
|-------|-------------|
| True Positive | Normal activity is correctly identified. |
| False Positive | Normal Activity is incorrectly identified as abnormal. |
| True Negative | Abnormal activity is correctly Identified. |
| False Negative | Abnormal activity is incorrectly identifies as normal. |

* Positive state always refers to normal activity.
* Negative state always refers to abnormal activity

### Intrusion Detection Response.
| Response | Description | Type |
|----------|-------------|------|
| Logging | Recording information about the event. | Passive |
| Notification | Communicating event-related information. | Passive |
| Shunning | Ignoring the event as it is not applicable. | Passive |
| Terminating | Ending the impacted process or session (Example: Forced RST) | Active/Inline  |
| Instructing | Making a configuration change (Example: Shut down port 80)  | Active/Inline |
| Deception | Allowing the attacker to think the attack was successful in order to gather information about the Intrusion. (Example: Honeypot ) | Active/Inline |

### UTM
Unified Threat Management (UTM) is the evolution of the
traditional firewall into an all inclusive device performing
multiple security functions such as firewall, IDS/IPS, gateway
anti-virus and anti-spam, content filtering, data loss preventing,
and user activity audit reporting.
* Advantages include reduced operational complexity and
overhead cost.
* Disadvantages include single-point-of-failure and vendor
dependency.
