- Increase password entropy to increase security against guessing or brute-force attacks
	- No single words
	- Mix upper and lower case letters, numbers, special characters
	- Length > 8 characters
## Password age and expiration
- Password age
	- How long since a password was modified
- Password expiration
	- Passwords work for a certain amount of time until they do not work
- Critical systems may require passwords to expire more frequently
## Password manager
- Use a separate password for each account; one compromised account will not make other accounts accessible
- Stores all passwords into a single database
	- [[Encrypting data|Encrypted]], protected
	- Can include multifactor tokens
## Passwordless authentication
- Authentication without a password
- Facial recognition
- Security key
- TouchID
- Often used with additional authentication factors
## Just in time permissions
- Grant admin access for a limited amount of time
	- No permanent administrator rights
- Narrows the scope of an attack
#### Process
1. Request access from a central clearing house / password vault
2. The vault sets a control for each requesting user, granting different levels of access
3. Creates a new set of credentials based on the primary set on an ephemeral basis