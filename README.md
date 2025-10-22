# 🏋️‍♂️ EvoluFit — Progressive Web App de Monitoramento de Treinos

**EvoluFit** é um **PWA (Progressive Web App)** voltado para o **monitoramento físico** e **acompanhamento do progresso de treinos**, com foco em:

- ⚡ Performance  
- 📱 Praticidade  
- 🎨 Design responsivo  

O objetivo é permitir que o usuário acompanhe **treinos, metas e evolução corporal diretamente do navegador**, sem depender de integrações externas — por enquanto.

---

## 🌐 Arquitetura Geral

```mermaid
flowchart TD
    A[Frontend Vercel PWA] --> B[AWS API Gateway]
    B --> C[AWS Lambda Golang]
    C --> D[(Amazon RDS PostgreSQL)]
    C --> E[S3 Armazenamento de mídias]
