- A file that contains a public key and digital signature to uniquely identify users 
## Content of digital certificates
- Follows the **X.509** standard
- Certificate details
	- Serial number
	- Version
	- Signature algorithm
	- Issuer
	- Name of the certificate holder
	- Public key
	- Extensions
	- ...
## Root of trust
- Someone or something that determine what websites to trust; an inherently trusted component
- Hardware, software, firmware, or other component
	- [[Encryption technologies#Hardware Security Module (HSM)|HSM]], [[Encryption technologies#Secure enclave|secure enclave]], [[AAA framework#Certificate authority (CA)|Certificate Authority]], etc
## Subordinate certificate authority
- A certificate authority who signs and manages certificates on the behalf of a root, to limit the exposure to a root authority 
## Certificate Signing Requests (CSR)
- For a website hosted online to be trusted by a users browser (trusted by the browsers trusted [[AAA framework#Certificate authority (CA)|CA]]), the website owner must send a certificate signing request (CSR)
![[Screenshot 2024-08-22 152136.png]]
---
## Certificate types
#### Private certificate authorities
- An in-house [[AAA framework#Certificate authority (CA)|CA]] to issue and manage certificates for an organization
- An entity that issues certificates to be used within a specific organization
- The CA's root certificate is distributed within the organization to establish trust
- Accomplished through third-party software packages like
	- Windows Certificate Services
	- OpenCA
#### Self-signed certificates
- Created and signed by the entity that owns the certificate
- Not trusted by external systems; used within an organization
#### Wildcard certificate | Subject Alternative Name (SAN)
- An extension to an X.509 certificate
- Allows a certificate to support many different domains. Certificates are based on the name of the server via a wildcard name
	- A wildcard certificate for `*.example.com` covers `mail.example.com`, `shop.example.com`, etc
---
## Revoking certificates
#### Certificate Revocation List (CRL)
- Maintained by the [[AAA framework#Certificate authority (CA)|certificate authority]]
- A list of all the certificates that have been revoked, hosted on a URI
- Any certificate located in the CRL will not be trusted by the browser
#### Online Certificate Status Protocol (OCSP) stapling
- The browser checks for certificate revocation, rather than the CA
- The webserver sends the browser the status of its' certificate (stapling the OCSP status) into the SSL/TLS handshake
	- This status is digitally signed by the [[AAA framework#Certificate authentication (CA)|CA]]