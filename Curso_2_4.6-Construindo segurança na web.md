# Pergunta


Após implementar o protocolo HTTPS no projeto de uma plataforma de e-commerce, sua equipe quer garantir que a comunicação entre o cliente e o servidor não apenas seja criptografada, mas também otimizada para manter uma boa experiência do usuário. Na reunião semanal de planejamento do trabalho de desenvolvimento e operações, você foi a pessoa designada para propor uma solução.


# Resposta
👉 Implementar um Load Balancer com terminação TLS (SSL Termination)

## 🧠 📌 Explicação objetiva

A solução envolve:

### 🔒 1. Segurança
O Load Balancer recebe conexões HTTPS
Realiza a terminação TLS (descriptografa o tráfego)

### 🔄 2. Distribuição eficiente
Após descriptografar, o Load Balancer:

🔀 Distribui as requisições entre múltiplos servidores

⚖️ Balanceia a carga

🚀 Melhora desempenho

### ⚡ 🎯 Por que essa implementação é ideal?
Centraliza o gerenciamento de certificados 🔐

Reduz carga nos servidores back-end ⚡

Permite escalabilidade horizontal 📈

Garante alta disponibilidade

### 🧪 💡 Exemplo prático

Load Balancer (Nginx / AWS ALB)

Recebe: HTTPS

Encaminha para servidores internos
🏁 ✅ Conclusão (resposta de prova)

👉 Utilizar um Load Balancer com terminação TLS para gerenciar conexões HTTPS e distribuir o tráfego de forma eficiente entre múltiplos servidores.
