# Estudo Poliana IA — Resumo e Andamento

> Última atualização deste resumo: 2026-09-08
> Gerado a partir do histórico de conversas do projeto "Estudo Poliana IA" no Claude.

---

## 🎯 Objetivo geral

Transição de desenvolvedora full stack EdTech (10 anos de experiência, foco em Moodle/Canvas/LTI) para **AI Engineer**, com foco em:
- Orquestração de LLMs e agentes
- RAG (Retrieval-Augmented Generation)
- Confiabilidade em produção

**Explicitamente fora de escopo:** data science clássica ou construção de modelos/redes neurais do zero.

### Contexto profissional atual
- Clientes atuais: Afya EAD, Gênios Educacional, RadSchool
- Projeto aBeelity (usa AWS Bedrock)
- Stack: PHP, Python (FastAPI), JavaScript, Node.js, React
- Infra: AWS (EC2, Bedrock, SES), Azure, servidor dedicado na OVH

---

## 📊 Diagnóstico e plano

- Avaliação prévia: **~65% de prontidão** para o papel de AI Engineer
- Pontos fortes já consolidados: Python, FastAPI, PostgreSQL, REST APIs, pensamento sistêmico, entrega B2B SaaS
- Plano de carreira faseado de **12 meses** já traçado em conversas anteriores
- Gaps de habilidade identificados para desenvolver:
  - Agentes LLM com tool calling
  - LangGraph
  - MCP (Model Context Protocol, Anthropic)
  - pgvector
  - Langfuse
  - Backend em Node.js

### Sequência de aprendizado recomendada
1. Fundamentos de LangGraph
2. Construir um agente real no domínio EdTech (ex: consultando API do Moodle)
3. Instrumentar com Langfuse
4. Estudar MCP

---

## ✅ Estado atual (checar se ainda está atualizado)

- Cursando **"Agentic AI"** na DeepLearning.AI — resumos em português sendo feitos transcript por transcript
  - Pelo menos 5 lições concluídas: workflows agênticos, espectro de autonomia de agentes, benefícios de pipelines agênticos, framework de dificuldade de aplicação real
- **Google Cloud Skills Boost** — challenge lab de Prompt Design in Agent Platform (Vertex AI) concluído com **100/100**
- **AWS CLF-C02 (Cloud Practitioner)**:
  - Semana 1 (Cloud Fundamentals) ✅
  - Semana 2 (Security/Compliance) ✅ — boas notas
  - Semana 3 (EC2, S3, RDS, Lambda, VPC — domínio de maior peso na prova) — em andamento
  - Semana 4 (Billing and Pricing) — pendente
  - Exame final — pendente

---

## 🔭 Próximos passos / horizonte

- [ ] Concluir Semana 4 do CLF-C02 (Billing and Pricing)
- [ ] Fazer o exame AWS CLF-C02
- [ ] Projeto de infraestrutura com colega (Felipe cuida do servidor dedicado/infra):
  - k3s em VMs Proxmox na OVH
  - Sistemas Node.js/React/PostgreSQL
  - Redis, Nginx Ingress, Cert-Manager
  - Stack de monitoramento planejada: Grafana + Prometheus + Loki

---

## 🧭 Decisões já tomadas (não relitigar sem novo motivo)

- **Não é necessário** construir redes neurais do zero no caminho de AI Engineer — confirmado em múltiplas conversas e por agente de IA consultado separadamente
- **Pós-graduação:** decisão contra pós-graduação tradicional brasileira em IA — currículos ficam defasados em relação ao ecossistema atual. Exceção: se Poli seguir docência no ensino superior, onde lato sensu é exigência formal
  - Pós-graduações brasileiras em IA tendem a ensinar data science clássica, defasada frente ao ecossistema atual de LLM/agentes
  - Cursos curtos + projetos reais têm melhor ROI para essa trajetória
  - **Questão em aberto:** se vale pursuit de pós-graduação (atualmente: não, salvo caminho de docência)
- Eventos do setor (AWS Summit São Paulo, TDC) são valiosos para networking/calibração de mercado, não para aprendizado de conteúdo
- Self-hosting do Langfuse no servidor OVH conta como item de portfólio em si
- Para o CLF-C02, a maior dificuldade é com nomes de serviços em inglês — mnemônicos e recursos visuais são o contra-ataque eficaz

---

## 🛠️ Ferramentas e recursos em uso

**Plataformas de estudo:** DeepLearning.AI, LangChain Academy, Google Cloud Skills Boost, AWS Skill Builder, Anthropic Academy, Hugging Face

**Cursos prioritários:**
- LangChain Academy — *Introduction to LangGraph* (gratuito, prioridade máxima)
- DeepLearning.AI — *AI Agents in LangGraph*
- DeepLearning.AI — *Evaluating AI Agents*
- Anthropic/DeepLearning.AI — curso de MCP

**Observabilidade:** Langfuse, self-hosted na OVH (tracing, custo/latência, versionamento de prompts, evals)

**Infraestrutura:** Servidor dedicado OVH, Proxmox, k3s, Docker, AWS (EC2, Bedrock, SES), Azure

**Bancos de dados:** PostgreSQL, pgvector (ponto de entrada recomendado para busca vetorial)

**Monitoramento:** Grafana / Prometheus / Loki

---

## 💬 Como as conversas neste projeto costumam funcionar

- Respostas em **português do Brasil**, tom casual
- Forte preferência por explicações **visuais, com analogias e interativas**, com código funcional real
- Estilo de aprendizado prático e gamificado (mnemônicos, cenários, quizzes, diagramas)
- Formato preferido para resumos de curso: **títulos em negrito + bullets + emojis** marcando seções, em português
- Trabalha os cursos de forma sequencial e sistemática — gosta de roadmap faseado com marcos definidos
- Direta e breve nas instruções uma vez que um formato já foi definido
- Prefere fundamentar o aprendizado em projetos reais do domínio EdTech/Moodle, em vez de exemplos genéricos

---

## 📝 Notas de uso deste arquivo

Este é um snapshot da memória armazenada sobre o projeto — não uma transcrição completa de todas as conversas. Se algo aqui estiver desatualizado (ex: progresso no AWS, estado do curso Agentic AI), vale confirmar comigo antes de seguir o plano a partir dele.
