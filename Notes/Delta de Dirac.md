Tags: #Tipo/Definição #Tópico/Cálculo #Em_progresso

Tipos: _Não Aplicável_ 
Exemplos: [[Sinal impulso unitário]]  
Construções: [[Pente de Dirac|$\Sha_T(t)$]]  
Generalizações: _Não Aplicável_

Propriedades: _Não Aplicável_  
Suficiências: _Não Aplicável_  
Equivalências: [[Delta de Kronecker]]  
Justificativas: _Não Aplicável_

```ad-abstract
title: Definição.

No plano, a função $\delta$ tem valor *infinito* no ponto zero e *nulo* para todo o restante da reta. Sua integral em toda a reta é definida como tendo valor 1. 

$$\int_{-\infty}^{\infty}\delta(x)dx = 1$$
```tikz
\begin{document}
\begin{tikzpicture}
% Definição dos eixos
\draw[->] (-3,0) -- (3,0) node[right] {$x$};
\draw[->] (0,-0.5) -- (0,2) node[above] {$y$};

% Desenho da seta delta
\draw[->, thick] (0,0) -- ++(0,1) node[right] {$\delta(x)$};

% Linhas para representar os eixos x e y
\foreach \x in {-2,-1,1,2}
    \draw (\x,0.1) -- (\x,-0.1) node[below] {$\x$};
    
	\draw (0.1, 1) -- (-0.1, 1) node[left] {$1$};
	\draw (0.1, 0) -- (-0.1, 0) node[left, yshift="-10pt"] {$0$};
\end{tikzpicture}
\end{document}
```

---
**Nota**. A função $\delta$ pode ser deslocada ao longo da reta

---
**Nota**. Seja $H(x)$ a [[Função passo de Heaviside|função de Heaviside]]. A função $\delta$ pode ser definida por:
$$
\delta(x) = \frac{\partial H}{\partial x} (x) \iff H(x) = \int_{-\infty}^{x}\delta(t)dt
$$

