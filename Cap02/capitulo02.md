##Representacion Numerica.

### 2.1.  Introdución.

*Desde hace tiempo el hombre en su vida diaria se expresa, comunica, almacenan información, la manipula, mediante letras y números. Para la representación numérica utiliza el sistema de representación decimal, en tanto que, dependiendo del idioma, dispone de un alfabeto que representa estas letras. Siguiendo el mismo principio que guía al hombre, las computadoras tienen su propio sistema de representación. Debido a su construcción basada fundamentalmente en circuitos electrónicos digitales, utiliza un sistema binario. Esto obliga a transformar a la representación binaria para que la maquina sea capaz de procesarlos.* 
Como veremos más adelante, tanto el sistema decimal como el binario están basados en los mismos principios. En ambos, la representación de un numero se afectúa por medio de cadenas de símbolos, los cuales representan una determinada cantidad dependiendo de cada símbolo y la posición que ocupa dentro de la cadena con respecto al denominado punto (o coma) decimal.  *
*Por cuestiones de índole técnica, los circuitos electrónicos que conforman una computadora suelen estar capacitados para reconocer señales eléctricas de tipo digital; por lo tanto, se hace necesario que los métodos de codificación internos tengan su origen en el sistema binario, y con ellos se pueda representar todo tipo de informaciones y ordenes que sean manejadas por la computadora.*
 *En los circuitos electrónicos suele representarse la presencia de tensión (electricidad) en un punto de un circuito por medio de un 1, en tanto que un 0 representa la ausencia de dicha tensión.*

## 2.2 Sistema de Numeracion

*Se denomina sistema de numeración al conjunto de simbolos y reglas que se utilizan para la representacion de datos numericos o cantidades. Un sistema de numeracion se caracteriza fundamentalmente por su base, que es el numero de simbolos distintos que utiliza y ademas es el coeficiente que determina cual es el valor de cada simbolo dependiendo de la posicion que ocupe.*
*Los sistemas de numeracion actuales son sistemas posicionales, en los que el valor relativo que representa cada simbolo o cifra de una determinada cantidad depende de su valor absoluto y de la posicion relativa que ocupa dicha con respecto a la coma decimal.*
##2.2.1. Teorema fundamental de la numeración
*Se trata de un teorema que relaciona una cantidad expresada en cualquier
sistema de numeración posicional con la misma cantidad expresada en el sistema
decimal. Supongamos una cantidad expresada en un sistema cuya base es B y
representamos por xi cada uno de los dígitos que contiene dicha cantidad, donde
el subíndice i indica la posición del dígito con respecto a la coma fraccionaria,
la posición se numera en forma creciente hacia la izquierda y decreciente hacia
la derecha de la coma (posición 0), en ambos casos de a 1.
El Teorema Fundamental de la Numeración dice que el valor decimal de una
cantidad expresada en otro sistema de numeración, está dado por la fórmula:
Número =
Xn
i=−m
(dígitoi) × (base)
i
(2.1)
donde el número en base B es . . . x4x3x2x1x0x−1x−2 . . . , o sea:
Número = x−m × B
−m + x−m+1 × B
−m+1 + · · · +
+ x−2 × B
−2 + x−1 × B
−1 + x0 × B
0 + x1 × B
1 + x2 × B
2 + · · · +
+ xn−1 × B
n−1 + xn × B
n
1 (2.2)*
##2.2.2. Sistemas decimal, binario y hexadecimal###
*El sistema que ha usado el hombre para contar desde hace bastante tiempo
es el denominado sistema decimal, adoptado por contar con los diez dedos de la
mano. El sistema decimal es uno de los denominados posicionales, que utiliza
un conjunto de 10 símbolos, xi0, 1, ..., 9. Un valor determinado o cantidad, que
se denomina número decimal, se puede expresar por la fórmula del Teorema 2.1,
donde la base es 10.*
###¿Cuál es la interpretación de la representación de la cantidad 3,1416?###
*Siguiendo el Teorema Fundamental de la Numeración, utilizando la base 10,
resulta*:
3, 1416 = 3 × 100 + 1 × 10−1 + 4 × 10−2 + 1 × 10−3 + 6 × 10−4
(2.3)

*El sistema binario es el sistema de numeración que utiliza internamente el
hardware de las computadoras actuales. La base o número de símbolos que
utiliza el sistema binario es 2, siendo los símbolos 0 y 1, los utilizados para la
representación de cantidades*.
*Utilizando el Teorema Fundamental de la Numeración*:
1001, 1(2 = 1 × 2
3 + 0 × 2
2 + 0 × 2
1 + 1 × 2
0 + 1 × 2
−1
(2.4)

*Al igual que los anteriores, el sistema hexadecimal es un sistema posicional
pero que utiliza dieciséis símbolos para la representación de cantidades. Estos
símbolos son los siguientes: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E y F; donde las
letras A, B, C, D, E y F equivalen a 10, 11, 12, 13, 14 y 15 del sitema decimal
respectivamente*.

###¿Qué número decimal representa el número hexadecimal 2CA?###
*Siguiendo el Teorema Fundamental de la Numeración:
2CA(16 = 2 × 162 + C × 161 + A × 160
(2.5)
2CA(16 = 2 × 162 + 12 × 161 + 10 × 160
(2.6)
2CA(16 = 512 + 192 + 10 = 714 (2.7)*

##2.2.3. Operaciones de Suma y Resta Binaria##
*Las operaciones aritméticas son similares a las del sistema decimal, con la
diferencia que se manejan sólo los dígitos 0 y 1. Al realizar la suma parcial de
dos dígitos, si el resultado excede el valor del máximo dígito (el 1) se debe pasar
el sobrante (denominado acarreo) a la suma parcial siguiente hacia la izquierda.
Sumemos los números binarios 100100 y 10110*
1 −→ carry
1 0 0 1 0 0
+ 1 0 1 1 0 =1 1 1 0 1 0

*En la resta binaria hay que tener en cuenta que al realizar las restas parciales
entre dos dígitos de idénticas posiciones, uno del minuendo y otro del sustraendo,
si el segundo excede al primero, se sustrae una unidad del dígito de más a la
izquierda en el minuendo –pedir prestado-. Si el dígito siguiente de la izquierda
es 0, se busca en los sucesivos teniendo en cuenta que su valor se multiplica por
dos a cada desplazamiento sucesivo a derecha.
Restemos los números binarios 111100 y 101010*
10 −→ borrow
1 1 1 ✁1 ✁0 0
- 1 0 1 0 1 0 = 0 1 0 0 1 0
 módulo = 10
 0 0 0 1 1 1 1 0 30(ca1


- *El primer bit es utilizado como bit de signo, si este es 0 el signo es positivo



- *El exponente se representa en exceso a 2





-  *Los restantes bits representan la fracción del número.*
*El rango de representación en punto flotante debe ser analizado teniendo en
cuenta los máximos y mínimos valores representables tanto con signo positivo
como negativo*:



- mínimo número negativo = −(mantisaMAX) × 
base exponente MAX


- máximo número negativo = −(mantisaM IN ) × base−exponenteMAX


- mínimo número positivo = mantisaM IN × base−exponenteMAX

- máximo número positivo = mantisaMAX × base exponente


- Caracteres alfabéticos

- Letras mayúsculas (A..Z sin la Ñ)

- Letras minúsculas (a..z sin la ñ)

- Cifras decimales: los números 0, 1, ..., 9

- Caracteres especiales

- Ordenes de control: Equivalen a las teclas enter, tabulación, esc, etc.


- 26 letras mayúsculas

- 10 cifras numéricas

- 28 caracteres especiales y de control