# Podcast de Estudo — Mini-episódios para ouvir na academia

> Objetivo: aproveitar os 30–40 min diários na academia pra reforçar, em áudio, os temas do [plan.md](plan.md).
> Formato: episódios curtos (8–10 min) — dá pra ouvir 3 a 4 por sessão, sem precisar prestar atenção em texto.

---

## 🎙️ Como funciona

1. Você me pede o roteiro de um episódio (ex: *"gera o roteiro do episódio 3 — closures em JS"*)
2. Eu escrevo o texto pronto pra narração, já no formato abaixo
3. Você transforma em áudio numa dessas opções:
   - **Google NotebookLM** ("Audio Overview") — cola o roteiro, ele gera até uma conversa entre duas vozes, de graça. É a opção mais rápida e com melhor qualidade de "podcast de verdade".
   - **ElevenLabs** (texto-para-voz) — voz mais natural, se quiser só uma narração direta
   - **Leitor de texto do celular/navegador** — mais simples, qualidade robótica mas funciona
4. Salva o MP3 no celular e ouve na academia

> Dica: gere 3–4 roteiros de uma vez (um dia de estudo) e transforme tudo em lote no NotebookLM antes da semana começar — economiza tempo.

---

## 🧱 Estrutura de cada episódio (o que eu sigo ao escrever)

| Bloco | Duração | Conteúdo |
|---|---|---|
| Gancho | ~30s | Uma pergunta ou situação real que puxa curiosidade ("Já teve um bug que só acontecia às vezes? Isso é...") |
| Conceito central | ~3–4 min | Explicação direta, sem jargão desnecessário, com analogia do dia a dia |
| Exemplo prático | ~2–3 min | Como isso aparece no código/trabalho real (PHP, Python, Node, React, SQL, AWS) |
| Truque de memorização | ~1 min | O mnemônico pra lembrar na hora da entrevista |
| Fechamento + pergunta de revisão | ~1 min | Resumo em 1 frase + uma pergunta pra você responder mentalmente (autoteste) |

---

## 📅 Temporada 1 — Módulo 00: Lógica & Algoritmos

> Aula completa (com exemplos e exercícios): [00-logica-algoritmos/](00-logica-algoritmos/) — cada episódio abaixo é uma seção da aula.
> Roteiros gerados ficam em [00-logica-algoritmos/podcast/](00-logica-algoritmos/podcast/).

- [x] Ep. 1 — Complexidade (Big O): por que entrevistador liga tanto pra isso → [roteiro](00-logica-algoritmos/podcast/ep1-big-o.md)
- [x] Ep. 2 — Arrays, listas encadeadas, pilhas e filas: quando usar cada um → [roteiro](00-logica-algoritmos/podcast/ep2-arrays-pilhas-filas.md)
- [x] Ep. 3 — Hash maps por dentro: como o acesso vira O(1) → [roteiro](00-logica-algoritmos/podcast/ep3-hashmaps.md)
- [x] Ep. 4 — Recursão explicada com caso base e caso recursivo → [roteiro](00-logica-algoritmos/podcast/ep4-recursao.md)
- [ ] Ep. 5 — Busca binária: a lógica de procurar num telefone impresso
- [ ] Ep. 6 — Two pointers e sliding window: o truque que resolve metade do LeetCode
- [ ] Ep. 7 — Ordenação: o que basta saber sobre quicksort e mergesort

## 📅 Temporada 2 — Módulo 01: Backend & dados

> Aula (quando criada): [01-backend/](01-backend/) e [03-sql-dados/](03-sql-dados/)

- [ ] Ep. 8 — REST de verdade: verbos, status codes e idempotência
- [ ] Ep. 9 — JWT vs. sessão: o que o entrevistador quer ouvir
- [ ] Ep. 10 — SQL JOINs como diagrama de Venn
- [ ] Ep. 11 — O que é o problema N+1 (e por que todo sênior é cobrado nisso)
- [ ] Ep. 12 — ACID em 4 palavras
- [ ] Ep. 13 — Pirâmide de testes: por que sua suíte não devia ter mais e2e que unitário

## 📅 Temporada 3 — Módulo 02: Frontend & arquitetura

> Aula (quando criada): [02-frontend/](02-frontend/)

- [ ] Ep. 14 — Closures em JavaScript, sem mistério
- [ ] Ep. 15 — Event loop: por que setTimeout(fn, 0) não roda na hora
- [ ] Ep. 16 — Regra dos hooks: "topo e reto"
- [ ] Ep. 17 — useMemo vs useCallback, de vez por todas
- [ ] Ep. 18 — Virtual DOM e por que a key da lista importa tanto
- [ ] Ep. 19 — CAP theorem em 5 minutos
- [ ] Ep. 20 — Cache, CDN e fila de mensagens: pra que serve cada um
- [ ] Ep. 21 — Como estruturar uma resposta de system design sem travar

## 📅 Temporada 4 — Módulo 07: Comportamental

> Aula (quando criada): [07-comportamental/](07-comportamental/)

- [ ] Ep. 22 — Método STAR: como transformar seu dia a dia em resposta de entrevista
- [ ] Ep. 23 — "Por que você quer sair do seu emprego atual?" — como responder sem soar negativo
- [ ] Ep. 24 — Perguntas pra você fazer no final da entrevista (e o que elas revelam sobre a empresa)
- [ ] Ep. 25 — Seu pitch: fullstack sênior + IA aplicada (Bedrock/LangGraph) como diferencial

## ☁️ Temporada bônus — Módulo 06: AWS CLF-C02

> Aula (quando criada): [06-aws/](06-aws/)

- [ ] Ep. 26 — Modelo de responsabilidade compartilhada, explicado com analogia de apartamento alugado
- [ ] Ep. 27 — EC2, S3, RDS, Lambda: o que cada um resolve
- [ ] Ep. 28 — IAM sem enrolação: usuário, role e política
- [ ] Ep. 29 — Billing: Free Tier, On-Demand, Reserved e Spot — qual escolher quando

---

## 🔁 Como pedir o próximo lote

Basta dizer algo como:
> "gera os roteiros dos episódios 1 a 4"

ou

> "gera o próximo episódio pendente"

e eu escrevo o texto completo, pronto pra colar no NotebookLM ou no leitor de texto. Vou marcando aqui quais já foram gerados/ouvidos conforme você for confirmando.
