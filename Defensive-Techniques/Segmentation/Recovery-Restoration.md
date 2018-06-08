# Data and System Recovery
A key component of disaster recovery is the ability to restore systems and data. Restoration requires that accurate and reliable copies of data and system configurations are maintained and tested.
* Traditional backup strategies use removable media (generally tape).
* Current/emerging strategies use local or remote online storage.
* Order of recovery should be related to the BIA.

### Removable Media
Considerations for where the backup media is stored include:
* Location (on-site/off-site)
* Distance
* Accessibility
* Environmental controls
* Physical security
* Logical security

### Online Storae
Considerations for where the online files are stored include:
* Location (on-site/off-site)
* Country (political and regulatory considerations)
* Environmental controls
* Physical security
* Logical security
* Sovereignty/ownership

### Traditional Backup Strategies
| Type    | Backup Progress  | Restore Process  |
|---------|------------------|------------------|
| Full Backup | Backs up all files | Full backup media |
| Differential | Backs up all files created or modified. since last full backup. Does not reset archive bit | Full backup + most recent differential. |
| Incremental | Backs up all changed files, Does reset archive bit. | Full backup + all subsequent incremental. |

### Traditional Backup Rotation
|  Strategy |  Rotation |
|-----------|-----------|
| Son | One full backup cycle (generally daily). The daily full backups are rotated on a daily basis. |
| Father—Son | Two full backup cycles (generally weekly and monthly) The daily (incremental or differential) backups are rotated on a daily basis. The weekly backups are rotated on a weekly basis. |
| Grandfather-Father-Son | Three or more full backup cycles (generally weekly, monthly, and annually). The daily (incremental or differential) backups are rotated on a daily basis. The weekly backups are rotated on a weekly basis. Monthly backups are rotated on a monthly basis. |

### Automated Backup Strategies
| Strategy | Description |
|----------|-------------|
| Hierarchical Storage Management (HSM) | Continuous backup using optical or tape jukeboxes. |
| Cloud Backup Services | Scheduled backup to a Internet location. |
| Disk Shadowing | Data is written to (and read from) two or more independent disks Process is transparent to the user. |
| Electronic Vaulting | Copies files as they are Changed and periodically transmitted to a backup location. |
| Remote Journaling | Copies transactions logs and periodically transmitted to a backup location. |
| Automated System Recovery (ASR) | Disk image that can be used to restore operating system files. |

### Replication
Replication is an automated process that streams copies of data to one or more locations in real time or near-time.

### Replication Strategies
| Type     | Process      |
|----------|--------------|
| Point-in-Time | Periodic snapshots replicated If replicated, snapshots are pointer-based, just changes transmitted. |
| Asynchronous Replication | Write is considered complete as soon as local storage commits. Remote storage updated with a slight time lag. |
| Synchronous Replication | Data written in two locations (local and remote). Both write operations must successfully complete before the system can proceed. Guaranteed zero data loss. |

### Cost vs. Complexity vs. Availability
##### Traditional Recovery
* Tape backup
* Low Complexity
* Low cost
* Recovery measured in hours to days.

##### Enhanced Recovery
* Automated Solutions
* Medium Complexity
* Low Cost
* Recovery measured in hours to days.
* More recoverable data.

##### Rapid Recovery
* Asynchronous Replication
* High Complexity
* Moderate cost
* Recovery measured in hours.

##### Continuous Availability
* Synchronous Replication
* High Complexity
* High cost
* Recovery measured in seconds
