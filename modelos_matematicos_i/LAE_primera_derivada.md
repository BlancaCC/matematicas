# Teorema Estabilidad asíntotica local

No me termina de convencer la demostración.
La cota no me gusta y la forma de buscar el epsilón tampoco. 

Propuesta-> Definir suceisión que vaya tomando el mínimo, los intercalos cerrados y acotado son compactos alcanza el mínimo. 
## Enunciado 
Si $\alpha$ es un punto de equilibrio del SDD {I,f} y f es derivable en I entonces: 
1. Si $|f'(\alpha)|<1$ entonces $\alpha$ es localmente asintóticamente estable.  
2. Si $|f'(\alpha)| > 1$ entonces $\alpha$ es inestable. 

(Nótese que este teorema no especifica que pasa para los casos que $\alpha$ sea 1 o -1)

## Demostración caso 2 

Se quiere ver que $\alpha$ es inestable, esto es, que no es estable, lo que matemáticamente significa que: 

$ \exists \varepsilon_0 > 0 $ para el cual, independientemente del $  \delta > 0$ que se tome,  esiste un $n_0 \in \mathbb N $ para el que se cumple que $| x_{0} - \alpha| < \delta $ pero  $| x_{n_0} - \alpha| > \varepsilon_0$ 

Por tanto si encontramos un $ \exists \varepsilon_0 > 0 $ que compla con esta condición habremos demostrado lo que buscábamos. 

Tomemos un  $x_0 \in ( I \cap (  \alpha- \delta , \alpha + \delta) ) - \{ \alpha\}$ fijo pero arbitario, 
en virtud del teorema del valor medio,  por no anularse nunca la deriva, sabemos que $f$ es monótoma e inyectiva, lo que significa que para cualquiera $x,y$ del intervalo distintos se tiene que $f(x) \neq f(y)  $  o equivalentemente $|f(x) - f(y) | \neq 0 $ 

Pues bien tomemos un $n \in \mathbb N $ 
 $|x_n - \alpha | $ 
 La primera igualdad se obtiene por cómo de definen los elementos de las órbitas de un SDD y al defininición de punto de equilibrio, la segunda por el teorema del valor medio:
  $|x_n - \alpha | = |f( x_{n-1}) - f(\alpha) |= |f'(c)||x_{n-1} - \alpha|$ donde $c$ está dentro del intervalo abierto que definen $x_{n-1}$y $\alpha$.
   Utilizando la hipótesis de que la derivada en valor absoluto está acotada inferiormente por 1 tenemos que 
$|x_n - \alpha | > |x_{n-1} - \alpha|$ . 
Esto serña siempre cierto para caalquier natural, ya que para el caso base también se cumple, esto se ve fácilmente repitiendo el  razonamiento anterior.
Por tanto hemos llegado a que
$|x_n - \alpha | > |x_0 - \alpha|$ 
Por tanto si tomamo $ \varepsilon_0 < |x_0 - \alpha|$


