# 📌 CONFIGURAÇÃO BÁSICA DE SWITCH (CISCO)

## 🔧 Endereçamento

```Router: 192.168.10.1/24```

```Switch (gerenciamento): 192.168.10.2/24```

## 📝 Alterar nome do switch
```
- enable
- configure terminal
- hostname SW_01
```

## 🔐 Definir senha do modo privilegiado
```
- enable
- configure terminal
- enable secret SENHA_FORTE
```

## 📢 Configurar Banner (MOTD)

```
- enable
- conf t
- banner motd ^
==============================

          NY_01

==============================
^
```
O ^ indica início e fim do texto do banner.

##  💾 Salvar configurações
```copy running-config startup-config```

## 🌐 Configurar IP de gerenciamento (VLAN 1)
```
- enable
- conf t
- interface vlan 1
- ip address 192.168.10.2 255.255.255.0
- no shutdown
- exit
```

## 🚪 Definir Gateway Padrão do Switch
```
- conf t
- ip default-gateway 192.168.10.1
```
## ✅ Testes
### Do Router ou PC:
```ping 192.168.10.2```

### Do Switch:
```ping 192.168.10.1```
