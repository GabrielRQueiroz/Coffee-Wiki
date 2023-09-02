Tags: #Tópico/Cálculo #Tipo/Proposição #Em_progresso

Provas: _Não Aplicável_
Referência: _Não Aplicável_
Justificativa: _Não Aplicável_

Especializações: _Não Aplicável_
Generalizações: _Não Aplicável_

```ad-question
title: Proposição.

A partir de uma aproximação inicial para a raiz, encontrar novas aproximações de modo iterativo.

---


**Localização** 
Analisar 
- continuidade, 
- classe de derivação, 
- sinal, 
- crescimento e 
- gráfico 

de $f$ prara encontrar intervalos fechados, cada um contendo uma, e somente uma, raiz de $f$ e garantir que estas são todas as raízes reais de $f$.

---

**Fase de refinamento**
A partir da aproximação inicial, melhorar o resultados até obter uma aproximação de precisão $\epsilon \gt 0$ prefixada (erro absolute menor que $\epsilon$).
```

---


**Exemplo**: $f(x)=x^3-9x+3$

|x|-5|-4|-3|-2|-1|0|1|2|3|4|5|
|---|---|---|---|---|---|---|---|---|---|---|---|
|f(x)| - | **-** | **+** | + | + | **+** | **-** | **-** | **+** | + | + |

Pelo TVI, $\exists \xi_{1}\in [-4,\, -3],\, \exists \xi_{2}\in [0,\, 1],\, \exists \xi_{3}\in [2,\, 3]$ tal que $\xi_i$ é raiz de $f$. 
Pelo TFA, $f$ possui exatamente 3 raízes complexas, logo temos que $\xi_i$ é única no intervalo e estas são todas as raízes de $f$.

**Exemplo**: $f(x)=x^3+3x-5$

|x|-5|-4|-3|-2|-1|0|1|2|3|4|5|
|---|---|---|---|---|---|---|---|---|---|---|---|
|f(x)| - | **-** | **+** | + | + | **+** | **-** | **-** | **+** | + | + |

Pelo TVI, $\exists \xi_{1}\in [-4,\, -3],\, \exists \xi_{2}\in [0,\, 1],\, \exists \xi_{3}\in [2,\, 3]$ tal que $\xi_i$ é raiz de $f$. 
Pelo TFA, $f$ possui exatamente 3 raízes complexas, logo temos que $\xi_i$ é única no intervalo e estas são todas as raízes de $f$.
