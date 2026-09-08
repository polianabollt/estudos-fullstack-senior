# Constitution — regras de organização deste repositório de estudos

> Este arquivo define como organizamos pastas, arquivos e conteúdo aqui dentro.
> Sempre que surgir um assunto novo, consultar (ou atualizar) este documento antes de criar algo solto na raiz.

---

## 📁 Estrutura de pastas atual

```
estudos/
├── index.html                  ← painel de podcast (GitHub Pages) — player + progresso
├── plan.md                     ← índice geral: sprint de estudo, checklist, status por área
├── podcast.md                  ← índice de episódios/roteiros de áudio
├── constitution.md             ← este arquivo
├── .gitignore                  ← mantém arquivos pessoais fora do repo público (ver Regra 9)
├── 00-logica-algoritmos/
├── 01-backend/
│   ├── node/
│   ├── python/
│   └── php/
├── 02-frontend/
│   ├── react/
│   └── javascript/
├── 03-sql-dados/
├── 04-testes-qualidade/        ← Cypress, TDD, pirâmide de testes, estratégia de testes
├── 05-arquitetura-devops/      ← Jenkins/CI-CD, Docker/k3s, Grafana/Prometheus/Loki
├── 06-aws/
├── 07-comportamental/          ← STAR, pitch, perguntas pro entrevistador
└── 08-ia-diferencial/          ← Bedrock, LangGraph, MCP — diferencial de AI Engineer
```

---

## 🧭 Regra 1 — Onde colocar teste unitário/integração vs. teste como tema

- Teste **de código específico** (PHPUnit, pytest, Jest testando uma função) mora junto do tema que ele testa → dentro de `01-backend/<linguagem>/` ou `02-frontend/react/`
- Teste **como assunto/estratégia** (Cypress/e2e, TDD, pirâmide de testes, o que é mockado vs. real) mora em `04-testes-qualidade/`
- Regra prática: "isso é uma técnica de escrever código, ou é uma disciplina que se aplica a qualquer código?" — técnica de código → pasta da linguagem; disciplina → `04-testes-qualidade`

## 🧭 Regra 2 — Assunto novo que não cabe em nenhuma pasta existente

1. Primeiro tentar encaixar no que já existe (ex: "cache" cabe em `05-arquitetura-devops`, não precisa de pasta nova)
2. Se realmente não couber, criar uma pasta nova na raiz, seguindo a numeração (próximo número disponível, ou renumerar se fizer mais sentido ficar entre duas existentes)
3. Nome da pasta: `kebab-case`, em português, minúsculo, sem acento quando possível (facilita digitar)
4. Atualizar este arquivo (a árvore acima) e o `plan.md` quando a pasta nova for criada

## 🧭 Regra 3 — Subpastas dentro de um tema

- Uma pasta de tema **só ganha subpastas quando o conteúdo justificar** — regra prática: a partir de 3 arquivos sobre sub-assuntos diferentes dentro da mesma pasta, vale separar
- Exemplo já aplicado: `01-backend` dividido em `node/ python/ php/` porque são linguagens distintas que ela usa profissionalmente
- Exemplo já aplicado: `02-frontend` dividido em `react/` (framework) e `javascript/` (linguagem/conceitos puros, ex: closures, event loop)
- Evitar criar subpasta vazia "por precaução" — criar quando o primeiro arquivo daquele sub-tema for escrito

## 🧭 Regra 4 — Papel de cada arquivo índice na raiz

- **`plan.md`** — fonte da verdade do progresso: sprint de 4 semanas, checkboxes, tabela de status por área. É o primeiro lugar a olhar pra saber "onde eu parei"
- **`podcast.md`** — lista de episódios em áudio, mapeados às mesmas áreas do `plan.md`, pra ouvir no trajeto/academia
- **`constitution.md`** — regras de organização (este arquivo). Não guarda conteúdo de estudo, só estrutura e convenções

## 🧭 Regra 5 — Convenção de nome de arquivo dentro das pastas

- `kebab-case.md`, descritivo e específico (ex: `01-backend/node/event-loop-vs-worker-threads.md`, não `notas.md`)
- Cada arquivo de roteiro de podcast fica na pasta do tema correspondente e é referenciado no `podcast.md` pelo nome/link
- Preferir 1 arquivo por sub-assunto a um arquivo gigante por pasta — facilita achar depois

## 🧭 Regra 6 — Atualização de status

- Sempre que um checkbox do `plan.md` for marcado, revisar se a linha correspondente na tabela "Status atual" também deve mudar
- Pastas novas criadas por esta regra devem entrar na tabela de status do `plan.md` também

