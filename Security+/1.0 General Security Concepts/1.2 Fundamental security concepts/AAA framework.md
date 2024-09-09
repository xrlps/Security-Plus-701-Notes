- Used for managing and securing access to a system and its resources
## Authentication
- Prove a user is who they claim to be via [[Non-repudation#Identification|identification]]
- Passwords and other authentication factors
## Authorization
- Based on your authentication, the level of access you are allowed
## Accounting
- Logging the resources used
- Login time, data sent and received, logout time
---
## Authenticating Devices
1. When a user wants to connect to a resource, they attempt to authenticate by sending identification, a [[AAA framework#Certificate authentication (CA)|digital certificate]], to a firewall or VPN concentrator
2. This device forwards the identification to a AAA server
3. The AAA server will send either a permit or deny message to the device, who will determine whether traffic from the user can be destined to the resource
## Certificate authority (CA)
- A device or software that is responsible for managing all the certificates in an enterprise or certificates of website
- The CA creates a certificate for each device or website, verifying its creation by **digitally signing the device's certificate** with the CA's own certificate
- The certificate can now be included on the device as an identification factor
---
## Authorization models
- Used to associate users with their access rights to a resource, given their authentication status
- A user is defined by a role, organization, or an attribute. These values define the level of access a user or users have
- An abstraction used to reduce complexity of creating the relationship between a user and resource
---
## AAA protocols
#### RADIUS
- Remote Authentication Dial-in User Service
- A commonly used AAA protocol
- Centralizes authentication for users
	- Routers, switches, firewalls
	- Server authentication
	- Remote VPN access
	- 802.1X network access