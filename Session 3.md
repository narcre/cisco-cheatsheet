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
switchport mode access
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
##### Group Interface By Range And Config Together
```
[no] interface range fa0/15 - 16
interface range fa0/15 , 11 , 2
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
###### VTP Modes Is Server | Client | Transparent
```
vtp mode client
```
##### Set Password By Encryption
```
service password-encryption
```
