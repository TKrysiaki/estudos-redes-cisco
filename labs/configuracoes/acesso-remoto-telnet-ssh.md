# Acesso Remoto em Switch e Router (Telnet e SSH)

## 🔴 Telnet (TCP porta 23)
### ⚠️ Telnet não é seguro (senha em texto puro). Em ambiente real, use sempre SSH.

### Comando para acessar:
```telnet 192.168.10.2```

### Se estiver bloqueado, configurar no dispositivo de destino:
```
enable
conf t
line vty 0 4
password (senha)
login
transport input telnet
end
```
### Depois tentar novamente o Telnet.

### Para sair da sessão:
```exit```

## SSH (TCP porta 22)
### Definir domínio (obrigatório para gerar chave)
### No Router
```
enable
conf t
ip domain-name cisco.com
```
### Gerar chave RSA
```crypto key generate rsa```

### Tamanho da chave:
```1024```

### Criar usuário local
```username admin secret 1234```

### Configurar VTY para usar SSH
```
line vty 0 4
login local
transport input ssh
exit
```

### Salvar configurações
```copy running-config startup-config```

## 🧭 Rotas Estáticas entre Roteadores

Para permitir comunicação entre as duas redes (192.168.10.0/24 e 192.168.20.0/24), foram configuradas rotas estáticas nos roteadores.


### Router 01
```Rede local: 192.168.10.0/24```
```Link entre roteadores: 10.0.0.1/30```

```ip route 192.168.20.0 255.255.255.0 10.0.0.2```

### Router 02
```Rede local: 192.168.20.0/24```
```Link entre roteadores: 10.0.0.2/30```

```ip route 192.168.10.0 255.255.255.0 10.0.0.1```

## ✔ Teste

Ping entre hosts das duas redes funcionando, confirmando roteamento correto.


## 🔵 Acessando via SSH de outro dispositivo
```
enable
ssh -l admin 192.168.10.2
```
Senha:
```1234```

Para sair da conexão:
```exit```










