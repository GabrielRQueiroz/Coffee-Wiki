Tags: #Tipo/Definição #Tópico/Elétrica #Em_progresso

Tipos: [[Sinal impulso unitário]], [[Sinal degrau unitário|Degrau unitário]], [[Sinais senoidais]], [[Sinais exponenciais]]
Exemplos: _Não Aplicável_  
Construções: _Não Aplicável_  
Generalizações: _Não Aplicável_

Propriedades: [[Amostragem de sinais]]  
Suficiências: _Não Aplicável_  
Equivalências: _Não Aplicável_  
Justificativas: _Não Aplicável_

```ad-abstract
title: Definição.
Um sinal é um conjunto de dados ou informações de grandeza que varia em função de uma variável aleatória qualquer, geralmente processados por [[Sistemas|sistemas]].
Seja $x(t)$ uma função que descreve um sinal ao longo do tempo. A *energia* de $x(t)$ é dada por
$$E_x=\int_{-\infty}^{\infty}|x(t)|^2dt$$
A *potência* de $x(t)$ é dada por
$$P_x=\lim\limits_{T\to\infty}\bigg({1 \over T} \int_{-T/2}^{T/2}|x(t)|^2dt\bigg)$$
```
---
**Nota**.  A potência $P_x$ será *nula* caso $E_x$ seja *finita*. Do contrário, sendo $E_x$ *infinita*, $P_x$ será *finita*.
$$P_x=\begin{cases} 0,  & |E_x|\lt\infty \\
|\alpha|<\infty, & \verb!caso contrário!
\end{cases}$$
