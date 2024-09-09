- A holistic approach to network security, requiring authentication when attempting to access _every_ resource
- Applies to every device, process, and user on the network, no matter if they have verified previously, are an employee, etc
- MFA, E2E, system permissions, firewalls, access controls
## Planes of operation
- To implement zero trust on a network, security devices are "broken down" to separate functional planes of operations
	- Physical components
	- Virtual components
	- Cloud components
- A logical separation of physical devices into different functional tasks
#### Data plane
- The part of the device (switch, router, firewall) that processes frames, packets, and network data
- Processing, forwarding, trunking, encrypting, NAT
#### Control plane
- Manages the actions of the data plane
- Determines how packets should be forwarded
- Routing tables, NAT table, MAC address table
## Adaptive identity
- Examining the identity of a user and other information gathered about the user to apply security controls
- Applying risk indicators to make authentication stronger, if needed
###### Example
- Where the user is logging in from
- What device the user is logging in from
- Whether the device they're logging in from is secured
#### Security zones
- Looks at the conversation path; the network in which the client is requesting from, to the network in which the client is requesting to
- Rules can be applied to zones to permit or deny traffic
- Traffic from an **untrusted** zone may be implicitly dropped when requesting data from a **trusted** zone
#### Policy enforcement point (PEP)
- The point at which policies or zones are applied
- Gathers all information about traffic, providing it to a [[Zero Trust#Policy Decision Point (PDP)|policy decision point]]
- Gets the permit or deny statement from the PDP to either allow or disallow traffic on a particular plane
![Zero Trust](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.forumsys.com%2Fwp-content%2Fuploads%2F2022%2F01%2FNIST-SP-800-207-Fig1.png&f=1&nofb=1&ipt=62683bbd443c86334156e01f2306a1187b0cefc8e83cf51dce8f0edf3eec35fa&ipo=images)
#### Policy Decision Point (PDP)
###### Policy Engine
- Examines the authentication and determines whether the traffic should be allowed or disallowed on the network
###### Policy Administrator
- Communicates with the Policy Enforcement Point
- Generates access tokens or credentials based on the result of the policy decision
- The access tokens are sent to the PDP to allow or disallow access
###### Subject
- A device, such as a laptop, desktop, or mobile device within the context of a zero-trust design
## Threat scope reduction
- Decreasing the number of possible entry points
- A network can only be accessed in a physical area
## Policy-driven access control
- Adds policies and [[AAA framework#Authorization|authorization]] based on the [[Zero Trust#Adaptive identity|adaptive identity]] of a user
