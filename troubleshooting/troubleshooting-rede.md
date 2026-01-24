# 🛠️ Troubleshooting de Rede — Passo a Passo

Troubleshooting é o processo de identificar e resolver problemas de rede
seguindo uma ordem lógica, do mais simples ao mais complexo.

---

## ✅ Passo 1 — Camada Física

Verificar:
- Cabo conectado?
- LED da porta está aceso?
- Wi-Fi está ligado?

Comandos:
- (não há comando, é verificação física)

Problemas comuns:
- Cabo ruim
- Porta queimada
- Wi-Fi desligado

---

## ✅ Passo 2 — Enlace (Rede Local)

Verificar:
- Placa de rede ativa?
- Recebeu endereço MAC?

Comandos:
- `ipconfig` (Windows)
- `ifconfig` ou `ip a` (Linux)

Problemas comuns:
- Driver de rede
- Interface desativada

---

## ✅ Passo 3 — IP (Camada de Rede)

Verificar:
- Tem endereço IP?
- Gateway configurado?

Comandos:
- `ipconfig`
- `ping 127.0.0.1`
- `ping SEU_GATEWAY`

Problemas comuns:
- DHCP não funcionando
- IP errado

---

## ✅ Passo 4 — Conectividade Externa

Testar:
- Ping para fora da rede

Comandos:
- `ping 8.8.8.8`

Se responder:
- Internet está funcionando
Se não responder:
- Problema no roteador ou provedor

---

## ✅ Passo 5 — DNS

Verificar:
- Nome de site resolve?

Comandos:
- `ping google.com`
- `nslookup google.com`

Se IP responde mas nome não:
- Problema é DNS

---

## ✅ Passo 6 — Aplicação

Verificar:
- Serviço está ativo?
- Porta está aberta?

Comandos:
- `netstat -an`
- `ss -tuln` (Linux)

Problemas comuns:
- Firewall bloqueando
- Serviço parado

---

## 🔁 Dica Importante

Sempre teste **de baixo para cima** (modelo OSI/TCP-IP):
1. Físico
2. Rede local
3. IP
4. Internet
5. DNS
6. Aplicação

Isso evita perder tempo.

---

## 🎯 Onde isso é usado?

- Suporte técnico
- Redes corporativas
- Laboratórios no Packet Tracer
- Segurança da informação

