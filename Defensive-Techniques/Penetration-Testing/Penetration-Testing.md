# Penetration Testing
The objective of penetration testing is to evaluate the security of a target by identifying and attempting to exploit vulnerabilities, improper configurations, and hidden points of entry. (Ethical Hacking.)
* Penetration testing mimics real-world attack methodology.
* Penetration testing generally involves exploiting combinations of vulnerabilities on one or more systems.
* Penetration testing can be useful for determining incident detection and response capabilities.

### Penetration Testing Approaches

| Position | Description |
|----------|-------------|
| Black Box (Blind) | Penetration testing team is not provided any details of the target environment. |
| Double Blind | Penetration testing team is not provided any details of the target environment Target personal (Incident handler, security engineers, etc..) have no knowledge of the test. |  
| Gray Box | Penetration testing team is provided limited information about the target environment. |  
| White Box (Targeted) | Both the penetration testing team and internal personal are knowledgeable and work in concert.|

### Testing Relationship
| Characteristics | White Box | Black Box |
|-----------------|-----------|-----------|
| Relationship | Cooperative | Adversarial|
| Credentials | May or may not be provided. | None |
| Advantages | More efficient. | Valid test of incident detection and incident response capabilities. |

## Red Team | Blue Team
| Position | Description |
|----------|-------------|
| Red Team | External entities that emulate the behaviors and techniques of likely attackers. |
| Blue Team | Internal Security team (Defenders)|

### Rules of  Engagement

A rules of engagement (ROE) document details the parameters and expected testing team conduct of the test/ assessment/audit.
* Included in the ROE should be target environment and objective, scenario and approach, level of knowledge, constraints, notifications data handling requirements and reporting expectations.

### Penetration Testing Vs. Vulnerability

A penetration test is designed to exploit ( Actual or proof of concept) Weakness in the target environment.
* Not to be confused with a vulnerability scan which looks for known vulnerabilities in the target environment and reports potential exposures.

### Penetration Test Phases

1. Passive Reconnaissance
2. Active Reconnaissance.
3. Exploitation
4. Additional Research
5. Continued Exploitation
6. Reporting
7. Research and exploitation are iterative processes.

### Passive Reconnaissance (Passive recon):
Is information gather using publicly available resources. The Target has no knowledge of the activity.
* Identifying IP addresses and subdomains
* Identifying external and 3rd party relationships.
* Identifying people, personal information and contact information.
* Identifying technologies in use
* Identifying content of interest ( e.g. web, email and remote access portals. )

### Passive Recon Tools
| Tool | Description |
|------|-------------|
| WHOIS | Domain records whois.icann/org
| Maltego | Email Addresses, internal phone numbers, DNS records, IP Addresses. Geolocations, Social Networking.|
| Google | Searches (People, Jobs, technologies, files, portals, consoles, webmail)|
| Netcraft | Website Server and client side technologies |
| SEC EDGAR | Public company information |
| Passive Recon (FireFox Plugin) | MX records, DNS information.|

### Active Reconnaissance (Active Recon)
Uses technical tools to probe and discover information. The target may become aware aware of the activity and respond.
* Enumeration of devices, hosts, IP Address, Operating Systems, ports, applications, users/groups,  services  
* Identifying software / firmware versions and patch levels
* Mapping Network Connections.

### Active Recon Tools
| Tool | Description |
|------|-------------|
| Shodan | Web Crawler includes ports, operating systems, and host names. Also identifies public facing devices such as cameras and printers.|  
| Metagoofil | Extract metadata |
| FOCA | Enumerate users, folders, emails, software, operating systems. |
| Burpsuite | Web scanning |
| Nmap | Port Scanning |
| Nessus | Vulnerability Scanning |

### Exploitation
Is the stage where the testers exploit target systems to compromise them. Depending upon the ROE, this phase may be undertaken as “Proof of concept” or actual exploit. Research and exploitation are iterative processes.
* Persistence is the act of installing or modifying services, installing malware or rootkits, creating backdoors, and/or creating accounts that will survival reboots.
* Pivoting is the act of using weakness on one system to access a better protected system.
* Escalation of privileges is the act of exploiting a vulnerability to gain elevated access to a resource.

### Exploit Tools
| Tool | Description |
|------|-------------|
| Metaspoloit | Attack Simulator|
| W3afis | Web application attack|
| backtrack | Packet sniffing and injection|
| Cain & Abel | Cracking encrypted passwords or network keys.|
| SQLmap | Exploiting SQL injection |

### Reporting:
Penetration test reports should include vulnerability findings, exploit activities, and recommendations for mitigation.
* Vulnerability finders should be categorized and referenced appropriate with CVE notation.
* Exploit activities should be documented with enough details so that they are reproducible.
* Mitigation recommendations should be prioritized and as applicable, include risk reduction and security enhancements recommendations.

### Pen Test Results Criteria

| Component | Description|
|-----------|------------|
| Scope | What system and devices are in scope / out-of-scope?|
| Frequency | How often is the test conducted?|
| Stage | What stage of the target environment?|
| Type | Was the testing manual or automated?|
| Qualifications | What is the qualifications of the testers? |
| Rating Scale | What rating scale are they using - proprietary, open source, government? |
| Results | How comprehensive are the results? How clearly are they presented?
Remediation Plan | Are remediation actions documented? Is enough information presented so that the findings can be replicated?|
