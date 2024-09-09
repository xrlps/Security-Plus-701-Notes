## Virtual Private Network (VPN)
- [[Encrypting data|Encrypts]] data traversing a network
- Managed with a **concentrator**
## Concentrator
- A purpose built device designed to be the endpoint for host devices to connect to
- Can be deployed with
	- A firewall
	- Software-based solutions
	- Client software that allows hosts to connect and authenticate to the concentrator
## VPN Encryption
- A user encrypts their traffic then sends it over the internet. The receiving VPN concentrator decrypts the traffic and sends it to the destination network
- The original packet (incl. IP header and data) is encrypted
	- This encrypted packet is embedded into a new packet, with an IP header, IPsec Header, and IPsec trailer
#### VPN IP Header
![[ipsec-esp-transport-mode-ip-packet-2993670845.png]]
## SSL/TLS (Secure Sockets Layer VPN)
- On-demand access to a network from a remote device
- A VPN client installed on a host or ran on a browser - the sending client encrypts the traffic
- The traffic reaches a [[Secure Communication#Concentrator|VPN concentrator]], who decrypts the traffic and sends it to its destination
## Site-to-site IPsec VPN
- Always-on access to a network from a remote network
- The client sends unencrypted traffic to a [[Firewalls|firewall]] who acts as a [[Secure Communication#Concentrator|VPN concentrator]], who encrypts traffic, forwards to another firewall who decrypts the traffic, that sends the unencrypted traffic to the destination
## SD-WAN
- Software Defined Networking in a Wide Area Network
- A WAN built for the cloud
- With SD-WAN, cloud-based applications can communicate directly to the cloud, without needing to communicate through a central point
#### Secure Access Service Edge (SASE)
- A next generation VPN
- SASE clients are installed on all devices
- Allows for secure connections when using [[Secure Communication#SD-WAN|SD-WAN]]
- Places security technologies in the cloud, located close to the existing cloud services