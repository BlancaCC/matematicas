# Relación de ejercicios I

Nota: Ejercicion incompleto y mal en el ajuste, aún no tocar
## Ejercicio 5 
En un hospital están estudiando la cantidad en sangre (medida en cc.) de un cierto fármaco que se administra una
vez cada cuatro horas. Se sabe experimentalmente que durante cada periodo de cuatro horas el cuerpo elimina una
cierta fracción p no nula del medicamento en sangre. Se pide
a) Describa con una ecuación en diferencias el modelo anterior, esto es, modele la cantidad del fármaco en sangre
en cada periodo.
b) Calcule la solución de la ecuación en diferencias anterior.
c) ¿Existe un punto de equilibrio?
d ) Determine asintóticamente la cantidad del fármaco en sangre.
e) Si la fracción eliminada por el cuerpo es p = 0,8, determine la cantidad de fármaco que se debe admisistrar cada 
4 horas para que la concentración converja hacia 6cc. 

### Solución   

a) Notación usada en el modelo: 
- Sea F una cantidad fija del fármaco que se administra cada cuatro horas. 
- $Xn_n $ cantidad del medicamento en sangre, donde n es un múltimo de cuatro. 
- p fracción del medicamento en sangre que se anula cada cuatro horas. 

El modelo que describe esta situación es: $X_{n+1} = F + (1-p)X_n$
Es una recorencia no homgénea lineal de orden 1

b) Solución a la recurrencia anterior: 
Una ecuación no homogénea lineal se puede expresar de la siguiente manera: 
$ X_n = Z_n + X^* $
Donde $Z_n$ es la homogénea asociada y $X*$ es la solución contante

$Z_{n+1} = (1-p)Z_n$ una progresión geométrica cuya solución es $Z_n = (1-p)^n K$,
k es una constante cuyo valor está por determinar. 

$X^* = F + (1-p)X^* $  despejando $ X* = \frac ^F_{p-1}$
En difinitiva la solución general es de la forma $Xn = (1-p)^n K +  \frac ^F_{p-1} $
Para calcula la ecuación particular partamos a que en el instante 0 se ha indectado por primera vez el medicamento
la cantidad de medicamento es F $X_0 = k +\frac ^F_{p-1} = F \Rightarrow k = F+ \frac ^F_{1-p}  $

Solución particular : $X_0 = (1-p)^n (F+ \frac ^F_{1-p})  +\frac ^F_{p-1}$


c y d) Existencia punto de equilibrio y cantidad de fármaco asintóticamente.
- Caso p < 1
Ecuación estríctamante mónótoma, para que hubiera un punto de equilibrio debería de en algún momento ser constante, diverge positivamente. 
- Caso p >= 1
No tendría sentido el modelo propuesto, ya que tomaría valores negativos, lo que pondrá de manifiesto que el medicamento
se ha eliminado antes que la nueva administración del medicamento. 
Teóricamente con la ecuación dada divergería negativamente o se mantendría constante en $F+ \frac ^F_{1-p})$

e)

 



