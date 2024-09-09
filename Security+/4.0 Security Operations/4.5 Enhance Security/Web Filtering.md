## Content filtering
- Controls traffic based on data with the application content
	- URL filtering, website category filtering
- Controls inbound and outbound data
- Protection against malicious sites known to have malware
#### URL scanning
- Allow or restrict based on URL/URI
- Based on [[Web Filtering#Block rules|block rules]]
- Often integrated into [[Network-based Firewall#Next-generation Firewall (NGFW)|NGFW]]'s
#### Agent-based
- Software installed on a client to filter out traffic
- Usually managed from a central console
- Users can be located anywhere to have the filters still be applied
#### Proxies
- Can be used for content scanning
- See [[Network Appliances#Proxy server|Network Appliances]]
#### Block rules
- Based on a specific URL 
	- * .testsite.com
- Usually managed by category of website, rather than specific URL domain 
	- Gambling, hacking, malware, news, etc
- Different dispositions, example
	- Educational: Allow
	- Home and garden: Allow and alert
	- Gambling: Block and alert
#### Reputation
- Filter URLs based on the perceived risk of the data on the site
	- Good reputation - allowed
	- Bad reputation - blocked
- Different levels of reputation
	- Trustworthy
	- Low risk
	- Medium risk
	- Suspicious
	- High risk
- Often automated - sites are scanned and assigned a reputation
- Managers can administratively assign a reputation
#### DNS filtering
- Configuring a DNS server to not provide a user with the IP address of the domain name - prevent DNS lookup based on domain
- 