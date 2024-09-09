- Important for disaster planning
- Many different implementations
	- Total amount of data
	- Type of backup
	- Backup media
	- Storage location
	- Backup and recovery software
	- Day of the week
- Backups should be tested with [[Recovery Testing|recovery testing]]
## Location
- Organizations often use a combination of [[Backups#Onsite backup|onsite]] and [[Backups#Offsite backup|offsite]] backups
#### Onsite backup
- The data and backup media are located in the same location
- Data is immediately available
- Quick restoration
#### Offsite backup
- Data is transferred to different locations over the internet or WAN link
- Restoration can be performed from anywhere
- Long term storage backups
## Frequency
- How often to backup
- May have multiple backup sets
	- Daily, weekly, and monthly
## Encryption
- Backup data should be encrypted, so that the data is only readable to those with the recovery key
- Especially useful for cloud backups and storage
## Snapshots
- Useful on virtual machines and cloud environments
- An instant backup of an entire system
	- Saves the current configuration and data
- Easy to tell the data changed when comparing to previous snapshots
## Replication
- Take a single source of data and backup to multiple locations at almost real-time
- If a disaster happens at the main source, the replicate data can be used to restore with the most up to date data
## Journaling
- Power goes out while writing data to storage - this data is likely corrupted
	- Recovery can be complicated, remove corrupted files, restore from backup
- Before writing to storage, write that data to a journal entry. Once the journal is written, write the data to storage
- If the system goes down once the journal has been written and the data has not been written to storage, once the system goes up, it can read from the journal and update itself with the new data
- 