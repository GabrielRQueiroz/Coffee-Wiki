Tags: #Type/Definição #Topic/Cálculo #Em_progresso

Tipos: _Não Aplicável_ 
Exemplos: [[Sinal degrau unitário]]  
Construções: _Não Aplicável_  
Generalizações: _Não Aplicável_

Propriedades: _Não Aplicável_  
Suficiências: _Não Aplicável_  
Equivalências: _Não Aplicável_  
Justificativas: _Não Aplicável_

```ad-abstract
title: Definição.

A função passo de Heaviside, ou passo unitário, geralmente denotada por $H$ ou $\theta$, tem valor *zero* para argumentos negativos e *um* para argumentos positivos e é definida como:

$$
H(x):=\begin{cases}
1, & x\geq 0 \\
0, & x\lt 0
\end{cases}
$$


```tikz
\begin{document}
\begin{tikzpicture}
% Definição dos eixos (com alcance reduzido em 1 unidade)
\draw[->] (-3,0) -- (3,0) node[right] {$x$};
\draw[->] (0,-0.5) -- (0,2) node[above] {$y$};

% Desenho da função degrau de Heaviside
\draw[-, thick] (-3,0) -- (0,0);
\draw[-, thick] (0,1) -- (3,1);

% Linha vertical pontilhada com ponto no centro
\draw[dashed] (0,0) -- (0,1);
\draw[fill=white] (0,0.5) circle (2pt);

% Linhas para representar os pontos no eixo x
% \foreach \x in {-2,-1,1,2}
%     \draw (\x,0.1) -- (\x,-0.1) node[below] {$\x$};

% Marcador para os pontos no eixo y
\draw (0.1,1) -- (-0.1,1) node[left] {$1$};
\draw (0.1,0) -- (-0.1,0) node[left, yshift="-10pt"] {$0$};
\end{tikzpicture}
\end{document}
```

**Nota**. Seja $\delta(x)$ a [[Delta de Dirac|função de delta de Dirac]]. A função $H(x)$ pode ser definida por:
$$
H(x) = \int_{-\infty}^{x}\delta(t)dt \iff \delta(x) = \frac{\partial H}{\partial x} (x)
$$
---
**Nota**. No contexto da [[Probabilidade e estatística|probabilidade e estatística]], a função de Heaviside é a [[Função distribuição acumulada|função distribuição acumulada]] (FDA) de uma [[Variáveis aleatórias|variável aleatória]], cujo valor é quase certamente ([q.c.](https://pt.wikipedia.org/wiki/Quase_certamente)) 0.