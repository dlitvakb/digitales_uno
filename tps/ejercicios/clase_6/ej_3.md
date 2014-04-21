* Transformar la siguiente suma de productions en un
  Mapa de Karnaugh
* Armar la tabla de verdad

f = ~D~CBA + ~DC~B~A + DC~BA + DCBA + DC~B~A + ~D~C~BA + D~CB~A

```
D | C | B | A || f
0 | 0 | 0 | 0 || 0
0 | 0 | 0 | 1 || 1
0 | 0 | 1 | 0 || 0
0 | 0 | 1 | 1 || 1
0 | 1 | 0 | 0 || 1
0 | 1 | 0 | 1 || 0
0 | 1 | 1 | 0 || 0
0 | 1 | 1 | 1 || 0
1 | 0 | 0 | 0 || 0
1 | 0 | 0 | 1 || 0
1 | 0 | 1 | 0 || 1
1 | 0 | 1 | 1 || 0
1 | 1 | 0 | 0 || 1
1 | 1 | 0 | 1 || 1
1 | 1 | 1 | 0 || 0
1 | 1 | 1 | 1 || 1
```


```
DC \ BA
   | 00 | 01 | 11 | 10
00 |  0 |  1 |  1 |  0
01 |  1 |  0 |  0 |  0
11 |  1 |  1 |  1 |  0
10 |  0 |  0 |  0 |  1
```

