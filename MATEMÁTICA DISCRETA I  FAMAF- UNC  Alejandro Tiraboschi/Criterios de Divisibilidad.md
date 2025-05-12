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