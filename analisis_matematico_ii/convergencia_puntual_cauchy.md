FALTA EL RECÍPROCO
# Proposición  
Una sucesión $ f_k : A \longrightarrow \mathbb{R^m}$ converge puntualemente si y solo si 
para cada x del dominio dicha sucesión es de Cauchy. 

## Demostración   

### Condición suficiente

Se quiere ver que $ \forall x $ y para todo épsilon positivo
existe un natural a partir del cual cualquier pareja k,q de naturales
mayores que él cumplen que $ |f_k(x) - f_q(x)| < \epsilon$

$ |f_k(x) - f_q(x)| = |f_k(x) -f(x) +f(x) - f_q(x)| < |f_k(x) -f(x)| + |f(x) - f_q(x)| $

Por la hipótesis de convergencia puntual sabemos que
 $ \forall x $ y para todo épsilon positivo
existe un natural a partir del cual cualquier  k  natural
mayor que él cumplen que $ |f_k(x) - f(x)| < \fract{\epsilon}{2} $

por tanto podemos terminar de acotar tal desigualdad. 
$ |f_k(x) - f_q(x)|  < |f_k(x) -f(x)| + |f(x) - f_q(x)|  < \fract{\epsilon}{2} + \fract{\epsilon}{2} = \epsilon $

Demostrando con ello lo que se buscaba. 


### Recíproco
Se quiere porbar que tal sucesión converge puntualmente, 
es decir: sea cual sea el $x$ del dominio y el  épsilon positivo
existe un natural a partir del cual cualquier k naturales
mayor que él cumple que $ |f_k(x) - f(x)| < \epsilon $


Por ser de Cauchy sabemos que para cualquier elemento x del dominio 
y épsilon positivo existe un natural a partir del cual cualquier pareja
p,q de naturales ambos mayores que el cumplen que 

$ \epsilon > | f_q(x) - f_p(x)|$

Desarrollando y acotando por desigualdad triangular llegamos a que: 
$ \epsilon > | f_q(x) - f_p(x)| = | f_q(x)- f(x) - f_p(x) + f(x)| $
