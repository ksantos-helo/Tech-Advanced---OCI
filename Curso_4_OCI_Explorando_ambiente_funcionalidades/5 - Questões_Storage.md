# 📘 Revisão para Certificação OCI

Material resumido com explicações objetivas e emojis para facilitar a memorização 🚀

---

## 🧠 1) Object Storage - Nível Archive

**❓ Pergunta:**  
Você criou um bucket no nível Archive. Qual afirmação **NÃO é válida**?

**✅ Resposta correta:** 

❌ O bucket de armazenamento Archive pode ser atualizado para o armazenamento Standard.

**💡 Explicação:**

- 🚫 Buckets **Archive NÃO podem ser convertidos** para Standard  
- ⏳ Tempo mínimo de armazenamento: **90 dias**  
- 🔒 Objetos **não são acessados diretamente**  
- 🔄 É necessário **serem restaurados para o nível Standard antes de serem lidos.**

**📌 Resumo:**  
> Archive = barato 💰 + acesso lento 🐢 + retenção longa 📦  

---

## 💾 2) Block Volume - Durabilidade

**❓ Pergunta:**  
Qual recurso garante durabilidade e proteção contra falhas?

**✅ Resposta correta:**  
✔️ **Replicação**

**💡 Explicação:**

- 📀 Dados são replicados automaticamente  
- 🏗️ Replicação ocorre dentro do mesmo **Availability Domain**  
- 🔁 Protege contra falhas de hardware  

**📌 Resumo:**  
> Replicação = segurança + alta disponibilidade 🛡️  

---

## ⚡ 3) Block Volume - Alto Desempenho

**❓ Pergunta:**  
Qual nível atende ≥ 90 IOPS/GB e até 90.000 IOPS?

**✅ Resposta correta:**  
🚀 **Ultra High Performance**

**💡 Explicação:**

- ⚡ Até **225 IOPS/GB**  
- 📊 Até **300.000 IOPS por volume**  
- 🧠 Ideal para:
  - Banco de dados de alta performance  
  - Sistemas críticos  

**📌 Resumo:**  
> Ultra High Performance = máximo desempenho 💥  

---

## 🔐 4) Object Storage - URL Pré-autenticada

**❓ Pergunta:**  
Qual o propósito da URL pré-autenticada?

**✅ Resposta correta:**  
🔗 **Fornecer acesso temporário e seguro a um objeto específico**

**💡 Explicação:**

- ⏳ Define tempo de expiração  
- 🔓 Permite acesso **sem autenticação adicional**  
- 📤 Ideal para compartilhamento seguro de arquivos  

**📌 Resumo:**  
> URL pré-auth = acesso temporário + seguro 🔐  

---

## 🗄️ 5) Object Storage - Melhor custo para backup

**❓ Pergunta:**  
Qual nível usar para backup de longo prazo com menor custo?

**✅ Resposta correta:**  
📦 **Archive**

**💡 Explicação:**

- 💰 Mais barato da OCI  
- 🕒 Acesso lento (necessário restaurar antes)  
- 📚 Ideal para:
  - Backups  
  - Dados raramente acessados  

**📌 Resumo:**  
> Archive = custo baixo 💸 + longo prazo 📆  

---

# 🎯 Dica Final para a Prova

💥 Foque nessas diferenças-chave:

| Serviço | Destaque |
|--------|---------|
| 📦 Archive | Barato, acesso lento, retenção longa |
| 💾 Block Volume | Replicação automática |
| ⚡ Ultra High Performance | Máximo desempenho |
| 🔐 Pre-auth URL | Acesso temporário e seguro |

---

## 🚀 Estratégia de Memorização

- 🧩 **Archive** → backup e longo prazo  
- ⚙️ **Block Volume** → performance e durabilidade  
- 🔐 **Pre-auth** → compartilhamento seguro  
- ⚡ **Ultra High** → cargas críticas  

---

📌 **Dica:** Essas questões caem muito em prova! Foque nos detalhes de cada serviço.
