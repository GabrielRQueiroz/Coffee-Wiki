Tags: #Tipo/Definição #Tópico/Elétrica #Em_progresso

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

$$
 \overline{(A \oplus B)} = \overline A \overline B + AB
$$

```tikz  
\usepackage{circuitikz}
\begin{document}
\begin{tikzpicture}
    \draw (0,0) node[xnor port] (xnor) {};
    \draw (xnor.in 1) -- ++(-1,0) node[left] {$A$};
    \draw (xnor.in 2) -- ++(-1,0) node[left] {$B$};
    \draw (xnor.out) -- ++(1,0) node[right] {$\overline{(A \oplus B)}$};
\end{tikzpicture}
\end{document}

```
