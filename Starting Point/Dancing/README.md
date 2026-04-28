Dancing - Hack The Box

🧠 Skills Learned

- SMB enumeration
- Accessing network shares
- Basic file discovery

🔍 Enumeration

Started with an nmap scan:

nmap <target-ip>

Results:

- Port 445 open → SMB service detected

🚪 Initial Access

Enumerated SMB shares using:

smbclient -L <target-ip> -N

Found accessible shares without authentication.

📂 Exploring the Server

Connected to a share:

smbclient //<target-ip>/<share-name> -U

- Listed files using: ls
- Found a file containing the flag

Downloaded it using:
get <filename>

🏁 Outcome

Successfully accessed SMB share and retrieved the file.

📌 Key Takeaways

- Always enumerate SMB when port 445 is open
- Anonymous access to shares is a common misconfiguration
- SMB can expose sensitive files easily

⚠️ Notes

This writeup avoids sharing sensitive details in respect of Hack The Box rules.
