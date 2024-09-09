## Physical segmentation
- Separating devices physically so that one device being compromised will not compromise the other
###### Example
- Web servers in one rack while database servers are on another
## Logical segmentation (VLANs)
- Allows for devices to be physically connected to each other but function logically as if they weren't
## SDN (Software Defined Networking)
- A single networking device has different functional planes of operation
	1. Data - forwards traffic from one device to another
	2. Control - manages the data plane, knows where traffic goes; routing tables, NAT tables
	3. Management - configuring and managing devices; SSH, [[Cloud Infrastructure#APIs|API]], SNMP
- Individual functions of operation can be split up
- A single device or interface can be used to programmatically configure multiple devices at once
![[Pasted image 20240825130021.png]]
