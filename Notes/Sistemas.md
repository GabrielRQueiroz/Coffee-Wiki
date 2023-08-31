Tags: #Tipo/Definição #Tópico/Elétrica #Em_progresso

Tipos: [[Sistema linear invariante no tempo|SLIT]] 
Exemplos: _Não Aplicável_  
Construções: _Não Aplicável_  
Generalizações: _Não Aplicável_

Propriedades: _Não Aplicável_  
Suficiências: _Não Aplicável_  
Equivalências: _Não Aplicável_  
Justificativas: _Não Aplicável_

```ad-abstract
title: Definição.
Um sistema é um conjunto de expressões matemáticas que determinam o valor de *sinais de saída $y(t)$* a partir dos valores de *variáveis de entrada $x(t)$*.
Estas expressões podem representar, por exemplo, os efeitos de um algoritmo implementado por um processador digital, ou o modelo matemático de um filtro eletrônico, ou de um dispositivo mecânico. 

Pode ser representado da forma:

$$x(t)\to y(t)$$

ou em driagramas de blocos:

```tikz
\begin{document}
\begin{tikzpicture}[auto, node distance=3cm]

% Definindo os blocos
\node (input) {$x(t)$};
\node [draw, rectangle, minimum width=3.5cm, right of=input] (block1) { e.g. $y(t)=2x(t)$ };
\node (output) [right of=block1] {$y(t)$};

% Conectando os blocos
\draw [->] (input) -- (block1);
\draw [->] (block1) -- (output);

\end{tikzpicture}
\end{document}
```

