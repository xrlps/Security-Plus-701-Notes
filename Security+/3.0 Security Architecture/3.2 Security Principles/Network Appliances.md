## Jump server
- A device that is on the inside of a network that allows access to outside, authorized devices
- Potential security concern
#### Connection process
1. An authorized external client connects to the jump server via SSH, tunnel, or VPN
2. Once connected, RDP, SSH, or "jump" to the destination 
![[Screenshot 2024-08-25 154114.png]]
---
## Proxy server
- Sits in the middle of devices and makes requests on the behalf of a user
- Useful for caching information, access control, URL filtering, content scanning, etc
#### Explicit proxy
- The proxy must be configured on the application of the client so that applications know how to use the proxy
#### Transparent proxy
- The end user is not aware of the use of the proxy
#### NAT proxy
- Translates a private IP address to a publicly routable IP address
#### Application proxy
- The proxy understands the way the application works
- A proxy may only know one application
	- HTTP
- Many proxies are multipurpose proxies
	- HTTP, HTTPS, FTP, etc
#### Forward proxy
- An internal proxy
- Proxies information from a source to a destination
1. A user sends traffic to a proxy server
2. A proxy server forwards this traffic to the internet (or to any destination) on the behalf of this user
3. The proxy server receives the response and checks the validity of the message - whether or not it is malicious
4. If valid, the server forwards the response back to the client
#### Reverse proxy
- Receives traffic from outside a network (like the internet) and forwards it to devices inside the internal network, on the outside device's behalf
- Can act as a caching server
#### Open proxy
- Receives inbound traffic from anyone and forwards it to the internet
- The proxy server can be a security concern since it can modify traffic
---
## Load balancer
- Takes load from one direction and distributes the load to multiple servers
- Invisible to the end user
- Provides [[Infrastructure Considerations#High availability (HA)|fault tolerance]]
![[0_CCK15OF3DizmOITk-624262550.png]]
#### Active/active load balancing
- All servers connected to a load balancer are active and are being used
- The load balancer can:
	- Configure/manage the load
	- Provide TCP offloading - doesn't need to setup a TCP connection for every user connecting to the servers; keeps a single TCP connection open for every user (for each server)
	- SSL offload
		- The load balancer decrypts the response from the user, sending unencrypted traffic to the server (to offload resources from the server). Data from the server to the load balancer is sent unencrypted, to which the load balancer will encrypt it before sending it out to the user
	- Cache data to provide faster responses
	- Prioritize traffic using QoS
	- Provide content switching to recognize type of requests being made to send specific requests to certain web servers
#### Active/passive load balancing
- Some servers are active, while other servers are on standby
- If an active server fails, the standby/passive server takes its place
---
## Sensors and collectors
- Traditional network devices like routers, switches, firewalls, etc, may have built in sensors
	- These sensors help aggregate information, like logs, from the devices
- Sensors can be installed as separate devices, with the purpose of collecting statistics from networking devices
- A **collector**, is a centralized database that collects all the statistics from sensors
	- A proprietary console (IPS, firewall)
	- A [[Mitigation Techniques#Monitoring|SIEM]] console
	- Syslog servers