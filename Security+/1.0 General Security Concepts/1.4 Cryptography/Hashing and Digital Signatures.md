## Hashing
- Cryptography represents data as a short string of text through a **hash**, often called a message digest or fingerprint
- An input (character, sentence, passage, etc) is placed through a hashing algorithm, which will output a unique string of text
- Changes to the input, whether minor or major, will significantly alter the output of the hash
- One way encryption. The hashed value cannot be turned back into its original text
- Used to verify [[Non-repudation#Proof of integrity|integrity]] or to create fingerprints
- A **collision** refers to two (or more) different inputs that create the same hash value. A hashing algorithm with known collisions is considered insecure
#### Verify files with hashes
- A file is put into a hashing algorithm to produce a unique hash
- When downloading this file, the downloaded file is compared to the posted hash value to confirm the legitimacy of the downloaded data
#### Storing hashed passwords
- Passwords are stored as a [[Hashing and Digital Signatures#Salt|salted]] hashes
###### Salt
- Random data added to a password when hashing
- Each user gets their own random salt value
- If users store the same password, the unique salt value will ensure that the hashed values do not look the same
- Prevents rainbow tables from working
	- A mapping of common passwords with their hashed values
#### Digital signatures
- Prove the message was not changed
- Prove the source of the message
- Make sure the signature isn't [[Non-repudation|fake]]
