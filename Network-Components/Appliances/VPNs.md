# Virtual Private Network

A virtual private network (VPN) is designed to facilitate secure
remote access communication over a public network.

* VPNs are a cost-effective alternative to dedicated point-to-point
connections by transforming the Internet into a secure circuit.
* VPNs isolate the network frames from the surrounding
networking using a process known as encapsulation or
tunneling.
* Full tunneling requires all traffic to be routed over the VPN.
* Split tunneling allows the routing of some traffic over the VPN
while letting other traffic directly access the Internet.

| Application | Description |
|-------------|-------------|
| Telnet Terminal Emulation Telnet Port 23 | facilitates the connection to a remote system and the execution of commands. Telnet provides basic authentication (user name and password) Telnet communication is clear text. |
| Secure Shell (SSH) Terminal Emulation port 22 | SSH facilitates the connection to a remote system and the execution of commands. SSH creates a secure encrypted tunnel to the remote system |
| Remote Desktop Software (RDP Port 3389) | Software or OS feature that allows a desktop environment to be run remotely.|
| Virtual Private Network (VPN) Port depends upon protocol | VPN is a secure private connection between two end points — Host-to-Host, Host-to-Network, or Network-to-Network |


### Proprietary VPN Protocols

PPTP is Microsoft’s implementation of secure communication over a VPN.
* Designed to secure Point-to-Point protocol (PPP).
* No longer considered secure.

L2TP is Cisco’s implementation of secure communication over a VPN.
* Combines Layer 2 Forwarding and PPTP.
* Can be used on IP and non-IP networks.

### SSL (TLS) VPN

SSL or its successor TLS for single or multiple connections using a browser.
* User connects to a SSL Gateway or endpoint.
* SSL VPN Portal is a single connection to multiple services.

SSL VPN is another option for creating secure connections to
servers.

* SSL portal VPN: A single SSL (or its successor TLS ) connection for
accessing multiple services on the web server, a page acts as a
portal to other services.
* SSL tunnel VPN: Used to access a server that is not a web server
and uses custom programming to provide access through a web
browser.

### IPsec - the default standard for IP—based VPNs.
* Host-to-host, host-to-site, and site-to-site connections.
* Native to IPv6 and a bolt-on to IPv4.
* Uses cryptography to provide authentication, integrity,
confidentiality, and non-repudiation.

### IPsec Modes
IPsec can be implemented in two modes.
1. Transport mode is used for end-to-end protection between
client and Server
* The IP Payload is encrypted.
* Transport is the default mode of IPsec.
2. Tunnel mode is used between server-server, server-gateway, or
gateway-gateway (two direct endpoints).
* The entire packet is encrypted.

### IPsec Protocols

IPsec uses two distinct protocols, Authentication Header (AH)
and Encapsulating Security Payload (ESP).

* The AH protocol provides a mechanism for authentication only.
AH provides data integrity, data origin authentication, and an
optional replay protection service.

* The ESP protocol provides data confidentiality (encryption) and
authentication (data integrity, data origin authentication, and
replay protection). ESP can be used with confidentiality only,
authentication only, or both confidentiality and authentication.

### IPsec SPI
A negotiated security association (SA) includes the algorithms
that will be used (hashing and encryption), key length, and key
information.
* Security associations are identified by a security parameter
index (SPI).
* Two separate SAs are established for each direction of data
communication.

### Standard VPN terms

##### Always-on VPN
An always—on VPN starts automatically as soon a client device
recognizes an Internet connection.
* Connection and authentication are transparent to the user.
