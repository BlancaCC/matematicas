# Cómo utilizar máxima para resolver ecuaciones diferenciales  

Esta información está basada en: 
http://maxima.sourceforge.net/docs/manual/es/maxima_21.html 


Declación de una ecuación de segundo orden


```
(%i5) 'diff(x,t)=x^2+x;
                                  dx    2
(%o5)                             -- = x  + x
                                  dt
								     ``` 


para resolver la ecuación 
```
 ode2(%i5,x,t);
(%o7)                    log(x) - log(x + 1) = t + %c
```

si sabemos que una solución de nuesta ecuación es  `x(t=1)=1`
podemos calcular la ecuación particular

```
(%i12) ic1(%o10,t=1,x=1);
(%o12)               log(x) - log(x + 1) = t - log(2) - 1
(%i13) 

```

