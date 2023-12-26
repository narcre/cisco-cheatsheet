##### Enter vlan Routing
```
do sh ip int br
interface GigabitEthernet 0/0
no shut
#in switch
switchport mode trunk
#sub interface (In Router)
int g0/0.10 #10 is name of vlan 10 for example
encapsulation dot1Q 10 #10 is name of vlan 10
ip address 10.10.10.1 255.255.255.0
```

###### With Switch in Layer 2
```
switchport trunk encapsulation dot1q
switchport mode trunk
ip routing
no switch port  # for set ip on port
```

```
#switch 0
vlan 10
interface fastEthernet 0/2
switchport access vlan 10
switchport mode trunk

#mls
switchport mode trunk
vlan 10
int vlan 10
int fastEthernet 0/1
ip address 20.20.20.1 255.0.0.0

do sh ip int brief
```

###### Rote Table For Router
```
#on router 1
#ip
ip route 60.60.60.60 255.255.255.255 172.20.20.2
#network
ip route 60.60.60.0 255.255.255.0 172.20.20.2
ip route 50.50.50.0 255.255.255.0 gigabitEthernet 0/0
```
