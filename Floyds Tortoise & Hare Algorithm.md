https://en.wikipedia.org/wiki/Cycle_detection

>The algorithm is named after [Robert W. Floyd](https://en.wikipedia.org/wiki/Robert_W._Floyd "Robert W. Floyd"), who was credited with its invention by [Donald Knuth](https://en.wikipedia.org/wiki/Donald_Knuth "Donald Knuth").[3](https://en.wikipedia.org/wiki/Cycle_detection#cite_note-knuth-3)[4](https://en.wikipedia.org/wiki/Cycle_detection#cite_note-4) However, the algorithm does not appear in Floyd's published work, and this may be a misattribution: Floyd describes algorithms for listing all simple cycles in a [directed graph](https://en.wikipedia.org/wiki/Directed_graph "Directed graph") in a 1967 paper,[5](https://en.wikipedia.org/wiki/Cycle_detection#cite_note-5) but this paper does not describe the cycle-finding problem in functional graphs that is the subject of this article. In fact, Knuth's statement (in 1969), attributing it to Floyd, without citation, is the first known appearance in print, and it thus may be a [folk theorem](https://en.wikipedia.org/wiki/Mathematical_folklore "Mathematical folklore"), not attributable to a single individual.[6](https://en.wikipedia.org/wiki/Cycle_detection#cite_note-6)


This algorithm is essentially a two pointer strategy for linked list cycle detection.

The premise is that one pointer iterates sequentially while the other moves at double the others speed. 

Starting at the same point, `T` moves 1 while `H` moves 2.

```
                      > [] > [] >
[T, H] > [] > [] > []             []
                      < [] < [] <
```

```
                    > [] > [] >
[] > [T] > [H] > []             []
                    < [] < [] <
```

```
                   > [H] > [] >
[] > [] > [T] > []              []
                   < [] < [] <
```

```
                   > [] > [] >
[] > [] > [] > [T]             [H]
                   < [] < [] <
```

```
                  > [T] > [] >
[] > [] > [] > []              []
                  < [H] < [] <
```

```
                  > [H] > [T] >
[] > [] > [] > []              []
                   < [] < [] <
```

```
                  > [] > [] >
[] > [] > [] > []             [T, H]
                  < [] < [] <
```

Now that the tortoise and hare have met, you can take the meeting point and the head and walk them back together until they meet to find the origin of the cycle.

```
               > [] > [] >
[P] > [] > [] > []             [M]
               < [] < [] <
```


```
                   > [] > [] >
[] > [P] > [] > []             []
                   < [] < [M] <
```

```
                   > [] > [] >
[] > [] > [P] > []              []
                   < [M] < [] <
```

```
                     > [] > [] >
[] > [] > [] > [P,M]             []
                     < [] < [] <
```