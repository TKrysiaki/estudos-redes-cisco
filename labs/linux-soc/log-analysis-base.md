# Log Analysis — Base

## Objetivo
Analisar logs SSH após simulação de ataque brute force.

## Ambiente
- Kali Linux (attacker)
- Ubuntu Server (target)
- SSH habilitado

## Logs analisados
/var/log/auth.log

## Comandos utilizados
grep sshd /var/log/auth.log
grep "Failed password" /var/log/auth.log
wc -l

## Evidências
- múltiplas tentativas de login falhadas
- identificação do IP atacante
- horários registrados no log

## Conclusão
Ataque brute force identificado com sucesso através da análise de logs SSH.
