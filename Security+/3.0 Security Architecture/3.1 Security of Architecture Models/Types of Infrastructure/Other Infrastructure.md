## On-premise
- Allows for customization of security posture - full control
- An on-site team can manage security better than one in a cloud, although more expensive
- Local teams maintain uptime and availability
## Centralized vs decentralized
- Most organizations are physically decentralized
	- Different locations, usage of cloud providers, different operating systems, etc
- A single centralized system may be created to aggregate information for all systems in an organization
	- While the centralized system makes things convenient, it introduces a single point of failure
## Virtualization
- Runs many different operating systems and applications on the same piece of hardware
- Each application instance has its *own* operating system, even if the applications share the same OS
![[Virtualization-660-2930277952.png]]
## Containerization
- Contains everything needed to run an application - code and dependencies
- Applications all share the same OS
- Applications are isolated from each other and can replace applications when one falls over
![[1_V5N9gJdnToIrgAgVJTtl_w-1786962223.png]]
## IoT (Internet of Things)
- Convenience devices
	- Sensors
	- Smart lights
	- Fitness watches
	- ...
- Weakly secured
## SCADA/ICS
- Supervisory Control and Data Acquisition System
- Large-scale, multi-site Industrial Control Systems (ICS)
- Provides a centralized view and place of configuration to manufacturing equipment
- Must be highly secured
- Cannot be accessed from the internet
## RTOS (Real-Time Operating System)
- An operating system designed to handle tasks and processes with strict timing requirements
- Must be able to immediately respond to events
###### Example
- Ensuring that brakes in a car respond immediately and are not dependent on the other functions of the car
## Embedded system
- Hardware and software are designed for a specific function
###### Example
- Smart watches, smart lights, etc