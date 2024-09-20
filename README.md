# Ejercicios: Carrera de tortugas
Autor: Toñi Reina

## Ejercicio 1
Implementa una función ```tortugas``` para simular una carrera de dos tortugas que están compitiendo en una carrera. Cada tortuga comienza en la posición 0, pero avanzan a diferentes velocidades. Tu objetivo es simular la carrera y mostrar quién llega primero a la meta, que está en la posición que se pasa como parámetro a la función.

Reglas:

- La tortuga A avanza 1 ó 2 pasos aleatorios en cada turno.
- La tortuga B avanza 1, 2, ó 3 pasos aleatorios en cada turno.
- El bucle `while` debe ejecutarse hasta que una de las tortugas llegue a la posición de la meta (o más).
- En cada iteración del bucle, el programa debe mostrar las posiciones actuales de ambas tortugas.

Instrucciones:

- Usa la estructura `while` para hacer que las tortugas avancen mientras ninguna ha alcanzado la meta.
- Usa la función `random.randint()` para generar de forma aleatoria el número de pasos que avanzan.
- Al finalizar el bucle, indica qué tortuga ganó o si fue un empate.

Ejemplos de ejecuciones son las siguientes:

- La meta está en la posición 10 y gana la tortuga B.
```python
    >>tortuga(10)
    Tortuga A está en 2, Tortuga B está en 1
    Tortuga A está en 3, Tortuga B está en 4
    Tortuga A está en 4, Tortuga B está en 5
    Tortuga A está en 6, Tortuga B está en 7
    Tortuga A está en 8, Tortuga B está en 10
    ¡Tortuga B ganó!
```
- La meta está en la posición 3 y hay un empate.
```python
    >>tortuga(3)
    Tortuga A está en 2, Tortuga B está en 1
    Tortuga A está en 3, Tortuga B está en 4
    ¡Es un empate!
```
 - La meta está en la posición 3 y gana la tortuga A.
```python
    >> tortugas(3)
    Tortuga A está en 2, Tortuga B está en 1
    Tortuga A está en 4, Tortuga B está en 2
    ¡Tortuga A ganó!
```

Implementa una función ```tortugas``` para simular una carrera de dos tortugas que están compitiendo en una carrera. Cada tortuga comienza en la posición 0, pero avanzan a diferentes velocidades. Tu objetivo es simular la carrera y mostrar quién llega primero a la meta, que está en la posición que se pasa como parámetro a la función.


## Ejercicio 2: 

Implemente una segunda versión de la simulación llamada `tortuga_con_sorpresas`, que además de la meta tiene como parámetro una probabilidad (un número entre 0 y 1), que indica la probabilidad de que una tortuga resbale en la carrera y retroceda una serie de casillas de forma aleatoria.

Instrucciones:

- Probabilidad de resbalón:  Para implementar esto genere para generar un número entre 0 y 1. Por ejemplo, si la probabilidad de resbalón es del 5% y el número aleatorio que ha generado número es menor que 0.05, significa que la tortuga ha resbalado.
- El número de pasos que retrocede la tortuga también debe ser aleatorio.
- Las tortugas no pueden retroceder a posiciones negativas. Use la función`max(0, posicion)`, que devolverá 0 si posicion tiene un valor negativo, en otro caso devolverá posición, ya que max devuelve el máximo de dos números.
