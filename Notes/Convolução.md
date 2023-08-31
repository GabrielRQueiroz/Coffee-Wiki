Tags: #Tipo/Definição #Tópico/Cálculo #Em_progresso

Tipos: _Não Aplicável_  
Exemplos: _Não Aplicável_  
Construções: _Não Aplicável_  
Generalizações: _Não Aplicável_

Propriedades: [[Teorema da convolução|$\Fo\{f*g\}=\Fo\{f\}\cdot\Fo\{g\}$]]  
Suficiências: [[Função absolutamente integrável|$f(x)$ e $g(x)$ devem ser absolutamente integrável nos intervalos $[-\infty,\,0]$, $[0,\,\infty]$ ou $[-\infty,\,\infty]$]]  
Equivalências: _Não Aplicável_  
Justificativas: _Não Aplicável_

```ad-abstract
title: Definição.

**Convolução** é um *operador linear* que, a partir de duas funções dadas, resulta numa terceira que mede a soma do produto dessas funções ao longo da região subentendida pela superposição delas em função do deslocamento existente entre elas.

A notação para a convolução de $f$ e $g$ é $f * g$. Sejam $x$ a variável independente e $u$ o deslocamento, a fórmula é definida pela integral:
$$
(f*g)(x)=h(x)=\int_{-\infty}^{\infty}f(u)\cdot g(x-u) \, du
$$

O resultado gráfico da convolução é o seguinte:
<center>
	<img src="https://upload.wikimedia.org/wikipedia/commons/b/b9/Convolution_of_spiky_function_with_box2.gif" width="40%" height="100px" />
	<img src="https://upload.wikimedia.org/wikipedia/commons/6/6a/Convolution_of_box_signal_with_itself2.gif" width="40%" height="100px" />
</center>
```
