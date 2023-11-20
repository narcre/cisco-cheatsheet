##### Port Status On Switch
```
# do sh ip int br
```
##### Change Port Status To Shutdown and Up
```
shutdown
no shutdown
```
##### Switch To Port Config Mode
```
interface FastEthernet0/1
```
##### Config Port Type (Access Or Trunk)
```
interface mode access
switchport mode trunk
```
##### Create Vlan
```
vlan 10
```
##### Asign Access Port To Vlan
```
switchport access vlan 10
```
##### Vlan Status And Change Name
```
do sh vlan brief
do sh int trunk
name cloud
```

##### Set Ip and subnet To Vlan
```
int vlan 10
ip add 10.10.10.10 255.0.0.0
```
##### ‌Ban Special Vlan For Broadcasting
```
switchport trunk allowed vlan remove/[add] 20
```
##### Create Vlan For Brodcast To All Switch With vtp(vlan trunking protocol)
```
do sh vtp status
vtp domain cloud
vtp password 123
```
##### Change default vtp type(server to client)
```
vtp mode client
```
