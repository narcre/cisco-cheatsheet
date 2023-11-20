##### To get into Privileged Mode
```
enable
en
```
##### To get into Config Mode
```
conf t
```
##### Change HostName
```
hostname cloud
```
##### Cable Connection Or Remote CLI For Switch Sesstions
```
line console 0
line vty 5 15
```
##### RAM and NVRAM Command 
```
do show run
show run
```
##### Set Password on Console 0 (In Privileged Mode)
```
password 123
login
```
##### Ram Clear
```
reload
```
##### Set and Unset Password on Config Mode
```
conf t
enable pass 456
no enable password
```
##### Set Secret (hash password)
```
enable secret 456
no enable secret
```
##### write on VRAM
```
> wr
# do wr
# copy running-config startup-config
```
##### See RAM and NVRAM Configs And Clear Them
```
show startup-config (nvram)
sh run (ram)
erase startup-config
write erase
```
##### Set UserName And Password
```
conf t
username reza secret 123
line console 0
login local
```

##### See Mac Address Of Connected Devices
```
show mac address-table dynamic
```
