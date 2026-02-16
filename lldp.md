# LLDP (Link Layer Discovery Protocol)

## Protocolo de camada 2 utilizado para descobrir dispositivos vizinhos na rede.
É um protocolo padrão de camada 2 usado para descoberta de dispositivos vizinhos na rede. Permite que equipamentos compartilhem automaticamente informações como identificação do dispositivo, porta conectada, nome do sistema, capacidades (roteador, switch etc.) e endereços IP/MAC.

Por ser um protocolo multivendor, funciona entre equipamentos de diferentes fabricantes, ao contrário de protocolos proprietários como o CDP (Cisco). Isso facilita a visualização da topologia e o gerenciamento em ambientes heterogêneos.

As informações trocadas pelo LLDP ficam armazenadas em bancos MIB e podem ser consultadas via SNMP para monitoramento e gerenciamento de rede.

Os dispositivos enviam anúncios LLDP periodicamente pelas interfaces físicas ou sempre que ocorre alguma alteração na rede.


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


## Obs.: LLDP deve estar habilitado nos dois dispositivos para troca de informações.
