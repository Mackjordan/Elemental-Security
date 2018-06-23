# Business Impact Analysis

The objective of a Business Impact Analysis (BIA) is to identify the impact of a disruption on mission-essential services, systems, and infrastructure.

* Essential means that the absence of or disruption of services would result in significant, irrecoverable, or irreparable harm to the organization, employees, business partners, constituents, community, or country.

### BIA Use Case
A Business Impact Analysis (BIA) is used by management to:
* understand organizational continuity requirements
* make investment decisions
* guide the development of incident response, disaster recovery, and business contingency (continuity) plans.

### Fundamental BIA Questions
The BIA process should answer the following questions.
* What is the organization’s essential business process?
* What is the impact of a disruption (e.g. life, property, safety, finance, reputation)
* What are the related resources (critical systems) and dependencies including single point of failure? SPOP
* What are the process, system, and data recovery requirements (e.g order of restoration)?
The outcome of BIA is a prioritized matrix of services, systems, and infrastructure.

# Business Impact Metrics
| Abbr | Metric | Definition |
|------|--------|------------|
| MTD | Maximum Tolerable Downtime | Maximum time a process/service can be unavailable without causing significant harm to the business. |
| MTO | Maximum Tolerable Outage | Maximum time a process/service can be unavailable without causing significant harm to the business. |
| RTO | Recovery Time Objective |Amount of time allocated for system recovery. Must be less than the maximum amount of time a system resource can be unavailable before there is an unacceptable impact on other system resources or business process. |
| RPO | Recovery Point Objective | Acceptable data loss. The point in time, prior to a disruption or system outage that data can be recovered. |
| MTBF | Mean Time Between Failures | Measure of reliability (using stated in hours) |
| MTTR | Mean Time to Repair | Average time to repair a failed component or device. |


### RPO | RTO Timeline
* RPO = 90 Minutes
* RTO = 3 Minutes  

___<___ Recovery Point Objective <___Failure___> Recovery Time Objective ___>___

___Weeks Days Hours Minutes___ ----------        ___Minutes Hours Days Weeks___   

### Business Impact Analysis Process
1. Identify Essential Services & Dependencies
2. Determine Maximum Tolerable Downtime (MTD)
3. Determine Recovery Point Objective (RPO)
4. Identify Infrastructure and Dependencies inc. MTBF and MTTR
5. Determine Current RTO & RPO
6. Gap Analysis
7. Report to Management
