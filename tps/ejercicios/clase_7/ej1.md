## Desarrollar una Expresion 4x16 a partir de decodificadores 2x4, sin emplear logica adicional

### Tabla de Verdad

```
 E3 | E2 | E1 | E0 || S15 | S14 | S13 | S12 | S11 | S10 | S09 | S08 | S07 | S06 | S05 | S04 | S03 | S02 | S01 | S00
  0 |  0 |  0 |  0 ||   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   1
  0 |  0 |  0 |  1 ||   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   1 |   0
  0 |  0 |  1 |  0 ||   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   1 |   0 |   0
  0 |  0 |  1 |  1 ||   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   1 |   0 |   0 |   0
  0 |  1 |  0 |  0 ||   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   1 |   0 |   0 |   0 |   0
  0 |  1 |  0 |  1 ||   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   1 |   0 |   0 |   0 |   0 |   0
  0 |  1 |  1 |  0 ||   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   1 |   0 |   0 |   0 |   0 |   0 |   0
  0 |  1 |  1 |  1 ||   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   1 |   0 |   0 |   0 |   0 |   0 |   0 |   0
  1 |  0 |  0 |  0 ||   0 |   0 |   0 |   0 |   0 |   0 |   0 |   1 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0
  1 |  0 |  0 |  1 ||   0 |   0 |   0 |   0 |   0 |   0 |   1 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0
  1 |  0 |  1 |  0 ||   0 |   0 |   0 |   0 |   0 |   1 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0
  1 |  0 |  1 |  1 ||   0 |   0 |   0 |   0 |   1 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0
  1 |  1 |  0 |  0 ||   0 |   0 |   0 |   1 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0
  1 |  1 |  0 |  1 ||   0 |   0 |   1 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0
  1 |  1 |  1 |  0 ||   0 |   1 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0
  1 |  1 |  1 |  1 ||   1 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0 |   0
```

### Implementacion

```
     | H
  ___|___
_|E3   c3|______________________________
_|E2   c2|___________________       ___|___
 |     c1|_______________    |  ___|    S15|_
 |     c0|___________    |   |  |  |    S14|_
 |_______|           |   |  _)__)__|    S13|_
                     |   | | |  |  |    S12|_
                     |   | | |  |  |_______|
                     |   | | |  |
                     |   | | |__)______
                     |   | |    |   ___|___
                     |   | |    |  |    S11|_
E1-------------------)---)-)-------|    S10|_
            |        |   | |     __|    S09|_
            |        |   | |    |  |    S08|_
            |        |   | |    |  |_______|
E0----------)--------|---|-------
            |        |   |___)_________
            |        |       |      ___|___
            |________)_______)_____|    S07|_
                     |       |  |  |    S06|_
                     |       |  |  |    S05|_
                     |       |  |  |    S04|_
                     |       |  |  |_______|
                     |       |  |
                     |_______)__)______
                             |  |   ___|___
                             |  |__|    S03|_
                             |     |    S02|_
                             |_____|    S01|_
                                   |    S00|_
                                   |_______|
```

