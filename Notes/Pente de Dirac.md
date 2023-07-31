Tags: #Type/Definição #Topic/Cálculo #Em_progresso

Tipos: _Não Aplicável_ 
Exemplos: _Não Aplicável_  
Construções: [[Amostragem de sinais|$(\Sha_{T}\cdot x)(t)=\sum\limits_{k=-\infty}^{\infty}x(t)\delta(t-kT)$]]  
Generalizações: _Não Aplicável_

Propriedades: [[Série de Fourier do pente de Dirac|$\Sha_{T}(t)=\frac{1}{T}\sum\limits_{n=-\infty}^{\infty}e^{j2\pi n {t\over T}}$]], [[Transformada de Fourier do pente de Dirac|$\Fo\{\Sha_T\}={2\pi\over T}\sum\limits_{k=-\infty}^{\infty}\delta(\omega -k{2\pi\over T})$]]
Suficiências: _Não Aplicável_  
Equivalências: _Não Aplicável_  
Justificativas: _Não Aplicável_

```ad-abstract
title: Definição.
Também conhecido como **função sha**, **trem de impulsos** e **função de amostragem**, o pente de Dirac é uma distribuição feita a partir de [[Delta de Dirac|Deltas de Dirac]]:
$$
\Sha_{T}(t)= comb_T(t) := \sum\limits_{k=-\infty}^{\infty} \delta(t-kT), \, k\in\mathbb{Z}
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
