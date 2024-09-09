- The protocols used to transfer emails include relatively few security checks - easy to spoof
- DNS servers can be configured to validate emails
## Mail gateway
- Evaluates the source of inbound email messages
- Can block or filter emails before they reach the internal mail server
- If exists on-prem, will likely be located in a [[Network-based Firewall#Screened subnet|screened subnet]]
## Sender policy framework (SPF)
- Prevents email spoofing; allows domain owners to specify which mail servers are permitted to send emails on behalf of their domain
- A list of the authorized mail servers are added to a DNS TXT record
	- Receiving mail servers perform a check to see if incoming mail came from an authorized host
	- The TXT record is publicly visible to everyone on the internet
## Domain keys identified mail (DKIM)
- A mail server digitally signs all outgoing mail
	- The public key is in the DKIM TXT record
- The signature is validated by the receiving mail servers - not usually seen by the end user
#### Process
1. The domain owner generates a public-private key pair. The public key is published in the DNS records for the domain
2. When sending an email, the mail servers uses the private key to generate a [[Hashing and Digital Signatures|digital signature]] for the unique email. This signature is added to the email as a DKIM-Signature header
3. The recipient of the email uses the domain owners public key to encrypt the email and generates a hash
4. The recipient of the email compares its generated hash with the hash created by the sender, to verify [[Encryption and Integrity Methods|integrity]]
## DMARC
- Domain-based Message Authentication, Reporting, and Conformance
- An extension of [[Email Security#Sender policy framework (SPF)|SPF]] and [[Email Security#Domain keys identified mail (DKIM)|DKIM]]
- A policy of what receiving email servers should do with emails not validated using SPF and DKIM
	- Written into a DNS TXT record
	- i.e. accept all, send to spam, reject the email
- **Compliance** reports are created to list the emails that have been verified or not
	- Sent to the domain owner
- 