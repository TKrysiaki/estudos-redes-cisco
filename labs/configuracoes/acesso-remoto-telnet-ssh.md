# Acesso Remoto em Switch e Router (Telnet e SSH)

## 🔴 Telnet (TCP porta 23)

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
```
enable
conf t
ip domain-name cisco.com
```
### Gerar chave RSA
```crypto key generate rsa```

### Tamanho da chave:
````1024```

### Criar usuário local
```username admin secret cisco```

### Configurar VTY para usar SSH
```
line vty 0 4
login local
transport input ssh
exit
```

### Salvar configurações
```copy run start```

## 🔵 Acessando via SSH de outro dispositivo
```
enable
ssh -l admin 192.168.10.2
```
Senha:
````cisco```

Para sair da conexão:
```exit```










