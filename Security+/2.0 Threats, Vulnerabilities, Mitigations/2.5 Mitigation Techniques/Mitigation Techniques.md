- The process of reducing the impact of a security event or potential security event
## Patching
- Frequent updates increases security and system stability
- Scheduled patches
	- Monthly, quarterly
- Unscheduled patches
	- Needed to quickly fix an active exploit
## Encryption
- Encrypting data limits the amount of access that an attacker has
- File level encryption - Windows EFS
- Full disk encryption (FDE)
## Monitoring
- Logging information from devices can help identify security events
- May be integrated into devices
- A a [[Security Tools#SIEM|SIEM]] is often used
## "Least privilege"
- Limiting the amount of devices with administrative access
- By default, all users have limited access - reducing the scope of a potential attack
## Configuration enforcement
- Performing a **posture assessment** - checking device patch version, [[Hardening Techniques#Endpoint detection and response (EDR)|EDR]] version, certificate status
- Systems that are out of compliance may be quarantined until they pass the posture assessment
## Decommissioning
- Destroying or deleting information from previously used devices
- Mostly associated with storage devices
	- Hard drives
	- SSD
	- USD drives