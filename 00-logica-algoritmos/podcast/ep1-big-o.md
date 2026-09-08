# Episódio 1 — Complexidade (Big O)

> Duração alvo: 8–10 min · Módulo 00 — Lógica & Algoritmos · Seção de referência: "1. Complexidade (Big O)" na aula
> Cola esse texto direto no NotebookLM (Audio Overview) ou num leitor de texto pra ouvir.

---

**[GANCHO]**

Já teve aquele momento em que seu código funcionava liso no ambiente de teste, com dez, vinte registros... e na produção, com cem mil, começou a travar? Isso quase sempre tem nome: complexidade. E é exatamente sobre isso que todo entrevistador técnico pergunta antes de qualquer outra coisa — porque é o jeito mais rápido de saber se você entende o que o seu código está fazendo por baixo dos panos, não só se ele "funciona".

**[CONCEITO CENTRAL]**

Big O não mede o tempo exato que seu código leva — não é um cronômetro. Big O mede a tendência de crescimento: se eu dobrar o tamanho da entrada, o que acontece com o tempo de execução? Ele dobra também? Quadruplica? Nem muda?

Existe uma escala, da melhor pra pior, que você vai ouvir o tempo inteiro em entrevista: O de 1, O de log n, O de n, O de n log n, O de n ao quadrado, e O de 2 elevado a n.

O 1 significa "não importa o tamanho dos dados, é sempre instantâneo" — pegar o primeiro item de uma lista, por exemplo. O log n é tipo cortar o problema pela metade a cada passo — vou te dar um exemplo sensorial daqui a pouco. O n é o mais comum: você olha cada item da lista uma vez. O n log n é o custo de boa parte dos algoritmos de ordenação. E o n ao quadrado e o dois elevado a n são os vilões — são os que fazem seu sistema travar quando os dados crescem.

**[EXEMPLO PRÁTICO]**

Pensa assim: você tem uma lista de cem clientes. Se o seu código passa por cada cliente uma vez, fazendo alguma verificação simples, isso é O de n — cresce na mesma proporção que os dados.

Agora imagina que, pra cada cliente, você compara ele com todos os outros clientes da lista — tipo, verificar se tem algum duplicado, comparando um a um, todo mundo com todo mundo. Isso é um loop dentro de outro loop, na mesma lista. Cem clientes viram dez mil comparações. Mil clientes viram um milhão de comparações. Isso é O de n ao quadrado, e é exatamente esse tipo de código que funciona liso com dados de teste e trava em produção.

O sinal mais confiável, e o mais fácil de pegar numa entrevista ou numa revisão de código: você tem um for dentro de outro for, os dois passando pela mesma coleção de dados? Desconfie. Isso quase sempre é O de n ao quadrado.

**[TRUQUE DE MEMORIZAÇÃO]**

Pra gravar a ordem da escala, canta ela como se fosse subindo uma escada musical: "um... log... linear... n-log... quadrado... exponencial". Repete isso três vezes agora, em voz alta ou só na cabeça — um, log, linear, n-log, quadrado, exponencial. E toda vez que você ver um for dentro de outro for na mesma lista, o alarme que deve tocar na sua cabeça é: "quadrado".

**[FECHAMENTO + PERGUNTA DE REVISÃO]**

Resumindo em uma frase: Big O é sobre tendência de crescimento, não tempo exato, e o sinal mais comum de alerta é loop dentro de loop na mesma coleção.

Agora a pergunta pra você responder mentalmente, sem olhar em nada: se o seu código tem dois loops separados, um depois do outro, passando pela mesma lista — não um dentro do outro, mas em sequência — isso ainda é O de n, ou já virou O de n ao quadrado? ... Pensa um pouco. ... A resposta é: continua sendo O de n. Dois loops em sequência somam o trabalho, não multiplicam — loop dentro de loop é que multiplica. É uma pegadinha clássica de prova de lógica, guarda essa diferença.

Próximo episódio: arrays, listas encadeadas, pilhas e filas — e quando escolher cada uma.
