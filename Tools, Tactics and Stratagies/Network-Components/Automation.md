# Automation
The goal of automation is to improve quality of service, increase agility, and reduce risk.
* Automation reduces or eliminates manual dependencies and human error.
* Automation initiatives can be tactical (e.g. automatic patching) or strategic (tied to a business objective).

### Risk Reduction
Risk is the measurement of the likelihood and the impact of a threat event occurring.
* Risk is mitigated when controls are implemented that reduce the likelihood or the impact (or both).
* Automation can be used to mitigate (lower) risk.

### Automation initiatives
##### provisioning
* Automatic provisioning and de-provisioning of resources based upon demand (e.g. scalability, elasticity)

##### Non-presistence
* Changes are not permanent. Endinga session will force a reset

##### information Security Continuous Monitoring (ICSM)
* Ongoing awareness of information security, vulnerabilities, and threats to support organizational risk management solutions (e.g. vulnerability scanning, configuration and patch management, anti-malware tools, network configuration management, and audit)

##### configuration Validation
Compare and validate configurations between a master (reference) system and target systems.

##### Imaging
Build and deploy preconfigured standardized servers and desktops

### Templates and Images
Templates and master images are used to standardize builds, manage configurations, and support rapid deployments.
* A master image is a copy of the ref- n-ce system. A master image is also known as a golden image or a parent image. Images are used in both the physical and virtual  environments.  
* A template is a pre-configured virtual machine used for multiple deployments. Virtual configuration files have .vmtx extensions.

### Nonpresistance
##### Snapshot
* A copy of a system state at a point in time.
* Snapshots are used in both physical and virtual environments for
recovery purposes.
* A VM snapshot includes all of the files that make up the virtual
machine. This includes disks, memory, and other devices, such as
virtual network interface cards.

##### Revert to Known State
* The known good point to which a system can recover.
* Microsoft operating systems refer to this as Last Known Good.
* Databases refer to this as a Checkpoint.

##### Rollback to Known Configuration
* Restores the system to a chosen earlier point in time.
* Leaves file intact.

##### Live Boot Media
* Bootable media that creates a temporary non—persistent end node.

### Scalability
Scalability is the ability of the system to automatically accommodate larger loads by adding resources — either making hardware stronger (scale up) or adding additional nodes (scale out).
* Scalability adapts to the "Work increase" by "Provisioning" the resources in an " Incremental" manner.
* Scalability enables organization to meet expected demands for services.
* Scalability is one of the primary drivers of cloud adoption.

### Elasticity
Elasticity is the ability to fit the resources needed to cope with loads dynamically. When the load increases, more resources are added and when demand decreased, resources are removed.
* Elasticity adapts to both the “workload increase” as well as "workload decrease“ by "provisioning and pre-provisioning" resources in an"'autonomic" manner.
* In the elastic environment, the available resources match the
"current demands" as closely as possible.
* Elasticity enables an organization to meet unexpected changes in the demand for services.
* Elasticity is important in pay-per-use cloud environments.
