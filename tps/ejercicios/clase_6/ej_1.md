# Simplificar el mapa de Karnaugh anterior
  por minitermino o maxitermino

### Por minitermino

```
C \ BA
  | 00  | 01 | 11 | 10
0 | ( 1 |  1 | ( 1 |  1 ))
1 |   0 |  0 | ( 1 |  1  )
```

f(x) = ~C + B

### Por maxitermino

```
C \ BA
  | 00  |  01  | 11 | 10
0 |  1  |   1  |  1 |  1
1 | ( 0 |  0 ) |  1 |  1
```

f(x) = ~C + B
