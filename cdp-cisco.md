# 📡 Cisco CDP – Configuração e Verificação

## Acessar modo privilegiado
```enable```

## Verificar status do CDP
```bash
show cdp
```

## Ativar CDP globalmente (se necessário)
```bash
conf t
cdp run
```


## Ver dispositivos vizinhos
```show cdp neighbors```


## Ver detalhes dos vizinhos
```show cdp neighbors detail```


## Ver opções disponíveis do comando
```show cdp neighbors ?```


## Filtro personalizado (listar apenas IPs)
```show cdp neighbors detail | include IP address```


## Ativar CDP em uma interface específica
```bash
interface g0/1
cdp enable
```


## Desativar CDP em uma interface
```
interface g0/1
no cdp enable
```


## 📌 Observação:
### CDP é um protocolo proprietário Cisco usado para descobrir dispositivos diretamente conectados.
