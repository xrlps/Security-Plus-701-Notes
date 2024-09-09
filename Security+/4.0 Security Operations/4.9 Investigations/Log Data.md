- Detailed security-related information
	- Blocked and allowed traffic flows
	- Exploit attempts
	- Blocked URL categories
	- DNS sinkhole traffic
- Log data is usually all aggregated on a [[Security Tools#SIEM|SIEM]]
## Types/Methods of logging
#### Firewall logs
- Logs the source/destination IP, port numbers, disposition
- [[Network-based Firewall#Next-generation Firewall (NGFW)|NGFW]]'s log the application used, URL filtering categories, anomalies and suspicious data
#### Application logs
- Windows - event viewer / application log
- Linux/macOS - /var/log
#### Endpoint logs
- Endpoint events are correlated with [[Network-based Firewall#Intrusion Prevention System (IPS)|IPS]] data to determine a specific security event
#### OS security logs
- Monitoring applications
- Authentication details
#### IPS/IDS logs
- Usually integrated into an [[Network-based Firewall#Next-generation Firewall (NGFW)|NGFW]]
- Contain information about known vulnerabilities and generic security events
#### Network logs
- Switches, routers, access points, VPN concentrators
- Log any network changes
	- Routing updates
	- Authentication issues
	- Network security issues
## Metadata
- Data that describes other data sources
- Contains detailed information about general data
###### Example
- An image contains the following metadata
	- Type of phone
	- GPS location
	- Date taken
## Vulnerability scans
- See [[Vulnerability Scanning]]
## Automated reports
- Report generators are built into a [[Security Tools#SIEM|SIEM]] or created by a third-party
## Dashboards
- Real-time information status of operating systems
- Predefined or built into a [[Security Tools#SIEM|SIEM]]
## Packet captures
- Gathers packets on the network or in the air
- Allows viewing of detailed traffic information
