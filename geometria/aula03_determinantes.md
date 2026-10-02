# determinantes

## calculo determinantes

### matriz 1x1

O determinante desse tipo de matriz é justamente seu elemento

$$
M = 
\begin{bmatrix}
1
\end{bmatrix}
$$

$$
det(M) = 1
$$

### matriz 2x2 

em matrizes 2x2 o determinante é decidido multiplicando os valores na diagonal principal, depois os da diagonal secundária e então somando os valores.


$$
M = 
\begin{bmatrix}
1 && 2 \\
3 && 4
\end{bmatrix}
$$

$$
det(M) = 1.4 - 2.3 
$$

$$
det(M) = 4 - 6 = -2
$$

### matriz 3x3

Tem diferentes metodos para calcular o determinante de matrizes 3x3

#### Metodo regra de Sarrus

nesse metodo você pega as 2 primeiras colunas da matriz e as repete na direita dela. Depois você faz o produto da diagonal principal e mais 2 diagonais indo a direita, após isso fazer a mesma coisa com a diagonal secundária indo para as diagonais também a direita.

Após os calculos deve subtrair o resultado da diagonal principal com o da diagonal secundária e terá o determinante da matriz

$$
M = 
\begin{bmatrix}
1 && 2 && 3\\
4 && 5 && 6 \\
7 && 8 && 9
\end{bmatrix}
$$


$$
\begin{bmatrix}
1 && 2 && 3 && 1 && 2 \\
4 && 5 && 6 && 4 && 5 \\
7 && 8 && 9 && 7 && 8
\end{bmatrix}
$$

> diagonal principal
$$
1.5.9 + 2.6.7 + 3.4.8 = 225
$$

> diagonal secundária
$$
3.5.7 + 1.6.8 + 2.4.9 = 225
$$

> determinante
$$
det(M) = 225 - 225 = 0
$$

#### Metodo de Laplace

Para etender esse metodo é necessário entender 2 novos conceitos

##### Menor complementar    

A menor complementar diz respeito a um elemento da matriz. para achar a menor complementar de um elemento $a_{ij}$ dentro de uma matriz de ordem >= 2, precisa suprimir a coluna e linha desse elemento. A menor complementar será o determinante dos elementos que sobrarem.

$$
M =
\begin{bmatrix}
1 && 2 && 3 \\
3 && 5 && 6 \\
7 && 8 && 9 \\
\end{bmatrix}
$$

vamos achar a menor complementar de 1

$$
D = 
\begin{bmatrix}
5 && 6 \\
8 && 9
\end{bmatrix}
$$

$$
5.9 - 8.9 = 45 - 72 = -27
$$

> o menor complementar do elemento 1 é -27

##### Complemento algebrico (cofator)

o complemento algébrico se define em $A_{ij}$ na seguinte equação:

> $D_{ij}$ é o menor complementar

$$
A_{ij} = (-1)^{i + j} . D_{ij}
$$

no exemlo anterior o complemento álgebrico de 1 (primeiro elemento) seria calculado assim:

$$
A_{11} = (-1)^{1+1} . -27
$$

$$
A_{11} = (-1)^{2} . -27
$$

$$
A_{11} = 1 . -27
$$

$$
A_{11} = -27
$$


> o complemento álgebrico de 1 nessa matriz é -27

> esse calculo parece que sempre da o valor do menor complementar ou 
positivo ou negativo depedendo da posição

Agora vamos para o metodo em si, para calcular o determinante de uma matriz vamos pegar uma linha ou coluna inteira e somar os produtos dos elentos e seus cofatores.

$$
det(M) = \sum_{j} a_{ij} . A_{ij}
$$

## Matriz adjunta

suponhamos que tem uma matriz $M$, a matriz adjunta é a matriz $M$ mas cada elemento é trocado pelo seu cofator ($A_{ij}$) e depois a matriz é tranposta. O resultado vai ser a matriz adjunta dessa matriz, que é representada por $adj(M)$ ou $M*$.

### Calculo matriz inversa

com a matriz adjunta podemos achar a matriz inversa de uma matriz. é possivel com o seguinte calculo:

$$
M^-1 = \frac{1}{det(M)}.adj(M)
$$

> por ser uma divisão quando o determinante de uma matriz for 0 não é possível calcular a matriz inversa