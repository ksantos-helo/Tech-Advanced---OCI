# 📌 Monitoramento de Processos e Agendamento com Cron

O monitoramento de processos e o uso de cron jobs são fundamentais para manter servidores eficientes, disponíveis e seguros. Com isso, é possível automatizar tarefas como análise de desempenho, verificação de serviços e monitoramento de logs.

🛠️ Atividades Práticas

## 🔹 1. Monitorar uso de CPU

Script para listar os processos que mais consomem CPU:

```
#!/bin/bash

echo "Top 5 processos por uso de CPU:"
ps aux --sort=-%cpu | head -n 6
```

Explicação:

ps aux → lista todos os processos
--sort=-%cpu → ordena pelo maior uso de CPU
head -n 6 → mostra os 5 primeiros + cabeçalho


## 🔹 2. Monitorar uso de Memória

Script para listar os processos que mais consemem memória:
```
#!/bin/bash

echo "Top 5 processos por uso de memória:"
ps aux --sort=-%mem | head -n 6
```

Explicação:

Similar ao anterior, mas ordena por uso de memória (%mem)

## 🔹 3. Verificar se um processo está em execução
```
#!/bin/bash

processo="nginx"

if pgrep $processo > /dev/null; then
  echo "$processo está em execução."
else
  echo "$processo não está em execução."
fi
```

Explicação:

pgrep → busca o processo pelo nome
> /dev/null → oculta a saída
if → verifica se o processo existe


## 🔹 4. Analisar logs de erro do sistema
```
#!/bin/bash

echo "Últimas 10 linhas de mensagens de erro:"
tail -n 10 /var/log/syslog | grep "error"
```

Explicação:

tail -n 10 → pega as últimas 10 linhas do log
grep "error" → filtra apenas mensagens de erro


## 🔹 5. Monitoramento automático com cron
📄 Script
```
#!/bin/bash

echo "Mensagens de erro - $(date)" >> /caminho/do/log_monitorado.txt
tail -n 5 /var/log/syslog | grep "error" >> /caminho/do/log_monitorado.txt
```

Explicação:

$(date) → registra data e hora
>> → adiciona ao arquivo sem sobrescrever
salva as últimas 5 mensagens de erro


⏰ Configuração do Cron
```
0 */2 * * * /caminho/do/seu/script.sh
```

Explicação:

Executa o script a cada 2 horas

Estrutura:

minuto hora dia mês dia-da-semana

## ✅ Resumo Final

ps, grep, sort → monitoramento de processos

pgrep → verificação de serviços

tail + logs → análise de erros

cron → automação de tarefas
