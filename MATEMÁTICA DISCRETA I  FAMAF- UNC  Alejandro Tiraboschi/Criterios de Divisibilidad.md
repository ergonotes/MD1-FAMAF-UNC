Un número $n$ en base $10$ se escribe como $n = d_k \cdot 10^k + \dots + d_1 \cdot 10 + d_0$, donde $d_0$ es el último dígito. Lo usaremos para las demostraciones. 
###### **Divisibilidad por $2$**
**Regla**: El número debe terminar en un dígito par ($0, 2, 4, 6$ u $8$).
Queremos que $n \equiv 0 \pmod{2}$, y como $10 \equiv 0 \pmod{2}$, todas las potencias de $10$ son divisibles por $2$. Entonces $n \equiv d_0 \pmod{2}$, y $n$ es divisible por $2$ si y solo si $d_0 \equiv 0 \pmod{2}$.
****
###### **Divisibilidad por $3$ y por $9$**
**Regla**: La suma de los dígitos del número debe ser divisible por $3$. Lo mismo aplica para el $9$, pero la demostración será con el $3$. 
Observemos que $10 \equiv 1 \pmod{3}$, entonces $10^k \equiv 1^k \equiv 1 \pmod{3}$. Y por lo tanto $d_i \cdot 10^i \equiv d_i \cdot 1 \equiv d_i \pmod{3}$ y sumando todos los términos, $n = d_k \cdot 10^k + \cdots + d_0 \equiv d_k + \cdots + d_0 \pmod{3}$. Por lo tanto, $n \equiv 0 \pmod{3}$ si y sólo si la suma de los dígitos $d_k + \cdots + d_0 \equiv 0 \pmod{3}$.
****
###### **Divisibilidad por $4$**
https://grok.com/share/bGVnYWN5_0cdb375d-9c64-4fc3-847f-3aeb6f47e877
****
###### **Divisibilidad por $11$**
**Regla**: La suma alternada de los dígitos (suma de dígitos en posiciones impares menos suma de dígitos en posiciones pares, contando desde la derecha) debe ser divisible por $11$.
Como $10≡−1 \pmod{11}$, entonces $d_i \cdot 10^i \equiv d_i \cdot (-1)^i \pmod{11}$ y expresando todos los términos $n \equiv d_0 \cdot (-1)^0+d_1 \cdot (-1)^1+\cdots \equiv d_0-d_1+d_2-d_3+ \cdots \pmod{11}.$ Y eso mismo es la suma alternada $(d_0+d_2+ \cdots)-(d_1+d_3+ \cdots).$ Y por lo tanto, $n \equiv 0 \pmod{11}$ si la suma alternada es divisible por $11$.
**Ejemplo con $n=123456$:
- Dígitos desde la derecha (posiciones): $6$ ($1ª$, impar), $5$ ($2ª$, par), $4$ ($3ª$, impar), $3$ ($4ª$, par), $2$ ($5ª$, impar), $1$ ($6ª$, par).
- Suma de posiciones impares: $6 + 4 + 2 = 12$.
- Suma de posiciones pares: $5 + 3 + 1 = 9$.
- Suma alternada: $12−9=3$.
- Vemos que $3$ no es divisible por $11$.