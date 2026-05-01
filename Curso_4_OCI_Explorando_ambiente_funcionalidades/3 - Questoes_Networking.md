# ☁️ Qual afirmação sobre o emparelhamento de Rede de Nuvem Virtual (VCN) entre dois VCNs NÃO é válida?

🟢 ☑️ A) Uma conexão de emparelhamento de VCN é uma conexão baseada em VPN.

O emparelhamento de VCN não é baseado em VPN; é uma conexão de rede entre dois VCNs que permite o roteamento de tráfego entre eles usando endereços IP privados.

☑️ B) VCNs emparelhados podem existir na mesma região da OCI.


☑️ C) VCNs emparelhados podem existir em diferentes regiões da OCI.


☑️ D) VCNs emparelhados não podem ter CIDRs sobrepostos.

###📘 Explicação

O VCN Peering (Emparelhamento de VCN) na OCI é uma conexão privada interna entre duas VCNs, feita pela infraestrutura da Oracle Cloud.

➡️ Não utiliza VPN tradicional pela internet.

Características do Peering:

🔒 Tráfego privado

⚡ Baixa latência

🌐 Rede interna Oracle

🚫 Sem internet pública no caminho

🔗 Comunicação entre VCNs

# ✅ Por que as outras estão corretas?
### ✔️ VCNs emparelhados podem existir na mesma região da OCI.

Correto. Isso é chamado de:

🔗 Local Peering
### ✔️ VCNs emparelhados podem existir em diferentes regiões da OCI.

Correto. Isso é chamado de:

🌍 Remote Peering
### ✔️ VCNs emparelhados não podem ter CIDRs sobrepostos.

Correto.

📌 As faixas de IP precisam ser diferentes para evitar conflito de roteamento.



# ☁️ Qual afirmação sobre uma Rede de Nuvem Virtual (VCN) é verdadeira?

🟢 ☑️ A) Uma VCN pode residir apenas em uma única região, mas pode abranger vários domínios de disponibilidade.
Uma VCN é uma rede privada virtual configurada em data centers da Oracle em uma única região da OCI e pode abranger todos os domínios de disponibilidade dessa região.

☑️ B) Uma VCN pode ter apenas uma sub-rede pública e mais de uma sub-rede privada.


☑️ C) Uma VCN pode abranger regiões da OCI.


☑️ D) Uma VCN pode ser usada com apenas uma instância.

# ❌ Por que as outras estão erradas?
### ❌ Uma VCN pode ter apenas uma sub-rede pública e mais de uma sub-rede privada.

Errado.

➡️ Uma VCN pode ter múltiplas subnets públicas e privadas, conforme necessidade.

### ❌ Uma VCN pode abranger regiões da OCI.

Errado.

➡️ Cada VCN pertence a uma única região.

Para conectar regiões diferentes usa-se:

🔗 Remote Peering
🌍 DRG
VPN / FastConnect
### ❌ Uma VCN pode ser usada com apenas uma instância.

Errado.

➡️ Uma VCN pode hospedar várias instâncias e recursos.

# ☁️ Qual componente NÃO é criado por padrão com a criação de uma Rede de Nuvem Virtual?

☑️ A) Lista de Segurança Padrão


☑️ B) Opções de DHCP Padrão


☑️ C) Tabela de Rota Padrão


🟢 ☑️ D) Gateway de Emparelhamento Local Padrão

Quando você cria uma VCN, uma tabela de rota padrão, uma lista de segurança padrão e opções de DHCP são criadas automaticamente, mas um Gateway de Emparelhamento Local (LPG) não é criado por padrão.

#📘 Explicação

Quando uma VCN é criada na OCI, alguns componentes básicos são gerados automaticamente para funcionamento inicial da rede.

### ✅ Criados por padrão:

🔐 Lista de Segurança Padrão
Regras básicas de tráfego (entrada/saída).

📡 Opções de DHCP Padrão
DNS, nome de host e parâmetros de rede.

🛣️ Tabela de Rota Padrão
Define rotas dentro da VCN.


# ☁️ Qual tráfego de camada OSI é suportado pelo Balanceador de Carga de Rede da OCI?

☑️ A) Camada 5 (sessão)


☑️ B) Camada 7 (aplicação)


🟢 ☑️ C) Camada 4 (transporte)
O Balanceador de Carga de Rede da OCI opera na camada 4 do modelo OSI, que é a camada de transporte.

☑️ D) Camada 2 (enlace de dados)

# 📘 Explicação

O OCI Network Load Balancer (NLB) opera principalmente na:

🌐 Camada 4 do Modelo OSI – Transporte

Essa camada trabalha com protocolos como:

TCP

UDP

Função:
Encaminhar conexões rapidamente

Alta performance

Baixa latência

Grande volume de tráfego

➡️ Ideal quando velocidade e disponibilidade são prioridade.

# ❌ Por que as outras estão erradas?
### ❌ Camada 5 (sessão)

Não é a camada principal usada pelo NLB.

### ❌ Camada 7 (aplicação)

Camada 7 é normalmente usada pelo Load Balancer tradicional, com recursos inteligentes como:

HTTP/HTTPS

Regras por URL

SSL termination

### ❌ Camada 2 (enlace de dados)

Relacionada a MAC address e rede local física.

Não se aplica ao NLB OCI.

# ☁️ Qual componente da VCN bloqueia o tráfego de entrada, mas permite o tráfego de saída para a internet?

☑️ A) Gateway de Serviço


☑️ B) Gateway de Internet


☑️ C) Gateway de Roteamento Dinâmico


🟢 ☑️ D) Gateway NAT
Um Gateway NAT em uma VCN permite que instâncias em uma sub-rede privada iniciem conexões com a internet, mas impede conexões de entrada não solicitadas da internet.

# 📘 Explicação

O NAT Gateway na OCI permite que recursos em uma subnet privada acessem a internet somente para saída, sem aceitar conexões iniciadas de fora.

🎯 Comportamento:

✅ Tráfego de saída para internet

❌ Tráfego de entrada da internet bloqueado

🔒 Mantém instâncias privadas protegidas
Exemplo:

Uma VM privada pode:

Atualizar pacotes

Baixar dependências

Acessar APIs externas

Mas não pode ser acessada diretamente da internet.

# ❌ Por que as outras estão erradas?
### ❌ Gateway de Serviço

Usado para acessar serviços públicos da OCI de forma privada (ex: Object Storage).

### ❌ Gateway de Internet

Permite tráfego de entrada e saída com a internet pública.

### ❌ Gateway de Roteamento Dinâmico (DRG)

Usado para conexão privada com:

On-premises

Outras VCNs

Outras regiões

FastConnect / VPN

# 🎯 O que cai na prova (resumo final)

✔️ VCN Peering = conexão privada (não é VPN)  
✔️ Local Peering = mesma região  
✔️ Remote Peering = regiões diferentes  
✔️ CIDR não pode se sobrepor  
✔️ VCN = 1 região apenas  
✔️ VCN pode ter várias sub-redes e recursos  
✔️ Load Balancer NLB = camada 4  
✔️ NAT Gateway = saída internet apenas  
✔️ Internet Gateway = entrada e saída internet  
✔️ LPG não é criado automaticamente  
