Tags: #Tipo/Proposição #Tópico/Álgebra #Em_progresso

Provas: _Não Aplicável_
Referência: _Não Aplicável_
Justificativa: _Não Aplicável_

Especializações: [[Método de Quine-McCluskey]]
Generalizações: _Não Aplicável_

```ad-question
title: Proposição.
```

---
**Exemplo**. Seja o conjunto de primos implicantes

| Agrupamento | Primo implicante |
|---|---|
|$T_{0} \to 2,3$| 0 0 1 x |
|$T_{1} \to 2,10$| x 0 1 0 |
|$T_{2} \to 8,10$| 1 0 x 0 |
|$T_{3} \to 3,7$| 0 x 1 1 |
|$T_{4} \to 5,7,13,15$| x 1 x 1 |

	Na tabela de implicantes por mintermos

| Implicantes | 2 | 3 | 5 | 7|8|10|13|15|
|---|--- |--- |--- |---|---|---|---|---|
|$T_{0} \to$(2,3)| x | x |--- |---|---|---|---|---|
|$T_{1} \to$(2,10)| x |--- |--- |---|---| x |---|---|
|$T_{2} \to$(8,10)|--- |--- |--- |---| x | x |---|---|
|$T_{3} \to$(3,7)|--- | x |---| x |---|---|---|---|
|$T_{4} \to$(5,7,13,15)|--- |--- | x | x |---|---| x | x |
| $M_i$ | $T_{0}+T_{1}$ | $T_{0}+T_{3}$ | $T_{4}$ | $T_{3}+T_{4}$ |$T_{2}$|$T_{1}+T_{2}$| $T_{4}$ | $T_{4}$ |

Pelo método de Petrick:
$$
\begin{align}
S&=M_{2}\cdot M_{3}\cdot M_{5} \cdot M_{7} \cdot M_{8} \cdot M_{10} \cdot M_{13} \cdot M_{15}
\\~\\&=(T_0+T_1)\cdot(T_0+T_{3})\cdot T_{4}\cdot (T_{3}+T_{4}) \cdot T_{2}\cdot(T_1+T_{2})\cdot  \cancel T_{4} \cdot \cancel T_{4}
\\~\\&=(T_{0}+T_{1})\cdot (T_{0}+T_{3})\cdot (T_{3}T_{4}+T_{4})\cdot (T_{1}T_{2}+T_{2})
\\~\\&=(T_{0}+T_{1})\cdot (T_{0}+T_{3})\cdot T_{4}\cdot T_{2}
\\~\\&=(T_{0}+T_{0}T_{3}+T_{0}T_{1}+T_{1}T_{3})\cdot T_{4}\cdot T_{2}
\\~\\&=T_{0}T_{4}T_{2}+T_{0}T_{3}T_{4}T_{2}+T_{0}T_{1}T_{4}T_{2}+T_{1}T_{3}T_{4}T_{2}
\end{align}
$$
- Todas as combinações acima são soluções distintas possíveis. Como $\{T_{0},\,T_{4},\,T_{2}\}$ tem menos termos, a função mínima será composta por ela:
$$
F=T_{0}+T_{2}+T_{4}
$$