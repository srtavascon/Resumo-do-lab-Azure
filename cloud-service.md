
# ☁️ Tipos de Serviços de Nuvem & Modelo de Responsabilidade Compartilhada

 Este resumo descreve os principais modelos de serviços em nuvem e o modelo de responsabilidade compartilhada, com foco na plataforma Microsoft Azure, mas aplicável a qualquer provedor de nuvem confiável.

---

## 🌐 Modelos de Serviço em Nuvem

Existem três modelos principais de serviço em nuvem:

### 1. IaaS – Infrastructure as a Service
- **Descrição**: Fornecimento de infraestrutura básica de computação — servidores, armazenamento e redes.
- **Responsabilidades do cliente**: Sistema operacional, middleware, runtime, dados, aplicações e segurança.
- **Exemplos**: Máquinas Virtuais do Azure, Amazon EC2.

### 2. PaaS – Platform as a Service
- **Descrição**: Fornece uma plataforma gerenciada com ferramentas de desenvolvimento, banco de dados e serviços de hospedagem.
- **Responsabilidades do cliente**: Aplicações e dados.
- **Exemplos**: Azure App Services, Google App Engine, Heroku.

### 3. SaaS – Software as a Service
- **Descrição**: Fornecimento de aplicações completas prontas para uso via navegador, sem necessidade de manutenção pelo cliente.
- **Responsabilidades do cliente**: Uso e gerenciamento de dados.
- **Exemplos**: Microsoft 365, Gmail, Salesforce.

---

## 🔄 Modelo de Responsabilidade Compartilhada

A responsabilidade pela segurança e gerenciamento dos recursos é dividida entre o **provedor de nuvem** e o **cliente**, dependendo do modelo de serviço:

| Componentes                     | On-Premises | IaaS        | PaaS            | SaaS           |
|--------------------------------|-------------|-------------|------------------|-----------------|
| Aplicações                     | Cliente     | Cliente     | Cliente          | Provedor        |
| Dados                          | Cliente     | Cliente     | Cliente          | Cliente         |
| Runtime                        | Cliente     | Cliente     | Provedor         | Provedor        |
| Middleware                     | Cliente     | Cliente     | Provedor         | Provedor        |
| Sistema Operacional            | Cliente     | Cliente     | Provedor         | Provedor        |
| Virtualização                  | Cliente     | Provedor    | Provedor         | Provedor        |
| Servidores / Armazenamento     | Cliente     | Provedor    | Provedor         | Provedor        |
| Rede / Datacenter              | Cliente     | Provedor    | Provedor         | Provedor        |

> ✅ No modelo **on-premises**, **toda a responsabilidade é do cliente**.  
> ✅ No modelo **SaaS**, **toda a infraestrutura e plataforma é responsabilidade do provedor**.

---

## 📌 Observações

- O modelo de responsabilidade compartilhada varia conforme o serviço utilizado.
- Mesmo em SaaS, **a segurança dos dados do usuário ainda é responsabilidade do cliente**.
- Compreender esses modelos é essencial para adotar práticas seguras na nuvem.

---

**Tags**: `IaaS` `PaaS` `SaaS` `Azure` `Cloud Computing` `Responsabilidade Compartilhada`
