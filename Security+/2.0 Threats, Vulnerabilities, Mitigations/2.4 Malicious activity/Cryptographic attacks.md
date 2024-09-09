## Birthday attack
- Accomplished through [[Hashing and Digital Signatures|hash]] collisions; a brute force attempt at identifying a single hash value that can be created from two different text inputs
- Larger hashes values make birthday attacks more difficult to produce
## Match-the-hash
1. An attacker obtains a list of hashed passwords (e.g. from a compromised database)
2. They generate passwords and hash them
3. The generated hashed passwords are compared to the list of hashed passwords. If equal, they have obtained the clear-text password
## Downgrade attack
- Forcing systems to use a less secure version of a protocol or encryption method
	- Rather than attack the cryptography, attackers attempt to find weaknesses in the implementation of the cryptography
#### TLS fallback
- An attack where the client downgrades to an older version of the TLS protocol
#### SSL stripping
- A combination of an [[On-path Attack|on-path attack]] and downgrade attack
- An attacker rewrites URLS HTTP/HTTPS
![[Pasted image 20240824162901.png]]