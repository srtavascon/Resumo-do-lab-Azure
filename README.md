# Resumo-do-lab-Azure
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab Microsoft Azure na DIO

# Computação em Nuvem - Microsoft Azure ☁️

## 1️⃣ Introdução à Computação em Nuvem

A computação em nuvem permite acesso remoto a serviços e recursos computacionais via internet, com escalabilidade e pagamento conforme o uso.

**Modelos de implantação:**

- **On-Premises**: infraestrutura local.
- **Cloud**: todos os serviços na nuvem.
- **Modelo Híbrido (Hybrid Cloud)**: mistura de On-Premises + Cloud.

---

## 2️⃣ Modelos de Serviço na Nuvem

- **IaaS (Infrastructure as a Service)**: infraestrutura como serviço (servidores, rede, VMs).
  - Ex.: Azure, AWS, Oracle.
- **PaaS (Platform as a Service)**: plataforma de desenvolvimento e hospedagem.
- **SaaS (Software as a Service)**: software pronto para uso.
  - Ex.: Office 365, Gmail.

---

## 3️⃣ Regiões e Zonas

- **Regiões**: local físico dos datacenters.
- **Zonas de Disponibilidade**: subdivisões dentro das regiões para garantir alta disponibilidade.

**Objetivo:** reduzir latência e aumentar a resiliência.

---

## 4️⃣ Capex vs Opex

- **Capex (Despesas de Capital):** alto custo inicial em infraestrutura.
- **Opex (Despesas Operacionais):** pagamento conforme o uso.

---

## 5️⃣ Estrutura do Azure

Organização dos recursos:

- **Assinatura Azure → Grupos de Recursos → Recursos**

---

## 6️⃣ Serviços de Computação

- **Máquinas Virtuais (VMs):** servidores virtuais com recursos configuráveis.
- **Serviços de Container:**
  - **Azure Container Instances (ACI):** executa containers rapidamente.
  - **Azure Kubernetes Service (AKS):** orquestrador de containers.
  - **Azure App Service:** hospedagem de aplicações web.
  - **Azure Container Registry (ACR):** armazenamento privado de imagens Docker.
- **Docker:** ferramenta de criação e execução de containers.
- **Imagens Docker:** contém código e dependências.

---

## 7️⃣ Serviços de Rede

- **VNet (Virtual Network):** rede virtual privada.
- **Clusters:** grupo de servidores trabalhando em conjunto com alta disponibilidade.

---

## 8️⃣ Armazenamento no Azure

- **Contas de Armazenamento:** ponto de entrada para recursos de armazenamento.
- **Redundância:** múltiplas cópias dos dados (LRS, GRS, ZRS).
- **Tipos de Armazenamento:**
  - **Blob Storage:** armazenamento de objetos (arquivos, imagens, vídeos).
  - **File Storage:** compartilhamento de arquivos.
  - **Queue Storage:** filas de mensagens.
  - **Table Storage:** armazenamento NoSQL.
- **Camadas de Acesso:**
  - **Hot:** acesso frequente.
  - **Cool:** acesso eventual.
  - **Archive:** acesso raro.
- **Azure Data Box:** dispositivo físico para grandes transferências de dados.
- **Hands-on:** Blob Storage costuma ser o primeiro serviço prático.

---

## 9️⃣ Funções e Serverless

- **Azure Functions:** execução de funções sob demanda (serverless).

---

## 🎯 Resumo Visual

| Tema | Conceito |
|------|----------|
| Modelos | IaaS, PaaS, SaaS |
| Implantação | On-Premises, Cloud, Hybrid |
| Organização | Assinatura > Grupo de Recursos > Recursos |
| Rede | VNet, Cluster |
| Armazenamento | Blob, File, Queue, Table |
| Computação | VM, Containers (ACI, AKS), App Service |
| Ferramentas | Docker, Azure Functions |
| Regiões | Regiões e Zonas de Disponibilidade |
| Finanças | Capex vs Opex |

---

📌 _Resumo elaborado com base em anotações de estudo sobre Microsoft Azure - Computação em Nuvem._
