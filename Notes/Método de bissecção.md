Tags: #Tipo/Proposição #Tópico/Cálculo

Provas: [[Estudo de convergência do método da bissecção]]
Referência: _Não Aplicável_
Justificativa: _Não Aplicável_

Especializações: [[Método da posição falsa]]
Generalizações: _Não Aplicável_

```ad-question
title: Proposição.
Seja $f:[a,\, b] \to \R$ uma função contínua tal que $f(a)\cdot f(b) \lt 0$. Em outras palavras, $\exists \, \xi \in (a,\, b)$ tal que $f(\xi)=0$. Suponhamos, então, por implicidade, que $\xi$ é a **única raiz** de $f$.

A melhoria do valor pode ser feita de tal modo que a cada $k$-ésima interação, avalia-se se $|b{_k}-a_{k}|\lt \epsilon$. Não sendo, obtém-se o valor médio $M_k=\frac{a_k+b_k}{2}$ e determina-se o menor intervalo onde se encontra $\xi$.
```

---
**Nota**. Dado um erro $\epsilon \gt 0$, o objetivo é encontrar um intervalo de tamanho $\leq \epsilon$ contendo $\xi$.

---

**Exemplo**. Qual o zero da função $f(x)=x^3-5$?

|$x$|0|1|2|...|
|---|---|---|---|---|
|$f(x)$|$-$|$-$|$+$|...|


> Pelo TVI, a raiz deve estar entre $x=1$ e $x=2$.


$$
\begin{aligned}
\begin{align}

& \frac{\partial}{\partial x}f(x)= 3x^{2}\gt 0 \quad\forall x \in \R
\\\\
& \therefore \xi \in [1,\,2] \verb! é a única raiz real de ! f. 

\end{align}
\end{aligned}
$$
> Para um erro $\epsilon = 0.2$, tem-se que $[a,\,b]=[1,\,2],\, |b-a|=1 \gt \epsilon$. Logo, precisamos de um novo intervalo mais curto para diminuir o erro.

$$
\begin{aligned}
\begin{align}
M_0=\frac{a_0+b_0}{2}=\frac{1+2}{2}=\frac{3}{2}=1.5
\end{align}
\end{aligned}
$$
> Com o novo valor proveniente da bissecção, avaliamos onde $\xi$ se encontra:

|$x$|1|1.5|2|
|---|---|---|---|
|$f(x)$|$-$|$-$|$+$|

> Pelo TVI, a raiz deve estar entre $x=1.5$ e $x=2$, ou seja, $\xi \in [1.5,\,2]$

$$
\begin{aligned}
\begin{align}
& |b_1-a_1|=|2-1.5|=0.5 \gt \epsilon
\\\\
& \therefore \verb!O erro ainda está grande!
\\\\
& M_1=\frac{a_1+b_1}{2}=\frac{1.5+2}{2}=1.75

\end{align}
\end{aligned}
$$
> Com o novo valor proveniente da bissecção, avaliamos onde $\xi$ se encontra:

|$x$|1.5|1.75|2|
|---|---|---|---|
|$f(x)$|$-$|$+$|$+$|

 > Pelo TVI, a raiz deve estar entre $x=1.5$ e $x=1.75$, ou seja, $\xi \in [1.5,\,1.75]$

$$
\begin{aligned}
\begin{align}
& |b_2-a_2|=|1.75-1.5|=0.25 \gt \epsilon
\\\\
& \therefore \verb!O erro ainda está grande!
\\\\
& M_2=\frac{a_2+b_2}{2}=\frac{1.5+1.75}{2}=1.625

\end{align}
\end{aligned}
$$
> Com o novo valor proveniente da bissecção, avaliamos onde $\xi$ se encontra:

|$x$|1.5|1.625|1.75|
|---|---|---|---|
|$f(x)$|$-$|$-$|$+$|

 > Pelo TVI, a raiz deve estar entre $x=1.625$ e $x=1.75$, ou seja, $\xi \in [1.625,\,1.75]$

$$
\begin{aligned}
\begin{align}
|b_3-a_{3}|& =|1.75-1.625|=0.125 \lt \epsilon
\\\\
\therefore \overline \xi & = \frac{1.625+1.75}{2}
\\
\\&=1.687 \verb! é uma raiz de precisão ! \epsilon.
\\\\
\end{align}
\end{aligned}
$$
