
https://visualgo.net/en/list

Doubly linked lists are a collection of nodes that point to two other nodes or null. These nodes have three elements which are the value it contains, a pointer to the next node, and another pointer to the previous node. Doubly linked lists are `null terminated` meaning that the the first and last nodes, or the head and tail pointers, point to a `null` value.

```
	   [head]      [value]     [value]     [value]     [tail]
	   [pointer] > [pointer] > [pointer] > [pointer] > [pointer] > null
null < [pointer] < [pointer] < [pointer] < [pointer] < [pointer]
```

| Method   | [[Big O]] |
| -------- | --------- |
| getNth   | O(n)      |
| addFirst | O(1)      |
| addEnd   | O(1)      |
| remove   | O(n)      |


```java
 public class DoubleListNode {
 
	int val;

	ListNode next;
	ListNode last;

	ListNode() {}
      
	ListNode(int val) {
		this.val = val;
	}
      
	ListNode(int val, ListNode next, ListNode last) {
		this.val = val;
		this.next = next;
		this.last = last;
	}
	
}
```