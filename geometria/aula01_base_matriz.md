# Matrizes

## Diagonais

matrizes teram uma diagonal definida pelas expressões a seguir. Tais expressões consideram que é uma matriz quadrada.

### Diagonal principal 

$$
a_{ij} | i = j
$$

ou seja 11 22 33 e assim por diante

### Diagonal secundária

$$
a_{ij} | i + j = n + 1 
$$

**n** é a ordem da matriz quadrada. Digamos que a matriz é de ordem 3 então a diagonal será: 13, 22, 31. Pois a soma da linha e coluna é ingual a ordem da matriz + 1, no primeiro exemplo 1 + 3 = 4.

## Tipos de matriz

### Triangular

Uma matriz é uma matriz triangular quando os elemntos abaixo ou acima da diagonal principal são nulos

> matriz triangular superior
$$
MTS = 
\begin{bmatrix}
1 & 2 & 3 \\
0 & 5 & 6 \\
0 & 0 & 9
\end{bmatrix}
$$


> matriz triangular inferior
$$
MTI =
\begin{bmatrix}
1 & 0 & 0 \\
6 & 5 & 0 \\
5 & 4 & 9
\end{bmatrix}
$$

### identidade

Identidade é um tipo especial que a diagonal principal é 1 e o resto dos espaços são nulos. Ela é representada por $ I_n $ e são matrizes quadradas

$$
I_3 =
\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$


$$
I_4 =
\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1 
\end{bmatrix}
$$

### Transposta

matriz tranposta é quando se tem uma matriz e troca o lugar da coluna pelo da linha. Se a matriz é chamada de $A$ a matriz transposta vai ser chamada $A^T$

$$
A =
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\ 
\end{bmatrix}
$$

$$
A^T =
\begin{bmatrix}
1 & 4  \\
2 & 5  \\ 
3 & 6 \\ 
\end{bmatrix}
$$

#### Propriedades matriz transposta

1) $(A^T)^T = A$

2) $(A ± B)^T = A^T ± B^T$

3) se $A = A^T$, $A$ se chama matriz simetrica


## observações da aula

- Ficou um pouco confuso as leis de formação de matrizes. Verificar no material base caso necessário