## Stored data encryption
- The following forms of stored data are typically encrypted in an enterprise
	- Data on storage devices (SSD, HDD, USB, cloud storage, etc), also called data at rest
	- Entire disk partitions
	- Individual files
## Database encryption
- Often done through transparent encryption
	- Encrypts all database information with a symmetric key
- Individual columns inside a database can be encrypted. A separate symmetric key may be used for each column
## Transport encryption
- Protects data traversing the network
- HTTPS, client-based VPNs, site-to-site VPNs with IPsec
---
## Encryption algorithms
- Both sides (sender and receiver) must agree on the encryption algorithm before encrypting the data
- Algorithms have their own pros & cons
	- Security level, speed, complexity of implementation
#### Key lengths
- Larger keys are typically more secure, slowing down or preventing brute force attacks
- 128-bit or larger [[Public Key Infrastructure (PKI)#Symmetric encryption|symmetric keys]] are common
- 3072 bits or larger [[Public Key Infrastructure (PKI)#Asymmetric encryption|asymmetric keys]] are common
#### Key stretching
- Continuously hashing or encrypting data, adding additional layers of security
- Hash a password, hash the hash of a password, ...