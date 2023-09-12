Tags: #Tipo/Definição #Em_progresso

Tipos: _Não Aplicável_ 
Exemplos: _Não Aplicável_  
Construções: _Não Aplicável_  
Generalizações: _Não Aplicável_

Propriedades: _Não Aplicável_  
Suficiências: _Não Aplicável_  
Equivalências: _Não Aplicável_  
Justificativas: _Não Aplicável_

```ad-abstract
title: Definição.
Sistema de referenciamento que permite a localização de um ponto qualquer em um espaço de formato esférico através das coordenadas $(r,\,\theta,\,\phi)$.

- A *distância radial* $r$ é a distância Euclidiana do ponto $P$ à origem $O$;
- O *azimute* $\theta$ é o ângulo entre a direção azimutal de referência à projeção ortogonal do segmento de linha $OP$ no plano $xy$;
- A *inclinação* (ou ângulo polar) $\phi$ é o ângulo entre a direção zênite e o segmento de linha $OP$,
onde:

$
\begin{align}
x &= r\sin\phi\cos\theta
\\y &= r\sin\phi\sin\theta
\\z &= r\cos\phi
\\r &= \sqrt{x^2+y^2+z^2}
\end{align}
$

```tikz
\usepackage{tikz-3dplot}

\begin{document}

\usetikzlibrary{angles,quotes}

\tdplotsetmaincoords{50}{105} % Define os ângulos de visão

\begin{tikzpicture}[scale=2,tdplot_main_coords]

\coordinate (A) at (0.5,0,0);
\coordinate (O) at (0,0,0);
\coordinate (B) at (0.5,0.5,0);
\coordinate (P) at (1,1,2);
\coordinate (C) at (0.5,0.5,1);
\coordinate (D) at (0,0,0.5);
% Eixos
\draw[->] (0,0,0) -- (2,0,0) node[left]{$x$};
\draw[->] (0,0,0) -- (0,2,0) node[right]{$y$};
\draw[->] (0,0,0) -- (0,0,2) node[above]{$z$};

% Pontos de origem
\draw (0,0,0) node[anchor=east]{$O$};

% Ponto (1,1,1)
\draw[fill] (P) circle [radius=0.1];
\draw (P) node[above right] {$P$};

\draw[dashed] (1,1,0) -- (P);
\draw[dashed] (1,1,0) -- (O);
\draw[solid] (O) -- (P);
\draw (0.5,0.5,1) node[right] {$r$};

% Ângulo \theta
\pic [draw, -, black, angle eccentricity=1.5, "$\theta$"] {angle = A--O--B};

% Ângulo \phi
\pic [draw, -, black, angle eccentricity=1.5, "$\phi$"] {angle = C--O--D};

\end{tikzpicture}

\end{document}
```
