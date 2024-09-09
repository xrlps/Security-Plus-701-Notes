## Data at rest
- Data stored on a storage device
	- Hard drive, SSD, flash drive, etc
- Should be encrypted
	- Whole disk encryption
	- Database encryption
	- File or folder encryption
- Apply permissions to this data via
	- Access control lists
## Data in transit
- Data transmitted over the network
- If not encrypted, there is not much protection as the data travels
- [[Firewalls|Firewalls]] or [[Intrusion Prevention|IPS]] can set policies to prevent unknown or malicious traffic from traversing the network
- Encryption technologies like [[Secure Communication#SSL/TLS (Secure Sockets Layer VPN)|TLS]] or [[Secure Communication#Site-to-site IPsec VPN|IPsec]] can be used to provide additional security
## Data in use
- Data is actively processing in memory
	- System RAM, CPU registers, cache
- Almost always decrypted - often a target to attackers
## Data sovereignty
- Data that resides in a country is subject to the laws of that country
- Laws may prohibit where data is stored, for example (**GDPR**)
	- Data collected on EU citizens must be stored in the EU
## Geolocation
- Uses technologies to determine where a user is
- Can use one of the following technologies
	- GPS - very accurate
	- 802.11 wireless - less accurate
	- IP address - not very accurate
- Geolocation can be used to manage data access, preventing access to or from different countries
