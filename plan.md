# Plano de Entrevistas — Dev Fullstack Sênior

> Início: 2026-09-08
> Objetivo: passar em entrevistas técnicas (testes de lógica, provas de conhecimento, live coding) para vagas fullstack sênior, aproveitando a transição em andamento para AI Engineer.
> Visual completo (com truques de memorização e banco de perguntas): artifact "Plano de Entrevistas Sênior" — link salvo no Claude Code, pedir pra reabrir se precisar.
> Contexto de carreira mais amplo (AI Engineer, AWS, Langfuse etc.) está em [estudo-poliana-ia-resumo.md](estudo-poliana-ia-resumo.md) — este arquivo aqui é o braço "entrevistas" desse plano.

---

## 🗓️ Sprint de 4 semanas

### Semana 1 — Base sólida (lógica + linguagens)
- [ ] Big O e complexidade (O(1) → O(2ⁿ))
- [ ] Arrays, hash maps, pilhas, filas
- [ ] Recursão, busca binária, two pointers, sliding window
- [ ] JS: closures, promises, event loop (microtask vs macrotask)
- [ ] PHP/Python: OOP e boas práticas
- [ ] 10 exercícios LeetCode Easy (filtro "Top Interview 150")

### Semana 2 — Backend & dados
- [ ] REST: verbos, status codes, idempotência
- [ ] Autenticação: JWT, OAuth2, sessão vs. token
- [ ] Montar CRUD com FastAPI + JWT do zero (cronometrado, 2h)
- [ ] SQL: joins, subqueries, GROUP BY/HAVING, índices, N+1
- [ ] ACID e transações
- [ ] Git flow (rebase vs merge, resolver conflito de verdade)
- [ ] Pirâmide de testes + 1 suíte pytest/jest num endpoint real

### Semana 3 — Frontend & arquitetura
- [ ] React: hooks (regra do topo), useMemo vs useCallback
- [ ] Virtual DOM, reconciliação, keys em listas
- [ ] Context vs Redux/Zustand
- [ ] System design: escala vertical/horizontal, cache, filas, CAP theorem
- [ ] Praticar estrutura de resposta de design (requisitos → estimativa → arquitetura → gargalos)
- [ ] **AWS CLF-C02 — Semana 4 (Billing and Pricing)** ⚠️ pendente há um tempo

### Semana 4 — Simulação real
- [ ] 2–3 mock interviews (live coding, narrando raciocínio em voz alta)
- [ ] Preparar 5 histórias STAR (conflito, prazo apertado, decisão técnica, falha/aprendizado, liderança)
- [ ] Gravar-se respondendo cada STAR em voz alta (2 min cada)
- [ ] Simulado oficial AWS Skill Builder
- [ ] **Exame AWS CLF-C02**
- [ ] Preparar elevator pitch citando Bedrock/LangGraph como diferencial

---

## 📌 Status atual

| Área | Status |
|---|---|
| Algoritmos & lógica | não iniciado |
| Backend / APIs | não iniciado |
| SQL | não iniciado |
| Frontend / React | não iniciado |
| System design | não iniciado |
| AWS CLF-C02 | semana 3 concluída, falta semana 4 + exame |
| Comportamental (STAR) | não iniciado |

> Atualizar esta tabela conforme for avançando — assim a gente sabe onde focar sem reabrir tudo do zero.

---

## 🎯 Diferencial a destacar em entrevistas

10 anos em fullstack EdTech (Afya EAD, Gênios Educacional, RadSchool) + experiência real com AWS Bedrock no projeto aBeelity + estudo ativo de LangGraph/MCP/Langfuse. Poucos candidatos fullstack sênior já têm essa combinação cloud + IA aplicada — vale mencionar isso na etapa comportamental e no pitch inicial.

---

## 🔁 Como usar este arquivo

- Marcar os checkboxes conforme for estudando cada tópico
- Se surgir uma vaga específica, pedir pra ajustar as prioridades do sprint pra stack daquela vaga
- Revisar a tabela de status antes de cada sessão de estudo pra saber onde retomar
- Temas em áudio para reforçar no trajeto/academia: ver [podcast.md](podcast.md)
