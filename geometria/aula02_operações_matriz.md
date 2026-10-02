# Operações matriz

## Adição e subtração

Adição e subtração de matrizes acontecem em matrizes de mesmo tamanho. Ela funciona adicionando ou subtraindo cada elemento com o respectivo espaço na outra matriz

> exemplo adição

$$
\begin{bmatrix}
1 & 5 \\
-2 & 9 \\
\end{bmatrix}

+ 

\begin{bmatrix}
2 & 3 \\
10 & 1 \\
\end{bmatrix}

= 

\begin{bmatrix}
3 & 8 \\
8 & 10 \\
\end{bmatrix}
$$

A subtração funciona da mesma forma

### propriedades adição

1. é comutativa: $A + B = B + A$

2. é associativa: $(A + B) + C = A + (B + C)$

3. Tem elemento neutro na adição: $\exists M | A + M = A$

4. Teme elemento simetrico: $\exists A' | A + A' = M$

5. $(A ± B)^T = A^T ± B^T$

## Multiplicação

### por número escalar

quando multiplicando uma raiz por um número escalar (número real qualquer), se multiplica o número escalar por cada elemento da matriz.

### multiplicação de matrizes com matrizes

para se multiplicar matrizes elas tem que seguir uma regra: o número de colunas de uma matriz tem que ser o mesmo que o número de linhas da outra. O resultado sempre vai ter o tamanho das linhas da primeira matriz e das colunas da segunda.

$$
A_{3x2} * B_{2x3} = C_{3x3}
$$

O algoritimo dessa multiplicação é:

> $c_{ij}$ é cada elemento da nova matriz gerada na multiplicação

$$
c_{ij} = \sum_{k=1}^{n} a_{ik} + b_{kj}
$$

Simplificando você pega a primeira linha da primeira matriz e multiplica pela primeira coluna da segunda. Isso vai gerar o primeiro elemento. Após multiplique a primeira coluna e gere o segundo elemento da nova matriz. Depois de passar todas as colunas deça uma linha e repita o processo.

### propriedades da multiplicação de matrizes

1. não é comutativa: $A * B ≠ B * A$

2. é associativa: $(A * B) * C = A * (B * C)$

3. é distributiva à direita em relação à adição : $(A + B)*C = A*C + B*C$

3. é distributiva à esquerda em relação à adição : $C*(A + B) = C*A + C*B$

4. Matriz identidade é o elemento neutro da multiplicação de matrizes


## Matrizes invertiveis

Uma matriz $A$ é invertivel se, e somete se, existir uma matriz $B$ que a multiplicação em ambas as formas ($A.B$ e $B.A$) é ingual a uma matriz identidade.

Tem um teorema que diz que se $A$ é invertível então $B$ é única.

$$
A.B = B.A = I_n
$$

> se não tem matriz inversesa a matriz se chama matriz singular

### Calcular a matriz invertivel

supondo que temos uma matriz e sabemos que se multiplicado por outra matriz ela se tornara $I_n$. 

$$
A . B = I_n
$$

podemos substituir B por uma matriz com simbolos variaveis a multiplicar $A.B$ assim vamos obter varias equações em cada espaço que podemos usar em conjunto para descobrir o valor das variaveis