# Isolation techniques
Isolation is when segments, devices, or sessions need to be segregated from the environment so as not to cause harm or to be harmed.

* Physical
* Air Gapped
* Virtual
* Logical

### Logical Isolation
A virtual local area network (VLAN) logically compartmentalizes the network into segments which can be restricted.
* The physical port and switch they are connected to is associated with a specific VLAN (not to be confused with virtualization).
* Devices in a VLAN can be located anywhere inside the network.
* Use Case: VLANs allow users/devices with similar characteristics (e.g. access to sensitive data, criticality, third-party access) to be grouped together.

### Virtualized
Visualization* technology creates multiple environments (virtual machines) from a single physical hardware system
* Virtual machines (VMs) provide fault and security isolation at the hardware level including memory and CPU access.
* Virtual switch facilitates communications between virtual machines checking packets before moving them to the destination.
* Use Case: Virtual machine (VM) uses include testing, forensic investigation, high security applications, and resource intensive applications.

### Air Gapped Network
Air gapped network is isolated from any wired or wireless untrusted network or to any other computers that connect to a untrusted network.
* Best practice on air gapped devices is to disable access to removable media.
* Use cases: Air gapped networks are used in classified military environments, industrial control systems, and nuclear facilities.

### Physical Isolation
A physically isolated network is completely disconnected from any other network, period.
* ”Clean room” network/computer is located in a secured room or facility.
* Best practice on isolated systems is to have strict control over hardware and software devices.
* Use case: Creating digital code certificates
