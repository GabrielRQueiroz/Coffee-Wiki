Tags: #Tipo/Proposição #Tópico/Cálculo #Em_progresso

Provas: [[Método de Newton-Raphson (tangente)|$\phi(x)=x-\frac{f(x)}{f'(x)}$]]
Referência: _Não Aplicável_
Justificativa: [[Teorema do ponto fixo de Brouler]]

Especializações: _Não Aplicável_
Generalizações: [[Ponto fixo]]

```ad-question
title: Proposição.
Seja $f:[a,\,b]\to \R$ contínua.
É descrita a equação $f(x)=0$ na forma equivalente
$$
f(\xi)=0 \iff \xi-\phi(\xi)=0 \iff \xi=\phi(\xi)
$$

Logo, $\xi$ é raiz de $f$ se, e somente se, $\xi$ é ponto fixo de $\phi$.

```tikz
\usepackage{pgfplots}

\begin{document}

\begin{tikzpicture}
% Define a função phi(x) e o intervalo [a, b]
\pgfmathdeclarefunction{phi}{1}{\pgfmathparse{0.5*#1 + 0.3}}  % Função genérica de exemplo
\def\a{0.2}
\def\b{0.8}

% Crie o gráfico
\begin{axis}[
    xlabel={$x$},
    ylabel={$y$},
    domain=0:1,         % Domínio do gráfico
    samples=100,        % Número de amostras para suavidade
    legend pos=north west,
    grid=both,
    ymin=0, ymax=1,
    xmin=0, xmax=1,
]

% Plote y = phi(x)
\addplot[yellow, smooth, thick] {phi(x)};

% Plote y = x
\addplot[orange, dashed, thick] {x};

% Marque o ponto de interseção
\addplot[mark=*, mark options={fill=red, scale=0.7}] coordinates {({phi(0.6)}, {phi(0.6)})} node[right] {Ponto Fixo};

% Adicione uma legenda
\legend{$y = \phi(x)$, $y = x$}

\end{axis}
\end{tikzpicture}

\end{document}
```
---

**Nota**. É necessária que $\Im(\phi) \subseteq \Dom(\phi)$ para que a iteração seja possível.

**Exemplo**. $x^2+x-6=0$
$$
\begin{align}
&f(x)=0\iff x^{2}+x-6=0 \iff x=6-x^{2}=\phi_{1}(x)
\end{align}
$$