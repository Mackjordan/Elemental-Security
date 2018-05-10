# Physical and Data Layer devices

![OSI model](https://upload.wikimedia.org/wikipedia/commons/2/2b/Osi-model.png)

Network Data Transmission
Data transmission is the physical transfer of data over a
communication channel.
* Network data transmission components include communication
protocols, connectivity devices, and transmission media.

Network mode/s describe layers of communication. From a
security perspective, it is important to understand what happens
at each layer, the dependencies, and the weaknesses.
* The Open Systems Interconnection (OSI) reference model is
structured into seven layers.

### Networking Devices
| Layer # | Layer  | Device |
|---------|--------|--------|
| Layer 1 | Physical | Hubs, Repeaters |
| Layer 2 | Data Link | Bridges, Wireless Access Points, Switches |
| Layer 3 | Network | Multilayer, Switches, Router |
| Layer 4 | Transport | Load Balancer |

### Routers
Routers are Layer 3 forwarding devices.
* Routers forward packets using IP addresses and routing
protocols.
* Access can be control via port or IP address ACL.
* Routers can perform NAT functions. .
* Routers support different WAN technologies.
* Routers support various routing protocols such as RIP, OSPF,
EIGRP, and BGP.

### Routing Loop.
A routing loop happens when a data packet is continually routed
through the same routers over and over. The data packets
continue to be routed within the network in an endless circle
and can cause a denial of service.
There are three loop prevention techniques:
* Split horizon prevents a router from advertising a route back
onto the interface from which it was learned.
* Route poisoning is when the router detects a failed route and
sends out a advertisement with an infinite metric.
* Hold down prevents a router from learning new information
until a timeout period has been reached.

### Hubs and Repeaters
Hubs and repeaters are OSI Layer 1 devices.
* Repeaters amplify signals.
* Hubs retransmit a signal received on one connection point to all
ports.
* Hubs are unsecure LAN devices (anyone can sniff the
packets) that should be replaced with switches for security
and increased bandwidth.

### Bridge
Bridges are OSI Layer 2 two port (input and output) devices that
connect LANS using the same protocol.
* Bridges filter traffic based on MAC address, amplify signals, and
can be used to connect dissimilar media.
* Wireless access points are bridges for wireless and wired IP
traffic.

### Switches
Switches are multi-port forwarding devices that enable high-speed
passing of data and error checking.
* Layer 2 switches filter traffic by MAC addresses.
* Layer 3 switches filter traffic by IP address and have routing
capabilities.
* Aggregation Layer 2 switch that provides connectivity for other
switches.
* Managed switches provide the ability to configure, manage, and
monitor the device via:
* Serial console command-line interface
* Remote Telnet, SSH, HTTP, or HTTPS interface
* Embedded simple network management protocol

### VLANS
VLAN management allows for the software configuration of end
stations to be logically grouped together, even if they are not
located on the same physical network switch. This allows the
grouping of hosts with a common set of requirements to
communicate as if they were attached to the same broadcast
domain.

### Port Security
Port security is a dynamic feature that can be used to limit and
identify the MAC addresses of the stations that allow access to
the same physical port.
* Limiting the number of allowable MAC addresses on a switch
port using port security effectively shuts down a MAC address-
flooding DDoS attack.

### Flood Guard
A flood guard is a protection feature designed to identify
scenarios that will overwhelm the network (e.g. SYN attack,
ping, port floods) and reducing tolerance.
* By reducing tolerance, it is possible to reduce the likelihood of a
successful DoS attack. If a resource—inbound or outbound—
appears to be overused, then the flood guard kicks in.

### Spanning Tree Protocol
Spanning Tree Protocol (STP) prevents switching loops and
broadcast storms. Shortest Path Bridging (SP3) is a replacement
for legacy STP.
* A switching loop occurs in when there is more than one Layer 2
path between two endpoints (e.g. multiple connections
between two network switches or two ports on the same
switch connected to each other).
* The loop creates broadcast storms as broadcasts and multi-casts
are forwarded by switches out every port, the switch or switches
will repeatedly rebroadcast the broadcast messages flooding the
network.

### Access Control Lists
Access control lists (ACLs) are used to filter router traffic.
* Limit network traffic to increase network performance.
* Provide traffic flow control.
* Provide a basic level of security for network access by defining
which part of the network/server/service can be accessed by a
host and which cannot.
* Granular control over traffic entering or existing the network.

### Anti-spoofing
IP Spoofing is used by attackers to fake the source packet
address to appear as if it is a trusted address.
* Access control list (ACL) entries can be used as a spoofing
control. lngress (incoming) packets are inspected. If the address
belongs to the internal network or the router itself, the ACL
instructs the packet be dropped.

### Load Balancer
Load Balancer improves the distribution of workloads across
multiple computing resources and prevents resource overload
(resulting in a denial of service).
* One of the most commonly used applications of load balancing
is to provide a single Internet service from multiple servers,
sometimes known as a server farm.
* A virtual IP is a virtual single address presented externally that
maps back to multiple internal physical IP addresses.

### Load Balancer Scheduling
Load balancing scheduling techniques include affinity, round robin DNS and persistence.
* Affinity is the process of associating a user's IP address with a single server.
* Persistence is the process of associating application layer
information with a single server.
— Round—robin DNS associates multiple IP addresses with a single
domain name. Clients are given IP address in a round-robin
fashion.

### High Availability (HA) Mode
| HA Mode | Description |
|---------|-------------|
| Active / Passive Pair | The primary load balancer services the requests. The second load balancer operates in listening mode to constantly monitor the performance of the primary load balancer. If the active device fails, the passive device automatically takes over.
| Active / Active Pair | In Active/Active mode, two or more load balancers aggregate the network traffic load, and working as a team, distribute it to the network servers. If either device fails, service continues. |

### Wireless Access Point
A wireless access point (WAP or AP) bridge wireless and wired IP
traffic.
* An AP act as a central transmitter and receiver of wireless
signals.
* An AP can either be a stand-alone device or router integrated.
* Fat (thick) access points have 802.11 security, management and
performance standalone functionality built-in.
* Thin access points minimize device intelligence and offload
configuration features and management to an associated
controller.

### Set Service Identifier (SSID)
A Set Service Identifier (SSID) is a code that identifies
membership with a wireless access point.
* All wireless devices that want to communicate on a network
must have their SSID set to the same value as the WAP SSID to
establish connectivity with the WAP.
* By default, a WAP broadcasts its SSID every few seconds.
* This broadcast can be stopped so that a attacker can't
automatically discover the SSID and hence the WAP.
* However, because the SSID is included in the beacon of
every wireless frame, it is easy for a hacker equipped with
sniffing equipment to discover the value and fraudulently
join the network.

### MAC Filtering
MAC filtering can be enabled to specify the MAC address of
devices permitted to connect (allow or deny) to the WAP.
* Frames can be sniffed to discover a valid MAC address, which
the attacker could then spoof.

### 802.11i
IEEE 802.11i is a port—based network access control standard. It
provides per—user, per-session, mutual strong authentication, for
wireless networks.

### Signal Strength and Band Selection
| Specification | Data rate | Frequency | Distance |
|---------------|-----------|-----------|----------|        
| 802.11 | 2 Mbps | 2.4 GHZ | 100 m |
| 802.11b | 11 Mbps | 2.4GHz | 140m |
| 802.11a | 54Mbps | 5GHz | 120m |
| 802.11g | 54 Mbps | 2.4GHz | 140m |
| 802.11n | 150 Mbps | 2.4 / 5 GHZ | 250m |

### Wireless Antennas
| Type | Description / Placement |
|------|-------------------------|
| Omnidirectional   |  An omnidirectional antenna radiates transmissions out and redirects transmissions in from all directions (360 degrees). Generally used inside a building. |
| Directional | A directional antenna focuses the signal in a specific direction. Generally used to connect buildings. |
