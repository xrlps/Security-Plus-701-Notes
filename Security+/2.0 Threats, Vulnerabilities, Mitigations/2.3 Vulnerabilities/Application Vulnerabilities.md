## Memory Injections
- Common running processes in memory
	- DLLs (Dynamic Link Libraries)
	- Threads
	- Buffers
	- Memory management functions
- Malware can either run its own process, or inject itself in existing processes
- When malware injects itself into a process, it has the same privilege levels of that process
#### DLL injection
- Attacker puts a path to where the malicious DLL is into a target process
- As the target process runs, it will run the path referencing the malicious DLL, then load the malicious DLL into memory allowing malware to run on the system
- Using fully qualified paths "Files\MyApp\lib\example.dll" rather than search paths "example.dll" can help mitigate DLL injection
#### Buffer overflow
- Overwriting a buffer with additional memory so that this memory overflows to other application buffers
- Attackers check for potential openings where application developers did not properly perform bounds checking
#### Integer overflow
- A value exceeding the storage capacity of a variable is input or computed, causing it to "wrap around" or truncate
- See [welivesecurity.com - integer overflow](https://www.welivesecurity.com/2022/02/21/integer-overflow-how-it-occur-can-be-prevented/)
## Race condition
- When two events happen at the same time in an application, and the application is unaware that this is happening
- If not prepared for, the application can act unexpectedly
#### Time-of-check to time-of-use (TOCOU)
1. Retrieve some data value
2. Wait a period of time
3. Do something with the value
- During step 2, if another event is running that can cause the data value to change, causing step 3 to potentially have unexpected results