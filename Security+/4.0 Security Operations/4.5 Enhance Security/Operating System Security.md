## Active directory (AD)
- A database of everything on the network
	- Computers
	- User accounts
	- File shares
	- Printers
	- Groups
- Stored in a central, redundant database
- Primarily Windows-based
- Centralized access control
	- Users login using their AD credentials
	- Determine which users can access resources
## Group policy
- Helps set up different configurations and permissions for users stored in the AD
- A central console that allows configuration of:
	- Login scripts
	- Network configurations (QoS)
	- Security parameters
## Security-Enhanced Linux (SELinux)
- Linux traditionally uses **DAC**
	- Discretionary Access Control
	- The user can decide rights and permissions to resources
- Adds mandatory access control (MAC) to Linux, overriding DAC
- Limits application access to users on Linux - implementation of [[Mitigation Techniques#"Least privilege"|least privilege]]
## Root of Trust
- A hardware-based root of trust (like a [[Encryption technologies#Trusted Platform Module (TPM)|TPM]]) that ensures secure boot processes and cryptographic operations
