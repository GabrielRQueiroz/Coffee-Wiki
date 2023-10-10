Tags: #Tipo/Proposição #Tópico/Álgebra #Em_progresso

Provas: _Não Aplicável_
Referência: [[Matriz inversa por decomposição LU]]
Justificativa: _Não Aplicável_

Especializações: _Não Aplicável_
Generalizações: _Não Aplicável_

```ad-question
title: Proposição.

Seja o sistema linear com $n$ equações e $n$ variáveis dado na forma matricial $A_{n\times n} \times X_{n\times 1}=B_{n\times 1}$. A matriz pode ser decomposta em
$$
A=L\cdot U, \verb! onde!
$$
$$
L=\begin{pmatrix} 
1 & 0 & \ldots & 0 \\
* & 1 & \ddots & \vdots \\
\vdots & * & 1 & 0 \\
* & \ldots & * & 1
\end{pmatrix}

\verb! e !

U=\begin{pmatrix} 
* & * & \ldots & * \\
0 & * & * & \vdots \\
\vdots & \ddots & * & * \\
0 & \ldots & 0 & *
\end{pmatrix}.
$$

Então, $AX=B \iff LUX=B$.
1. Sendo $L\cdot Y=B$, obtemos o vetor $Y$
2. Sendo $U\cdot X=Y$, obtemos a solução $X$.
```
