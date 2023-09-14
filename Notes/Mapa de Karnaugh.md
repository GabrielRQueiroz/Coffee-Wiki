Tags: #Tipo/Definição #Tópico/Elétrica #Em_progresso

Tipos: _Não Aplicável_ 
Exemplos: _Não Aplicável_  
Construções: _Não Aplicável_
Generalizações: _Não Aplicável_

Propriedades: [[Introdução de variável no mapa de Karnaugh|Variável introduzida]]  
Suficiências: _Não Aplicável_  
Equivalências: _Não Aplicável_  
Justificativas: _Não Aplicável_

```ad-abstract
title: Definição.

```tikz
\begin{document}

\begin{tikzpicture}[scale=0.7]
% Células do mapa de Karnaugh
\foreach \x in {0,1,2,3}
  \foreach \y in {0,1,2,3}
    \draw (\x,\y) rectangle (\x+1,\y+1);

\node[above] at (-0.5,4) {$AB \over CD$};

% Rótulos dos eixos
\foreach \x/\xbin in {0/00,1/01,2/11,3/10}
  \node[above] at (\x+0.5,4.2) {$\xbin$};
\foreach \y/\ybin in {0/00,1/01,2/11,3/10}
  \node[left] at (-0.2,\y+0.5) {$\ybin$};

% Termos nos quadrados
\node at (0.5,3.5) {$0$};
\node at (1.5,3.5) {$1$};
\node at (2.5,3.5) {$0$};
\node at (3.5,3.5) {$1$};

\node at (0.5,2.5) {$1$};
\node at (1.5,2.5) {$0$};
\node at (2.5,2.5) {$1$};
\node at (3.5,2.5) {$0$};

\node at (0.5,1.5) {$0$};
\node at (1.5,1.5) {$1$};
\node at (2.5,1.5) {$0$};
\node at (3.5,1.5) {$1$};

\node at (0.5,0.5) {$1$};
\node at (1.5,0.5) {$0$};
\node at (2.5,0.5) {$1$};
\node at (3.5,0.5) {$0$};

\end{tikzpicture}

\end{document}
```
e