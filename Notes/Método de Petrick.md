Tags: #Tipo/Proposição #Tópico/Álgebra #Em_progresso

Provas: _Não Aplicável_
Referência: _Não Aplicável_
Justificativa: _Não Aplicável_

Especializações: _Não Aplicável_
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

Pelo método de Petrick:
$$
\begin{align}
S&=(T_0+T_1)\cdot(T_0+T_{3})\cdot T_3\cdot(T_!+T_2)\cdot(T_3+T_4)
\\~\\&=(T_0+\cancel{T_0T_3}+\cancel{T_1T_0}+T_1T_3)\cdot T_3\cdot(T_!+T_2)\cdot(T_3+T_4)
\\~\\&=(T_0+T_1T_3)\cdot T_{3}\cdot (T_!+T_2)\cdot(T_3+T_4)
\\~\\&=(T_0T_3+T_1T_3)\cdot(T_1T_3+T_1T_4+T_2T_3+T_2T_4)
\end{align}
$$
