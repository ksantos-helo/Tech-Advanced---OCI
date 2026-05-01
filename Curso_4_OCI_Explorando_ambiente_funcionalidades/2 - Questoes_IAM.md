# ☁️  Qual componente de Gerenciamento de Identidade e Acesso ajuda a organizar vários usuários em uma equipe?

↪️ Grupos
Grupos no OCI Identity and Access Management (IAM) são usados para organizar vários usuários em uma equipe, facilitando a gestão de permissões e acessos.


# ☁️  Qual afirmação sobre o OCI Identity and Access Management é verdadeira?
↪️ Ele permite controlar o acesso para um grupo de usuários.

O OCI Identity and Access Management (IAM) permite controlar o acesso para um grupo de usuários, facilitando a gestão de permissões e acessos aos recursos na nuvem.

# ☁️ Qual afirmação sobre os compartimentos do OCI NÃO é verdadeira?
↪️ É uma prática recomendada criar todos os seus recursos no compartimento raiz.
Não é uma prática recomendada criar todos os recursos no compartimento raiz. Compartimentos são usados para organizar e isolar recursos, proporcionando um nível mais refinado de controle de acesso.

# ☁️ Qual NÃO é um componente do OCI Identity and Access Management?
↪️ Grupo de Segurança de Rede
O Grupo de Segurança de Rede é um componente do OCI Networking, não do IAM. O IAM no OCI consiste em Principais, Políticas, Federação e alguns outros componentes.


O Network Security Group (NSG) ou Grupo de Segurança de Rede é um recurso de rede e segurança de tráfego, não de Identity and Access Management.

## 🎯 Função do NSG:

Controlar tráfego de rede para recursos, como:

🌐 Regras de entrada (Ingress)

🌐 Regras de saída (Egress)

🔒 Liberação de portas

🖥️ Proteção de instâncias

➡️ Pertence à área de Networking, não IAM.

## ✅ Por que os outros são componentes do IAM?
## ✔️ Políticas

Definem permissões de acesso.

Exemplo:
Allow group DevOps to manage instances

## ✔️ Principais (Principals)

Entidades que podem receber permissões:

👤 Usuários

👥 Grupos

🤖 Recursos/Serviços

### ✔️ Federação

Integra identidades externas:

Microsoft AD
SSO
Provedores externos

# ☁️ Como um recurso no OCI é identificado?

☑️ A)  Com ID da Tenancy

☑️ B) Com Nome do Compartimento

🟢 ☑️ C) Com OCID

Cada recurso no OCI é identificado por um Oracle Cloud Identifier (OCID) único, que é usado para identificar o recurso.

☑️ D) Com Nome de Usuário


# 🎯 O que cai na prova (OCI IAM - Identity and Access Management)

---

# 👥 Organização de usuários

## 📌 Grupos (Groups)

✅ Organizam vários usuários em equipes  
✅ Facilitam gestão de permissões  
✅ Usados para aplicar políticas em conjunto  

👉 Exemplo:
- DevOps Team
- Finance Team
- Admins

---

# 🔐 OCI IAM (Identity and Access Management)

## 🎯 Função principal

✅ Controlar acesso aos recursos da OCI  
✅ Definir permissões por usuário ou grupo  
✅ Garantir segurança e governança  

---

## 🧠 O que cai na prova

✔️ IAM controla acesso de usuários e grupos  
✔️ Permissões são dadas via **políticas (Policies)**  
✔️ Usuários fazem parte de grupos  

---

# ❌ Compartimentos (Pegadinha de prova)

## 📦 Compartments

- Usados para organizar recursos
- Usados para isolamento e segurança

## ❌ ERRADO (cai muito):

🚫 “Criar tudo no compartimento raiz”

👉 Isso NÃO é recomendado

---

## 🎯 Correto:

✔️ Usar múltiplos compartments  
✔️ Segmentar por projeto / equipe / ambiente  

---

# 🚫 O que NÃO faz parte do IAM

## ❌ Network Security Group (NSG)

👉 Não é IAM

### 📌 Ele pertence a:

🌐 Networking (rede)

### 🎯 Função:

- 🔒 Controlar tráfego de rede
- 🚪 Regras de entrada (Ingress)
- 🚪 Regras de saída (Egress)
- 🖥️ Proteger instâncias

---

# 🔑 Componentes do IAM

## 👤 Principals (Principais)

✔️ Usuários  
✔️ Grupos  
✔️ Serviços  

---

## 📜 Policies (Políticas)

✔️ Definem permissões  
Ex:
- “Grupo DevOps pode gerenciar instâncias”

---

## 🔗 Federation

✔️ Integra identidades externas  
- Microsoft AD  
- SSO  
- Provedores externos  

---

# 🆔 Identificação de recursos OCI

## 🎯 OCID

✔️ Oracle Cloud Identifier  
✔️ ID único de cada recurso na OCI  

---

## ❌ Não é usado:

🚫 Nome de usuário  
🚫 Nome do compartimento  
🚫 Apenas label simples  

---

# 🎯 O que cai na prova (resumo final)

✅ Groups = organizam usuários em equipes  
✅ IAM = controla acesso a recursos OCI  
✅ Policies = definem permissões  
✅ Compartments = organizam e isolam recursos  
🚫 Não usar compartimento raiz para tudo  
🚫 NSG NÃO é IAM (é Networking)  
✅ OCID = identificador único de recursos  
