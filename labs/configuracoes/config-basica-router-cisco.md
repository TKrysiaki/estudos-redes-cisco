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
```

```bash
Teste de conectividade
ping 192.168.1.10
```

## Renomenando Router
```bash
enable
conf t
hostname hostname R1
```

## Salvando as Configurações
```bash
copy running-config startup-config
