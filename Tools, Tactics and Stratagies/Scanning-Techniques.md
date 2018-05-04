# Scanning Techniques

### Vulnerability Scanning
The objective of vulnerability scanning is to identify vulnerabilities in the target environment and report potential exposures including rogue devices. Scanning is generally considered a passive activity.
* Scanning can be intrusive or non-intrusive.
* Scanning authentication can be credentialed or non-credentialed.

### Non-intrusive Vulnerability Scanners
Non-intrusive scanning applications identify the active operating system, applications, and ports by scanning the target system’s attributes ( e,g, inspecting the file system for specific files or files versions, checking the regerity for specific values, looking for security updates, discover which services are listening.
* Non-intrusive scanners can report on but do not attempts to exploit vulnerabilities.
* Non-intrusive scanners can report on misconfigurations.
* Non-intrusive scanners do not take action to resolve security problems.

### intrusive Vulnerability Scanners
Intrusive scanning applications probe devices, examine response, and validate vulnerabilities.
* Intrusive scanners can be used to simulate an attack.
* Intrusive scanners can take action to autonomously resolve security issues, such as blocking a potentially dangerous IP Address.

### Pen Test Results Criteria
|   | Non-credentialed | Credentialed |
|---|------------------|--------------|
| Explanation | No Authentication | Account is authenticated to simulate being a user or administrator on the system / website. |
| Advantages  | Easier, Quicker, Uses less system resources and inexpensive |  Comprehensive |
| Disadvantages | Incomplete findings. | Requires Configuring accounts, Time Consuming, Resource intensive and may result in unintended consequences including denial of service and high volume of alerts.|

### Pen Test Results Criteria
| Tool | Reporting | Examples |
|------|-----------|----------|
| Port Scanner | Identification of open ports, fingerprint OS | Nmap, SuperScan |
| Network Map | Map of devices and applications | Nmap, SpiceWorks |
| Vulnerability Analyzer | Identification of Published vulnerabilities | OpenVAS, Nessus |
| Configuration Analyzer | Identification of configuration errors of lack of controls | Microsoft Baseline Security Analyzer (MBSA), Lynis |

### Beware of false findings
| State | Description |
|-------|-------------|
| False Positive | Normal is incorrectly identified as abnormal.|
| False Negative | Abnormal is incorrectly identified as normal.|

### Scanning & Analysis Best Practices
Vulnerability scanning and configuration analysis best practices include:
* Creating an inventory of network assets.
* Identifying critical assets.
* Determining Frequency of scanning.
* Confirming Scope.
* Ensuring the scanning / analysis application is current.
* Establishing and documenting timelines and thresholds
