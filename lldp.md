# LLDP (Link Layer Discovery Protocol)

## Protocolo de camada 2 utilizado para descobrir dispositivos vizinhos na rede.
Funciona entre equipamentos de diferentes fabricantes (multivendor).

### Verificar status
```show lldp```

### Ativar LLDP no switch Cisco
```
enable
conf t
lldp run
```

### Ver dispositivos conectados
```show lldp neighbors```

### Informações detalhadas dos vizinhos
```show lldp neighbors detail```

## Obs.: O LLDP precisa estar habilitado nos dois dispositivos para que as informações sejam trocadas.
