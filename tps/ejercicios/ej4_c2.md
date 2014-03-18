Representar para una compuerta Logica NAND de 3 entradas:
 * Expresion
 * Tabla de verdad
 * Simbolo Logico
 * Diagrama Temporal

## Expresion

f = ~(A . B . C)

## Tabla de verdad

| C | B | A | f |
| 0 | 0 | 0 | 1 |
| 0 | 0 | 1 | 1 |
| 0 | 1 | 0 | 1 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 1 |
| 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 0 |

## Simbolo Logico

C --| \
B --|  )o-- f
A --| /

## Diagrama Temporal

C _ _ _ _ - - - -
B _ _ - - _ _ - -
A _ - _ - _ - _ -
f - - - - - - - _
