# Episódio 3 — Hash maps por dentro

> Duração alvo: 8–10 min · Módulo 00 — Lógica & Algoritmos · Seção de referência: "3. Hash maps por dentro" na aula
> Cola esse texto direto no NotebookLM (Audio Overview) ou num leitor de texto pra ouvir.

---

**[GANCHO]**

Imagina que você quer achar o contato "Felipe" na sua agenda de telefone. Se a agenda estivesse desorganizada, você teria que ler nome por nome até achar. Mas seu celular acha instantaneamente, não importa se você tem cinquenta ou cinco mil contatos. Como? É basicamente a mesma ideia por trás de um hash map, provavelmente a estrutura de dados mais usada em código de verdade — e mais cobrada em entrevista.

**[CONCEITO CENTRAL]**

Um hash map guarda pares de chave e valor — tipo, o nome "Felipe" aponta pro número de telefone dele. A mágica é como ele decide onde guardar cada coisa: ele pega a chave, calcula um número a partir dela — isso se chama hash — e usa esse número pra decidir direto em qual "gaveta" guardar o valor.

Por isso o acesso é praticamente instantâneo, o que a gente chama de O de 1 em média: ele não procura item por item, ele calcula matematicamente onde a coisa está e vai direto lá. É a diferença entre folhear uma lista telefônica inteira e simplesmente saber, de cabeça, em qual página determinado sobrenome está.

**[EXEMPLO PRÁTICO]**

O uso mais clássico de hash map em entrevista é o seguinte problema: você tem uma lista de números e um valor alvo, e precisa achar dois números da lista que somados dão esse alvo. A solução ingênua é comparar cada número com todos os outros — isso é o tal do O de n ao quadrado que a gente viu no episódio um, loop dentro de loop.

A solução esperta usa um hash map como uma espécie de "caderninho do que eu já vi". Você percorre a lista uma única vez. Pra cada número, você calcula qual seria o complemento dele — quanto falta pra chegar no alvo — e pergunta pro caderninho: "eu já vi esse complemento antes?". Se já viu, achou o par, acabou. Se não viu, anota esse número no caderninho e segue pro próximo. Isso transforma um problema de O de n ao quadrado em um problema de O de n — uma passada só pela lista, com uma consulta instantânea a cada passo.

Esse padrão de raciocínio — "eu já vi isso antes?" — resolve uma quantidade enorme de exercícios: caracteres repetidos numa string, números duplicados numa lista, agrupar palavras que são anagramas umas das outras. Sempre que a solução óbvia for "pra cada item, eu procuro de novo em tudo", pare e pergunte: dá pra trocar essa busca repetida por uma consulta num hash map?

**[TRUQUE DE MEMORIZAÇÃO]**

A frase-gatilho é: "eu já vi esse valor antes?". Toda vez que você perceber que sua solução está comparando um item com todos os outros de novo e de novo, essa pergunta é o sinal de que um hash map troca a busca lenta por uma consulta rápida.

**[FECHAMENTO + PERGUNTA DE REVISÃO]**

Resumo: hash map calcula a posição da chave em vez de procurar, o que dá acesso O de 1 em média, e o padrão "já vi isso antes" é o gatilho mental pra saber quando usar um.

Pergunta de revisão: se o hash map calcula a posição direto pela chave, por que às vezes, no pior caso, o acesso pode virar O de n, lento como percorrer uma lista inteira? ... Pensa um pouco. ... É quando acontece uma colisão: duas chaves diferentes calculam o mesmo número de hash e caem na mesma gaveta. Nesse caso, aquela gaveta vira uma listinha, e no pior dos casos você precisa percorrer ela inteira. Na prática, com uma função de hash bem feita, isso quase nunca acontece — mas é o tipo de detalhe que mostra profundidade numa entrevista.

Próximo episódio: recursão — o caso base, o caso recursivo, e por que ela usa a mesma ideia de pilha que você já conhece.
