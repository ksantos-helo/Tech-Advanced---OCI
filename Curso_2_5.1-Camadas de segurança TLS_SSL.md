
## 🔐 HTTPS, SSL e TLS — Resumo

- O **HTTPS** é a versão segura do HTTP  
- Ele utiliza **TLS/SSL** para criptografar a comunicação entre cliente e servidor  
- O 🔒 cadeado no navegador indica que o site é seguro (ex: https://google.com)

---

## ⚠️ Sites sem HTTPS
- Navegadores exibem aviso de **"não seguro"**
- Dados podem ser interceptados

---

## 🧩 SSL vs TLS

### 🔹 SSL (Security Socket Layer)
- Criado nos anos 90  
- Primeira camada de segurança  
- Hoje considerado **menos seguro** (vulnerável)

### 🔹 TLS (Transport Layer Security)
- Evolução do SSL  
- Mais **seguro e moderno**  
- Corrige falhas do SSL  
- Amplamente usado atualmente

---

## 🔑 Como funciona a segurança

- Uso de:
  - Certificado digital  
  - Chave privada  
- Criação de uma **chave de sessão**
- Essa chave:
  - Criptografa os dados  
  - É temporária (válida apenas durante a sessão)

---

## 🔄 Comunicação segura (passo a passo)

1. Usuário acessa uma URL  
2. Servidor envia certificado digital  
3. Cliente valida o certificado  
4. É criada uma conexão segura  
5. Dados passam a ser criptografados  

---

## 🔌 Sobre Sockets

- São "portas" de comunicação entre sistemas  
- Permitem troca de dados entre cliente e servidor  
- Muito usados na internet (ex: HTTP, SSH)

---

## 🚀 Conclusão

- HTTPS protege a comunicação na web  
- TLS é o padrão atual de segurança  
- Criptografia garante confidencialidade e integridade dos dados  
