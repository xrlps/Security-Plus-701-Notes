- A term in cryptography that refers to the policies, procedures, hardware, software, and people, that are responsible for creating, distributing, managing, storing, and revoking digital certificates
- Also refers to the [[AAA framework#Certificate authentication (CA)|mapping of public keys]] to people or devices 
## Symmetric encryption
- A single, shared key is used to
	- Encrypt data
	- Decrypt data
- Often called the **shared key algorithm** or shared secret
- Does not scale well
- Fast to use, less overhead than, yet often combined with, [[Public Key Infrastructure (PKI)#Asymmetric encryption|asymmetric encryption]]
![[Pasted image 20240822120506.png]]
## Asymmetric encryption
- Two (or more) mathematically related keys are used to
	- Encrypt data
	- Decrypt data
- Often called **public key cryptography**
- Key roles include:
	- Private key; a secret key that is used for decrypting data. Data encrypted by the public can can only be decrypted by the private key; must be kept private
	- Public key; a key that is used for encrypting data; can be publicly shared
![[Pasted image 20240822121322.png]]
## Key escrows
- The facility that holds private keys
