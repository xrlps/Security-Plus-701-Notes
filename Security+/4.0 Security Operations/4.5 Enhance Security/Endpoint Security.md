- Endpoint - device used by a user
## Edge vs access control
- Control at the edge
	- The edge is where the inside of the network meets the outside
	- Internet link
	- Managed through [[Network-based Firewall#Firewall rules|firewall rules]]
- Access control
	- Limit a device's access to certain data
## Posture assessment/Health checks
- Checking devices to see that they are properly secured and up to date
- Includes [[Securing Wireless and Mobile#BYOD|BYOD]]'s
- Performed before a device connects to the network
- Checks one of the following
	- Device's certificate
	- Anti-virus running
	- Corporate applications installed
	- Disk encryption used
	- ...
- A proper response must be implemented if/when a device fails a posture assessment, like quarantining, etc
#### Persistent agents
- Permanently installed onto a system
- Performs [[Endpoint Security#Posture assessment|posture assessment]] on a regular basis, not just when connecting to a network
#### Dissolvable agents
- No installation required
- Runs during the posture assessment
- Terminates when no longer required
#### Agentless NAC
- Integrated with [[Operating System Security#Active directory (AD)|AD]]
- Checks are made during logins and logouts of the AD
## Endpoint detection and response (EDR)
- See [[Hardening Techniques#Endpoint detection and response (EDR)|Hardening Techniques]]
- Runs as an agent on an endpoint
## Extended detection and response (XDR)
- An evolution of [[Hardening Techniques#Endpoint detection and response (EDR)|EDR]]
- Increases the scope of investigations to more than just the endpoint; interprets data from multiple systems at once
- Added network-based detection
- Correlate endpoint, network, and cloud data
- Watches user behavior analytics
	- Creates a baseline of normal activity - requires data analysis over an extended period
	- Watches for any unusual traffic, using a set of rules, pattern matching, and statistical analysis
