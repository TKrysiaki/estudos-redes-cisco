# 📡 Modelo OSI — As 7 Camadas da Rede

O **Modelo OSI (Open Systems Interconnection)** é um modelo teórico que explica como os dados trafegam em uma rede, da aplicação até o meio físico.

Ele é dividido em **7 camadas**, cada uma com uma função específica.

---

## 🧩 Camadas do Modelo OSI

### 7. Aplicação
Onde ficam as aplicações usadas pelo usuário.  
Exemplos: `HTTP`, `FTP`, `SMTP`, `DNS`

---

### 6. Apresentação
Responsável por formatar, comprimir e criptografar os dados.  
Exemplos: `SSL/TLS`, compressão, conversão de formatos

---

### 5. Sessão
Gerencia a sessão de comunicação entre dois dispositivos.  
Funções: abertura, manutenção e encerramento da conexão

---

### 4. Transporte
Garante a entrega dos dados (ou não, dependendo do protocolo).  
Protocolos:  
- `TCP` → confiável, com controle de erros  
- `UDP` → rápido, sem garantia de entrega  
Trabalha com **portas**

---

### 3. Rede
Responsável pelo endereçamento e roteamento dos pacotes.  
Protocolos e dispositivos:  
- `IP`  
- Roteadores (Routers)

---

### 2. Enlace de Dados (Data Link)
Comunicação dentro da rede local.  
Funções:  
- Endereço MAC  
- Controle de acesso ao meio  
Dispositivos: Switches  
Tecnologias: Ethernet

---

### 1. Física
Transmissão dos bits no meio físico.  
Inclui:  
- Cabos  
- Conectores  
- Sinais elétricos ou ondas de rádio (Wi-Fi)

---

## 🎯 Para que o Modelo OSI é usado?

- Entender como as redes funcionam
- Facilitar diagnóstico de problemas:
  - Problema no cabo? → Camada 1
  - Sem IP? → Camada 3
  - Aplicação não conecta? → Camada 7
- Base para estudos de redes, segurança e análise de tráfego (Wireshark, Packet Tracer)

---

## 📌 Observação

Na prática, a internet usa o **modelo TCP/IP (4 camadas)**, mas o OSI é essencial para estudo e troubleshooting.
