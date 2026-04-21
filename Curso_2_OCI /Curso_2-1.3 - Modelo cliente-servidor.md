## 🌐 DevOps + HTTP + Modelo Cliente-Servidor (Resumo)

Em DevOps, o objetivo é conectar desenvolvimento e operações, garantindo que a aplicação funcione tanto no ambiente de desenvolvimento quanto para as pessoas usuárias em produção.

As aplicações web geralmente são disponibilizadas em servidores, utilizando ferramentas como Nginx ou Apache.

### 🔗 Comunicação na Web

A comunicação entre o computador da pessoa usuária (cliente) e o servidor acontece por meio do protocolo **HTTP (Hypertext Transfer Protocol)**, responsável pela troca de dados na web.

Essa comunicação funciona como uma troca de mensagens:
- O cliente envia uma requisição
- O servidor processa e responde

---

### 🧠 Modelo Cliente-Servidor

- **Cliente:** navegador ou aplicação (front-end)
- **Servidor:** backend que processa requisições

---

### ⚙️ Exemplo prático (Projeto AluraBooks)

1. Iniciar o backend:
```bash
cd api-alurabooks
npm run start-auth
```

Iniciar o frontend:
```
cd curso-react-alurabooks
npm start
```

Acessar no navegador:
```
http://localhost:3000
```

## 🔍 Monitorando a comunicação (DevTools)
No navegador:

Clique com botão direito → Inspecionar

Aba Network (Rede)

Ali você vê todas as requisições HTTP feitas pela aplicação.

## 📡 Exemplo de requisição
Ao cadastrar um usuário:

Método: POST

Endpoint: /public/registrar

Status: 200 OK (sucesso)

📥 Payload: dados enviados (nome, email, senha)
📤 Response: resposta do servidor

## 🔑 Pontos importantes
HTTP é a base da comunicação web

Toda interação gera uma requisição

O servidor responde com um status (ex: 200, 404, 500)

Front-end e back-end se comunicam constantemente

## ✅ Conclusão

O funcionamento de aplicações web segue o modelo cliente-servidor, onde o HTTP permite a troca de informações entre quem faz a requisição (cliente) e quem responde (servidor).
