Tags: #Tipo/Definição #Tópico/Elétrica #Em_progresso

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

O decodificador é um componente que transforma um código binário de entrada de $N$ bits em $M$ linha de saída (onde $N$ pode ser qualquer inteiro e $M$ é um inteiro menor ou igual a $2^{N}$), de modo que a saída será ativada por uma única combinação das possíveis entradas.

| $x_{0}$ | $x_{1}$ | $x_{2}$ | Enable | $m_{0}$ | $m_{1}$ | $m_{2}$ | $m_{3}$ | $m_{4}$ | $m_{5}$ | $m_{6}$ | $m_{7}$ |
|---|---|---|--------|---|---|---|---|---|---|---|---|
| 0 | 0 | 0 |   1    | 1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 |   1    | 0 | 1 | 0 | 0 | 0 | 0 | 0 | 0 |
| 0 | 1 | 0 |   1    | 0 | 0 | 1 | 0 | 0 | 0 | 0 | 0 |
| 0 | 1 | 1 |   1    | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 0 |
| 1 | 0 | 0 |   1    | 0 | 0 | 0 | 0 | 1 | 0 | 0 | 0 |
| 1 | 0 | 1 |   1    | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 0 |
| 1 | 1 | 0 |   1    | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 |
| 1 | 1 | 1 |   1    | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 |
| x | x | x |   0    | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |

- O Enable é uma entrada que controla a ativação do componente, de modo que $E=0$ implique na 

```tikz
\usetikzlibrary{shapes,arrows,calc,arrows.meta}
\usepackage{circuitikz}
\usetikzlibrary{circuits.logic.IEC,calc}

\begin{document}
\begin{circuitikz}[circuit logic IEC]

% Decoder with Enable input
\node[and gate, inputs={nnnn}, and gate IEC symbol={Decoder 3:8}, text height=6cm, text width=4cm] (A) {};

% Inputs A, B, C, and Enable (E)
\foreach \V/\X in {1/x_{0}, 2/x_{1}, 3/x_{2}, 4/E}
{
  \draw ([xshift=-10pt]A.input \V) node[left] {$\X$} -- (A.input \V);
}

% Output lines
\foreach \C/\B in {0.111/m_{7}=111, 0.222/m_{6}=110, 0.333/m_{5}=101, 0.444/m_{4}=100, 0.555/m_{3}=011, 0.666/m_{2}=010, 0.777/m_{1}=001, 0.888/m_{0}=000}
{
  \draw ($ (A.south east)!\C!(A.north east) $) -- ++(10pt,0) node[left,xshift=-10] {$\B$};
}

\end{circuitikz}
\end{document}
```

