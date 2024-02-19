
https://visualgo.net/en/list

```java
 public class ListNode {
 
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