# Episódio 2 — Arrays, listas encadeadas, pilhas e filas

> Duração alvo: 8–10 min · Módulo 00 — Lógica & Algoritmos · Seção de referência: "2. Arrays, listas, pilhas e filas" na aula
> Cola esse texto direto no NotebookLM (Audio Overview) ou num leitor de texto pra ouvir.

---

**[GANCHO]**

Pensa no botão de desfazer, o Ctrl+Z. Ele sempre desfaz a última coisa que você fez, nunca a primeira. E pensa numa fila de impressora — o primeiro documento que você mandou imprimir é o primeiro que sai, mesmo que você mande mais dez depois. Esses dois comportamentos diferentes têm nome, e entender a diferença entre eles é uma das perguntas mais repetidas em teste técnico.

**[CONCEITO CENTRAL]**

A pergunta que cai em entrevista quase nunca é "o que é uma pilha" ou "o que é uma fila" — isso qualquer um decora. A pergunta de verdade é: "quando eu escolho uma em vez da outra?"

Array é a estrutura mais básica: uma sequência de posições, acesso instantâneo se você sabe o índice — pegar o item na posição cinco é sempre rápido, não importa se a lista tem dez ou dez milhões de itens. O problema do array aparece quando você precisa inserir ou remover algo no meio: aí ele precisa empurrar todo mundo pro lado, e isso fica lento com listas grandes.

Lista encadeada resolve esse problema — cada item aponta pro próximo, então inserir no meio é rápido, você só reorganiza os ponteiros. Mas em compensação, pra achar o item na posição cinco, você não tem atalho: precisa andar item por item desde o começo.

Pilha e fila são duas formas de organizar acesso restrito a essas listas. Pilha só deixa você mexer numa ponta — o topo. Você só pode colocar ou tirar do topo. É o que chamam de LIFO: last in, first out, o último que entrou é o primeiro que sai. Fila deixa você colocar numa ponta e tirar da outra — FIFO, first in, first out, o primeiro que entrou é o primeiro que sai.

**[EXEMPLO PRÁTICO]**

Volta pro Ctrl+Z: cada ação que você faz é empilhada. Quando você desfaz, o sistema tira do topo da pilha — a última ação, não a primeira. Se fosse uma fila, o Ctrl+Z desfaria a primeira coisa que você fez no documento inteiro, o que não faz sentido nenhum. Por isso desfazer é sempre implementado com pilha.

Agora a fila de impressora: o primeiro arquivo que você mandou é processado primeiro, mesmo que você mande outros depois — ninguém "fura fila". Isso é literalmente uma fila, FIFO. E é o mesmo princípio usado numa busca em largura, aquela técnica de percorrer uma árvore ou um grafo nível por nível — sempre processando primeiro quem entrou primeiro na fila de espera.

**[TRUQUE DE MEMORIZAÇÃO]**

Pilha é uma pilha de pratos empilhados — você só consegue tirar o de cima, nunca o de baixo sem derrubar tudo. Fila é fila de banco — quem chegou primeiro é atendido primeiro, ninguém pula a frente. Guarda essas duas imagens: pilha de pratos, fila de banco.

**[FECHAMENTO + PERGUNTA DE REVISÃO]**

Resumo: array é acesso rápido por posição mas caro pra inserir no meio; lista encadeada é o contrário; pilha restringe acesso a uma ponta só, LIFO; fila restringe a duas pontas, FIFO.

Pergunta de revisão: um problema clássico de entrevista é verificar se os parênteses de uma expressão estão balanceados — tipo, abrir três parênteses e fechar só dois. Qual estrutura resolve isso de forma natural, pilha ou fila? ... Pensa um pouco. ... É pilha. Toda vez que abre um parêntese, você empilha; toda vez que fecha, você desempilha. Se sobrar alguma coisa na pilha no final, ou se você tentar desempilhar uma pilha vazia, os parênteses não fecham certo.

Próximo episódio: hash maps por dentro — como o acesso vira praticamente instantâneo.
