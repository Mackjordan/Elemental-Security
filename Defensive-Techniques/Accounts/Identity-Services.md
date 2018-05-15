# Identity and Access Services
Identity and access services is a term used to describe authentication, authorization, and accounting functions.
* An authentication protocol is used solely for user verification (authentication).
* AAA architecture protocols are used for verifying the user (authentication), controlling access to server data (authorization), and monitoring network resource and information needed for billing of service (Accounting).

### Authentication, authorization and Accounting (AAA)
AAA is a framework for contro,||in access (Authentication),
enforcing access policies (authorization) and auditing usage (Accounting). Industry standard implementations include RADIUS and TACACS+.

### Network Protocol
| Acronym | Protocol Name | Service |
|---------|---------------|---------|
| PAP | Password Authentication Protocol | Authentication |
| CHAP / MS-CHAP | Challenge Handshake Authentication Protocol / Microsoft Challenge Handshake Authentication Protocol | Authentication |
| EAP | Extensible Authentication Protocol | Authentication |
| NTLM | NT Lan Manager | Authentication |
| RADIUS | Remote Authentication Dial-In User Server. | AAA |
| TACACS | Terminal Access Controller Access Control System | AAA |
| Kerberos | Authentication System Mutual | Authentication |


### Password Authentication Protocol (PAP)
PAP is the most basic authentication protocol.
* Authentication is initialized by the user.
* User name and password is presented in clear text to an authentication server. If the credentials match what is in the server’s credentials table, then the user is authenticated.
* Very insecure and susceptible to eavesdropping and MiTM attacks.

### Challenge Handshake Authentication Protocol (CHAP)
CHAP and MS—CHAP relies on challenge text and a hashing algorithm.
* Authentication is initialized by the server and can be performed repeatedly throughout the session.
* Server sends a random string of characters (challenge text). The user appends the string to his/her password, hashes the result, and sends it to the server. The server applies the same function. If the results match, the user is authenticated.
* MS-CHAP is Microsoft’s version of CHAP that extends functionality for Microsoft networks.

### CHAP Process
1. User enters login name and password at login screen.
2. Workstation (WS) sends the user name (Not password) to the authentication server.
3. The authentication Server (AS) verifies that the user name exists in its DB, generates a unique sting of challenge text, and sends to the user.
4. The WS login process receives the challenge text. The WS hashes the user password, appends it to the challenge text, and hashes the entire string.
5. The WS sends the hash value to the AS.
6. The AS looks up the user account and extracts the stored hash value of the user's password, appends it to the challenge text, and hashes the entire string.
7. The AS server compares its calculated hash value with the hash value received from the user.
8. If the hashes are identical, the user is successfully authenticated. If the hashes are different, the authentication fails.

### Extensible Authentication Protocol (EAP)
EAP is a general authentication framework.
* There are more than 40 EAP-methods
* EAP is widely used in 802.11 (wireless) networks.

### NT Lan Manager (NTLM)
NTLM is a suite of Microsoft protocols used for authentication.
* NTLM uses challenge-response (similar to CHAP) for authentication.
* Hashed password values are stored on the server not salted and are vulnerable to brute force attacks.
* NTLM is vulnerable to ”Pass-the-Hash" attacks where captured credentials from one machine can be successfully used to gain control of another machine.
* Microsoft recommends not using NTLM. Kerberos is the preferred authentication method.

### Remote Authentication Dial-in User Service (RADIUS)
RADIUS networking protocol provides centralized AAA management services.
* RADIUS became a IETF Internet Standard in 1997.
* RADIUS does not separate authentication and authorization transactions.
* RADIUS is used mainly for network access (e.g. ISP, wireless 802.1x, remote).
* RADIUS reporting includes who joined the network, how did they authenticate, how long were they on, and what types of endpoints are on the network.

### Terminal Access Controller Access Control System (TACACS+)
TACACS+ networking protocols provide centralized AAA management services.
* TACACS+ was developed by Cisco and is proprietary.
* TACACS+ does separate authentication and authorization transactions.
* TACACS+ uses TCP for transport and encrypts the entire packet.
* TACACS+ is used mainly for device administration (e.g. switch, router).

### RADIUS vs. TACACS+
|    | RADIUS | TACACS+ |
|----|--------|---------|
| Protocol | UDP or TCP | TCP |
| Port(s)  | 1812 & 1813 or 1645 & 1646 | 49 |
| Encryption | Only the password | Entire payload |
| authorization \ authorization | Combines authentication and authorization | separates authorization and authorization |
| Primary Use | Network Access | Device Administration |

### Kerberos Security
The Kerberos Server should be a hardened single purpose server. The Kerberos Server is a single point of failure and should be implemented in high availability mode.

Kerberos is a single sign—on (SS0) system that can be embedded in operating systems and directory services (including Microsoft Active Directory) to provide secure mutual authentication.

##### Kerberos Server Components
* Key Distribution Center (KDC)
* Authentication Server (AS)
* Ticket Granting Service (TGS)
* Ticket Granting Ticket (TGT)
* Resource Server
* Trust Principal

##### Kerberos Process

1. Initial CHAP-based authentication between the user and the Kerberos Server.
2. The Kerberos Ticket Granting Service (TGS) generates a Ticket Granting Ticket (TGT).
3. The TGT Access Token is provided to the user. The TGT is protected using symmetric key cryptography.
4. When the user attempts to access a trusted resource, the user sends a copy of the TGT back to the KDC with details of the request.
5. The KDC validates the TGT and generates a limited lifetime Session Ticket. The KDC sends the sessions Ticket back to the user.
6. The session Ticket has 2 encrypted halves (One for the user and one for the resource server.) containing authentication details and symmetric session key.
7. The user decrypts his half of the session ticket, write(Again) the details of resource request, encrypts it with the session key, and sends the session ticket to the resource server.  
8. The resource server decrypts its half of the ticket, verifies the details of the request, and uses the decrypted session key to decrypt the user request. If matching, the user is authenticated to the resource server.
9. Using the session key, the resource server encrypts a portion of the user's authentication data and sends the encrypted data back to the user.
10. If the user can successfully decrypt the message, then the mutual authentication is successful.
