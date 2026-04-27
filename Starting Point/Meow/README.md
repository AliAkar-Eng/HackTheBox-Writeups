Meow - Hack The Box

🧠 Skills Learned

- Basic enumeration
- Telnet usage
- Trying default credentials

🔍 Enumeration

I started with an nmap scan to identify open ports and services:

nmap -sC -sV <target-ip>

Results:

- Port 23 open → Telnet service detected

🚪 Initial Access

Since Telnet was open, I connected using:

telnet <target-ip>

I tried common usernames and found that:

- "root" worked without a password

🏁 Privilege Escalation

Already logged in as root, so no escalation needed.

📌 Key Takeaways

- Always scan first (enumeration is critical)
- Telnet is insecure and often misconfigured
- Default credentials can give instant access

⚠️ Notes

This writeup avoids sharing sensitive details in respect of Hack The Box rules.
