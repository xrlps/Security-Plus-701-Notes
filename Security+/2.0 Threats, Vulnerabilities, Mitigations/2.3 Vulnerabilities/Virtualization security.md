## VM escape protection
- Protects against an attacker getting access to one VM, escaping it, and taking control over the host OS or other guest VMs
## Resource reuse
- When a hypervisor allows virtual machines to collectively use more RAM than is physically available on the host, it can lead to unintended data sharing between the VMs, which introduces potential risks
- Can be mitigated with **volume encryption**
	- Encrypting an entire disk volume/partition rather than individual files