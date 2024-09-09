- An attack when an attacker wants access to the raw network data
- Requires one or more of the following to work
	- Network tap
	- [[On-path Attack#ARP poisoning / spoofing|ARP poisoning]]
	- [[Malware|Malware]]
## Credential replay
- An attacker finds a way to receive a clients outgoing traffic
- An attacker uses the clients outgoing traffic to replicate a legitimate data stream (like account authentication)
- Can be mitigated with encryption, salting, or session IDs so that a server cannot accept a password more than once
#### Session hijacking (Sidejacking)
- An attack gets access to a clients session ID to login to their accounts without the need for a username, email, or password
- Can be prevented with end-to-end [[Encrypting data|encryption]] protocols like HTTPS 