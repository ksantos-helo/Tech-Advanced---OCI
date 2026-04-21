# 🔐📡 Resumo — Segurança, HTTP/HTTPS e Wireshark (DevOps)

---

## 🧠 Conceitos principais
- 🌐 Aplicações web usam **HTTP** para comunicação cliente-servidor  
- 🔓 HTTP **NÃO é seguro** → dados trafegam em texto aberto  
- 🔒 HTTPS adiciona **criptografia (SSL/TLS)** → protege os dados  

---

## 🕵️ Wireshark (Análise de Rede)
- 📡 Ferramenta para **capturar e analisar pacotes em tempo real**
- 🔍 Permite:
  - Diagnosticar problemas de rede  
  - Analisar protocolos (HTTP, TLS)  
  - Investigar segurança  

### ⚠️ Descoberta importante
- Com filtro:
   ```
  bash
  tcp.port == 8000 && http
    ```
Foi possível ver:

📧 Email

🔑 Senha
➡️ Dados expostos na rede

### 🔒 Problema do HTTP
❌ Dados trafegam sem proteção

❌ Vulnerável a interceptação (sniffing)

❌ Informações sensíveis ficam visíveis

### 🔐 Solução: HTTPS
✅ Usa SSL/TLS para criptografia

✅ Dados ficam ilegíveis (criptografados)

✅ Mais segurança na comunicação

### 🔑 OpenSSL
🛠️ Ferramenta para:

Gerar chave privada (server.key)

Gerar certificado digital (server.crt)

### ▶️ Comando principal:
```
openssl req -x509 -sha256 -nodes -days 365 -newkey rsa:2048 -keyout server.key -out server.crt
```

### 🧾 Certificado e Chave
🔐 Chave privada → fica no servidor (segredo)

🪪 Certificado digital → identidade do servidor

🔑 Contém:

Chave pública

Dados da organização

Assinatura digital

### 🔄 Criptografia no HTTPS
🔐 Assimétrica
Usa 2 chaves (pública + privada)

Mais segura, porém mais lenta

⚡ Simétrica
Usa 1 única chave

Mais rápida

🚀 Como o HTTPS funciona:
🔑 Usa criptografia assimétrica no início

🔄 Cria uma chave de sessão (simétrica)

⚡ Comunicação continua de forma rápida e segura

### 🧪 Teste prático (Wireshark)
Antes (HTTP):
👀 Dados visíveis

❌ Inseguro

Depois (HTTPS):
```
tcp.port == 8000 && tls
```

🔒 Dados ilegíveis

✅ Seguro

### 🧩 DevSecOps
🔐 Segurança integrada ao DevOps

👥 Responsabilidade de todo o time

🎯 Objetivo:

Proteger aplicações

Garantir confiabilidade

### 🎯 Conclusão
HTTP → ❌ inseguro

HTTPS → ✅ seguro (criptografia)

Wireshark mostrou na prática a diferença

OpenSSL permite implementar segurança no projeto

HTTPS usa combinação de criptografia para segurança + performance 🚀
