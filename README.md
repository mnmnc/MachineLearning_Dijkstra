MachineLearning_Dijkstra
========================

Finding shortest path through undirected weighted graph with Dijkstra algorithm.


## INPUT

### GRAPH
```python
# K---P---T---X---Z
# |   |   |   |   |
# G---L---Q---U---Y
# |   |   |   |   |
# D---H---M---R---W
# |   |   |   |   |
# B---E---I---N---S
# |   |   |   |   |
# A---C---F---J---O
```
### SAME GRAPH WITH WEIGHTS
```python
# K-3-P-3-T-3-X-2-Z
# |25 |10 |4  |3  |2
# G-1-L-2-Q-2-U-2-Y
# |20 |8  |3  |2  |3
# D-2-H-3-M-2-R-1-W
# |10 |4  |2  |3  |2
# B-3-E-2-I-2-N-2-S
# |6  |4  |3  |3  |2
# A-4-C-1-F-2-J-3-O
```

### SAME GRAPH AS DICTIONARY
```python
graph = {
        'A' : [ {'B':6},        {'C':4} ],
        'K' : [ {'G':25},       {'P':3} ],
        'Z' : [ {'X':2},        {'Y':2} ],
        'O' : [ {'J':3},        {'S':2} ],
        'B' : [ {'A':6},        {'D':10},       {'E':3} ],
        'D' : [ {'B':10},       {'H':2},        {'G':20} ],
        'G' : [ {'K':25},       {'D':20},       {'L':1} ],
        'P' : [ {'K':3},        {'L':10},       {'T':3} ],
        'T' : [ {'P':3},        {'Q':4},        {'X':3} ],
        'X' : [ {'T':3},        {'U':3},        {'Z':2} ],
        'Y' : [ {'Z':2},        {'U':2},        {'W':3} ],
        'W' : [ {'Y':3},        {'R':1},        {'S':2} ],
        'S' : [ {'W':2},        {'N':2},        {'O':2} ],
        'J' : [ {'O':3},        {'N':3},        {'F':2} ],
        'F' : [ {'J':2},        {'I':3},        {'C':1} ],
        'C' : [ {'F':1},        {'E':4},        {'A':4} ],
        'E' : [ {'B':3},        {'C':4},        {'H':4},        {'I':2} ],
        'H' : [ {'D':2},        {'E':4},        {'L':8},        {'M':3} ],
        'L' : [ {'H':8},        {'G':1},        {'P':10},       {'Q':2} ],
        'Q' : [ {'L':2},        {'T':4},        {'U':2},        {'M':3} ],
        'U' : [ {'Q':2},        {'X':3},        {'R':2},        {'Y':2} ],
        'R' : [ {'U':2},        {'W':1},        {'N':3},        {'M':2} ],
        'N' : [ {'R':3},        {'S':2},        {'J':3},        {'I':2} ],
        'I' : [ {'M':2},        {'N':2},        {'F':3},        {'E':2} ],
        'M' : [ {'I':2},        {'H':3},        {'Q':3},        {'R':2} ]
}
```

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
