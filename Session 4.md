##### Connect To Switch By SSH And Telnet
```
ip ssh version 2
ip domain name
SIC.net hostname cloud
#connect with telnet
telnet 10.10.10.100

#create key for ssh
crypto key generate rsa
line vty 0 4 transport input ssh

#ssh by node commandprompt
ssh -l [user] [ip]

#Show Online Users
do sh users
```
