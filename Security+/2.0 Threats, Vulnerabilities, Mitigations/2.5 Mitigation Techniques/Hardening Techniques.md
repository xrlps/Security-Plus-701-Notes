- Ways to increase the security of a device or a system
## System hardening 
- Frequent updates
- Implement password complexity policies
- Limit the privilege level of accounts
- Limit access to devices
- Add anti-virus and/or anti-malware
- Changing from default password or device configuration
## Encryption
- [[Mitigation Techniques#Encryption|See mitigation techniques]]
- Encrypt all network communication through VPNs
## Endpoint detection and response (EDR)
- A method of threat protection from malware to help combat existing and complex malware
- Can detect threats through mechanisms like
	- Behavioral analysis
	- Machine learning
	- Process monitoring
	- Signatures
- Can perform [[Incident Planning#Root cause analysis|root cause analysis]]
- May isolate a system, quarantine a threat, or rollback to previous configurations
## Host-based firewall
- Software-based firewall that allow or deny ingress and egress application traffic
- Runs on individual devices; can be managed from a central console
## Host-based Intrusion Prevention System (HIPS)
- Built into [[Hardening Techniques#Endpoint detection and response (EDR)|EDR]] or anti-malware software
- Watches traffic inbound to a single system to check for traffic that may be known vulnerabilities
- Secures OS and application configurations
- Looks for signatures, heuristics, or behavioral changes
	- If a core file gets changed, an alert can be sent
## Open ports and services
- Limiting the number of open ports
- Controlling port access with a firewall
## Removing unnecessary software
- Removing [[Spyware & Bloatware#Bloatware|bloatware]] can lower the changes of exploitation as a higher number of applications can increase the chances of an insecure application
