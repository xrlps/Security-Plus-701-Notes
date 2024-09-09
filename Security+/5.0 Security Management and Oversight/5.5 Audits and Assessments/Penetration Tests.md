## Physical penetration testing
- OS security can be circumvented by physical means - physical security is an underrated aspect of securing systems
- Access and test physical security
	- Test entering buildings without keys
	- Check doors, windows, elevators, etc
	- ...
## Pentesting perspectives
#### Offensive
- Red teamers
- Attack the system and look for vulnerabilities to exploit
#### Defensive
- Blue teamers
- Identify attacks in real-time
- Prevent unauthorized access
#### Integrated
- Using a combination of both red and blue teamers
- Red teamers attack a system. After finding a vulnerability, they pass the information to blue teamers who patch the system
#### Working knowledge
- How much a pentester knows about the test
- Known environment
	- The organization gives full disclosure of the environment to the pentester
- Partially known environment
	- A mix of known and unknown
	- Focus is on certain systems or applications
- Unknown environment
	- The pentester knows nothing about the system
	- "blind test"
#### Reconnaissance
- Used by the pentester to understand as much as they can about the security posture of the network
	- i.e. Firewalls, security configurations, applications running, open ports
- Helps determine the focus on key systems
###### Passive reconnaissance
- Learn as much as you can from open sources - not directly interacting within the customers network
	- i.e. Social media, corporate website, forums, social engineering
###### Active reconnaissance
- Directly interacting with the network to understand the security posture
- Visible on network traffic and logs
- Relatively easy to be seen
- i.e. Ping sweep, port scan, OS scans, DNS queries