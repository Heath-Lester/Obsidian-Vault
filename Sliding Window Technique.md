
>Form a window over some **portion** of **sequential** data, them **move** that window throughout the data to **capture** different parts of it.


```
[1, 3, 7, 9, 2, 4]
 ^  ^               <- Window
```

```
[1, 3, 7, 9, 2, 4]
    ^  ^           <- move window to right
```

```
[1, 3, 7, 9, 2, 4]
             ^  ^  <- shift window to right or to end
```

Can only be used where a condition of the data or result is related to some sort of continuity, contiguousness. Maybe, maybe not.

Can be used for:
 - Comparisons
 - Aggregations