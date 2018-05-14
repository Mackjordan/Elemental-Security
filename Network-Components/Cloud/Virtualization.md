# Virtualization
Virtualization is technology that creates multiple environments from a single physical hardware system. In essence, a single physical machines emulates multiple systems. Server virtualization allocates the resources of the host to guest server (virtual) computers.
* The physical host computer hardware has processor, memory, storage, and networking components. Specialized software dynamically allocates resources.
* Guest computers (virtual machines) act exactly as though they are physical machines each with independent operating systems, applications, and network connections.

### Virtual Machines Concepts
##### Portioning
* Run multiple operating systems on one physical machine.
* Divide system resources between virtual machines (automatic resource allocation).

##### Isolation
* Provide fault and security isolation at the hardware level.
* Preserve performance with advanced resource controls.

##### Encapsulation Recovery
* Save the entire state of a virtual machine to files.
* Move and copy virtual machines as easily as moving and copying files.

#### Hardware Independence
* Provision or migrate any virtual machine to any physical server.

##### High Available
* Support application high availability (failover clustering) and ensure that services are always available when running inside VMs.

### Hypervisors
Hypervisors are software or firmware components that can virtualize system resources.
* Type 1 (bare metal/native) hypervisors run directly on the system hardware.
   * Direct access to hardware. No operating system to load as the hypervisor is the operating system (e.g. VMWare vCenter)
* Type 2 (hosted) hypervisors run on a host operating system that
provides virtualization services.
   * Type 1 is faster and more efficient but with greater hardware requirements and expense.

https://csrc.nist.gov/publications/drafts/800-125a/sp800-125a_draft.pdf

### Containers
Containers are the products of operating system virtualization without a hypervisor.

* Containers provide a lightweight virtual environment (instances).
* 0S containers are virtual environments that share the kernel of the host operating system but provide user space isolation.
* Application containers are virtual environments that share the kernel of the host operating system designed to package and run a single service

https://csrc.nist.gov/publications/drafts/800-190/sp800-190-draft2.pdf

### Network Virtualization
Network Virtualization (NSX) is the complete reproduction of a physical network in software.
* Network Virtualization presents logical networking devices and services (e.g. logical ports, switches, routers, firewalls, load balancers, VPNs).
* Virtual networks offer the same features and guarantees of a physical network with the operational benefits and hardware independence of Virtualization.

https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-125B.pdf

### Desktop Virtualization (VDI)
Virtual Desktop Infrastructure (VDI) is virtualization technology that hosts a desktop operating system on a centralized server in a data center.
* Persistent VDI provides each user with his or her own desktop which can be customized and saved for future use, much like a traditional physical desktop.
* Nonpersistent VDI provides a pool of uniform desktops that users can access when needed. Nonpersistent desktops revert to their original state each time the user logs out.

### VM Sprawl and Avoidance
Virtualization sprawl occurs when the number of virtual machines is out of control — potentially unmanaged, unnecessary and not in compliance with licensing agreements.
* Virtual machines should be treated the same as physical computers and subject to asset management, capacity, and configuration management.
* Virtual machine lifecycle management dashboard tools show. how many virtual machines are running on a network, which physical machines are hosting them, where their storage is located, what software or operating system (OS) licenses are associated with them, and who created them.

### VM Escape Protection
A virtual machine escape occurs when a virtual machine and the host operating system interact. This should never happen.
* Over time, multiple exploited vulnerabilties ave been identified.
* It is essential that VM hosts are included in organizational vulnerability and patch management programs.
