# Olá, eu sou o Pedro Brandão 👋

**Desenvolvedor Full Stack e Dados (TypeScript / Python)** · Brasília, DF

Desenvolvedor em início de carreira, com atuação prática em sistemas reais:
- **Ímpetus** (desde 2022): evoluo uma plataforma web de aulas, agendamento e pagamentos.
- **Embrapa** (bolsista): cuido de automação de dados e infraestrutura.

Sou formado em Administração e curso pós-graduação em Ciência de Dados (IPOG), o que me ajuda a traduzir a necessidade do negócio em solução técnica.

Programo com apoio do **Claude Code**, mantendo as decisões técnicas e testando cada entrega.

## 🛠️ Stack

**Linguagens:** TypeScript / JavaScript, Python, SQL
**Web:** React, Next.js (API Routes), Flask, HTML5, CSS3, APIs REST, webhooks, autenticação
**Dados e ML:** PostgreSQL (Supabase), Pandas, scikit-learn, PySpark (Spark MLlib), NLTK, Power BI
**Infra:** Docker, Nginx (proxy reverso), PM2, UFW, VPN, Linux (Ubuntu), Vercel
**Qualidade:** Vitest, Git/GitHub com pull requests

## 🚀 Projetos em destaque

### 📉 Previsão de Churn com ML e Retenção com IA
Base pública de 7 mil clientes: tratamento dos dados e comparação entre Regressão Logística e Random Forest com validação cruzada.
- **Modelo escolhido:** Regressão Logística, pelo recall (0,80 no teste, AUC 0,835).
- **Versão em PySpark:** o mesmo pipeline refeito com Spark MLlib.
- **Uso do resultado:** faixas de risco validadas contra o churn real (7% a 61%), que alimentam mensagens de retenção com a API do Claude.

🔗 [etl-python-churn-strategy](https://github.com/PedroBLS/etl-python-churn-strategy)

### 🔎 gupy-search
Ferramenta de linha de comando em TypeScript (Bun) para buscar vagas pela API pública da Gupy, com 7 testes automatizados. Também funciona como skill do Claude Code.
- **Contexto:** criada ao adaptar um agente open source de busca de vagas ao mercado brasileiro.
- **Como foi feita:** dirigi o Claude Code na escrita do código.

🔗 [gupy-search](https://github.com/PedroBLS/gupy-search)

### 💬 Classificação de Sentimentos em Tweets (PLN)
TF-IDF + Random Forest sobre 41 mil tweets, com pré-processamento em NLTK. Acurácia de 0,46 em 5 classes, contra 0,27 do chute. O README traz a análise dos erros e os próximos passos.

🔗 [classificationtext-corona](https://github.com/PedroBLS/classificationtext-corona)

### 🎓 Plataforma de Gestão Educacional (Ímpetus)
Aplicação web em Next.js, TypeScript e Supabase (PostgreSQL) para agendamento de aulas e pagamentos. Atuo da definição de requisitos à correção de falhas em produção, incluindo a integração com a API de pagamentos Asaas e a depuração de webhooks. *Repositório privado, posso apresentar em entrevista.*

### 🐍 Sistema de Aulas Particulares (versão anterior, Flask)
A primeira versão do sistema da Ímpetus, em Python com Flask e SQLAlchemy.
- Login por perfil (admin, professor e aluno).
- Cadastro de alunos e professores e agendamento de aulas.
- Relatórios em PDF.

🔗 [sistema-escolaparticular](https://github.com/PedroBLS/sistema-escolaparticular)

### 🏢 Site Institucional (Ímpetus)
Site institucional responsivo publicado no GitHub Pages.
🔗 [institutoimpetus](https://github.com/PedroBLS/institutoimpetus)

## 📈 Próximos estudos

- RAG, agentes e MCP com a API do Claude
- AWS na prática (Lambda, S3, IAM, CloudWatch)
- Google Analytics 4 e Looker Studio

## 📫 Contato

- **Email:** pedro.brandaols@gmail.com
- **LinkedIn:** [linkedin.com/in/pedro-brandaols](https://www.linkedin.com/in/pedro-brandaols)
