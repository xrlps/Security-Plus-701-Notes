- Networks are constantly being monitored for potential attackers
- Monitor all entry points
	- Logins
	- Running services
- Usually displayed in a status dashboard
## Computing resources to monitor
#### Systems
- Authentication - logins from strange places
- Server monitoring - service activity, backups, software versions
#### Applications
- Availability - uptime and response times
- Data transfers - increases or decreases in rates
- Security notifications - from the developer/manufacturer
#### Infrastructure
- Remote access systems - employees, vendors, guests
- Firewall and IPS reports - increase or type of attack
## Logging
- Contains information about device, system, and application activity
- Log aggregation platforms like [[Security Tools#SIEM|SIEM]] are used to consolidate different logs from distant resources to a single system
## Scanning
- The threat landscape is constantly changing, so [[Vulnerability Scanning|scanning]] must be actively performed
- Check systems and devices
	- OS versions
	- Installed applications
	- Potential anomalies
- Gather as much raw details into a database to be [[Security Monitoring#Reporting|reported]] on later
## Reporting
- Analyzing the data gathered from scanning
	- Create "actionable" reports - what to do next based on reports
- Ad hoc reports may be created
	- Determine the result of a "what if" scenario
## Archiving
- Archive data over an extended period
- May be mandated
	- State or federal law
	- Organizational requirements
## Alerting
- Real-time notification of security events
	- Increase in authentication errors
	- Large file transfers
- Notification methods
	- SMS
	- Email
	- Security console/SOC
#### Alert response and remediation
- Quarantine
	- Locking a vulnerable system to prevent a potential security issue from spreading
- Alert tuning
	- Prevent false positives and false negatives
- 