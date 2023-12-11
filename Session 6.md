##### DHCP
```
int fa0/2
switchport mode acess
do sh int trunk
do sh ip int brief
switchport access vlan 10
do sh vlan brief

ip dhcp pool vlan10
network 10.10.10.0 255.0.0.0


ip dhcp excluded-address 10.10.10.1
dns-server 10.10.10.1
default-router 10.10.10.250
```
##### set ip on switch by dhcp
```
vlan 10 
int fa0/1
switchport mode trunk
switchport access vlan 10
exit
int vlan 10
ip address dhcp



sh cdp neighbors detail
int fastEthernet 0/2
no cdp enable
```

##### on all
```
no cdp run
do sh cdp
cdp run
```
##### see client
```
do sh arp
```
##### aggregate and ether channel
```
int range fastEthernet 0/1-4
switchport mode trunk
channel-group 1 mode desirable # auto
sh etherchannel summary
```
