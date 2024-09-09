- Giving the right permissions to the right people at the right time to prevent unauthorized access
- Restricts access and prevents extended, unneeded high level access
- Identity lifecycle management
	- Every entity gets a digital identity
- Access control
	- Defines what entity gets access to what
- Authentication and authorization
	- Entities prove who they claim to be
- Identity governance
	- Track an entity's resource access
## Provisioning/deprovisioning user accounts
- Access is applied when needed and revoked when not needed
- Occurs for certain events - hiring, transfers, promotions
- Account details include:
	- Name
	- Attributes
	- Group permissions
	- ...
## Permission assignments
- Each entity gets limited permissions
	- Just enough to do their job
- Usually group assignments
- Storage and files are exclusively private to a user
- Users do not have privileged access to the operating system
## Identity proofing
- **Resolution** - who the system thinks you are
- **Validation** - gathering information from a user (password, security questions)
- **Verification/Attestation** - additional details to verify identity (passport, in-person meeting)
## Gaining access
- Usually done with a [[AAA framework|AAA]] server
---
## Authentication methods
#### Single sign-on (SSO)
- An authentication method typically used in web applications
- Provides credential one time
	- Get access to all available resources
	- No additional authentication required
- Usually limited by time; requires authentication after the timer runs
#### Lightweight directory access protocol (LDAP)
- An authentication and authorization protocol for accessing directories over an IP network based on the [[Identity and Access Management (IAM)#X.500|X.500]] standard
- Directories refer to a database or service used to store data about network resources such as users, groups, and devices
###### X.500 
- A framework that defines how data should be structure and accessed
- attribute=value pairs
	- i.e. ST=London (ST is the state, province, or country within a country)
- Builds a tree structure (directory information tree) to organize users, devices, etc
	- Container objects are the country, organization, organizational units
	- Leaf objects are the users, computers, printers, files
![[x500-1812068450.gif]]
## Authentication frameworks using SSO
#### Security assertion markup language (SAML)
-  Open standard for authentication and authorization through a third-party database using [[Identity and Access Management (IAM)#Single sign-on (SSO)|SSO]]
- Not designed for mobile devices
###### Process
- The user is redirected, by the resource, to authenticate to the SAML server. If successful, a SAML token is generated which is presented to the resource server
#### OAuth
- Authorization framework that allows third-party applications to obtain access to a user's resources without exposing their credentials
- Not an authentication protocol
	- Combined with authentication protocols like OpenID to handle [[Identity and Access Management (IAM)#Single sign-on (SSO)|SSO]] authentication
#### Federation
- Allows network access without using a local authentication database
- Provides [[Identity and Access Management (IAM)#Single sign-on (SSO)|SSO]] and more
- Does not use a local authentication database
- The third-parties must establish a trust relationship
###### Example
- Rather than creating an account on https://test.com, log in to the site with a facebook account
