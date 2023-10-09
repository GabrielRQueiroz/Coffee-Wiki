Tags: #Tipo/Proposição #Tópico/Cálculo #Em_progresso

Provas: _Não Aplicável_
Referência: _Não Aplicável_
Justificativa: _Não Aplicável_

Especializações: _Não Aplicável_
Generalizações: [[Método da posição falsa]]

```ad-question
title: Proposição.
A partir do [[Método de Newton-Raphson (tangente)|método de Newton-Raphson]], $x_{k+1}=\phi(x_k)=x_{k}-\frac{f(x_{k})}{f'(x_{k})}$. O valor de $f'(x_{k})$ pode ser aproximado pelo quoeficiente das diferenças
$$
f'(x_{k})\approx \frac{f(x_{k})-f(x_{k-1})}{x_{k}-x_{k-1}}
$$


Logo, a função de transferência $\phi(x)$ terá o valor
$$
\phi(x_{k})=x_{k}-\left[\frac{f(x_{k})}{\frac{f(x_{k})-f(x_{k-1})}{x_{k}-x_{k-1}}}\right] 
= \frac{x_{k-1}f(x_{k})-x_{k}f(x_{k-1})}{f(x_{k})-f(x_{k-1})}
$$

tornando necessário dois palpites iniciais $x_{0},\, x_{1} \in [a,\,b]$. Se $\epsilon \gt 0$ então $|x_{1}-x_{0}| \gt \epsilon$
```
