# 🔧 Configuração básica de Router Cisco


## 📡 Descobrindo as interfaces


```bash
enable
show ip interface brief

conf t
interface g0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit

interface g0/1
ip address 192.168.2.1 255.255.255.0
no shutdown
exit

show ip interface brief
ping 192.168.1.10

copy running-config startup-config
no shutdown
