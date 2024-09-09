## Intrusion Prevention System (IPS)
- Designed to watch traffic traverse the network and filter/discard malicious traffic, through the use of signatures
- Can filter one of the following
	- Exploits against OS's or applications
	- [[Application Vulnerabilities#Buffer overflow|Buffer overflows]]
	- [[Web-based#Cross-site scripting (XSS)|Cross-site scripting]]
	- [[Web-based#SQL Injection (SQLi)|SQL injection]]
	- ...
- May be used in conjunction with an **IDS** (Intrusion Detection System) to alert when receiving malicious traffic
## Failure modes
- The failure mode type is especially important when the system is connected [[Intrusion Prevention#Active monitoring|inline]]
#### Fail-open
- When a system fails, data continues to flow
#### Fail-closed
- When a system fails, data does not flow
## Device connections
#### Active monitoring
- System is connected inline
- Data can be blocked as it passes in real-time
- The [[Intrusion Prevention#Intrusion Prevention System (IPS)|IPS]] can block malicious traffic before it reaches a device
#### Passive monitoring
- A copy of the network traffic is examined, sent to the destined device, and the IDS or IPS
- Data cannot be blocked in real-time
- Does not block malicious traffic, only alerts when receiving a copy of malicious traffic
- Called an IDS design because the [[Intrusion Prevention#Intrusion Prevention System (IPS)|IPS ]]is configured to act as an IDS