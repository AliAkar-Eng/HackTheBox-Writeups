Fawn - Hack The Box

🧠 Skills Learned

- FTP enumeration
- Anonymous login
- Basic file retrieval

🔍 Enumeration

I started with an nmap scan to identify open ports and services:

nmap -sV <target-ip>

Results:

- Port 21 open → FTP service detected

🚪 Initial Access

Since FTP was open, I attempted anonymous login:

ftp <target-ip>

Credentials used:

- Username: anonymous
- Password: empty

Login was successful.

📂 Exploring the Server

After logging in:

- Listed files using: ls
- Found a file containing the flag

Downloaded it using:
get <filename>

🏁 Outcome

Successfully accessed the FTP server and retrieved the file.

📌 Key Takeaways

- Always check for anonymous FTP access
- Misconfigured services can lead to easy entry
- Enumeration is the most important step

⚠️ Notes

This writeup avoids sharing sensitive details in respect of Hack The Box rules.
