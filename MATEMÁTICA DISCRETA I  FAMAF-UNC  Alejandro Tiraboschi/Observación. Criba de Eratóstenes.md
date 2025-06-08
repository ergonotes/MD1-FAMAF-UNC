Una forma de encontrar números primos. Algoritmo que permite hallar todos los números primos menos que un número natural dado $n$.
**Cómo funciona:**
1. **Crea una lista** de números enteros desde $2$ hasta $n$ (ignora el $0$ y el $1$, ya que no son primos).
2. **Inicializa** marcando todos los números como "potencialmente primos".
3. **Comienza con el primer número primo**, que es $2$:
    - Marca todos sus múltiplos ($4, 6, 8, ...$) como no primos, ya que cualquier múltiplo de un número primo no puede ser primo.
4. **Pasa al siguiente número** que no esté marcado como no primo (el próximo primo, por ejemplo, $3$):
    - Marca todos sus múltiplos ($6, 9, 12, ...$) como no primos.
5. **Repite** este proceso para cada número no marcado hasta que llegues a un número mayor o igual a la raíz cuadrada de $n$. No necesitas seguir más allá, porque cualquier número compuesto mayor ya habría sido marcado por un factor menor.