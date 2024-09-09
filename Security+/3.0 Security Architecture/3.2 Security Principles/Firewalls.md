- Control the flow of traffic between two ports
- Filter against the type of content inside traffic
- Protect against malicious content
## Network-based firewalls
- Control traffic through the use of a purpose built device
- Encrypt traffic
	- VPN between sites
- Can be layer 3 devices (routers)
	- Provide NAT
	- Authenticate dynamic routing protocol communication
#### Traditional Firewall
- Control traffic based on OSI layer 4
#### Next Generation Firewall (NGFW) 
- Control traffic based on OSI layer 7
- Often called
	- Application layer gateway
	- Stateful multilayer inspection
	- Deep packet inspection
- Performs full packet decoding for all packets traversing the network
- Can view specific application layer content, for example
	- Allow users to scroll on YouTube but not post
- Has a list of known vulnerabilities, like an [[Intrusion Prevention#Intrusion Prevention System (IPS)|IPS/IDS]]
## UTM/All-in-one security appliance
- Unified Threat Management (UTM) or Web security gateway
- Handle many different services at once, including:
	- URL filtering and content inspection
	- Malware inspection
	- Filter for spam
	- Routing and switching
	- CSU/DSU
	- [[Firewalls#Network-based firewalls|Firewall]]
	- [[Intrusion Prevention#Intrusion Prevention System (IPS)|IPS/IDS]]
	- Bandwidth shaper, for QoS
	- VPN endpoint
## Web application firewall (WAF)
- Analyze input into web application
	- Applies rules to HTTP/HTTPS conversations
	- Allow or deny based on expected inputs, like [[Web-based#SQL Injection (SQLi)|SQL injections]], which can exploit an application