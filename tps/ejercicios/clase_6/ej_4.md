# Transformar la siguiente suma de productos no estandar
  en un Mapa de Karnaugh

f = ~C~B + D~C + DC~B + D~CB~A + ~D~C~BA + D~CBA

```
D | C | B | A || f
0 | 0 | 0 | 0 || 1
0 | 0 | 0 | 1 || 1
0 | 0 | 1 | 0 || 0
0 | 0 | 1 | 1 || 0
0 | 1 | 0 | 0 || 0
0 | 1 | 0 | 1 || 0
0 | 1 | 1 | 0 || 0
0 | 1 | 1 | 1 || 0
1 | 0 | 0 | 0 || 1
1 | 0 | 0 | 1 || 1
1 | 0 | 1 | 0 || 1
1 | 0 | 1 | 1 || 1
1 | 1 | 0 | 0 || 1
1 | 1 | 0 | 1 || 1
1 | 1 | 1 | 0 || 0
1 | 1 | 1 | 1 || 0
```


```
DC \ BA
   | 00 | 01 | 11 | 10
00 |  1 |  1 |  0 |  0
01 |  0 |  0 |  0 |  0
11 |  1 |  1 |  0 |  0
10 |  1 |  1 |  1 |  1
```

