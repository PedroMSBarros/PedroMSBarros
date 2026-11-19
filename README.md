# 👋 Olá, sou Pedro Barros

**Estudante de Defesa Cibernética | SOC Analyst N1 em formação | Blue Team | Full-Stack Developer**

Baseado em São Paulo 🇧🇷, cursando **Defesa Cibernética na Impacta**. Meu foco é **Segurança da Informação — SOC, monitoramento e detecção de ameaças** — com base sólida em desenvolvimento full-stack. Fundador da [Metazoa Store](https://metazoastore.vercel.app/#/), e-commerce de aquarismo que desenvolvi e mantenho sozinho, do frontend ao banco de dados.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pedro-barros-aa02402b2/) [![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PedroMSBarros)

---

## 🔐 Cybersecurity

**Experiência prática**
- 🧪 **SOC Lab próprio** — Wazuh SIEM + Sysmon, simulação e detecção de ataques reais mapeados ao MITRE ATT&CK — [Mini SOC Lab](https://github.com/PedroMSBarros/Mini-Soc-Lab)
- 🤖 **Triagem de alertas com IA** — pipeline Python sobre o Wazuh Indexer com roteamento entre modelos Claude — [AI SOC Analyst](https://github.com/PedroMSBarros/AI-SOC-Analyst)
- 🕵️ **Auditoria de segurança em aplicação web** (cliente real, autorizada) — identificação de *broken access control* crítico (bypass de restrições de UI via chamadas diretas à API), ausência de security headers, JWT com expiração excessiva e falta de rate limiting no login
- 🛡️ **Segurança aplicada nos meus projetos** — Row Level Security (RLS), OAuth 2.0, CORS, gestão de secrets via variáveis de ambiente, auditoria de políticas de acesso

**Certificações e formação**
- **Cisco/Splunk Cybersecurity Defense Analyst Pathway** — 8 cursos: SOC fundamentals, SIEM, Splunk SPL
- **Fortinet NSE 1 & NSE 2** — Fortinet Certified Fundamentals in Cybersecurity
- **Cisco NetAcad** — Conceitos Básicos de Rede & Introdução à Cybersegurança
- **AWS Academy** — Cloud Security Foundations & Lab Project: Cloud Security Builder *(em andamento)*
- **Microsoft SC-200** — Security Operations Analyst *(em preparação)*

---

## 🛠️ Tecnologias e Ferramentas

**Segurança & SOC**

![Wazuh](https://img.shields.io/badge/Wazuh-3AB7E5?style=flat&logo=wazuh&logoColor=white) ![Sysmon](https://img.shields.io/badge/Sysmon-0078D4?style=flat&logo=windows&logoColor=white) ![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat&logo=splunk&logoColor=white) ![MITRE ATT&CK](https://img.shields.io/badge/MITRE_ATT%26CK-C8102E?style=flat&logoColor=white) ![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C94?style=flat&logo=kalilinux&logoColor=white) ![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=flat&logo=metasploit&logoColor=white) ![VirtualBox](https://img.shields.io/badge/VirtualBox-183A61?style=flat&logo=virtualbox&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white) ![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

**Backend, Dados & IA**

![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat&logo=supabase&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat&logo=postgresql&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white) ![Claude API](https://img.shields.io/badge/Claude_API-D97757?style=flat&logo=anthropic&logoColor=white)

**DevOps & Infra**

![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white) ![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=flat&logo=cloudinary&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)

---

## 🚀 Projetos em Destaque

### 🛡️ [Mini SOC Lab](https://github.com/PedroMSBarros/Mini-Soc-Lab)

Laboratório de detecção de ameaças construído do zero com **Wazuh SIEM, Sysmon e VirtualBox** (Wazuh Manager, vítima Windows 10 e atacante Kali Linux). Pipeline completo Sysmon → Wazuh Agent → Manager → Indexer → Dashboard. Simulação e detecção de 3 ataques reais com mapeamento ao **MITRE ATT&CK** e evidência forense documentada:
- Brute Force SMB — `T1110`
- PowerShell Abuse — `T1059.001` / `T1105`
- Privilege Escalation via Unquoted Service Path — `T1574.009`

### 🤖 [AI SOC Analyst Assistant](https://github.com/PedroMSBarros/AI-SOC-Analyst)

Assistente de triagem e investigação de alertas que consome o Wazuh Indexer e roteia cada alerta por severidade entre dois modelos Claude (**Haiku** para triagem, **Sonnet** para investigação profunda). Deduplicação por regra + agente em janela de 30 minutos **reduziu o custo de operação em ~51%**; rastreamento real de tokens, dashboard em Streamlit e notificações no Discord. Validado contra ataques reais via Kali/Metasploit — incluindo a descoberta de um **gap de visibilidade no ruleset padrão do Wazuh**.

### 🐠 [Metazoa Store](https://github.com/PedroMSBarros/Metazoa-store)

E-commerce de aquarismo em produção, construído do zero com **React 19, Vite, Tailwind CSS e Supabase**. Catálogo com **600+ peixes e plantas e 900+ produtos** em 30+ categorias, de água doce e marinha, carrinho integrado ao WhatsApp, PWA e backend protegido com RLS. Destaques técnicos:
- Migração de 700+ imagens para o **Cloudinary** com script idempotente e retry automático, com otimização de imagem por URL
- Sistema de **variantes de tamanho** (um card por espécie, seletor de tamanho)
- **Motor de busca próprio**: palavras em qualquer ordem, comparação fonética, tolerância a erros de digitação (distância Damerau), sinônimos do aquarismo e ranking por relevância
- Carrossel de novidades na Home e paginação client-side
- Experiência mobile-first — a maior parte do tráfego vem do celular

🔗 [metazoastore.vercel.app](https://metazoastore.vercel.app/#/)

### 📊 [Metazoa Finanças](https://github.com/PedroMSBarros/Metazoa-financas)

Sistema de gestão completo para o negócio, usado no dia a dia da loja e instalável como **PWA**: vendas multi-item com frete e desconto, despesas e **lucro real**, kanban de pedidos em espera, fila de envios, base de clientes com alertas de recontato, calendário de tarefas e painel de insights. Acesso restrito via **GitHub OAuth** e **RLS owner-only** em todas as tabelas. Stack: HTML/CSS/JavaScript, Supabase, Chart.js.

---

## 📊 GitHub Stats

![](https://github-stats-extended.vercel.app/api?username=PedroMSBarros&show_icons=true&theme=dark&hide_border=true&count_private=true)
![](https://github-stats-extended.vercel.app/api/top-langs/?username=PedroMSBarros&layout=compact&theme=dark&hide_border=true)

---

## 📫 Contato

Em busca de oportunidades como **SOC Analyst N1 / Blue Team**. Também aberto a posições de **Desenvolvimento Full-Stack**.

📧 Entre em contato pelo [LinkedIn](https://www.linkedin.com/in/pedro-barros-aa02402b2/)
