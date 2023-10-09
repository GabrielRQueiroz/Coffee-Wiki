Tags: #Tipo/Proposição #Tópico/Cálculo #Em_progresso

Provas: _Não Aplicável_
Referência: _Não Aplicável_
Justificativa: _Não Aplicável_

Especializações: _Não Aplicável_
Generalizações: [[Método da posição falsa]]

```ad-question
title: Proposição.
Seja $f(x)=0 \iff \phi(x)=x$, em $[a,\,b]$ ([[Método do ponto fixo]]). A função de iteração 
$$
\phi(x)=x-\frac{f(x)}{f'(x)}
$$
pode ser utilizada diante das condições:

1. $f$, $f'$ e $f''$ são contínuas em $[a,\,b]$;
2. $f'(x)\neq 0,\, \forall\; x\in [a,\,b]$; e
3. $x_0\in[a,\,b]$ está "suficientemente próximo" de $\xi$.

```

**Prova**. 
$$
\begin{align}
&\phi(x)=x
\\ \iff &x-\frac{f(x)}{f'(x)}=x
\\ \iff &-\frac{f(x)}{f'(x)}=0
\\ \iff & f(x)=0, \, \verb!se ! f'(x)\neq0 \, \forall x\in[a,\,b]
\end{align}
$$