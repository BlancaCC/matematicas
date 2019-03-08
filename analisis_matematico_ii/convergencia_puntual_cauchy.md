FALTA EL RECÍPROCO
# Proposición  
Una sucesión $ f_k : A \longrightarrow \mathbb{R^m}$ converge puntualemente si y solo si para cada $x$ del dominio dicha sucesión es de Cauchy. 

## Demostración   

### Condición suficiente

Se quiere ver que $ \forall x $ y para todo épsilon positivo existe un natural a partir del cual cualquier pareja k,q de naturales mayores que él cumplen que $ |f_k(x) - f_q(x)| < \epsilon$

$ |f_k(x) - f_q(x)| = |f_k(x) -f(x) +f(x) - f_q(x)| < |f_k(x) -f(x)| + |f(x) - f_q(x)| $

Por la hipótesis de convergencia puntual sabemos que $ \forall x $ y para todo épsilon positivo existe un natural a partir del cual cualquier  k  natural mayor que él cumplen que $ |f_k(x) - f(x)| < \frac{\epsilon}{2} $que la distancia con una función f 

por tanto podemos terminar de acotar tal desigualdad. 
$ |f_k(x) - f_q(x)|  < |f_k(x) -f(x)| + |f(x) - f_q(x)|  < \frac{\epsilon}{2} + \frac{\epsilon}{2} = \epsilon $

Demostrando con ello lo que se buscaba. 


### Recíproco
Se quiere porbar que tal sucesión converge puntualmente, 
es decir: sea cual sea el $x$ del dominio y el  épsilon positivo
existe un natural a partir del cual cualquier $k$ natural
mayor que él cumple que $ |f_k(x) - f(x)| < \epsilon $


Por ser de Cauchy sabemos que para cualquier elemento $x$ del dominio 
y épsilon positivo existe un natural $n_0$ a partir del cual cualquier pareja
p,q de naturales ambos mayores que el cumplen que 

$ \epsilon > | f_q(x) - f_p(x)|$

Pues bien se tiene esta aparentemente inocente apreciación : si  $n_0 < q $ entonces se cumple que $ n_0 < q < q+1 < \lim _{q   \rightarrow  \infty} q $ 

A partir del cual y teniendo en cuenta que la sucesión es de Cauchy: 

Llamemos $f(x)$ al supuesto límite de la sucesión $\{f_k(x) \}$ y veamos que existe el natural mínimo que acote en una constante real positva la distancia de los elementos de la sucesión con su límite: 
$ \epsilon > |f_q(x) - f_p(x) | \geq \lim _{q   \rightarrow  \infty} |f_q(x) - f_p(x) | = |f_p(x) - f(x) |$

Por tanto, en virtud de que la sucesión era de Cauchy, existe una natural $n_0$, dependiente del elemento del dominio y épsilon real positivos fijados, para el cual se cumple la definición de convergencia puntual. 

Probando de esta manera el recípro y con ello esta equivalencia. 
