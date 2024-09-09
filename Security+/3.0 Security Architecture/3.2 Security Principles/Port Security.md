- A type of security that requests authentication details before accessing the resources on a connection
- Commonly used on wireless networks, can be used in wired networks
## Extensible Authentication Protocol (EAP)
- An authentication framework applied to networks and connections, typically used on wireless AP
- Manufacturers can build their own EAP method
- EAP is integrated with [[Port Security#802.1X|802.1X]]
	- EAP provides the authentication protocol
	- 802.1X prevents access to the network until the authentication succeeds
- Used in conjunction with an authentication database
	- RADIUS
	- TACACS+
	- ...
#### 802.1X
- IEEE standard that manages and prevents access to a network until the authentication succeeds
- Often called Port-based Network Access Control (**NAC**)
#### 802.1X device roles
- Supplicant - the client or the device trying to connect to the network
- Authenticator - the device aggregates the connection from the supplicant to the network
- Authentication server (AS) - validates the client credentials
#### Connection process
1. A supplicant sends an initialization message to the authenticator
2. The authenticator responds to the supplicant with an EAP-Request, asking for client information
3. The supplicant responds with an EAP-Response, providing its credentials
4. The authenticator passes the EAP-Response to the authentication server
5. The AS sends a message to the authenticator, asking for additional details from the supplicant
6. The authenticator forwards this message to the supplicant, who responds to the authenticator providing additional details about itself. The authenticator forwards the details to the AS
7. Based on the details in the supplicants message, the AS will either tell the authenticator to permit or deny traffic from the supplicant
## Kerberos
- A network authentication protocol designed to provide secure authentication over a non-secure network
- Uses a ticket-based system to authenticate users
#### Key distribution center (KDC)
- Consists of an [[AAA framework#Certificate authority (CA)|authentication server]] and a ticket granting server (TGS)
#### Tickets
- Used to prove identity and establish secure connection