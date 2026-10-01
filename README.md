# Olá, eu sou o Pedro Brandão 👋

**Desenvolvedor Full Stack e Dados (TypeScript / Python)** · Brasília, DF

Desenvolvedor em início de carreira, com atuação prática em sistemas reais:
- **Ímpetus** (desde 2022): evoluo uma plataforma web de aulas, agendamento e pagamentos.
- **Embrapa** (bolsista): cuido de automação de dados e infraestrutura.

Sou formado em Administração e curso pós-graduação em Ciência de Dados (IPOG), o que me ajuda a traduzir a necessidade do negócio em solução técnica.

Programo com apoio do **Claude Code**, mantendo as decisões técnicas e testando cada entrega.

## 🛠️ Stack

**Linguagens:** TypeScript / JavaScript, Python, SQL
**Web:** React, Next.js (API Routes), Tailwind CSS, Flask, HTML5, CSS3, APIs REST, webhooks, autenticação
**Dados e ML:** PostgreSQL (Supabase), BigQuery, ETL, dbt, Power BI (DAX), Pandas, scikit-learn, PySpark (Spark MLlib), NLTK
**Infra:** Docker, Nginx (proxy reverso), PM2, UFW, VPN, Linux (Ubuntu), Vercel, AWS (Lambda, S3, EventBridge, CloudWatch, IAM)
**Qualidade:** Vitest, Testing Library, pytest, CI com GitHub Actions, Git/GitHub com pull requests

## 🚀 Projetos em destaque

### 🎫 Central de Chamados (Help Desk)
Front-end em **React + TypeScript (Next.js)** e **Tailwind CSS**, construído a partir de um layout do Figma e **responsivo do celular ao desktop**.
- **Telas:** painel com indicadores de fila e **SLA**, lista de chamados com filtro, detalhe do chamado e formulário de abertura com validação.
- **Do layout à interface:** reproduzi o layout do Figma e desenhei, no mesmo estilo, o que ele não tinha: a versão mobile, o detalhe e o formulário.
- **Qualidade:** 11 testes com Vitest e Testing Library, e CI no GitHub Actions.

🔗 [helpdesk-chamados](https://github.com/PedroBLS/helpdesk-chamados) · **[▶ ver online](https://helpdesk-chamados.vercel.app)**

### 📉 Previsão de Churn com ML e Retenção com IA
Base pública de 7 mil clientes: tratamento dos dados e comparação entre Regressão Logística e Random Forest com validação cruzada.
- **Modelo escolhido:** Regressão Logística, pelo recall (0,80 no teste, AUC 0,835).
- **Versão em PySpark:** o mesmo pipeline refeito com Spark MLlib.
- **Uso do resultado:** faixas de risco validadas contra o churn real (7% a 61%), que alimentam mensagens de retenção com a API do Claude.

🔗 [etl-python-churn-strategy](https://github.com/PedroBLS/etl-python-churn-strategy)

### 🏛️ Painel de Compras Públicas (PNCP)
ETL em Python que coleta cerca de 155 mil contratações públicas da Lei 14.133 (abr a set/2026) da API de Dados Abertos do Compras.gov.br e grava no PostgreSQL (Supabase), com carga incremental e upsert. Transformações e testes de qualidade em **dbt** (18 passos no `dbt build`), rodando tanto no PostgreSQL quanto no **BigQuery**, com resultados idênticos nos dois.
- **Qualidade de dados:** as regras excluem 4.469 registros com valores inconsistentes na fonte (um deles estimado em R$ 3,9 trilhões).
- **Carga diária na AWS:** Lambda agendado pelo EventBridge, cópia bruta no S3 e alarme de falha no CloudWatch com aviso por e-mail (SNS).
- **Dashboard no Power BI:** o pregão eletrônico tem **28,7%** de economia mediana; a dispensa, 1,5%.

🔗 [painel-compras-publicas](https://github.com/PedroBLS/painel-compras-publicas)

### 🤖 Assistente de Vagas com MCP + RAG
Servidor **MCP** em Python com 4 ferramentas para o Claude: buscar vagas na Gupy, ver detalhes, indexar e achar as vagas **mais parecidas com um CV**.
- **Busca semântica (RAG):** as descrições são quebradas em trechos com sobreposição e transformadas em embeddings multilíngues locais (fastembed/ONNX), guardados no **pgvector** (Supabase) com índice HNSW.
- **Resultado:** a busca devolve o trecho da vaga que mais combinou, e o Claude explica o encaixe.

🔗 [vagas-mcp-rag](https://github.com/PedroBLS/vagas-mcp-rag)

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

- Agentes com a API do Claude
- Backend da Central de Chamados (API, PostgreSQL e login)
- Terraform (infraestrutura como código)
- Google Analytics 4 e Looker Studio

## 📫 Contato

- **Email:** pedro.brandaols@gmail.com
- **LinkedIn:** [linkedin.com/in/pedro-brandaols](https://www.linkedin.com/in/pedro-brandaols)
