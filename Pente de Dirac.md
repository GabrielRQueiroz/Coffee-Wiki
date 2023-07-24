Tags: #Type/Definição #Topic/Cálculo #Em_progresso

Tipos: _Não Aplicável_ 
Exemplos: _Não Aplicável_  
Construções: [[Amostragem de sinais]]  
Generalizações: _Não Aplicável_

Propriedades: _Não Aplicável_  
Suficiências: _Não Aplicável_  
Equivalências: _Não Aplicável_  
Justificativas: _Não Aplicável_

```ad-abstract
title: Definição.
Também conhecido como **função sha**, **trem de impulsos** e **função de amostragem**, o pente de Dirac é uma distribuição feita a partir de [[Delta de Dirac|Deltas de Dirac]]:
$$
\Sha_{T}(t)= comb(t) := \sum\limits_{k=-\infty}^{\infty} \delta(t-kT), \, k\in\mathbb{Z}
$$

```tikz
\usepackage{pgfplots} 

\begin{document}
\begin{tikzpicture}
\begin{axis}[
    samples=9,
    ymax=1.5,
    ymin=0,
    xmax=4.5,
    xmin=-4.5,
    yticklabels={},
    xtick={-4,-3,-2,-1,0,1,2,3,4}, 
    xticklabels={-4T,-3T,-2T,-T,0,T,2T,3T,4T},
    ycomb,
    thick,
    width=12cm, % Largura do gráfico
    height=6cm, % Altura do gráfico
]

% Plot dos deltas de Dirac com as coordenadas ajustadas
\addplot+[mark=triangle, black] coordinates {(-4,1) (-3,1) (-2,1) (-1,1) (0,1) (1,1) (2,1) (3,1) (4,1)};

\end{axis}

\end{tikzpicture}
\end{document}
```
---
**Nota**. Como o pente de Dirac é uma função *periódica*, ela pode ser representada como uma [[Série de Fourier|série de Fourier]] por meio da soma de exponenciais complexas:
$$
\Sha_T(t)={1\over T}\sum\limits_{n=-\infty}^{\infty}e^{2\pi jn\frac{t}{T}}
$$

<center>
	<img src="https://public.dm.files.1drv.com/y4m1HWYiHtipBUvcyqtk-5tmP5IssyL451cPt-wGYkG9MwcjpjEyJN-xjJCvU6-5V_w5nIMMv4JGOXr2skdKZ6FGN0PBsMW2haiJRStn3cEyy-vZEct79D_aoNOQScWTL241YdaYzoYr-K6mUSMyndBIDRR8LxWB7rciRry5b8cmFFdS34zzJ5TXEYAYD61ekILLxfsiqRSwQ8K3K4Z4WQQv9Ws1GfQ09K2mfkJHTj_LUQ"  width="50%" height="260" />
</center>
