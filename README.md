# 🏋️‍♂️ EvoluFit — Progressive Web App de Monitoramento de Treinos

**EvoluFit** é um **PWA (Progressive Web App)** voltado para o **monitoramento físico** e **acompanhamento do progresso de treinos**, com foco em:

- ⚡ **Performance**
- 📱 **Praticidade**
- 🎨 **Design responsivo**

O objetivo é permitir que o usuário acompanhe **treinos, metas e evolução corporal diretamente do navegador**, sem depender de integrações externas — **por enquanto**.

---

## 🚧 Estado Atual do Projeto

Atualmente, o projeto **ainda está na fase inicial de preparação**.  
Nenhuma linha de código do MVP foi desenvolvida até o momento — apenas **configurações iniciais na AWS** foram feitas, como parte do planejamento de infraestrutura.

As etapas concluídas até agora incluem:

- Planejamento de arquitetura em nuvem (AWS);
- Configuração básica de contas e permissões iniciais;
- Estruturação de repositórios no GitHub para colaboração.

O **desenvolvimento do MVP** (Produto Mínimo Viável) ainda será iniciado, com foco em **prototipar as principais funcionalidades** do EvoluFit.

---

## 🧩 Objetivo do MVP

O MVP do **EvoluFit** visa construir uma base funcional que permita:

- Criar e acompanhar **rotinas de treino personalizadas**;
- Registrar **progresso corporal** (peso, medidas, fotos, etc.);
- Definir **metas e desafios individuais**;
- Visualizar **evolução em gráficos e tabelas**;
- (Futuro) Participar de **competições com amigos** e comparar desempenho.

---

## 🌐 Arquitetura Geral

A aplicação foi pensada com uma arquitetura **serverless e escalável**, utilizando serviços AWS integrados com o PWA hospedado na Vercel.

```mermaid
flowchart TD
    A[Frontend Vercel PWA] --> B[AWS API Gateway]
    B --> C[AWS Lambda Golang]
    C --> D[(Amazon RDS PostgreSQL)]
    C --> E[S3 Armazenamento de mídias]
