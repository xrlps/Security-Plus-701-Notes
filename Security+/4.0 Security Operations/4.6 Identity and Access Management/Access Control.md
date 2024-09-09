- Controls the type of information someone can access at a certain time 
- The process of ensuring only authorized rights are exercised
- Policy definition
## Access control types
#### Least privilege
- See [[Mitigation Techniques#"Least privilege"|Mitigation Techniques]]
#### Mandatory access control (MAC)
- Every file or folder gets a label - the OS limits the operations possible on an object based on security clearance levels
#### Discretionary access control (DAC)
- The user that creates the data has control over the data they can access
	- As the owner, you control who has access
- Flexible access control; weak security
#### Role-based access control (RBAC)
- Different levels of privilege based on a predefined role 
	- Manager, director, team lead
- Rights are gained implicitly, based on their role
- Windows uses Groups to provide role-based access control
#### Rule-based access control
- Access is determined through system enforced rules from a system administrator
- When trying to access an object (like an application) the system checks the ACLs for that object and determines whether that user can access the object
#### Attribute-based access control (ABAC)
- Combines different criteria, almost aware of its' context
	- Resource information
	- IP address
	- Time of day
	- Desired action
	- Relationship to the data
## Access control rules
#### Time of day restriction
- Restricting access during certain times or days of the week
