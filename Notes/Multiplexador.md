Tags: #Tipo/Definição #Tópico/Elétrica #Em_progresso

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

```tikz
\usepackage{tikz}
\usetikzlibrary{shapes, arrows, positioning}

\begin{document}
\begin{tikzpicture}

% Nodes for inputs D0, D1, D2, D3
\node (D0) at (-2, -0.5) {$D_{0}$};
\node (D1) at (-2, -1.5) {$D_{1}$};
\node (D2) at (-2, -2.5) {$D_{2}$};
\node (D3) at (-2, -3.5) {$D_{3}$};

% Nodes for control inputs S0 and S1
\node (S0) at (0.5, -5) {$S_{0}$};
\node (S1) at (1.5, -5) {$S_{1}$};

% Multiplexer rectangle
\draw (0,0) rectangle (2,-4);
\node[align=center] at (1, -0.5) {Multiplexer\\4:1};

% Control signal lines
\draw[->] (S0) -- (0.5, -4);
\draw[->] (S1) -- (1.5, -4);

% Input lines
\draw (D0.east) -- (0,-0.5);
\draw (D1.east) -- (0,-1.5);
\draw (D2.east) -- (0,-2.5);
\draw (D3.east) -- (0,-3.5);

% Output line
\draw (2, -2) -- (2.5, -2) node[right] {$F$};

\end{tikzpicture}
\end{document}
```

