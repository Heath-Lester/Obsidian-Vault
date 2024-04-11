
https://visualgo.net/en/list

Linked lists are essentially a collection of nodes that point to another node or null. Nodes have two elements which are the value it contains and a pointer to the next node. Linked lists are `null terminated` meaning that the last node, or the tail's pointer points to a `null` value.

```
[head]      [value]     [value]     [value]     [tail]
[pointer] > [pointer] > [pointer] > [pointer] > [pointer] > null
```

| Method   | [[Big O]] |
| -------- | --------- |
| getNth   | O(n)      |
| addFirst | O(1)      |
| addEnd   | O(n)      |
| remove   | O(n)      |

```java
 public class ListNode {
 
	int val;

	ListNode next;

	ListNode() {}
      
	ListNode(int val) {
		this.val = val;
	}
      
	ListNode(int val, ListNode next) {
		this.val = val;
		this.next = next;
	}
	
}
```

