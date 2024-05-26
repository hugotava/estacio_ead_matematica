# Matemática e Lógica :bookmark_tabs:

## Princípios de contagem
### Agrupamentos combinatórios
---
  ### Arranjo: $A^n_p = \frac{n!}{(n-p)!}$
  * Exemplo: De quantas maneiras podemos fazer filas com 5 alunos, se dispomos de 12 alunos?
  * Solução: $\frac{12!}{(12-5)!} = \frac{12!}{7!} = \frac{12 \times 11 \times 10 \times 9 \times 8 \times 7!}{7!} = 12 \times 11 \times 10 \times 9 \times 8 =  95040$
---
  ### Permutação: $P_n = n!$
  * Exemplo:
    Calcule o número de anagramas das palavras TRAPO e da palavra PUBLICAR.
  * Solução TRAPO:
    $P_5 = 5! = 5 \times 4 \times 3 \times 2 \times 1 = 120$
  * Solução PUBLICAR:
    $P_8 = 8!  = 8 \times 7 \times 6 \times 5! = 8 \times 7 \times 6 \times 120 = 40320$
---
  ### Combinação: $C^n_p = \frac{A^n_p}{p!} = \frac{n!}{(n-p)! \times p!}$
  * Exemplo: Determine quantos subconjuntos de 3 elementos podemos construir a partir de um conjunto com 7 elementos.
  * Solução:
    - Os últimos exemplos abordados tratam, basicamente, de ordenar objetos. Mas há situações em que a ordem dos objetos não é relevante. Esse exemplo é uma dessas situações, pois as notações { a, b, c } e { a, c, b }, { b, c, a },
{ b, a, c }, { c, a, b } e { c, b, a } representam o mesmo conjunto, cujos elementos são a, b e c.
    - Se a, b e c são 3 dos 7 objetos do conjunto, então estamos contando as 6 filas diferentes como subconjuntos diferentes, que são, na verdade, iguais. Ora, então, ordenando 7 objetos 3 a 3 obtemos: $A^7_3 = \frac{7!}{(7-3)!} = \frac{7!}{4!} = \frac{7 \times 6 \times 5 \times 4!}{4!} = 7 \times 6 \times 5 = 210$
    - Mas de cada três objetos escolhidos estamos contando $3! = 6$ vezes o mesmo conjunto! Então, para ajustar nosso resultado devemos dividir o resultado anterior por $3! = 6$. Logo, podemos formar $210 ÷ 3! = 35$ subconjuntos de 3 elementos a partir de um conjunto com 7 elementos.
    - Esse tipo de situação nos remete ao terceiro agrupamento básico, utilizado em contagem, e que chamamos de combinação de n objetos tomados p a p, ou n escolhe p, em que não importa a ordem dos objetos, mas apenas o subconjunto formado por eles. Então, no caso geral, devemos dividir o número de filas por p! para contarmos uma única vez cada uma das p! filas que compõem o mesmo conjunto.
    - Eis a solução com Combinação: $C^7_3 = \frac{A^7_3}{3!} = \frac{7!}{(7-3)! \times 3!} = \frac{7!}{4! \times 3!} = \frac{7 \times 6 \times 5 \times 4!}{4! \times 3!} = \frac{7 \times 6 \times 5}{ 3 \times 2 \times 1} = \frac{7 \times 6 \times 5}{6} = 7 \times 5 = 35$
---



Para determinar quantos subconjuntos de 3 elementos podemos construir a partir de um conjunto com 7 elementos, usamos a fórmula das combinações. A combinação de \( n \) elementos tomados \( k \) de cada vez é dada por:

$C(n, k) = \frac{n!}{k!(n-k)!}$

No caso, temos $n = 7$ e $k = 3$. Substituindo esses valores na fórmula, temos:

$C(7, 3) = \frac{7!}{3!(7-3)!} = \frac{7!}{3!4!}$

Podemos escrever $7!$ e $4!$ de forma que possamos cancelar os fatores comuns:

$7! = 7 \times 6 \times 5 \times 4!$

Então, a fórmula se torna:

$C(7, 3) = \frac{7 \times 6 \times 5 \times 4!}{3! \times 4!}$

Os $4!$ no numerador e no denominador se cancelam:

$C(7, 3) = \frac{7 \times 6 \times 5}{3!}$

Agora, calculamos $3!$:

$3! = 3 \times 2 \times 1 = 6$

Então, a expressão fica:

$C(7, 3) = \frac{7 \times 6 \times 5}{6}$

Podemos simplificar $6$ no numerador e no denominador:

$C(7, 3) = 7 \times 5 = 35$

Portanto, o número de subconjuntos de 3 elementos que podemos formar a partir de um conjunto com 7 elementos é:

$\boxed{35}$
