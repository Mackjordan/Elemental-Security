# Secure Communication Protocols
The function of a secure protocol is to ensure confidentiality,
integrity, or availability, or any combination thereof.
* Secure protocols are commonly used in network management
and communications; often replacing older insecure protocols.

### Secure Communications Protocols
##### SSL / TLS:
Secure Socket Layer/Transport Layer Security
##### HTTPS:
Hyper Text Transfer Protocol Secure
##### FTPS
File Transfer Protocol Secure (FTP Secure)
##### S/MIME
Secure/Multipurpose Internet Mail Extensions
##### Secure POP3
Secure Post Office Protocol 3 (SSL-POP, POP3S)
##### Secure IMAP
Secure Internet Message Access Protocol (lMAP4-SSL)

### Secure Sockets Layer (SSL)
Developed in 1995, Secure Sockets Layer (SSL) is used to establish a secure communication channel between two TCP sessions by negotiation. Default SSL port is 443.
* In 2015, SSL 3.0 was deprecated. New vulnerabilities continue to be
discovered. SSL2.0 and 3.0 should be disabled.

SSL connection breakdown:
1. Client makes a connection request.
2. The server secure connection needed.
3. The client send the security capabilities.  
4. Encrypted Session Established.

### Transport Layer Security (TLS)
TLS is used to establish a secure communication channel between two TCP sessions using a cryptographic key exchange. Default TLS port is 443.
* TLS is the successor and recommended replacement for SSL. TLS 1.1 or higher
should be used. TLS 1.0 has been broken.

TLS connection breakdown:
1. Session Establishment
2. Cryptographic Key Exchange
3. Encrypted Session Established

### SSL / TLS Accelerators
SSL / TLS encryption/decryption is processor intensive operation.
* SSL / TLS Application Specific Integrated Circuits (ASIC) are processers that are specifically designed to perform SSL / TLS operations.
* SSL / TLS Accelerator is an ASIC appliance that sits between a user and a server, accepting SSL / TLS connections from the client and sending them via a private network to the server unencrypted.

### SSL Decryptors
SSL decryptors are controversial perimeter devices (either built into the firewall or standalone appliance) used to decrypt SSL/TLS packets, inspect the contents, re-encrypt, and forward the packet.

### Hypertext Transfer Protocol (HTTPS)
Hypertext Transfer Protocol (HTTP) is the underlying protocol used by websites and defines what actions browsers and webservers should take in response to commands. HTTP is a clear text protocol and subject to eavesdropping, replay and MiTM attacks.
* HTTPS (Hypertext Transfer Protcol Secure) is an extension to HTTP that adds support SSL and TLS order to encrypt communication between a browser and a website (TCP Port
443).
* Use case: secure web connectivity and authentication.

### File Transfer Protocol (FTP)
FTPS is used for file access, file transfer, and file management. Authentication data and payload are transmitted in clear text and subject to eavesdropping, replay,
and MiTM attacks.
* FTPS (File Transfer Protocol Secure) is an extension to FTP that
adds support for SSL and TLS in order to encrypt the file transfer
channel (TCP port 99O or 21)
* Don’t confuse FTPS with SFTP. SFTP uses SSH and port 22.
* Use case: Secure file transfer

### Email Security
##### Secure POP3
POP3 is used to receive email from an email server to a local email account.
* Downloaded files are removed from the email server (default).
* POP3 allows cleartext authentication (port 110)
* Use case: Secure POP3 is an extension of POP3 that supports SSL / TLS for secure login (port 995)
##### Secure IMAP
IMAP is used to receive email from an email server to a local email account.
* Downloaded files remain on the email server - important if you use multiple devices
to access email.
* IMAP allows clear text authentication (port 143)
* Use case: Secure IMAP is an extension of IMAP that supports SSL / TLS for secure
login(port 993).
##### S/MIME
S/MIME is a protocol for sending digitally signed and encrypted emails
* Use case: encryption (confidentiality), and digital signature (integrity and non-
repudiation)

