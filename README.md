# 🏋️‍♂️ EvoluFit — Progressive Web App de Monitoramento de Treinos

O **EvoluFit** é um **PWA (Progressive Web App)** voltado para **monitoramento físico e progresso de treinos**, com foco em performance, praticidade e design responsivo.  
O objetivo é permitir que o usuário acompanhe seus treinos, metas e evolução corporal diretamente do navegador — **sem depender de integrações externas** por enquanto.

## 🌐 Arquitetura Geral

```mermaid
flowchart TD
    A[Frontend (Vercel / PWA)] --> B[AWS API Gateway]
    B --> C[AWS Lambda (Golang)]
    C --> D[(Amazon RDS - PostgreSQL)]
    C --> E[S3 - Armazenamento de mídias]
