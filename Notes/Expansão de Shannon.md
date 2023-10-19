Tags: #Tópico/Álgebra #Tipo/Teorema #Em_progresso

Provas: _Não Aplicável_
Referência: _Não Aplicável_
Justificativa: _Não Aplicável_

Especializações: _Não Aplicável_
Generalizações: _Não Aplicável_

```ad-info
title: Teorema.
Seja $F(x_{1},\,x_{2},\,\ldots,\,x_{n})$. Esta pode ser escrita em sua forma canônica
$$
\begin{gather}

F(x_{1},\,x_{2},\,\ldots,\,x_{n})=x_{1}\cdot F(1,\,x_{2},\,\ldots,\,x_{n}) + \overline{x_{1}}\cdot F(0,\,x_{2},\,\ldots,\,x_{n})
\\~\\
\iff
\\~\\
F(x_{1},\,x_{2},\,\ldots,\,x_{n})=(x_{1}+F(0,\,x_{2},\,\ldots,\,x_{n}))\cdot (\overline{x_{1}}+F(1,\,x_{2},\,\ldots,\,x_{n}))
\end{gather}
$$

```
---

**Exemplo**. $AB+A\overline C+BC = AB+\overline A C$
$$
\begin{align}
\begin{aligned}
&\verb!Prova:!
\\
&AB+A\overline C+BC
\\
&=AB(C+\overline C)+\overline A(B+\overline B)C + (A+\overline A)BC
\\
&=\cancel {ABC} + AB\overline C +\cancel {\overline ABC} + \overline A \overline B C+ABC+\overline ABC
\\
&=ABC +  AB\overline C + \overline A\overline B C+ \overline A BC
\\
&=AB(C+\overline C)+\overline AC(B+\overline B)
\\
&=AB+\overline AC
\end{aligned}
\end{align}
$$