### Secure Network and Admin Protocols
| Acronym | Name |
|---------|------|
| NTP | Network Time Protocol. |
| LDAP \ LDAPS | Lightweight Directory Access Protocol. |
| SSH | Secure Shell. |
| SRTP | Secure Real-time Transport Protocol |
| SNMP | Secure Network Management Protocol |
| DHCP / 82 | Dynamic Host Configuration Protocol Option 82 |
| DNSSec | Domain Name System Security. |

### Network Time Protocol (NTP)
NTP is a networking protocol for clock syncronization. Simple Network Time Protocol (SNTP) is a simplified version of NTP.
* NTP is intended to synchronize all participating computers to within a few milliseconds of Coordinated Universal Time (UTC).
* Current version is NTP v4.
* NTP is not considered a secure protocol however time synchronization is an important foundational element.
* NTP and SNTP port is UDP 123.
* Use case: Time synchronization.

### Lightweight Directory Access Protocol (LDAP)
LDAP is an open, vendor-neutral protocol for accessing and maintaining
distributed directory information services.
* A directory service is the centralized collection and distributed
database (domain) of user data, computers, and trusted
entities.
* Microsoft Active Directory (AD) is Microsoft’s implementation
of LDAP in conjunction with Kerberos (TCP port 389).
* LDAPS is used to protect LDAP credentials for non-Microsoft
clients (TCP port 636).
* Use case: Manage objects and users including authentication,
rights and permissions, and trust relationships.

### Secure Shell (SSH)
SSH is a cross platform protocol that establishes a secure connection between an SSH server and an SSH client.
* Secure Shell (SSH) is used to administer systems remotely,
provide a command shell on a remote network, or tunnel other
protocols (TCP port 22).
* Secure Shell is a secure replacement for cleartext, telnet, rlogin, rsh, and rsync.
* SFTP is a file transfer protocol that uses Secure Shell (SSH) to
transfer files.
* Use case: Remote access and administration.

### Secure Real-time Transport Protocol (SRTP)
SRTP is an extension of Real—time Transport Protocol (RTP) that incorporates enhanced security featured for voice over IP (VoIP), audio, and video transmissions.
* SRTP uses encryption and authentication to minimize risk of denial of service and replay attacks.
* SRTP uses UDP port 5004.
* Use case: Secure voice and video.


### Simple Management Network Protocol (SMNPv3)
SMNP is used for managing and monitoring IP devices.
* Devices that typically support SNMP include cable modems, routers, switches, servers, workstations, and printers.
* Components include managed devices, agents, and a management station.
* Version 3 (SMNPv3) added cryptographic security features and is a replacement for cleartext V1 and V2.
* Agents listen on UDP port 161. Managers receive notifications (traps) on UDP port 162.
* Use case: Manage and monitor IP devices including switches and routers.

### Dynamic Host Configuration Protocol (DHCP)
DHCP is used to dynamically assign IP addresses and other parameters.
* DHCP has no native client / server authentication or
authorization.
* DHCP Option 82 provides information about the DHCP client (MAC or circuit ID), and the DHCP server uses this information to assign IP addresses / parameters.
* Internet Service Providers use this feature to restrict access to registered subscribers and authorized devices by requiring customer premises equipment authentication before allowing a device to connect to the network.
* DHCP clients listen on UDP port 67. Servers on UDP port 68.
* Use case: used to secure IP address allocation

### Domain Name Service (DNS)
DNS is used to resolve domain names (e.g. cnn.com) and associated hosts to IP addresses. DNS vulnerabilities allow an attacker to hijack this process resulting in
redirection and session hijacking.
* DNS Security Extensions (DNSSEC) is a technology that was a
developed to protect against such attacks by digitally 'signing'
the zone data assuring its validity.
* Caveat. In order to eliminate the vulnerability from the
Internet, DNSSec must be deployed at each step in the lookup
from root zone to final domain name.
* DNS uses TCP port 53.
* Use case: Secure domain name resolution
