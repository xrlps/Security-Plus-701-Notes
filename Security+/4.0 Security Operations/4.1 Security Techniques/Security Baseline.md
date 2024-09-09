- The security of an application and its environment should be well defined whenever it is running
	- Firewall settings, patch levels, OS file versions
- Integrity measurements checks should be
	- Performed often
	- Checked against well-documented baselines
	- Planned for failures to require immediate correction
## Establish baselines
- The list of security settings that should be associated with an application, OS, etc
- Often available from the manufacturer of the system
## Deploy baseline
- May require multiple deployment mechanisms; should be automated
- Test and measure baselines to avoid conflicts; some baselines from different manufacturers may conflict with each other
## Maintain baselines
- Once deployed, the baselines are likely to not change
- Sometimes baselines may require ongoing updates, for example:
	- A new vulnerability is discovered
	- An updated application is deployed
	- A new OS is used
- 