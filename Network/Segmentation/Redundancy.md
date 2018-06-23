# Redundancy, Availability and Resiliency
Availability is a measure of a system's uptime — the percentage of time that a system is actually operational and providing its intended service.
* For example, ”five nines” means the device should be up 99.999% of time and experience no more than 5.26 minutes of downtime per year.
* Resiliency is the capability to continue operating even when there has been a disruption or abnormal operating conditions.

### Single Point of Failure
A single point of failure (SPOF) is an element, object, or part of a system that, if it fails, causes the whole system to fail.
* Redundancy is duplication of critical components or functions with the intention of increasing reliability and mitigating the risks associated with single point of failure.
* Redundancy can be configured to require manual intervention (e.g. spare parts) or to be automatic (fail-over).

### Fault Tolerance
Fault tolerance is the capability of a system to continue to operate in the event of failure of one or more system components.
* Fault tolerant systems rely on redundant components (e.g. power supply, disk storage).
* Components are continually monitored for availability.
* Failures are transparent to users (with the exception of potential degradation of service).

### Active vs. Passive Redundancy
In a fault-tolerant system, the redundant hardware is either active or passive.
* Passive (standby) components are inactive until a failure occurs.
* Active components operate in parallel with the primary system to provide continuous service without noticeable interruption.

### Redundant array of independent disks (RAID)
RAID is a disk technology that combines multiple disk drive components into a logical unit for the purposes of fault tolerance (data redundancy) and/or performance improvement.

### RAID Configurations
| RAID Level | Description | Objective |
|------------|-------------|-----------|
| 0 | Data written (striped) across multiple disks | Performance only |
| 1 | Data mirrored on two identical drives | Fault Tolerance |
| 5 | Data written (striped) across three or more | Fault Tolerance and Performance |
| 6 | Data written (striped) across three or more, Drives With one parity stripe, Can auto-recover one drive. | Fault Tolerance |
| 10 (1+0) | Data is simultaneously mirrored and striped across several drives (min four drives) | Fault Tolerance and Performance |

### Swapping
In a fault-tolerant system, failed components are repaired without system downtime. Swapping is the process of replacing a failed component.
##### Warm Swap
* Is the ability to insert and remove hardware while the system is in a suspended state.
##### Hot swap
* Is the ability to insert and remove hardware while the system is running.
##### Hot plug
* Is the ability to add a component without interruption.

### High Availability
High-availability systems are clustered into resource groups and software manages the resources.
##### Asymmetric HA (active/passive)
* Requires primary and standby systems. When a failure occurs, the stand-by device takes over.
##### Symmetric HA (active/active)
* Requires two primary systems. Each machine monitors the other (heartbeat) and takes over when a failure occurs.
