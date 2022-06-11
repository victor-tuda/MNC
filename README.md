#### To-do
* Implementar o código do método MMQ
* Melhorar a representação gráfica da Dicotomia
* Implementar o README de Lagrange
* Implementar o README da Regra dos Trapézios

# Métodos Numéricos Computacionais
Repositório destinado a automatizar e representar gráficamente os seguintes métodos matemáticos:
* Dicotomia
* Forma de Lagrange
* Regra dos Trapézios
* Método dos Mínimos Quadrados (MMQ)

## Método da Dicotomia ou Bissecção
Utilizamos a dicotomia, para encontrar o valor 0 da função, para equações com grau elevado.

Por exemplo, uma função como f(x)=x³+4x²-10, podemos utilizar o método da Dicotomia para encontrar as raízes mais facilmente.

São três requisitos para utilizar o método numérico da Dicotomia:
* Equação a qual se deseja se extrair a raiz.
* Intervalo, valor máximo e mínino onde a raiz da equação se encontra.
* Precisão, erro tolerável.

Em seguida, seguir as etapas:
1. Obter um intervalo (a, b) onde exista uma raiz para a função dada.
2. Dividir o intervalo em duas partes iguais, calculando o ponto médio m, dado por: m = (a + b) / 2.
3. A partir de f(x) calcular f(a), f(b) e f(m).
4. Verificar em qual das metades está a raiz: Se f(a) * f(m) < 0, a raiz está entre a e m. Se f(b) * f(m) < 0, a raiz está entre b e m.
5. Verificar se o processo iterativo deve continuar: Verificar f(m) = 0 ou |f(m)| <= precisão.

Características da Dicotomia:
* Permite isolar raízes.
* Possui baixa velocidade de convergência, mas a convergência é garantida.
* É simples.
* Possui alto custo computacional
