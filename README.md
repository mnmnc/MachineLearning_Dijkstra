MachineLearning_Dijkstra
========================

Finding shortest path through undirected weighted graph with Dijkstra algorithm.


## OUTPUT

```python
Calculating from:  A
K       P       T       X       Z
|       |       |       |       |
G       L       Q       U       Y
|       |       |       |       |
D       H       M       R       W
|       |       |       |       |
6       E       I       N       S
|       |       |       |       |
0       4       F       J       O

Calculating from:  C
K       P       T       X       Z
|       |       |       |       |
G       L       Q       U       Y
|       |       |       |       |
D       H       M       R       W
|       |       |       |       |
6       8       I       N       S
|       |       |       |       |
0       4       5       J       O

Calculating from:  F
K       P       T       X       Z
|       |       |       |       |
G       L       Q       U       Y
|       |       |       |       |
D       H       M       R       W
|       |       |       |       |
6       8       8       N       S
|       |       |       |       |
0       4       5       7       O

Calculating from:  B
K       P       T       X       Z
|       |       |       |       |
G       L       Q       U       Y
|       |       |       |       |
16      H       M       R       W
|       |       |       |       |
6       8       8       N       S
|       |       |       |       |
0       4       5       7       O

Calculating from:  J
K       P       T       X       Z
|       |       |       |       |
G       L       Q       U       Y
|       |       |       |       |
16      H       M       R       W
|       |       |       |       |
6       8       8       10      S
|       |       |       |       |
0       4       5       7       10

Calculating from:  E
K       P       T       X       Z
|       |       |       |       |
G       L       Q       U       Y
|       |       |       |       |
16      12      M       R       W
|       |       |       |       |
6       8       8       10      S
|       |       |       |       |
0       4       5       7       10

Calculating from:  I
K       P       T       X       Z
|       |       |       |       |
G       L       Q       U       Y
|       |       |       |       |
16      12      10      R       W
|       |       |       |       |
6       8       8       10      S
|       |       |       |       |
0       4       5       7       10

Calculating from:  N
K       P       T       X       Z
|       |       |       |       |
G       L       Q       U       Y
|       |       |       |       |
16      12      10      13      W
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  O
K       P       T       X       Z
|       |       |       |       |
G       L       Q       U       Y
|       |       |       |       |
16      12      10      13      W
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  M
K       P       T       X       Z
|       |       |       |       |
G       L       13      U       Y
|       |       |       |       |
16      12      10      12      W
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  H
K       P       T       X       Z
|       |       |       |       |
G       20      13      U       Y
|       |       |       |       |
14      12      10      12      W
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  R
K       P       T       X       Z
|       |       |       |       |
G       20      13      14      Y
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  S
K       P       T       X       Z
|       |       |       |       |
G       20      13      14      Y
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  W
K       P       T       X       Z
|       |       |       |       |
G       20      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  Q
K       P       17      X       Z
|       |       |       |       |
G       15      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  D
K       P       17      X       Z
|       |       |       |       |
34      15      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  U
K       P       17      17      Z
|       |       |       |       |
34      15      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  L
K       25      17      17      Z
|       |       |       |       |
16      15      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  G
41      25      17      17      Z
|       |       |       |       |
16      15      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  Y
41      25      17      17      18
|       |       |       |       |
16      15      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  T
41      20      17      17      18
|       |       |       |       |
16      15      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  X
41      20      17      17      18
|       |       |       |       |
16      15      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  Z
41      20      17      17      18
|       |       |       |       |
16      15      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  P
23      20      17      17      18
|       |       |       |       |
16      15      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Calculating from:  K
23      20      17      17      18
|       |       |       |       |
16      15      13      14      16
|       |       |       |       |
14      12      10      12      13
|       |       |       |       |
6       8       8       10      12
|       |       |       |       |
0       4       5       7       10

Shortest path from Z to A:
Z
Y
W
R
N
J
F
C
A

```
