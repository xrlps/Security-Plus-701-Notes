- Passwords must not be stored as plaintexts and should instead be stored as a [[Hashing and Digital Signatures|hash]]
## Spraying attack
- Attack an account with the top three (or more) common passwords
	- If they don't work, move on to the next account to prevent lockouts, alarms, or alerts
## Brute force
- Trying every single possible combination of letters, characters, numbers, and special characters until the hash is matched
- Lengthy process that gets longer as the hash size gets longer
#### Online attack
- Repeatedly brute forcing a password on a websites login input field
- Most accounts will lockout after a number of failed attempts
#### Offline attack
- After obtaining a list of users and hashes, calculate a password hash and compare it to the stored hash
- "Infinite" attempts but requires large computational resources
- Typically attacks the Windows **SAM** and Linux **/etc/shadow** database/file that contains hashed passwords