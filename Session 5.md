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
