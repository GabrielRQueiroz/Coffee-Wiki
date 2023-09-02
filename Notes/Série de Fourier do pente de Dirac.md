Tags: #Tipo/Proposição #Tópico/Cálculo 

Provas: _Não Aplicável_
Referência: _Não Aplicável_
Justificativa: _Não Aplicável_

Especializações: _Não Aplicável_
Generalizações: _Não Aplicável_

```ad-question
title: Proposição.
Seja $\Sha_T$ um [[Pente de Dirac|pente de Dirac]] de período $T$. Dado que $\Sha_T(t)$ é uma função periódica, então
$$
\Sha_T(t)={1\over T}\sum\limits_{n=-\infty}^{\infty}e^{2\pi jn\frac{t}{T}}
$$
é a sua série de Fourier.
```
---
***Prova***. Seja evidente que $\Sha_T(t)$ é periódica com período $T$, ou seja
$$\Sha_T(t+T)=\Sha_{T(t),}\,\forall t.$$
A [[Série de Fourier|série complexa de Fourier]] para tal função periódica é definida por
$$\Sha_T(t)=\sum\limits_{n=-\infty}^{\infty}c_{n}e^{j2\pi n {t\over T}},$$
onde os *coeficientes de Fourier* são dados por
$$
\begin{align}
\begin{aligned}
c_{n}&={1\over T}\int_{t_0}^{t_0+T}\Sha_T(t)e^{-j2\pi n {t\over T}}dt \quad (-\infty\lt t_{0}\lt +\infty)
\\\\
&= {1\over T} \int_{-{T\over 2}}^{{T\over 2}}\Sha_T(t)e^{-j2\pi n {t\over T}}dt
\\\\
&= {1\over T} \int_{-{T\over 2}}^{{T\over 2}}\delta(t) e^{-j2\pi n {t\over T}}dt
\\\\
&={1\over T}e^{-j2\pi n {0\over T}}
\\\\
&={1\over T}.
\end{aligned}
\end{align}
$$
Logo, todos os coeficientes de Fourier são $\frac{1}{T}$ resultando em
$$\Sha_{T}(t)=\frac{1}{T}\sum\limits_{n=-\infty}^{\infty}e^{j2\pi n \frac{t}{T}}$$

---

**Nota**. Foi considerada a frequência $f=\frac{1}{T}$ expressa em $Hz$, porém uma análise com a frequência $\omega = \frac{2\pi}{T}$ em $rad/s$ é **equivalente**.