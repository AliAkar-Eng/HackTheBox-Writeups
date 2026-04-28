
Redeemer - Hack The Box

🧠 Skills Learned

- Redis interaction
- Accessing databases without authentication
- Retrieving stored data

🔍 Enumeration

Started with an nmap scan:

nmap <target-ip> failed so i did
nmap -p- <target-ip- --min-rate 5000 

Results:

- Port 6379 open → Redis service detected

🚪 Initial Access

Connected to Redis server:

redis-cli -h <target-ip>

Connection succeeded without authentication.

📂 Exploring the Database

- Listed keys:
  KEYS *

- Retrieved value:
  GET <key>

Found the flag stored in the database.

🏁 Outcome

Successfully accessed Redis instance and retrieved stored data.

📌 Key Takeaways

- Redis is often misconfigured with no authentication
- Always check for open databases
- Simple commands can expose sensitive data

⚠️ Notes

This writeup avoids sharing sensitive details in respect of Hack The Box rules.
