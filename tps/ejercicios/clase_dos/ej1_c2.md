Representar para una compuerta logica OR de 4 entradas:
 * Expresion
 * Tabla de verdad
 * simbolo logico
 * diagrama temporal

## Expresion

f = A + B + C + D

## Tabla de Verdad
| D | C | B | A | f |
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 0 | 1 | 1 |
| 0 | 0 | 1 | 0 | 1 |
| 0 | 0 | 1 | 1 | 1 |
| 0 | 1 | 0 | 0 | 1 |
| 0 | 1 | 0 | 1 | 1 |
| 0 | 1 | 1 | 0 | 1 |
| 0 | 1 | 1 | 1 | 1 |
| 1 | 0 | 0 | 0 | 1 |
| 1 | 0 | 0 | 1 | 1 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 0 | 1 | 1 | 1 |
| 1 | 1 | 0 | 0 | 1 |
| 1 | 1 | 0 | 1 | 1 |
| 1 | 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 1 | 1 |

## Simbolo Logico

   \\
D --\ \
C --|  \____ f
B --|  /
A --/ /
   //

## Diagrama Temporal

D _ _ _ _ _ _ _ _ - - - - - - - -
C _ _ _ _ - - - - _ _ _ _ - - - -
B _ _ - - _ _ - - _ _ - - _ _ - -
A _ - _ - _ - _ - _ - _ - _ - _ -
f _ - - - - - - - - - - - - - - -
