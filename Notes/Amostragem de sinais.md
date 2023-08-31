Tags: #Tipo/Proposição #Tópico/Elétrica #Em_progresso

Provas: _Não Aplicável_
Referência: [[Pente de Dirac]], [[Delta de Dirac]]
Justificativa: _Não Aplicável_

Especializações: _Não Aplicável_
Generalizações: _Não Aplicável_

```ad-question
title: Proposição.
Um sinal contínuo $x(t)$ pode ser converido em um sinal discreto $x[n]$ por meio da multiplicação do sinal contínuo por um [[Pente de Dirac|trem de impulsos unitários]] [[Impulso unitário|$\delta(t)$]] espaçados em intervalos regulares $T_s$:
$$
x[n] = x(t) \cdot \Sha_T(t)
$$

*Exemplo: *

```tikz
\usepackage{pgfplots} 

\begin{document}
\begin{tikzpicture}
\begin{axis}[
	xlabel={$t$},
    ylabel={$\sin(t)$},
    domain=-2*pi:2*pi, % Domínio de -2*pi a 2*pi (valores em radianos)
    samples=24,
    black,
    thick,
    width=12cm, % Largura do gráfico
    height=6cm, % Altura do gráfico
    axis lines=center, % Centralizar os eixos
    enlargelimits=false, % Evitar o aumento automático dos eixos
]
\addplot [ycomb, blue, mark=o] {sin(deg(x))};
\addplot [dashed] {sin(deg(x))}; % Plot da função seno pontilhada
\end{axis}
\end{tikzpicture}
\end{document}
```

