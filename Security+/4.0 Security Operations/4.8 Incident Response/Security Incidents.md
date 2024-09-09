## Preparation
- Communication methods
	- Contact information for those that must be informed when an incident takes place
- Incident handling hardware and software to mitigate the incident
- Incident analysis resources
	- Documentation, network diagrams, critical file hash values etc
- Incident mitigation software
	- Ready to use backup or replacement software
- Policies to follow
## Detection
- Proper policies and procedures must be clearly defined to detect an incident
## Analysis
- Deep and frequent analysis of [[Security Monitoring#Logging|logs]] to determine any attempted attacks to prepare for future potential ones
- Reading reports from [[Network-based Firewall#Intrusion Prevention System (IPS)|IPS]] or [[Security Tools#Anti-virus and anti-malware|anti-malware]] to detect attacks that are underway or have been successful 
## Isolation and containment
- Stop the attacker from running their attack as soon as detected to prevent spreading
- Using [[Application Security#Sandboxing|sandboxes]]
## Recovering
- Eradicating the bug
	- Remove malware
	- Disabled breached user accounts
	- Fix vulnerabilities
- Recover the system
	- Restore from a good backup or rebuild from scratch
	- Remove or replace compromised files
## Reflection
- Hosting a **post-incident meeting**
	- Invite everyone affected by the incident
	- Host the meeting as soon as the incident is resolved
#### Questions to ask
1. What happened
2. How did the incident plans work out
3. What would be done differently
4. What indicators to watch for next time
## Training for an incident
- Train the team *prior* to an incident; be ready when an incident is identified
	- Initial response
	- Investigation plans
	- Incident reporting
	- ...

