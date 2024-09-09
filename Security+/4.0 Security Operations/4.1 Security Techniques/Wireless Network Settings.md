- Encrypt all confidential traffic traversing the network
- Authenticate users before granting access
- Verify integrity of communication
	- Message Integrity Check (MIC)
## WPA2
- A wireless encryption protocol
- Insecure; the PSK can be brute forced
- Attackers can capture or derive the hash produced in the four-way handshake
	- With this hash, attackers can brute force the pre-shared key
- Anyone with the PSK has access to the network, there is no forward secrecy
## WPA3
- Changes the PSK authentication process to be more secure than previous wireless encryption protocols
- Includes mutual authentication; the client device and access point must be authenticated
- Shared session keys are created on device, rather than sent across the network
- No four-way handshake
#### GCMP
- Galois/Counter Mode Protocol
- A stronger encryption than [[Wireless Network Settings#WPA2|WPA2]]
- Includes data confidentiality with AES
- Includes a Message Integrity Check (MIC) with Galois Message Authentication Code (GMAC)
#### SAE
- Simultaneous Authentication of Equals
- A Diffie-Hellman derived key exchange with an authentication component
- Everyone uses different session keys, even with the same PSK
- Dragonfly handshake
## Wireless authentication methods
- Users connecting to a network can be authenticated through
	- Pre-shared key (PSK) / shared password
	- 802.1x / centralized authentication
#### Open system
- No authentication is required
#### WPA3-Personal / WPA3-PSK
- Everyone on the network uses the same 256-bit key to log in to the network
- Used in small networks (SOHO)
#### WPA3-Enterprise/WPA3-802.1X
- Authenticates users individually with a [[AAA framework|AAA]] authentication server (i.e., RADIUS)
- Used in corporate networks
## 802.1X 
- Port-based Network Access Control (NAC)
- Prevents access to a network until credentials are provided
- Used in conjunction with an [[AAA framework#RADIUS|authentication server]]
#### EAP
- Extensible Authentication Protocol
- A protocol used in the 802.1X process
- Allows for many different ways to authenticate
#### Authentication process with 802.1X
- See [[Port Security]]
