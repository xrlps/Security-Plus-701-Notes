## Availability
- System uptime, often represented as a percentage
#### Redundancy
- A backup that might not provide immediate convergence
	- May need to be powered on manually
#### High availability (HA)
- A backup/redundant system in case of failure that is always on and always available
- A "failover system"
- High costs
###### Example
- Software patches
- [[Infrastructure Considerations#High availability (HA)|Redundant]] systems
## Cost
1. Initial installation
2. Ongoing maintenance
3. Replacement or repair cost
4. Tax implications
## Responsiveness
- The length of time that an application takes to respond
## Scalability
- How quickly and easily the capacity of the system can change
## Ease of deployment
- Applications typically have many components
	- Web server
	- Database
	- Firewall
	- ...
- Hardware resources, cloud budgets, change control must be considered
## Risk transference
- A method of transferring risk to a third-party
###### Example: Cybersecurity insurance
- In the events of attacks, the business can recoup financial losses through its cybersecurity insurance policy
## Patch availability
- See [[Hardening Techniques#System hardening|system hardening]]
- Devices that cannot be patched, like [[Other Infrastructure#Embedded system|embedded systems]], may need additional security controls
## Power
- Power requirements of the organization
	- Data center vs an office building
- Backup services to provide [[Infrastructure Considerations#High availability (HA)|redundancy]]
	- UPS (Uninterruptible Power Supply)
	- Generators
## Compute
- The part of the application that does the thinking and processing of data
	- One or more processors (CPUs)
- Referred to as the *compute engine* in the cloud