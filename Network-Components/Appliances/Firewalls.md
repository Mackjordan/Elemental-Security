# Firewalls

The primary objective of a firewall is to isolate network segments by controlling ingress and egress access.
* Ingress means incoming and egress means outgoing.
* Firewalls are a preventive control because they can be configured to restrict
* ingress and egress network traffic, repel known attacks, manage non routable IP addresses, and anonymize internal addresses.
* Firewalls can be a detective control because they can be configured to log events and to send alerts.

### Firewall Security Features
| Feature | Description |
|---------|-------------|
| Packet Filtering (ALL)| Analyzes network packet addressing for malformed packets attacks and spoofed IP addresses.|
| Access Control Lists (ALL) | Restrict access including IP address, port, protocol, time/day, and custom rules.|
| State (ALL) | Stateless firmware treat each datagram individually Stateful firewalls are able associate packets with either previous or future packets to make inferences about datagrams or streams.|
| Application Layer Filtering | Apply rules that are specific to applications and services.|  
| Proxy Server | Accepts and forwards request from clients |
| Network Address Translation (NAT) | Map internal private IP addresses to public IP addresses.|

### Firewall Configuration Planning
| Requirement | Example Considerations |
|-------------|------------------------|
| Ingress / Egress Filtering | Allow by default - if not explicitly denied, then access is allowed. Deny by default (Implicit deny) - if not explicitly allowed, the access is denied. |
| NAT | Network address translation - private to public IP address mapping. |
| Business Rules | By IP addresses, protocols, ports. By user or group. By time or day.|
| Approvals and administration. | Process for approving a new rule. Process for approving an exception.|
| Monitoring / Logging | Configuration of logs, log review and log archive. |
| Review / Testing | Review of configuration and rule-set, identifying vulnerabilities, testing access, and exploits |

### Firewall ACL (Rules)
| Element | Description |
|---------|-------------|
| Permission | ALLOW or PERMIT to allow traffic. DENY to block traffic. |
| Protocol | Typically TCP or UDP (You can use IP to indicate both)|
| Source | Where the traffic is coming from  (Host, range, wildcard, ANY)|
| Destination | Where the traffic is going to (host, range, wildcard, ANY)|
| Port | Listening port (e.g. HTTP is port 80)|
| Deny | Last rule at the end of a ACL to block any traffic that wasn’t previously allowed can be a statement (explicit) or a command (implicit)|
