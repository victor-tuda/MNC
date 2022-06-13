#### To-do
* Implementar o código do método MMQ
* Melhorar a representação gráfica da Dicotomia
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

## Método da Forma de Lagrange
Utilizamos a forma de Lagrange para encontrar um valor que não está tabelado, a partir de uma tabela, e sem ter informações sobre a função que gerou a tabela.

Por exemplo:<br>
Obtem-se uma tabela relacionando a temperatura em ºC (T) e o calor específico da água (C).
| T | 20      | 25      | 30      | 35      | 40      | 45      |
|---|---------|---------|---------|---------|---------|---------|
| C | 0.99907 | 0.99852 | 0.99826 | 0.99818 | 0.99828 | 0.99849 |

Torna-se necessário saber:
* Qual a temperatura da água a 35.5ºC?
* Qual temperatura corresponde ao calor específico de 0,99837?

Para responder essas perguntar, iremos utilizar o método de interpolação polinomial de Lagrange:<br>
![image](https://user-images.githubusercontent.com/63505187/173398817-b2e65e2b-25f9-4fbb-801c-fd1f887fc8eb.png)<br>
![image](https://user-images.githubusercontent.com/63505187/173399175-49af69a8-3b99-4c87-bf9d-89d51b3851fa.png)

Exemplo da forma de Lagrange em uma interpolação para 2 pontos:<br>
![image](https://user-images.githubusercontent.com/63505187/173400169-717888bd-ac9a-4c0c-ad65-64085c532b97.png)<br>
Onde:<br>
![image](https://user-images.githubusercontent.com/63505187/173400732-1ff8bb35-96f1-474d-a8b6-d4b3c7b03c0e.png)

Exemplo da forma de Lagrange em uma interpolação para 3 pontos:<br>
![image](https://user-images.githubusercontent.com/63505187/173400970-6c7bf42b-3c74-491a-8d9c-31bc3d3454d0.png)<br>
Onde:<br>
![image](https://user-images.githubusercontent.com/63505187/173401059-6d049dbc-f3d2-415f-bd82-86623f42434f.png)<br>







