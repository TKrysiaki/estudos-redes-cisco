# 🌐 Modelo TCP/IP — As 4 Camadas da Internet

O **modelo TCP/IP** é o modelo usado na prática pela internet e pelas redes atuais.  
Ele possui **4 camadas** e é mais simples que o modelo OSI.

---

## 🧩 Camadas do Modelo TCP/IP

### 4. Aplicação
Reúne as camadas 7, 6 e 5 do OSI.  
Onde rodam os protocolos usados pelas aplicações.

Exemplos de protocolos:
- HTTP / HTTPS
- FTP
- SMTP / POP3 / IMAP
- DNS
- SSH

---

### 3. Transporte
Responsável pela comunicação entre origem e destino usando portas.

Protocolos:
- **TCP** → confiável, com controle de erros e retransmissão
- **UDP** → rápido, sem garantia de entrega

Funções:
- Controle de fluxo
- Segmentação dos dados
- Uso de portas (ex: 80, 443, 22)

---

### 2. Internet
Responsável pelo endereçamento lógico e roteamento dos pacotes.

Protocolos:
- IP (IPv4 / IPv6)
- ICMP (ping)
- IPsec

Dispositivos:
- Roteadores

Função principal:
- Escolher o melhor caminho até o destino

---

### 1. Acesso à Rede
Reúne as camadas 2 e 1 do OSI.

Inclui:
- Ethernet
- Wi-Fi
- Endereço MAC
- Cabos, placas de rede, sinais elétricos e rádio

Dispositivos:
- Switch
- Placa de rede (NIC)

---

## 🔁 Comparação OSI x TCP/IP

| OSI (7)            | TCP/IP (4)        |
|--------------------|------------------|
| Aplicação (7)      | Aplicação        |
| Apresentação (6)   | Aplicação        |
| Sessão (5)         | Aplicação        |
| Transporte (4)     | Transporte       |
| Rede (3)           | Internet         |
| Enlace (2)         | Acesso à Rede    |
| Física (1)         | Acesso à Rede    |

---

## 🎯 Por que o TCP/IP é importante?

- É o modelo realmente usado na internet
- Base para:
  - Configuração de redes
  - Wireshark
  - Packet Tracer
  - Segurança da informação
- Ajuda no diagnóstico de falhas de comunicação

---

## 📌 Resumo rápido

- OSI = modelo teórico para estudo
- TCP/IP = modelo prático usado no mundo real
