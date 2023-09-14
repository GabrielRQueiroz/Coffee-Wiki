Tags: #Tipo/Proposição #Em_progresso

Provas: _Não Aplicável_
Referência: _Não Aplicável_
Justificativa: _Não Aplicável_

Especializações: _Não Aplicável_
Generalizações: _Não Aplicável_

```ad-question
title: Proposição.
Seja $f(x)=0 \iff \phi(x)=x$, em $[a,\,b]$ ([[Método do ponto fixo]]):
1. $\phi$ e $\phi '$ são contínuas em $[a,\,b]$
2. $|\phi '(x)| \le L \lt x,\, \forall x\in [a,\,b]$
3. $x_0\in[a,\,b]$
Seja, então, $f:[a,\,b]\to\R,\, f,\, f'$ e $f''$ contínuas. Suponha que $\xi \in [a,\,b]$ seja a única raiz de $f$ em $[a,\,b]$
$$
f(x)\stackrel{?}{=}0
$$

Logo, $\phi(x)=x-\frac{f(x)}{f'(x)}$ é função de iteração de $f$.
```

---

**Prova**. 
$$
\begin{align}
&\phi(x)=x
\\ \iff &x-\frac{f(x)}{f'(x)}=x
\\ \iff &-\frac{f(x)}{f'(x)}=0
\\ \iff & f(x)=0, \, \verb!se ! f'(x)\neq0 \, \forall x\in[a,\,b]
\end{align}
$$