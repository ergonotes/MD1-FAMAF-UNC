%%El símbolo $\perp$ a veces se utiliza para indicar que dos números o expresiones son coprimos%%
##### **Ecuaciones Lineales Diofánticas**
**Aquellas con coeficientes enteros de las cuales se buscan las soluciones enteras.** 

> Su nombre debido a *Diofanto de Alejandra, 200-284*, quien fue quien desarrollo ese tipo de ecuaciones en su obra *La Aritmetica*.

Las ecuaciones diofánticas mas sencillas son las ecuaciones lineales de la forma $$a X +b Y =c$$ con $a,b,c Z \in$ donde $a$ y $b$ no son ambos nulos. 
En los problemas que involucran estas ecuaciones se busca encontrar todos los pares $x,y \in Z^2$ que son solución de la ecuación.
***
###### **Observación.** 
Si $a=0$ o $b=0$ (supongamos $b=0$), el problema se vuelve un problema de divisibilidad:  $aX +0 \cdot Y =c$ tiene solución entera si y solo si $a|c$.
***
###### **Ecuación diofántica y máximo común divisor.**$$\begin{align*}
&\text{Sean } a, b, c \in \mathbb{Z} \ \text{con } a, b \ \text{no nulos. La ecuación diofántica} \\
&\quad aX + bY = c \\
&\text{admite soluciones enteras si y solo si } (a : b) | c. \ \text{Es decir,} \\
&\exists \ (x_0, y_0) \in \mathbb{Z}^2 : a x_0 + b y_0 = c \iff (a : b) | c.
\end{align*}$$**Demostración.** **($\implies$)** Sea ($x_0,y_0$) $\in Z^2$ una solución entera, entonces, dado que $\text{mcd}(a,b)|a$ y $\text{mcd}(a,b)|b$, se concluye que $\text{mcd}(a,b)|a x_0 + b y_0 = c$. Por las propiedades de divisibilidad.
**($\Longleftarrow$)** Sabemos que existen $s,t \in Z$ tales que $\text{mcd}(a,b)=sa+tb$. Luego, dado que $\text{mcd}(a,b)|c,$ existe $k \in Z$ tal que $c=k \cdot \text{mcd}(a,b)$, y por lo tanto se tiene que $c=a(ks)+b(kt)$ y podemos tomar $x_0:=ks, \space y_0:=kt$.
Como $1|c,$ para todo $c \in Z,$ se obtiene inmediatamente el corolario siguiente.
****
Sean $a' X +b' Y = c'$ y $a X+b Y =c$ dos ecuaciones diofánticas. Decimos que son **equivalentes** si tienen exactamente las mismas soluciones $(x,y)\in Z^2$. $$\begin{align*}
&\text{Sean } a, b, c \in \mathbb{Z} \ \text{con } a, b \ \text{no nulos tales que } (a : b) | c. \\
&\text{Definamos } a' = \frac{a}{(a : b)}, \ b' = \frac{b}{(a : b)} \ \text{y} \ c' = \frac{c}{(a : b)}. \ \text{Entonces,}
\end{align*}$$$a' X +b' Y = c'$ y $a X+b Y =c$  son **EQUIVALENTES**.
Esto es claro ya que al dividir $a$ y $b$ por $(a : b),$ todos los factores comunes de $a$ y $b$ son "eliminados", debido a que por definición $(a : b)$ concentra todos los factores comunes entre $a$ y $b$. Y como resultado quedan los factores que son únicos para cada número, y por lo tanto, $a$ y $b$ se vuelven coprimos (Pensarlo con la descomposición prima de $a$ y $b$, y luego dividir por el $\text{mcd}$). Luego de la "coprimización", las dos ecuaciones tienen exactamente las mismas soluciones.
> Suele ser más simple hacer este proceso de "**coprimización**" de entrada para encontrar una solución particular: se escribe el $1$ como combinación entera de $a'$ y $b'$ : $1=sa'+tb'$ y luego haciendo $c'= c'sa'+c'tb'$ se obtiene por ejemplo $x_0 = c's$ e $y_0 = c't$.
***
###### **Ecuación diofántica con $a$ y $b$ coprimos.**$$\begin{align*}
&\text{Sean } a, b \in \mathbb{Z} \ \text{no nulos y coprimos. Entonces la ecuación diofántica} \\
&\quad a X + b Y = c \\
&\text{tiene soluciones enteras, para todo } c \in \mathbb{Z}.
\end{align*}$$Trataremos primero el caso $c=0$: el cual siempre tiene solución pues $(a : b)|0$. [[Ejemplo de Ecuación Diofántica igualada a cero]]$$\begin{align*}
&\text{Sean } a, b \in \mathbb{Z}, \ \text{no nulos.} \\
&\text{El conjunto } S_0 \ \text{de soluciones enteras de la ecuación diofántica } aX + bY = 0 \ \text{es} \\
&S_0 = \{ (x, y) : x = b' k, y = -a' k, k \in \mathbb{Z} \}, \ \text{donde } a' = \frac{a}{(a : b)} \ \text{y} \ b' = \frac{b}{(a : b)}.
\end{align*}$$**Demostración.** Se tiene $a X + b Y = 0$ y la expresión equivalente  $a' X + b' Y = 0$ donde $a'=a/(a:b)$ y $b'=b/(a:b)$ son coprimos.$$\begin{align*}
&\text{Ahora bien, sea } (x, y) \in \mathbb{Z}^2 \ \text{solución:} \\
&a' x + b' y = 0 \iff a' x = -b' y \\
&\implies a' | b' y \ \text{y} \ y | a' x \\
&\implies a' | y \ \text{y} \ b' | x \\
&\implies \exists j, k \in \mathbb{Z} : y = j a' \ \text{y} \ x = k b'.
\end{align*}$$Volviendo al primer renglón, resulta:$$a' (k b') = -b' (j a') \implies j = -k$$Es decir: $x=b'k$  e  $y=-a'k$ para el mismo $k \in Z$, entonces $(x,y)$ es solución. Se tiene $a'x+b'y=a'(b'k)+b'(-a'k)=0$.
La resolución completa de este caso particular nos sirve para resolver completamente una ecuacion lineal diofantica arbitraria.
***
Teniendo  $a X +b Y =c$  y sean $a,b,c \in Z,$ con $a,b$ no nulos. $$\begin{align*}
&\bullet \ S = \emptyset \ \text{cuando } (a : b) \nmid c. \\
&\bullet \ S = \{ (x, y) : x = x_0 + b' k, y = y_0 - a' k; k \in \mathbb{Z} \}, \ \text{donde } (x_0, y_0) \\
&\text{es una solución particular cualquiera de la ecuación y } a' = \frac{a}{(a : b)}, \ b' = \frac{b}{(a : b)} \ \text{cuando } (a : b) | c.
\end{align*}$$**Demostración.** Sabemos que si $(a : b) \nmid c$, la ecuación no admite solución. Cuando $(a : b) | c$, tenemos al menos una solución particular $(x_0,y_0) \in Z^2$, es decir, $ax_0+by_0=c$. Y se tiene:$$ax + by = c \iff ax + by = a x_0 + b y_0 \iff a (x - x_0) + b (y - y_0) = 0$$si pasamos restando y demás... Es decir, $(x,y)$ es solución de $a X +b Y =c$ si y sólo si $(x-x_0,y-y_o)$ es solución de $a X +b Y =0$. O sea, **por la demostración anterior** tenemos que existe $k\in Z$ tal que $$x - x_0 = b' k, \ y - y_0 = -a' k, \ \text{osea} \ x = x_0 + b' k, \ y = y_0 - a' k$$
***
En el libro fuente de este apartado se encuentran ejemplos de resoluciones de ecuaciones de este tipo...