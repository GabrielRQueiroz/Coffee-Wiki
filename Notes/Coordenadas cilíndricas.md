Tags: #Tipo/Definição #Tópico/Álgebra #Em_progresso

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
Sistema composto por um subsistema polar na base de um cilindro circular, de coordenadas $(\rho,\,\phi,\,z)$.

- A *distância radial* $\rho$ é a distância Euclidiana do ponto $P$ ao eixo $z$;
$$
\rho = \sqrt{x^{2}+y^{2}}\iff x=\rho\cos(\phi)
$$
- O *azimute* $\phi$ é o ângulo entre a direção de referência do plano $xy$ e a linha que liga a origem à projeção de $P$ em $xy$;
$$
\phi = \tan^{-1}\bigg\{\frac{y}{x}\bigg\} \iff y=\rho\sin(\phi)
$$
- A *coordenada axial* z é a altura do ponto ao plano $xy$.
$$
z=z
$$

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
% Eixos
\draw[->] (0,0,0) -- (2,0,0) node[left]{$x$};
\draw[->] (0,0,0) -- (0,2,0) node[right]{$y$};
\draw[->] (0,0,0) -- (0,0,2) node[above]{$z$};

% Pontos de origem
\draw (0,0,0) node[anchor=east]{$O$};

% Ponto (1,1,1)
\draw[fill] (P) circle [radius=0.1];
\draw (P) node[above right] {$P$};

\draw[dashed] (1,1,0) -- (0,0,0);
\draw (0.5,0.5,0) node[right] {$\rho$};
\draw[dashed] (1,1,0) -- (P);

% Ângulo \phi
\pic [draw, -, black, angle eccentricity=1.5, "$\phi$"] {angle = A--O--B};

\end{tikzpicture}

\end{document}
```
