# Configurações Básicas em Equipamentos Cisco (CLI)

## 🔹 Alterar Hostname

## Entrar em modo de configuração:
```enable > configure terminal```

---

## Alterar nome do equipamento:
Digite: 
```hostname NY-01```

---

## 🔐 Enable Secret (senha do modo privilegiado)

### Configurar senha:
Digite: 
```
enable > configure terminal > enable secret "SENHA"
(Substitua `SENHA` pela senha desejada.)
```

---

## ⏰ Relógio (Clock)

## Ver data e hora:
Digite: 
```show clock```
## Configuração manual (menos recomendada)
Digite:
```enable > clock set 21:30:00 15 jan 2026```
## Configuração via servidor NTP (recomendado)
Digite:
```enable > configure terminal > ntp setver 2.2.2.2```
(troque o 2.2.2.2 pelo ip do fornecedor)

---
## ⚠️ Banner MOTD (aviso de acesso)

## Configurar banner:
Digite: 
```enable > configure terminal > banner motd ^```
(digite a mensagem)
```
=========== ACESSO RESTRITO ===========
Somente pessoal autorizado
^
(O símbolo `^` é o delimitador de início e fim da mensagem.)
```

---
## 💾 Salvar Configurações

## Salvar configurações permanentes:
Digite: 
```enable > copy running-config startup-config```
Confirme com **Enter** quando solicitar.

---

#### 💡 Dica Importante
## Para remover qualquer configuração, use `no` antes do comando.
Exemplo:
```no ntp server 2.2.2.2```
