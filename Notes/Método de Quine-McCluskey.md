Tags: #Tipo/Proposição #Tópico/Álgebra

Provas: _Não Aplicável_
Referência: _Não Aplicável_
Justificativa: _Não Aplicável_

Especializações: _Não Aplicável_
Generalizações: _Não Aplicável_

```ad-question
title: Proposição.

Método utilizada na minização de funções booleanas. É um método razoável para simplificar funções com mais de 4 variáveis de entrada.

1. Obter a expansão de mintermos (implicantes) da função $F$ na forma de tabela verdade;
2. Reduzir a quantidade de implicantes através de aplicações da relação $AB+A\overline{B}=A$;
3. Selecionar o conjunto mínimo de implicantes primos da lista dos implicantes que foi gerada, obtendo os **primos essenciais**;
4. Então, agrupar os implicantes de $F$ conforme a quantidade de dígitos *"1"* presentes;
5. Para cada linha do agrupamento de $i$ dígitos, buscar uma linha no grupo com $i+1$ que tenha **apenas** um termo diferindo;
	1. *ex.:* $A\overline{B}C\overline{D}+A\overline{B}CD = A\overline{B}C$ ou ($1010+1011 = 101\verb!x!$);
6. Listar implicantes primos em linhas em uma tabela cujas colunas são os mintermos de $F$. Então, mapear cada mintermo associado aos implicantes primos:
	1. Se um mintermo estiver associado a **um, e somente um** mintermo, este deve permanecer na forma simplificada final;
	2. Se um implicante primo estive associada aos exatos mesmos mintermos dos implicantes anteriormente definidos, ele é considerado redundante e é removido da forma final.
```

---

**Exemplo**. Dada a função $S$ representada pela soma de produtos $\sum m(2,\,3,\,5,\,7,\,8,\,10,\,13,\,15)$., para o mapa de Karnaugh
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
  \node[left] at (-0.2,3.5-\y) {$\ybin$};

% Termos nos quadrados

\node at (0.5,3.5) {$0$};
\node at (1.5,3.5) {$0$};
\node at (2.5,3.5) {$0$};
\node at (3.5,3.5) {$1$};

\node at (0.5,2.5) {$0$};
\node at (1.5,2.5) {$1$};
\node at (2.5,2.5) {$1$};
\node at (3.5,2.5) {$0$};

\node at (0.5,1.5) {$1$};
\node at (1.5,1.5) {$1$};
\node at (2.5,1.5) {$1$};
\node at (3.5,1.5) {$0$};

\node at (0.5,0.5) {$1$};
\node at (1.5,0.5) {$0$};
\node at (2.5,0.5) {$0$};
\node at (3.5,0.5) {$1$};

\end{tikzpicture}

\end{document}
```
	Etapa 1

| Mintermos | Binário | Número de 1's |
|---|---|---|
| |8 4 2 1| |
| 2 | 0 0 1 0 | 1 |
| 3 | 0 0 1 1 | 2 |
| 5 | 0 1 0 1 | 2 |
| 7 | 0 1 1 1 | 3 |
| 8 | 1 0 0 0 | 1 |
| 10 | 1 0 1 0 | 2 |
| 13 | 1 1 0 1 | 3 |
| 15 | 1 1 1 1 | 4 |

	Etapa 2

| Mintermo | Binário |
|---|---|
| 2 | 0 0 1 0 |
| 8 | 1 0 0 0 |
|---|---|
| 3 | 0 0 1 1 | 
| 5 | 0 1 0 1 |
| 10 | 1 0 1 0 |
|---|---|
| 7 | 0 1 1 1 |
| 13 | 1 1 0 1 |
|---|---|
| 15 | 1 1 1 1 |

	Etapa 3

| Agrupamento | Primo implicante |
|---|---|
|$T_{0} \to 2,3$| 0 0 1 x |
|$T_{1} \to 2,10$| x 0 1 0 |
|$T_{2} \to 8,10$| 1 0 x 0 |
|$T_{3} \to 3,7$| 0 x 1 1 |
|$T_{4} \to 5,7$| 0 1 x 1 |
|$T_{5} \to 5,13$| x 1 0 1 |
|$T_{6} \to 7,15$| x 1 1 1 |
|$T_{7} \to 13,15$| 1 1 x 1 |

**Melhorando agrupamentos**:

| Agrupamento | Primo implicante |
|---|---|
|$T_{0} \to 2,3$| 0 0 1 x |
|$T_{1} \to 2,10$| x 0 1 0 |
|$T_{2} \to 8,10$| 1 0 x 0 |
|$T_{3} \to 3,7$| 0 x 1 1 |
|$T_{4} \to 5,7,13,15$| x 1 x 1 |

	Etapa 4

| Implicantes | 2 | 3 | 5 | 7|8|10|13|15|
|---|--- |--- |--- |---|---|---|---|---|
|(2,3)| x | x |--- |---|---|---|---|---|
|(2,10)| x |--- |--- |---|---| x |---|---|
|(8,10)|--- |--- |--- |---| x | x |---|---|
|(3,7)|--- | x |---| x |---|---|---|---|
|(5,7,13,15)|--- |--- | x | x |---|---| x | x |

- Os mintermos **5, 8 e 15** compõem apenas um implicante primo. Logo, esses implicantes *permanecem* na forma final: $(8,\,10),\;(5,\,7,\,13,\,15).$ 
- Sabendo os implicantes acima, temos que os implicantes $(2,\,10)$ e $(3,\,7)$ podem ser *removidos* da forma final.
- Resta somente o implicante $(2,\,3)$, que também pode compor a forma final:
$$
S=(2,\,3)+(8,\,10)+(5,\,7,\,13,\,15)=\overline{A}\,\overline{B}C+A\overline{B}\,\overline{D}+BD
$$