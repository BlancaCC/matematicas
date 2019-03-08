# Enunciado   
Da una ecuación resuelva esta recurrencia.
$T(n) = T ( \frac{n}{2})  T^2( \frac{n}{4})$

## Solución
1. Realizamos cambio de variable. $n = 2^m $ resultando
$T(2^m) = T ( \frac{2^m}{2}) + T^2( \frac{2^m}{4})$ 

Para reducir el orden aplicamos logaritmo en base 2 en ambos miembros  
$ \log_2 {T(2^m)} = \log_2{ T ( \frac{2^m}{2})  T^2( \frac{2^m}{4}) }$

Aplicando las promiedades de los logaritmos 
$ \log_2 {T(2^m)} = \log_2{ T ( \frac{2^m}{2})} +\log_2{  T( \frac{2^m}{4}) } + \log_2{ T( \frac{2^m}{4})}$

Renombramos: $ \log_2 {T(2^m)} = U( k)$

$ U( k) = U( k-1) + 2U(k-2)$ 

Estamos ante una ecuación linear homogénea de orden 2.

Polinomio característico: $ x^2 - x - 2 = (x+1)(x-2)$
Solución general: $T(k) = C_1 -1^k + c_2 2^k$
Solución general: $T({2^m}) = C_1 -1^{2^m} +c_2 2^{2^m}$

Ahora desacemos el cambio de variable  $n = 2^m $

Solución general: $T({2^m}) = C_1 -1^{ \log_2 n} +c_2 n$ 

Si calculáros la eficiencia sería $O(n)$


