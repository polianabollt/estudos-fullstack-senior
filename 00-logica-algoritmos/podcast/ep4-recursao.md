# Episódio 4 — Recursão

> Duração alvo: 8–10 min · Módulo 00 — Lógica & Algoritmos · Seção de referência: "4. Recursão" na aula
> Cola esse texto direto no NotebookLM (Audio Overview) ou num leitor de texto pra ouvir.

---

**[GANCHO]**

Pensa numa boneca russa, daquelas matryoshka — você abre uma e tem outra igual, um pouco menor, dentro. Você abre essa, tem outra dentro. Isso continua até chegar numa bonequinha sólida, que não abre mais. É basicamente a lógica de uma função recursiva: uma função que chama a si mesma, uma versão um pouco menor do mesmo problema, até chegar num caso simples o bastante pra responder direto.

**[CONCEITO CENTRAL]**

Toda função recursiva, sem exceção, precisa ter duas partes. A primeira é o caso base — a bonequinha sólida, o momento em que a função para de chamar a si mesma e simplesmente devolve uma resposta direta. A segunda é o caso recursivo — a parte que chama a função de novo, mas com um problema um pouco menor, um pouco mais perto do caso base.

Se faltar o caso base, ou se o caso recursivo nunca se aproximar dele, a função chama a si mesma pra sempre — e o programa quebra com um erro de estouro de pilha.

E repara nessa palavra: pilha. Não é força de expressão. Cada vez que uma função chama a si mesma, o computador empilha um novo "quadro" numa estrutura chamada pilha de chamadas — literalmente a mesma estrutura de dados pilha que a gente viu no episódio dois, aquela do Ctrl+Z, LIFO, o último que entra é o primeiro que sai. Cada chamada recursiva empilha; quando ela termina e devolve um valor, desempilha. Se você entendeu pilha no episódio dois, você já entende metade de como recursão funciona por dentro.

**[EXEMPLO PRÁTICO]**

Pensa no cálculo de fatorial. Fatorial de quatro é quatro vezes fatorial de três, que é três vezes fatorial de dois, que é dois vezes fatorial de um. E fatorial de um — esse é o caso base — a resposta é simplesmente um, sem precisar chamar nada de novo.

Então o computador empilha: preciso do fatorial de quatro, mas antes preciso do de três, mas antes preciso do de dois, mas antes preciso do de um. Ele chega no de um, que responde direto, sem empilhar mais nada. E aí ele começa a desempilhar de trás pra frente: fatorial de um é um, então fatorial de dois é dois vezes um, que é dois; fatorial de três é três vezes dois, que é seis; fatorial de quatro é quatro vezes seis, que é vinte e quatro. Reparou que a resposta só aparece depois que a pilha inteira desce de volta? É por isso que recursão pode gastar mais memória que um loop simples — cada chamada fica "esperando" na pilha até a de baixo responder.

**[TRUQUE DE MEMORIZAÇÃO]**

Antes de escrever qualquer recursão, responda duas perguntas em voz alta: "quando eu paro?" e "o que eu faço pra chegar mais perto de parar?". Se você não consegue responder as duas com clareza, ainda não está pronta pra escrever o código — vai travar no meio.

**[FECHAMENTO + PERGUNTA DE REVISÃO]**

Resumo: toda recursão tem caso base e caso recursivo, e por trás dela existe uma pilha de chamadas se enchendo e depois esvaziando — a mesma lógica LIFO da pilha que você já conhece.

Pergunta de revisão: pra somar os números de um a cem, você usaria recursão ou um loop simples? E por quê? ... Pensa um pouco. ... Na prática, um loop simples é mais eficiente aqui — ele não gasta memória empilhando cem chamadas. Recursão vale a pena quando o problema já é naturalmente hierárquico, tipo percorrer uma árvore, fazer backtracking, ou dividir um problema ao meio repetidamente, como no mergesort. Pra uma soma simples e sequencial, loop é a escolha mais direta.

Próximo episódio: busca binária — a lógica de procurar um nome numa lista telefônica impressa, sem folhear página por página.
