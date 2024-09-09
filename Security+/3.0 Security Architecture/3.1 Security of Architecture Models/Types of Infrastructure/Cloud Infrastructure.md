 - When using different cloud services like IaaS, SaaS, PaaS, different organizations hold different levels of responsibility for securing said service
 - Cloud providers usually provide a matrix of responsibilities so that security is well documented
## Example responsibility matrix
 ![[Pasted image 20240825123037.png]]

## Hybrid cloud
- Refers to the use of more than one public or private cloud
- Adds complexity for the level of security needed, for example
	- Network protection mismatches
	- Logs may be diverse and cloud-specific
## Third-party vendors in the cloud
- A third-party vendor may be used in conjunction with a cloud service
	- A third party vendor, like Splunk, may be used for data analytics in addition to a cloud service, like AWS servers
- A **vendor risk management policy** should be used to determine the best way to manage and maintain security for third-party vendors
- In additional to internal processes and cloud provider processes, an incident response should be prepared for third-party vendors in the cloud
## Infrastructure as Code (IoC)
- A method of managing and provisioning infrastructure using code and automation tools
- Infrastructure can be defined, updated, and versioned through configuration files rather than manual configuration
## Serverless architecture
- Function as a Service (FaaS)
- A in-house developer separates an application into individual, autonomous functions, which are then deployed on the cloud
- Managed by a third-party
## Microservices and APIs
- Hosting majority of application logic in the cloud, rather than on a device
- Security is built in to each microservice
#### APIs
- Application Programming Interface
- The middleman between a client and a microservice; allows a client to talk to or use a service
###### Microservice architecture
![[Pasted image 20240825125132.png]]

