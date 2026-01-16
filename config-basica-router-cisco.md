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
ping 192.168.1.10
copy running-config startup-config
no shutdown

Depois: **Commit changes**.

---

# ✅ ARQUIVO 2 — `README.md`

👉 Edite o README e **substitua tudo por isso**:

```md
# 📘 Estudos de Redes Cisco

Labs de estudo de redes Cisco (Packet Tracer) e comandos básicos de configuração de router.

---

## 📂 Conteúdos

### 🔧 Configuração de Router
- [Configuração básica de Router Cisco](config-basica-router-cisco.md)

### 🧪 Labs Packet Tracer
- lab1-rede-basica-router-switch.pkt — Rede básica com router e switch

---

## 🎯 Objetivo

Repositório criado para registrar minha evolução nos estudos de redes, com foco em prática e documentação dos comandos utilizados.
