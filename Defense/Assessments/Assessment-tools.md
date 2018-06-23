# Assessing Security Posture
The security posture of an organization refers to its overall
(cyber)security strength and capabilities.
* A security assessment is the examination and analysis of the
safeguards or controls.
* The objective of a security assessment is to determine the
security posture of an organization (including identification of
rouge devices).
* Passive assessment tools listen and/or capture data.
* Active assessment tools probe a target.

| Tools | Objective |
|-------|-----------|
| Protocol analyzer | Capture (”sniff”) and analyze packets. |
| Port scanner | Scan for open "listening” ports to identify services and applications.|
| Wireless scanner | Scan for wireless networks (e.g. SSID) |
| Network mapping | Discover and document physical and logical connections. |
| Banner grabbing | Determine operating systems and application versions. |
| Network enumeration | Discover and document device characteristics. |
| Vulnerability scanner | Scan for known vulnerabilities and exploit potential. |
| Compliance scanner | Determine compliance with specific policies and/or regulations.|
| Password cracker | Assess password strength. |
| Exploitation frameworks | Simulate real-world attacks. |

### Protocol Analyzer
###### Protocol analyzers are used to capture (”sniff”) and analyze data packets.
* Protocol analyzers can be used for troubleshooting and/or
assessment purposes.
###### Assessment examples:
* Determine protocols being used to secure a packet (e.g. SSL,
TLS).
* Determine if clear text passwords are being transmitted
(e.g. Telnet, FTP).
* Verify internal control detection effectiveness.
* Popular protocol analyzers include Wireshark, dSniff, ettercap
and tcpdump (command line).

### Port Scanner
Port scanners are used to document what inbound TCP and UDP
ports are open (”listening”) on a remote computer and what
associated services and/or applications are running.
* There are 65,535 ports. Ports 1-1023 are assigned and referred
to as well-known ports, 1,024-48,151 can be registered with
IANA and ports 49,151-65,535 are dynamic or private parts.
* Port scan can identity legitimate applications (e.g. 88/th
Kerberos) as well as malicious applications (e.g. 3700/tcp Portal
of Doom).
* Popular port scanners include Nmap, Superscan, and AngrylP
Scanner.

### Common Ports
| Port | Service |
|------|---------|
| 21 | FTP Control (20 is FTP Data) |
| 22 | SSH |
| 23 | Telnet |
| 25 | SMTP |
| 53 | DNS |
| 67 | DHCP |
| 80 | HTTP |
| 110 | POP3 |
| 119 | NNTP |
| 123 | NTP |
| 139 | NetBios (also UDP 137 and 138) |
| 143 | IMAP |
| 161 | SMNP |
| 443 | HTTPS |
| 389 | LDAP |

### Network Mapping
Network mapping tools are used to create physical and logical
diagrams.
* The majority of network mapping tools rely on probing IP
addresses.
* Popular network mapping tools include Solarwinds, Spiceworks,
ManageEngine, and Nmag.

### Banner Grabbing
Banner grabbing is the process of opening a connection, reading
the text response (banner) sent by the application, and inferring
the operating system or application.
* Banner grabbing is sometimes referred to as fingerprinting.
* Popular banner grabbing tools include Nmap, NetCraft, Kali
Linux, and netcat (command line).

### Network Enumeration
Network enumeration tools discover devices and characteristics
such as operating systems, open ports, listening network
services, shares, users and groups.
* Supports both credentialed and non-credentialed modes.
* Popular enumerations tools include DumpSec and Nessus.

### Vulnerability and Compliance Scanning
Vulnerability scanning identifies vulnerabilities and potential malicious code but does not exploit them.
* Supports both credentialed and non—credentialed mo
* Popular vulnerability scanners include NESSUS and GFI
LanGuard.
Compliance scanning compares configuration settings.
pre-configured policy standards and compliance 7
— Popular compliance scanners include NESSUS.

### Password Cracker
Password crackers are used to evaluate password or key
strength.
* Wireless password crackers capture packets and crack 802.11
WEP and WPA-PSK keys.
* Popular tools include Aircrack and AirSnort.
* Authentication password crackers attempt to cracked password
hashes either online (brute force) or offline (dictionary and
rainbow tables).
* Popular tools include Cain & Abel, John the Ripper, and
RainbowCrack.

### Exploitation Framework
An exploitation framework is an automated set of tools and
commands designed to simulate real-life attacks.
* Scanners check if a target is vulnerable to a exploit.
* Credential modules test credentials (brute force) against
network services.
* Exploit modules take advantage of identified vulnerabilities.
* Popular frameworks include BeEF (Browser Exploitation
Framework), RouterSploit for embedded devices, Metasploit

### Nmap
Nmap is a free open source tool https://nmap.org used to
discover hosts and services. To accomplish its goal, Nmap sends
specially crafted packets to the target host(s) and then analyzes
the responses. Nmap security assessment uses include:
* Identifying the network connections
* Identifying open ports
* Identifying new servers.
* Measuring response time
* Finding and exploiting vulnerabilities
