- Applications must be ran through the Quality Assurance (QA) process to test the code and security of the application
	- This lowers the chances of vulnerabilities to be pushed out in production
## Input validation
- Testing all different input types inside an application
- Being able to validate actual data vs expected data
- Data should be checked and corrected
- Attackers may use **fuzzers** to input different types of data in a field to see how the application may respond
## Secure cookies
- Cookies - information stored on a browser to track, personalize, and/or create a session
- A security risk if an attacker gets access to one
- Secure cookies are cookies that are only sent over an HTTPS connection
## Static code analyzer
- Static Application Security Testing (SAST)
- Helps identify vulnerabilities in the source code of applications, like:
	- [[Application Vulnerabilities#Buffer overflow|Buffer overflows]]
	- [[Web-based#SQL Injection (SQLi)|SQL injection]]
- Not all vulnerabilities can be identified with SAST
## Code signing
- To verify application [[Non-repudation#Proof of integrity|integrity]], an applications code is digitally signed by the developer using asymmetric encryption
- A trusted [[AAA framework#Certificate authentication (CA)|CA]] signs the developers public key
- Developer signs the code with their private key
## Sandboxing
- Ensuring that the application only has access to data needed for the application to work; limiting the scope of access an application has
- Used during development as a production technique
## Application security monitoring
- Monitoring real-time information about the application
	- Application usage
	- Access demographics
	- View blocked attacks [[Web-based|SQL injection]]
	- Anomaly detection