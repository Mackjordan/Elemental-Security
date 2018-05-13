# Zones
### Topology and Zones
Topology refers to the physical and logical structure of a networked environment including resources, connectivity devices, transmission medium, and protocols.
* Zones are divisions of the network based on functional, performance, and/or security requirements.

### Security Zones
Dividing a topology into security zones is useful for creating and enforcing security policies, controlling information flow, and securing network access.

### Security Zone
| Zone | Description |
|------|-------------|
| Untrusted | Networks over which the organization has no control (e.g. Internet)|
| DMZ | A network with connections to both untrusted and trusted networks.|
| Extranet | A network accessed by authorized external users (vendors, customers, partners) generally for the purpose of doing business.|
| Intranet | Private network accessed by authorized internal users.|
| Guest | A network specifically designed to accommodate guests and visitors.|
| Ad hoc | A peer-to-peer network that allows devices to communicate directly.|
| Wireless | A network that uses wireless transmissions.|
| Honeynet | A network used to attract attackers and study attack methods.|
| Remote | A network connection from another site or mobile location.|

### Three Classes of NAT address ranges:
* 2000040255255255
* 172 15.0.n 7172 31 255 255
* 192 152: a o 7 192 153 255 255


### Network address translation (NAT)
NAT is used to map external public facing IP addresses to internal private addresses.
* NAT transforms non-routable IP addresses to routable IP addresses.
* 10.0.0.0 — 10.255.255.255
* 172.16.0.0 — 172.31.255.255
* 192.168.0.0 — 192.168.255.255
* NAT devices (firewall) are stateful. They keep track of the communications between the internal and external hosts until the session is ended.
* NAT effectively ”anonymizes” the internal network from the Internet.

### A demilitarized zone (DMZ)
DMZ is used to segregate and secure servers that need connections to both trusted and untrusted networks (e.g. email servers, web servers, FTP servers).
* Firewalls are used to create DMZs.
* Firewall rules are used to further restrict ingress and egress traffic by source and destination addresses, port, and protocol.

### Extranet
An extranet is a private network segment specifically designed to be shared with and accessible by external entities (e.g. clients, vendors, suppliers).
* Extranets uses include collaboration, knowledge sharing, document sharing, data transfer, and procurement between organizations.
* Extranet can be a component of an externally facing website, an internal website or segment, or hosted by an application service provider.

### Intranet
An intranet is a secure private network used for sharing resources internally.
* An intranet is generally (but not exclusively) web-based and is used for internal collaboration and communication (e.g. SharePoint).

### Guest Network
A guest network is designed to provide visitors with controlled resource access. It is completely segregated from the internal LAN.
* The most common use case is to provide Internet access.
* Guest network can be wired or wireless.
* Wired ports should be clearly labeled.

### Remote Access
Remote access to a network can be configured using remote access programs or virtual private networks.
* A virtual private network (VPN)** is a secure tunnel between systems or networks (e.g. host to host, host to network and network to network).
* Remote access programs are connections that make use of remote access protocols (e.g. remote frame buffer [RFB]) to take over mouse and keyboard functions. Examples include VNC and PC Anywhere.
* Use of remote access programs should be limited by firewall rules and the service shut down when not in use.

### Honeynet
Honeypots are decoy systems used to examine attacker activity and techniques.
* High-interaction honeypots are ”live” systems.
* Low-interaction honeypots emulate the production environments.

Honeynets are multiple linked honeypots that simulate a
network environment.
