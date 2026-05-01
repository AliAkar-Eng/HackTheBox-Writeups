Responder Lab

1)Configuring ip to domain unika.htb

2)Running nmap and discovers 2 open ports 80 and 5985

3)from port 80 ie web app told target to connect to fileshare named test on an ip which is mine and used responder -I tun0 to trick the target into thinking im a legit server 
then he would connect via nt lan ie login with username and password.

4)Responder catched the hashed pass and cracked it using john the ripper

5)port 5985 was running winrm ie a service to remote manage windows we will try to login using the credentials we cracked and guess what it worked

using evil-winrm

6)inside the shell navigated to one of the users and got the flag

DONE

Note)Capturing credentials from one site and tryiung them into another is a critical vulnerability catch
