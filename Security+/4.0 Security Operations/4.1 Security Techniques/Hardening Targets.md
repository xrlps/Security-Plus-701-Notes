- Hardening guides are guides created by a products manufacturer that offer configurations to best secure an platform
- All devices must be configured to use non-default settings
## Mobile devices
- Frequent [[Mitigation Techniques#Patching|patching]]
- Control with an MDM
	- Mobile Device Manager
	- Helps monitor devices and push security updates
## Workstations
- User desktops and laptops
- Requires constant monitoring and updates of
	- Operating systems
	- Applications
	- Firmware
- Often updates are an automated process
- Remove unnecessary software
## Network infrastructure devices
- Switches, routers, firewalls, etc
- Purpose-built devices with an [[Other Infrastructure#Embedded system|embedded]] operating system
- Limited OS access
- Check with the manufacturer for [[Mitigation Techniques#Patching|patches]]
## Cloud infrastructure
- The cloud management workstation should be heavily secured and gated as it has access to most if not all cloud infrastructure
- The cloud management workstation should use [[Mitigation Techniques#"Least privilege"|least privilege]]
- Should be configured with [[Hardening Techniques#Endpoint detection and response (EDR)|EDR]]
- Backing up to separate cloud providers
## Servers
- [[Mitigation Techniques#Patching|Patching]], [[Mitigation Techniques#"Least privilege"|least privilege]], minimum password lengths
- Limit network access to and from the servers
- Install [[Malware|anti-malware]]
## SCADA/ICS
- See [[Other Infrastructure#SCADA/ICS|Other Infrastructure]]
## Embedded systems
- See [[Other Infrastructure#Embedded system|Embedded Systems]]
- Do not often get patches, when patches are out they can be important
- Should be on [[Protecting data#Segmentation|their own network]]
## RTOS (Real-Time Operating System)
- See [[Other Infrastructure#RTOS (Real-Time Operating System)|Other Infrastructure]]
- Run with the minimum amount of services
- Use a separate firewall
## IoT devices
- See [[Other Infrastructure#IoT (Internet of Things)|Other Infrastructure]]
- Weak defaults, manufacturers of IoT devices do not add much security by default
- Deploy updates quickly; can be a security concern if not updated
- Should be on [[Protecting data#Segmentation|their own network]]