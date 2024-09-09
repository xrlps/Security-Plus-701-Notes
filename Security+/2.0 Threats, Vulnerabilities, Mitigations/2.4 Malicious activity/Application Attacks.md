- Common low application attacks include HTML / [[Application Vulnerabilities#Memory Injections|SQL]] / XML / LDAP injection, [[Application Vulnerabilities#Buffer overflow|buffer overflows]], and [[Application Vulnerabilities|more]]
- Additional application attacks like [[On-path Attack|on-path attacks]] and [[Replay Attacks|replay attacks]] can be used to get credentials to then use an application
## Privilege escalation
- Exploiting a vulnerability to gain higher-level access to a system
#### Horizontal privilege escalation
- Moving from users of the same privilege access to get information that only one specific user will have
#### Mitigating privilege escalation
- Patching vulnerabilities
- Updating anti-virus/anti-malware software
- **Data execution prevention** - limit the area of memory that an executable can run
- **Address space layout randomization** - prevent a buffer overrun at a known memory address
## Cross-site request forgery
- **Cross-site request** A single website requesting data from multiple external website servers
- Also called **one-click** attack or session riding (XSRF, CSRF [sea surf])
###### Example
- A victim makes a request to a website on behalf of an attacker
1. Attacker creates a funds transfer request
2. Request is sent as a hyperlink to a user who may already be logged into the bank site
3. User clicks the link and unknowingly sends the transfer request to the bank website
4. Bank validates the visitor's funds and sends it to the attacker
## Server-side request forgery (SSRF)
- Exploits a server by making it send requests to internal or external resources on the behalf of an attacker
- Allows an attacker to access resources or services that the server has access to but is set up to be restricted from external access
## Directory traversal
- A vulnerability associated with a web server misconfiguration or web server software vulnerability
- A attacker or client can view the servers file directory