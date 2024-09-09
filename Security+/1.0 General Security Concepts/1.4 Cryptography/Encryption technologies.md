## Trusted Platform Module (TPM)
- A piece of hardware designed to provide cryptographic functions to a single device
- Unique keys are burned in the TPM 
![[Pasted image 20240822135047.jpg]]
## Hardware Security Module (HSM)
- A physical device used to manage, store, and protect cryptographic keys a wide scale
- Has a plug-in card or separate hardware to allow for different cryptographic functions
-  Cryptographic accelerators can be used to offload cryptographic functions
![[Pasted image 20240822135219.jpg]]
---
## Key management system (KMS)
- A centralized system that helps manage different types of keys from a single, third-party software usually cloud
- Keys created on the software can be assigned to specific users
- Keys are often rotated on regular intervals
- Logs key use and important events
---
## Keeping data private
#### Secure enclave
- A protected area for secrets, often implemented as a hardware processor, that keep data private even when a device is compromised
- Isolated from the main processor
- Has its own boot ROM
- Performs AES encryption in hardware