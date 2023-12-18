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
