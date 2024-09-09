## Code injection
- An attacker adding their information as code into a data stream
#### SQL Injection (SQLi)
- Can be done in input form or fields
###### Example website SQL query
- Query the database and select a user depending on their username
```SQL
	SELECT * FROM users WHERE name = 'UsernameHere'
```
###### Example SQLi
- The below selects all users, because '1' will always equal '1'
```SQL
	SELECT * FROM users WHERE name = 'abc123' OR '1' = '1'
```
#### Cross-site scripting (XSS)
- Originally called cross-site scripting because information from one site could be shared with another
- Commonly uses JavaScript
- An attacker sends a link containing a malicious script to a victim. The victim clicks the link, then visits a legitimate site. The legitimate site loads the malicious script, which sends victims data to the attacker (session cookies, etc)
###### Non-persistent (reflected) XSS attack
- An attack that uses websites that allow users to run scripts inside input fields, like a search box
###### Persistent (stored) XSS attack
- Attacker posts a message to a site that includes malicious payload
- All users that visit the post have the payloads code run into the browser