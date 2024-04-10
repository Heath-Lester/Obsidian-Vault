
https://visualgo.net/en/list

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