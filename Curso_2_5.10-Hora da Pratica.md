# 📚 Atividades com Postman

### 🔹 Atividade 1

➡️ Abra o Postman e clique em "Request" para criar uma nova solicitação

➡️ Insira a URL de um site de sua escolha

➡️ Selecione o método GET

➡️ Adicione parâmetros de consulta, por exemplo:
```
?search=termo
```
➡️ Clique em Send

➡️ 👀 Analise a resposta no painel para entender como os parâmetros afetam o resultado

### 🔹 Atividade 2

➡️ Crie uma nova solicitação no Postman

➡️ Utilize a mesma URL da atividade anterior

➡️ Selecione o método POST

➡️ No corpo (Body):

Escolha raw
Selecione o formato JSON

➡️ Insira um JSON de exemplo:
```
{
  "usuario": "user123",
  "senha": "123456"
}
```

➡️ Clique em Send

➡️ 🔍 Observe como o servidor processa os dados enviados

### 🔹 Atividade 3

➡️ Crie uma nova solicitação GET

➡️ Insira uma URL com parâmetro de caminho, por exemplo:

/usuarios/123


➡️ Clique em Send

➡️ 👤 Analise a resposta para obter dados específicos do usuário

### 🔹 Atividade 4

➡️ Abra uma solicitação GET existente

➡️ Altere parâmetros na URL, por exemplo:

```
?page=1 ➡️ ?page=2
```

➡️ Clique em Send

➡️ 📊 Observe como a resposta muda conforme o valor dos parâmetros

### 🔹 Atividade 5

➡️ Crie uma nova solicitação POST para autenticação

➡️ Insira a URL para obter o token

➡️ Inclua os dados necessários no corpo

➡️ Clique em Send para obter o 🔑 token

➡️ Use o token em uma nova requisição GET:

Acesse uma área protegida
Envie o token no Header (Authorization)

➡️ 🔐 Analise como funciona a autenticação e o acesso restrito
