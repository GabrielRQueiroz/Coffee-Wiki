Tags: #Tipo/Definição #Tópico/Elétrica

Tipos: _Não Aplicável_ 
Exemplos: _Não Aplicável_  
Construções: _Não Aplicável_  
Generalizações: _Não Aplicável_

Propriedades: [[Princípio da superposição|$\alpha x_1(t)+\beta x_2(t)\to \alpha y_1(t)+\beta y_2(t)$]], [[Teorema da convolução|$\Fo\{f*g\}=\Fo\{f\}\cdot\Fo\{g\}$]]  
Suficiências: _Não Aplicável_  
Equivalências: _Não Aplicável_  
Justificativas: _Não Aplicável_

```ad-abstract
title: Definição.

A *invariância no tempo* implica simplesmente que a definição das operações dos blocos **não pode mudar ao longo do tempo**. As expressões das funções equivalentes dos blocos só podem depender das variáveis de entrada, e nunca do tempo.

A *linearidade* dos sistemas implica que todas operações utilizadas no processamento dos sinais de entrada serão **lineares**. Ou seja, qualquer sistema linear pode ser decomposto nos seguintes blocos de processamento:
- Soma de sinais;
- Deslocamento no tempo;
- Multiplicação de um sinal por um escalar;
- Derivação de um sinal (variável) em relação ao tempo;
- Integração de um sinal (variável) em relação ao tempo.
```
---
**Nota**. A resposta ao impulso $\delta(t)$ de um sistema o caracteriza completamente, e seu sinal de saída é igual a seu sinal de entrada [[Convolução|convoluído]] por sua resposta a impulso.

---
**Nota**. Dadas duas respostas em frequência de dois sistemas, $H_1(\omega)$ e $H_2(\omega)$, se ligarmos a saída de um na entrada do outro, a resposta total em frequência do sistema será dada pela *multiplicação* das duas respostas:
$$
H_{total}(\omega)=H_1(\omega)\times H_2(\omega)
$$