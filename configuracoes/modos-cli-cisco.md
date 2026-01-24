# Comandos Cisco — Modos de Operação (CLI)

> Dica: a tecla `?` mostra os comandos disponíveis no modo atual.

## Modos

### 🔹 Switch> - User EXEC 
- Acesso limitado (somente visualização básica)

---

### 🔹 Switch# - Privileged EXEC
Entrar: 
```
enable
```
- Acesso total para visualização e comandos administrativos

---

### 🔹 Switch(config)# -Configuration mode
Entrar:
```
configure terminal
```
- Configurações globais do equipamento

---

### 🔹 Switch(config-if)# - interface mode
Entrar:
```
interface g0/1 ou interface g0/2 etc...
```
- Configurações valem somente para essa interface

---
### Dicas
```
Para voltar ao menu anteior usamos a palavra exit, ou para voltar direto para o Privileged EXEC usamos a palavra end
```
```Para mostrar os comandos disponiveis usamos a tecla "?" (interrogação)```
