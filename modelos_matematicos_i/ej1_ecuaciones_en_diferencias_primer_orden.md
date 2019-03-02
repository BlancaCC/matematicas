# Relación de ejercicios I, Ecuaciones en diferencias

## Ejercicio 5 
En un hospital están estudiando la cantidad en sangre (medida en cc.) de un cierto fármaco que se administra una vez cada cuatro horas. Se sabe experimentalmente que durante cada periodo de cuatro horas el cuerpo elimina una cierta fracción p no nula del medicamento en sangre. Se pide: 

a) Describa con una ecuación en diferencias el modelo anterior, esto es, modele la cantidad del fármaco en sangre en cada periodo.
b) Calcule la solución de la ecuación en diferencias anterior.
c) ¿Existe un punto de equilibrio?
d ) Determine asintóticamente la cantidad del fármaco en sangre.
e) Si la fracción eliminada por el cuerpo es p = 0,8, determine la cantidad de fármaco que se debe admisistrar cada  horas para que la concentración converja hacia 6cc. 

### Solución   

a) Notación usada en el modelo: 
- Sea F una cantidad fija del fármaco que se administra cada cuatro horas. 
- $X_n $ cantidad del medicamento en sangre, donde n representa que han pasado 4n horas desde el primer suministro del medicamento. 
- p fracción del medicamento en sangre que se anula cada cuatro horas. 

El modelo que describe esta situación es: $X_{n+1} = F + (1-p)X_n$
Es una recurrencia lineal no homgénea  de orden 1.

b) Solución a la recurrencia anterior: 
Una ecuación no homogénea lineal se puede expresar de la siguiente manera: 
$ X_n = Z_n + X* $
Donde $Z_n$ es la homogénea asociada y $X*$ es la solución contante

$Z_{n+1} = (1-p)Z_n$ una progresión geométrica cuya solución es $Z_n = (1-p)^n K$,
k es una constante cuyo valor está por determinar. 

$X* = F + (1-p)X* $  despejando $ X* = \frac{F}{p}$
En difinitiva la solución general es de la forma $Xn = (1-p)^n K +  \frac {F}{p } $
Para calcula la ecuación particular partamos de que en el instante 0 se ha indectado por primera vez el medicamento, es decir, su cantidad en sangre es F , despejando de aquí la incógnita: 
$X_o = k +\frac{F}{p} = F \Rightarrow k = \frac {F (p-1)}{p}  $

Solución particular : $X_n = (1-p)^n (\frac {F (p-1)}{p}  )  +\frac{F}{p}$


c y d) Existencia punto de equilibrio y cantidad de fármaco asintóticamente.
- Caso 0< p < 1
Ecuación estríctamante mónótoma, para que hubiera un punto de equilibrio debería de en algún momento ser constante, el límite cuando tiende a infinito es $\frac{F}{p}$. 
- Caso p > 1
Esto sería indicatico de que el midicamento se ha eliminado antes de volverlo a aplicar al paciente. 
Teóricamente podría haber momentos en los que el fármaco en sangre sean negativos, esto sería indicativo de que si se le hubiera suministrado más fármaco, este hubiera sido eliminado. 

El modelo propuesto no sería muy adecuado. 

- F < 0  o p < 0
Son casos que carecen de mucho sentido real. 

e) Cantidad suministrada para que converja hacia 6cc

Por el primer caso esplicado vemos que converge hacia $ \frac{F}{p}$ dado p=0.8 sólo quedaría despejar F:
$F = 4.8 cc$

Resultado el fármaco aplicado debería de ser $F = 4.8 cc$

 
## Ejercicio 8 

Para una explotación agrícola con abundancia de cereales se sabe que un número excesivo de cierta especie de aves resulta nocivo pero puede ser beneficioso en un número adecuado (como control de plagas). Se ha observado que,en ausencia de restricciones, la población de aves sigue un modelo de Malthus con tasa de crecimiento $\alpha$ = 0,5; es  decir, P_{n+1} = (1 + \alpha )P_n , n = 0, 1, . . .
siendo $P_n$ el número de aves en el recuento n (dado en cientos). Si no se establecen limitaciones, la población presentará un aumento que afectará negativamente a la explotación agrícola por lo que se toman medidas correctoras mediante la colocación de trampas por toda la explotación que permitan un control adecuado del tamaño de la población. De esta forma la tasa de  recimiento de la población pasa a ser del tipo:
$ \alpha = \alpha(P_n ) = 0,5 + \beta(1 − P_n ) $ con $ \beta > 0$ .
Se pide:
a) Bajo las medidas correctoras, deduzca la ecuación en diferencias que modela la dinámica de la población y calcule sus puntos de equilibrio.
b) Analice la estabilidad de los puntos de equilibrio según los valores de $\beta$.
c) Para $P_0 > 0 $ cualquiera, determine los valores de $\beta$ para los que la población no se extingue y se aproxima, a largo plazo, a un número no superior a 300 aves.

### Solución 
a) Modelo y puntos de quilibrio 
El modelo que se nos presenta se corresponde con el modelo de Verhulst, por tanto 
$ \frac{P_{n+1}- P_n}{P_n} = 0,5 + \beta(1 − P_n ) $, 
alcanzará un punto de equilibrio cuando $ \frac{P_{n+1}P_n}{P_n} = 0$ despejando, el miembro derecho resulta que alcancanza un punto de quilibrio en: 

$P_n = \frac{ 0,5 + \beta}{\beta}$ y la constantemente 0.

(¿Si se multuplicara por $P_n$ en ambos miembros, la solución cuadrática tendría las mismas soluciones?)


b) Analice la estabilidad de los puntos de equilibros según $\beta$

