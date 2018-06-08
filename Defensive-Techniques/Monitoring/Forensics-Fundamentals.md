# Forensics Investigation Fundamentals
Forensics is the process of using scientific knowledge for collecting, analyzing, and presenting evidence.
* Digital forensics is the application of science to the identification, collection, examination, and analysis of data (evidence) while preserving the integrity of the information.

### Digital Forensics Investigation Process
1. Evidence Collection
2. Data Acquisition
3. File Recovery
4. Examination
5. Analysis and Reporting
6. Testifying (If Necessary)
7. Archiving

### Evidence Collection and Preservation
Collection and preservation of physical and digital evidence is a critical aspect of forensic investigations. Rule of thumb—assume evidence will be used in a court of law and act accordingly.
* Preservation is key
* Act in order of volatility
* Maintain an evidentiary chain (Chain of Custody) for all physical and electronic evidence collected during the investigation.

### Digital Evidence
Digital evidence is any information or data of value to an investigation that is stored on, received by, or transmitted by an electronic device including:
* Device memory
* Media such as hard drives, USB drives, tapes, and other storage devices
* Logs, records, and audit trails
* Text messages, emails, pictures and videos, and Internet searches

### Preservation
Whenever possible, potential evidence should be kept as pristine as possible.

Contaminants include:
* Installing or run any diagnostic tools or scanning software
* Deleting files.
* Making any changes to the system including logging the user out
* Turning off the device (memory forensics is possible only if a device has not been turned off)

### Forensic Triggers
Scenarios that may trigger a forensic investigation include (but are not limited to)
* Malware (e.g. Border alert (IDS/FW/Filtering/logs, Local AV/lDS/Sandbox alerts, Execution — e.g. CryptoLocker)
* Disruption (e.g. DDoS)
* Unusual or suspicious activity (evidence based, hunch/gut)
* Situation at a connected source
* Threat Intelligence
* External notification (FBI, Secret Service)

### Legal Hold
A legal hold is an order that suspends the modification, deletion, and/or destruction of records and media.
* A legal hold can be issued to avoid evidence spoliation.
* Evidence spoliation is the intentional, reckless, or negligent withholding, hiding, altering, fabricating, or destroying of evidence.

### Order of Volatility
Order of Volatility refers to the acquisition of evidence before it disappears, is overwritten, or no longer useful. The goal is to create a snapshot of the environment as it existed at the time of the attack or incident.

For example:
1. Dynamic data (RAM)
2. Dump files
3. Temp files
4. Log files
5. Static data (media)

### Chain of Custody
A chain of custody establishes the proof that the items of evidence collected at the crime scene is the same evidence that is being presented in a court of law:
* Identifying information (e.g., the location, serial number, model number, hostname, media access control (MAC) addresses, and IP addresses of a computer)
* Name, title, and phone number of each individual who collected or handled the evidence during the investigation.
* Time and date (including time zone) of each occurrence of evidence handling
* Locations where the evidence was stored.

### Administrative Forensic Procedures
| Procedure     |  Description                                        |
|---------------|-----------------------------------------------------|
| Keep a log | Record all investigative activity—date, time, details. |
| Record Time Offset. | Record any differential between true and evidence time stamp. |
| Talk to Witnesses | Record witness statements as soon as possible. |
| Take pictures (screenshots) and videos | Capture information without chance of contamination. |
| Track Resources | Track man-hours, expenses and equipment costs. |
| Retention Policy | Determine how long evidence must be retained for and under whose control. |

### Data Acquisition
Action:
* Protect evidence from contamination.
* Acquire data in order of volatility.
* Use forensically sound memory and hard drive acquisition tools.
* Hash (fingerprint) the hard drives pre and post imaging.


### Data Acquisition Tools
| Tool           | Purpose                                  |
|----------------|------------------------------------------|
| Memory Imaging | Acquisition of short-term volatile data. |
| Write Blocker | Tool that intercepts inadvertent drive writes. |
| Bit Stream Image | Bit-by-bit copy of the source material that preserves all latent data in addition to files and directory structure Accessing an image does not modify its data. |
| Clone | Exact copy of the entire physical hard drive including all active and residual data and unallocated or slack space A cloned hard drive can be installed into the computer, and the computer will reboot and function as if the original drive were still installed. |

### Fingerprint for Authenticity & Integrity
(Hash of the Original) is equal to (Hash of the cloned media) and / or (Has of the examined media)

### File Recovery    
| Type  |  Purpose  |
|-------|-----------|
| Cluster | Fixed length blocks of disk space. Documented In a File Allocation Table or equivalent. |
| Slack space | Space between the end of a file and the end of the cluster. Slack space can contain data from RAM or segments of deleted files. |
| Unallocated (free) space | Clusters that are not allocated to a file. Clusters can contain deleted file fragments.  Carving is the process by which deleted files or fragments are recovered. |
| Metadata | Data about data — file system, application, pseudo. |

### Metadata
| Type            | Description           | Examples                           |
|-----------------|-----------------------|------------------------------------|
| File System Metadata | Created by the operating system and includes file attributes and security permissions. | File size, location, creation date, of last access, data of last write, and whether a file is hidden, compressed, or archived. |
| Application Metadata | Created by the specific application and includes user and file activity information. | Title, author, subject, keywords, creation and modification dates, time in use, and revision history. |
| Pseudo Metadata | Created by the user and is hidden or embedded in the document | Comments, track changes, formulas, speakers notes, embedded graphics, and audio or video files. |

### Active Logging
It is important to continue to (or start to) capture and analyze log data as it may be pertinent to the investigation.

### Examination
Forensic examination should be conducted by trained personnel. It is easy to contaminate or destroy evidence. The examiner should document all activity including action taken, tools or procedures used, and results.
* There are a number of open source and commercial forensic products available.
* Whenever possible, examinations should be conducted on exact images or replicas and not on the original data source.
