# w1ndow5_3num
This repo contains multiple commands that will aid in enumerating Windows OS.  *For educational purposes only and should be used ethically.

# System Enumeration

- systeminfo
- systeminfo | findstr /b /c:"OS Name" /c:"OS Versoin" /c:"System Type"
- wmic qfe - return info of system we are running it on qfe - when whas it last patched
- wmic qfe Caption,Description,HotFixID,InstalledOn
- wmic logicaldisk
- wmic logicaldisk get caption,description,providername
- wmic logicaldisk get caption

# User Enumeration

- whoami
- whoami /priv
- whoami /group
- net user
- net user "username"
- inetsrv>net localgroup
- inetsrv>net localgroup "group"


# Network Enumeration

- inetsrv>ipconfig
- inetsrv>arp -a
- netstat -ano (Internal Services are important also)

# Password Hunting

- findstr /si password *.txt
- findstr /si password *.txt *.config *.ini
- PayloadsAllTheThings Guide - [https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology and Resources/Windows - Privilege Escalation.md](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Windows%20-%20Privilege%20Escalation.md)


# Antivirus Enumeration: 

- sc queryex type= service
- netsh advfirewall firewall dump
- netsh firewall show state
- netsh firewall show config
- sc query windefend

