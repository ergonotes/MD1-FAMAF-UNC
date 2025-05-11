**Ejemplo.** Soluciones enteras de $18X + 27Y = 0$.
La solución mas simple es $x_0 = 0,$ $y_0 = 0$. O también se tiene $x_1 = 27,$ $y_1 = 18$. Así que la solución no es única, probaremos que son infinitas: Por lo mencionado arriba, la ecuación original es equivalente a la ecuación "coprimizada" $2X + 3Y = 0.$$$\begin{align*}
&\text{Ahora bien, sea } (x, y) \in \mathbb{Z}^2 \ \text{solución:} \\
&2x + 3y = 0 \iff 2x = -3y \\
&\implies 2 | 3y \ \text{y} \ y | 2x \\
&\implies 2 | y \ (\text{porque } 2 \perp 3) \ \text{y} \ 3 | x \ (\text{porque } 3 \perp 2) \\
&\implies y = 2j \ \text{y} \ x = 3k.
	\end{align*}$$Volviendo al primer renglón, resulta:$$2(3k) = -3(2j) \implies j = -k$$Es decir: $x = 3k$ e $y = -2k$ para algún $k \in Z$. Hemos probado que si encontramos un par $(x,y)$ solución entera $\implies$ existe $k \in Z$ tal que $x=3k$ e $y=-2k$. El conjunto de soluciones enteras es $S_0 = \{ (x, y) : x = 3k, y = -2k; k \in \mathbb{Z} \}$. (Observemos que si nos olvidamos de coprimizar la ecuación y nos quedamos, usando la misma estructura, con las soluciones de tipo $x = 27k,$ $y = 18k,$ $k \in Z$, perdemos soluciones ya que se nos escapa por ejemplo la solución $x_3 = 3$ $y_3 = -2$.) Este procedimiento se puede generalizar, y es generalizado en el apartado de [[Ecuaciones Diofánticas - Álgebra I - UBA - Teresa Krick]].