```
switchport mode dynamic desirable
switchport mode dynamic auto
```
##### voice and data vlan
```
vlan 10
vlan 11
interface range FastEthernet0/1 - 4
switchport mode access
switchport access vlan 10
switchport voice vlan 11
```

##### stp
```
conf t
spanning-tree mode rapid-pvst
```
```
sh spanning-tree summary
spanning-tree bpdugard enable
```
##### port security
```
conf t
int fa0/1
switchport port-security  mac-address sticky
switchport port-security maximum 1
switchport port-security violation protect #restrict | shutdown
show port-security int fa0/1
sh mac-address-table
```
