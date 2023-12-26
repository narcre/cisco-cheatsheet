##### Router Loopback Interface
```
interface loopback 40
ip address 192.168.10.10 255.255.255.0
```

##### Ping and Telnet with Source 
```
do ping 172.22.40.40 source loopback 40
do ping 172.22.40.40 source 192.168.10.10


telnet 172.22.40.40 /source-interface loopback 40
```

##### Show Route Table
```
do sh run | s ip route
do sh ip int br | s ip route
```

##### Defult Route
```
ip route 0.0.0.0 0.0.0.0 10.10.10.2
```
