# Security Information and Event Management (SIEM)

Security information and event management (SIEM) solutions
offer real-time data capture, event correlation analysis, and
reporting.

### Audit and Event Logs
Audit and event logs are a chronological record of events and
actions.
* Critical log sources include firewalls, IDS/IPS devices, proxy
servers, authentication servers and devices, operating systems,
and key applications.
* Audit logs are both a near-time and historical detective control.
* Routine log analysis is beneficial for monitoring access,
identifying security incidents, policy violations, fraudulent
activity, and operational issues.
* Logs are critical components of internal investigations and
forensic analysis. Logs should be stored on a WORM (write
once/read many) device.

### Log Analysis Tools
| Type | Description |
|------|-------------|
| Trend/ Variance Detection | Identifies anomalies in system or user behavior.|
| Attack Signature Detection | Identifies ”known” event or sequence of events.|
| Security Information and event Management (SIEM) | Automation tool. SIEM products can analyze data from many sources, identify significant events, report outcomes, and send alerts. SIEM products may integrate with threat intelligence feeds. SIEM products may also include security knowledge bases, incident tracking, and reporting capabilities |

### SIEM Techniques
Log analysis is a complex process.
* Time synchronization is the act of synchronizing with an
external time source with a time stamp protocol (e.g. NTP).
* Time normalization is the process of standardizing geographic
time to a single meta-time (e.g. UTC).
* Aggregation consolidates events from disparate devices and
systems.
* De-duplication filters out duplicate entries or excessive noise.
* Correlation ties individual log entries together based on related
information.

### SIEM Reporting
SIEM reporting generally includes:
* Automated alerts based on preset triggers (immediate issues) —
sent to a dashboard or via a communications channel.
* Graphic and text security, operational and compliance reporting.
