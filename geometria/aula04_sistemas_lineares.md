# sistemas lineares

## definição

são um sistema formado por um conjunto de equações lineares

equação linear são equações que seguem uma formula parecida com:

$$
a_1 x_1 + a_2 x_2 + a_3 x_3 + ... a_n x_n = b
$$

$a_1$, $a_2$, $a_n$ são os coeficientes da equação, são números reais e na equação tem que ter pelo menos um diferente de 0

$x_1$, $x_n$ são chamadas de variaveis ou icognitas

$b$ é um número real e chamado de termo idepedente

### exemplo

$$
x -2y + 5z = 10
$$

- os coeficientes ($a$) aqui são $1$ (omitido do lado do $x$), $-2$ e o $+5$

- $x$, $y$ e $z$ são as váriaveis

- o termo idepedente é o $10$

### Não é equação linear quando

- tiver um expoente maior que 1 na equação

- tiver multiplicações entre variaveis

- quando tiver funções dentro da equação  



## exemplos e tipos sistema linear 

### exemplo 1

$$
\begin{cases}
2x + y = 5 \\
x - y = 1
\end{cases}
$$

nesse sistema linear teriamos de achar um valor de x e de y que satisfaça ambas as equações.

nesse caso as duas equações representam retas diferentes, então existe apenas uma solução. Sistemas lineares assim são chamados de **determinado**.


### exemplo 2 

$$
\begin{cases}
2x + y = 5 \\
4x - 2y = 10
\end{cases}
$$

ambas as equações são multiplas uma da outra. Logo em um gráfico formariam uma mesma reta.

como a solução do sistema linear é o ponto em comum das retas e todos os pontos são em comum em duas retas iguais, esse é um sistema linear indeterminado

### exemplo 3

$$
\begin{cases}
2x + y = 5 \\
4x - 2y = 50
\end{cases}
$$

se fizessemos um gráfico desse sistema, as retas ficariam em paralelo mas nunca se encontrariam.

como não existe ponto em comum, é um sistema linear impossível.

## outras caracteristicas de sistemas lineares

é possível representar sistemas lineares com matrizes.

para isso:

- transforme os coeficientes em uma matriz 

o sistema linear

$$
\begin{cases}
2x + y = 5 \\
4x - 2y = 50
\end{cases}
$$

ficaria 

$$
A =
\begin{bmatrix}
2 && 1 \\
4 && 2
\end{bmatrix}
$$

- transforme as icognitas em uma martiz coluna.

$$
X =
\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

- transforme os termos idepedentes em uma matriz coluna

$$
B =
\begin{bmatrix}
5 \\
50
\end{bmatrix}
$$

no final a relação do sistema linear em matriz fica assim:

$$
A.X = B
$$

## sistemas lineares equivalentes

é quando 2 ou mais sistemas possuem uma mesma solução

## Solução dos sistemas lineares

### Regra de Cramer

$$
\begin{cases}
2x + y = 5 \\
x - y = 1
\end{cases}
$$

> primeiro pega os coeficientes, bota em uma matriz $D$ e calcula o determinante

$$
D =
\begin{bmatrix}
2 && 1 \\
1 && -1
\end{bmatrix}
= 
-3
$$

> após isso vamos pegar o determinante da mesma matriz, mas para achar o valor da primeira variavel vamos trocar a primeira coluna pelos termos indepedentes

$$
D_x =
\begin{bmatrix}
5 && 1 \\
1 && -1
\end{bmatrix}
= 
-6
$$

> agora faremos o mesmo para a segunda variavel


$$
D_y =
\begin{bmatrix}
2 && 5 \\
1 && 1
\end{bmatrix}
= 
-3
$$

> para finalizar precisamos fazer uma conta que nos dá a solução desde que tenhamos os determinantes achados acima

$$
x = \frac{D_x}{D}
$$

$$
x = \frac{-6}{-3} = 2
$$

$$
y = \frac{D_y}{D} = \frac{-3}{-3} = 1
$$

agora achamos a nossa solução

$$
S = {2, 1}
$$

### Metodo eleminação de Gauss

> é ensinado o sistema linear escalonado não anotei porque da para deduzir

O objetivo desse metodo é transformar o sistema linear em um sistema linear escalonado que é mais fácil de se resolver

para fazer isso é feito alguns passos:

- se faz uma matriz com os coeficientes + os termos indepedentes no final

- com tal matriz feita agora o objetivo é transformar ela em uma matriz triangular superior

as operações para transformar a matriz permitidas são:

1. trocar 2 linhas de posição

2. Multiplicar ou dividir qualquer linha por um número real não nulo

3. substituir uma linha por uma adição dela por outra que foi multipicada antes

