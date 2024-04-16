
Queues are a linear data structure that can only be accessed from the first or earliest element. This is also known as FIFO: First In, First Out.

```
[][][][][][][]
```

```
Dequeue
[][][][][][][] 
[][][][][][]   -> []
[][][][][][]
```

```
Enqueue
[]      [][][][][][] 
[] -> [][][][][][][]
      [][][][][][][]
```

```
Peek      v
[][][][][][] 
```

| Method   | [[Big O]] |
| -------- | --------- |
| lookup   | O(n)      |
| enqueue  | O(1)      |
| dequeue* | O(1)      |
| peek     | O(1)      |
\* dequeue removes the first element