## 🧭 Regra 7 — Molde obrigatório de "aula" (artifact) por módulo

Todo módulo (pasta numerada) que virar artifact de estudo segue este molde, validado no módulo 00 (Lógica & Algoritmos):

1. **Hero** — título do módulo + por que isso cai em prova/entrevista
2. **Índice (TOC)** com âncoras, numerado, cada item = 1 episódio futuro de podcast
3. **Seções em ordem de estudo**, cada uma com: explicação direta → exemplo de código real (quando aplicável) → box "🧠 truque" de memorização → exercício em `<details>` com resposta escondida → linha "Pratique em:" com sugestão concreta
4. **Checklist final** de autoavaliação livre ("consigo explicar X de cabeça")
5. **Mini-prova final obrigatória** — 8 questões de múltipla escolha (uma por conceito-chave da seção correspondente), correção via JS mostrando certo/errado + explicação por questão, resultado com corte de aprovação (referência usada: 6/8) liberando o próximo módulo
6. Mesma identidade visual entre módulos: paleta teal/âmbar, fontes Sora (títulos) + IBM Plex Sans (corpo) + IBM Plex Mono (código/labels), dark mode automático

Cada pasta de módulo ganha um `README.md` curto apontando pra esse artifact e listando o índice das seções (ex: `00-logica-algoritmos/README.md`).

## 🧭 Regra 8 — Relação entre a aula (artifact) e o episódio de podcast

O podcast **não lê a aula em voz alta** — ele é complementar, pensado pra ser ouvido sem tela (academia/trajeto):

- Prioriza **analogia e intuição** sobre código/tabela (ex: pilha = pilha de pratos, busca binária = lista telefônica impressa)
- Código vira **descrição verbal do raciocínio**, nunca sintaxe lida linha a linha
- Fecha com **a pergunta da mini-prova daquela seção em voz alta**, pra reforço por recall ativo (ela responde mentalmente andando), não releitura passiva
- Reaproveita o mesmo truque de memorização da aula como gancho de fechamento, pra criar reforço espaçado entre o que foi lido (aula) e o que foi ouvido (podcast) sobre o mesmo conceito

## 🧭 Regra 9 — Painel de podcast (GitHub Pages) e fluxo de publicação

O repositório é público no GitHub (`polianabollt/estudos-fullstack-senior`), com GitHub Pages ativo servindo `index.html` da raiz em `https://polianabollt.github.io/estudos-fullstack-senior/`. É um painel estático — sem servidor, sem build — com player de áudio por episódio e progresso salvo em `localStorage` do celular.

- **Artifact não hospeda áudio de verdade** — testado em 2026-09-08: a capacidade de assets não está disponível, e a política de segurança do Artifact bloqueia tocar mídia de qualquer host externo. Por isso o player mora no GitHub Pages, não num Artifact.
- Todo `.m4a` gerado vai direto na mesma pasta do roteiro correspondente (ex: `00-logica-algoritmos/podcast/ep1-big-o.m4a` ao lado de `ep1-big-o.md`)
- Ao adicionar um `.m4a` novo (ou um roteiro novo), atualizar a entrada correspondente no array `DATA` do `index.html` (campo `audio` e/ou `roteiro`)
- **Fluxo de publicação:** depois de adicionar/editar arquivos → `git add -A` → `git commit -m "..."` → `git push` → o GitHub Pages atualiza sozinho em menos de 1 minuto, mesmo link
- **Arquivos pessoais fora do escopo de estudo** (ex: `Cases.docx` com informação de cliente) ficam de fora via `.gitignore` — nunca versionar algo assim num repo público sem confirmar antes
- O progresso ("ouvido"/"não ouvido") é local por aparelho — não sincroniza entre celular e computador. Se isso incomodar no futuro, a alternativa é usar a capacidade `db` de um Artifact separado só pra tracking (não pro áudio)

---

## 🗳️ Decisões já tomadas (não relitigar sem novo motivo)

- Testes unitários vivem com a linguagem; testes como disciplina (e2e, TDD, estratégia) têm pasta própria — decidido em 2026-09-08
- Backend dividido por linguagem (node/python/php) desde o início, porque são usadas ativamente no trabalho real
- IA (Bedrock/LangGraph/MCP) tem pasta separada do backend, porque é tratada como diferencial de carreira, não como "só mais uma tech" do dia a dia
- Painel de podcast vive em GitHub Pages (repo público), não em Artifact — decidido em 2026-09-08 depois de confirmar que Artifact não consegue tocar áudio real nesta conta
