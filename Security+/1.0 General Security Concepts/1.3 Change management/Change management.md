- Defines the process used to handle the planning, implementing, and overseeing of system changes (software updates, application patches) to minimize disruption and ensure smooth transition
- Concerned with "what" needs to change
- A formal process associated when making a change to a system
- Defines the:
	- Scope of a change
	- Risk of a change
	- Frequency of a change
	- Installation process
	- Fallback procedures
	- ...
- Requires the creation of a plan
	- Typically requires end-user approval
	- Must be presented as a proposal to the change control board
	- Requires a [[Change management#Backout plan|backout plan ]] if the change doesn't work
## Change approval process
1. Complete the change control process form
	- The reason to make the change
	- Scope of the change
	- Date and time of the change
	- Affected systems and impact
	- Risks associated
## Change control process
1. An individual or entity that owns the process wants to make the change
	- This entity (the owner) manages the process, ensuring that it is followed and acceptable
2. Stakeholders or departments impacted on the change will input their thoughts on the change management process
## Impact analysis
- Determine the level of risks of adding the change
- Determine whether or not the change can negatively affect other systems
- Determine the risk of not making the change
- Uses a [[Change management#Sandbox environment|sandbox environment]] to safely test the change
## Sandbox environment
- Used to determine the aftermath of a change; helps test and confirm a change prior to deployment 
- No connection to the real world or production system
## Backout plan
- A way to revert changes in case a change goes bad
## Maintenance window
- The time in which a change occurs
- Changes are typically ran overnight to prevent potential production disruption
- Time of year is considered when making changes (a system may be busy during Christmas time)
## Standard Operating Procedure (SOP)
- A document where the change control process resides
- Guides individuals through specific processes within an organization, ensuring consistency and compliance 