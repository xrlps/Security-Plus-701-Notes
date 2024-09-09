- Provided through [[Infrastructure Considerations#Redundancy|redundancy]], [[Infrastructure Considerations#High availability (HA)|high availability]], [[Resiliency#Server clustering|server clustering]]
- Recovering from an outage or downtime
- Commonly referenced as **MTTR** (Mean Time to Repair) - the length of time to repair something that is no longer available with one that is available
## Server clustering
- Combining two or more servers to operate as a single server to hosts
- Allows for flexibility in increasing or decreasing capacity and availability
- Servers in a cluster share the same storage, on a single storage device
## Load balancing
- Uses a central load balancer to distribute load to separate servers
- Servers are unaware of each other
- Adds failover - if a server goes down, the load balancer balances traffic to all working servers
## Site resiliency
- The use of a recovery site
- System failovers move to the alternate processing site until the problem is addressed
#### Hot site
- An exact replica of the main site
- When applications, software, or hardware are updated at the main site, the hot site must be updated to the exact settings
#### Cold site
- An empty building with no hardware, data, or people
- In the case of system failovers, the data must be brought over to the cold site
#### Warm site
- In between cold and hot site - has some hardware and software but additional items must be brought over
#### Geographic dispersion
- The physical separation of a main site and recovery site to ensure that geographical disruptions that affect the main site do not affect the recovery site (tornados, hurricanes, etc)
## Platform diversity
- Using different OS's for different purposes to limit vulnerabilities that may be present in specific operating systems
## Multi-cloud systems
- Using different cloud providers to plan for outages, exploits, etc
## Continuity of operations planning (COOP)
- An alternative to technology, for example
	- Manual transactions
	- Paper receipts