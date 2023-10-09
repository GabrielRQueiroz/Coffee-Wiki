Tags: #Tipo/Teorema #Tópico/Álgebra #Em_progresso

Provas: _Não Aplicável_
Referência: [[Posto de uma matriz|$posto(A)$]], [[Núcleo da transformação linear|$Ker(T_{A})$]]
Justificativa: _Não Aplicável_

Especializações: _Não Aplicável_
Generalizações: _Não Aplicável_

```ad-info
title: Teorema.
Dado o sistema linear $A\cdot X = b$, onde $A_{m\times n},\, X_{n\times 1},\, b_{1\times m}$. Então:

1. Se $posto(A|b) \gt posto(A)$, o sistema não possui solução;
2. Se $posto(A|b) = posto(A) = n$, o sistema possui uma única solução;
3. Se $posto(A|b) = posto(A) = r \lt n$, o sistema possui infinitas soluções. O espaço (afim) $S$ de todas as soluções tem dimensão $n - posto(A)$.

Existindo solução, o conjunto $S$ de todas as soluções é o espaço afim paralelo a $Ker(T_{A})$ de dimensão $n-posto(A)$:
$$
S=X_{0} - Ker(T_{A}),
$$

onde $A\cdot X_{0}=B$ e $Ker(T_{A})$ é solução de $A\cdot X=\overline 0$
```
