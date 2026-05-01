# Qual é o principal propósito do Oracle Cloud Infrastructure Functions?

## ✅ Resposta correta:

➡️ Executar código em resposta a eventos ou solicitações HTTP.
O principal propósito do OCI Functions é executar código em resposta a eventos ou solicitações HTTP, fornecendo uma plataforma de computação sem servidor que permite aos desenvolvedores construir, implantar e executar aplicativos sem a necessidade de gerenciar a infraestrutura subjacente.

## 🧠 Explicação (resumo para prova)

O Oracle Functions é um serviço serverless (FaaS):

⚡ Executa código sob demanda

🔔 Disparado por eventos ou requisições HTTP

💰 Cobrança por execução (não fica rodando sempre)

👉 Ou seja, você não gerencia servidor, só envia o código.

## ❌ Por que as outras estão erradas?

🖥️ Implantar e gerenciar máquinas virtuais
→ Isso é Compute (VM)

🗄️ Serviço de banco de dados
→ Isso é OCI Database

📁 Armazenar arquivos
→ Isso é Object Storage

## 🎯 Dica de prova

Se aparecer:
🔔 evento

⚡ execução sob demanda

☁️ serverless

👉 Pense direto: Oracle Functions 🚀

# Quais dois parâmetros podem ser personalizados ao criar uma instância de computação de forma flexível?

✅ Respostas corretas:

✔️ Quantidade de memória
Ao criar uma instância de computação de forma flexível no OCI, os usuários podem personalizar o número de Oracle Cloud Processor Units (OCPUs) e a quantidade de memória alocada para a instância. O número de NICs virtuais e físicos não são parâmetros personalizáveis para instâncias de forma flexível.

✔️ Número de OCPUs
Ao criar uma instância de computação de forma flexível no OCI, os usuários podem personalizar o número de Oracle Cloud Processor Units (OCPUs) e a quantidade de memória alocada para a instância. O número de NICs virtuais e físicos não são parâmetros personalizáveis para instâncias de forma flexível.

## 🧠 Explicação (resumo para prova)

Na OCI, ao criar uma instância com shape flexível (flex), você pode ajustar:

🧠 OCPUs (CPU)

💾 Memória (RAM)

👉 Isso permite customizar performance e custo conforme necessidade.

## ❌ Por que as outras estão erradas?
🔌 Número de NICs físicos
→ ❌ Não é configurável pelo usuário (infraestrutura da OCI)

🌐 Número de NICs virtuais (VNICs)
→ ❌ Podem ser adicionadas depois, mas não fazem parte do shape flex

## 🎯 Dica de prova

Se aparecer “shape flexível”:

👉 Pense sempre:

🧠 CPU (OCPU)
💾 Memória (RAM)

🚀 Esses são os dois parâmetros principais!

# Qual tipo de armazenamento está associado às instâncias no serviço OCI Compute?

## ✅ Resposta correta:

➡️ Armazenamento em Bloco

O armazenamento em bloco é o tipo de armazenamento associado às instâncias no serviço OCI Compute. Ele fornece volumes de armazenamento de alta performance e baixa latência que podem ser anexados às instâncias para armazenar dados e aplicativos.

## 🧠 Explicação (resumo para prova)

As instâncias do OCI Compute usam:

💾 Block Storage (Armazenamento em Bloco)

👉 funciona como um HD/SSD anexado à máquina

Exemplos:

🔹 Boot Volume (disco do sistema)

🔹 Block Volume (disco adicional)

## ❌ Por que as outras estão erradas?

📁 Armazenamento de Arquivos (File Storage)
→ usado para compartilhamento via rede (NFS)

☁️ Armazenamento de Objetos (Object Storage)
→ usado para backups, imagens, arquivos estáticos

📄 Armazenamento de Arquivo
→ termo incorreto / duplicado

##  🎯 Dica de prova

Se a pergunta falar:

🖥️ instância / VM

💾 disco anexado

👉 resposta = Block Storage 🚀
