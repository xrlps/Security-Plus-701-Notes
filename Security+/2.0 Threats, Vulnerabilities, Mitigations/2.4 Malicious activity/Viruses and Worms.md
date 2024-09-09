## Virus
- Malware that can reproduce itself
- Requires a victim to execute a program
#### Program virus
- A part of an application
#### Boot sector virus
- Viruses that sit in the boot section of the computer and run as a system boots up
#### Script viruses
- Operating system and browser-based
#### Macro viruses
- Viruses that are written in macro languages, provided by safe applications, that take advantage of vulnerabilities of the application
#### Fileless virus
- Operates in memory; does not exist in the devices storage drive
- Avoids anti-virus detection
###### Common process
1. Victim clicks on a malicious link
2. Link takes them to a website which exploits a vulnerability
3. This exploit launches powershell (or an equivalent) and downloads the payload in RAM
4. The RAM runs powershell scripts and executables in memory, exfiltrates data, and damages files
5. Adds an auto-start to a registry to restart the virus when the device resets
---
## Worms
- Malware that self-replicates
- Doesn't require user intervention
- Replicate at the speed of a network
- Firewalls and IDS/IPS can mitigate worms but do not help once the worm is inside a network
