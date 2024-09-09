- The exchange of an encryption key must be done over a secure medium in order to keep the keys fully secured
## Out-of-band key exchange
- Avoids sending a symmetric key over the net
- Telephone, in-person
## In-band key exchange
- A key exchange over the network
- Protects the key with additional data
- Potentially using asymmetric encryption to deliver a symmetric key
- Faster and more practical than [[Key exchange#Out-of-band key exchange|out-of-band key exchanges]]
#### Session key
- Used for a short period of time, a session
- Client encrypts a random symmetric key with a server's public key
	- The server decrypts the shared key and uses it to encrypt data
	- The shared key is the session key
#### Deriving a symmetric key from asymmetric keys
- Creating the same symmetric key from a combination of a private key and public key
	- Alice combines her private key with Bob's public key to get a symmetric key
	- Bob combines his private key with Alice's public key to get a symmetric key
	- The two derived symmetric keys are equal![[Screenshot 2024-08-22 124708.png]]
