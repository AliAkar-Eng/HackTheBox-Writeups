1)nmap resulted in port 1433 open ms sql server

2)exploit smb share by smbclient //ip -L

3)found password in backup share that required no password to enter

4)installed impacket tools to interact with sql server

5)loged in using the found credentials using mssql-client

6)explored xp_cmdshell to write cmd commands in the sql server but it was a little tight so developed a reverse shell to my kali machineusing netcat

7)installed winpeas to further privelage escalate and found file named consolehost-history.txt and found administrator login credentials

8)loged in as the admin using psexec.py and found the flag

GOAL

Found misconfigured credentials and using them to login
