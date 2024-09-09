## Security Content Automation Protocol (SCAP)
- Consolidates vulnerabilities to a single format that many different security tools can understand
- Allows for different security tools to work together
## Benchmarks
- Applying security best practices to everything
	- OS, connections to cloud providers, mobile devices
## Agents/agentless compliance checks
- Check to see if the device is in compliance
	- Install a software agent onto the device
	- Run an on-demand agentless check
- Agents usually provide more detail
- Agentless runs without a formal install
## Security Information and Event Manager (SIEM)
- Consolidate all different logs to create a central source
- Compares different types of data - application access, authentication to devices, data transfer
- Can get information from servers, firewalls, VPN concentrators, SANs, cloud services, etc
- Includes a reporting engine
- See [[Mitigation Techniques#Monitoring|Mitigation Techniques]]
## Anti-virus and anti-malware
- Malware refers to the broad malicious software category
- Anti-malware refers to the security tool that stops
	- Spyware
	- Ransomware
	- Fileless malware
- Anti-virus refers to a specific type of malware
	- Trojans, worms, macro viruses
## Data loss prevention (DLP)
- Used to look for and block specific types of data on a system
	- Blocking social security numbers, credit card numbers, etc
- Prevents data leakage
- Often requires multiple solutions
	- Endpoint clients - DLP installed on a host; monitors **data in use**
	- On network devices - monitors **data in motion**
	- On a server - monitors **data at rest**
	- Cloud-based systems - monitors data entering and exiting the cloud system; can block malware, viruses, etc
## SNMP
- Simple Network Management Protocol
- A management protocol used to either request device statistics or be alerted when a specific policy has occurred
- Contains a database of data (MIB) - Management Information Base
- The database contains OIDs - Object Identifiers
- A network management station (like a router) can poll a device asking for statistics
	- The NMS uses UDP port 162
#### SNMP trap
- Allows a device running the SNMP agent to proactively send messages to an NMS over UDP 161
- Traps must be configured with policies, i.e. - send an SNMP trap after 5 CRC errors
## NetFlow
- Gather traffic statistics from all traffic flows
- NetFlow probe
	- Watches network communication
	- Can be built into a router or switch, or a standalone NetFlow probe device
	- Sends a copy of network records to the collector
- NetFlow collector
	- Creates reports and details about traffic flows
## Vulnerability scanner
- See [[Vulnerability Scanning]]
