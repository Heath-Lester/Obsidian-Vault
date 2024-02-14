Stacks and Queues are linear data structures that can only be traversed sequentially of which only one data element can be reached at a time.


You can build stacks and queues with arrays or linked lists.

[[Stacks]]
[[Queues]]

Arrays are better for stacks because arrays benefit from cache locality. Arrays cans be traversed more quickly because the elements in the array are stored adjacently in memory. Also the pop functionality in stacks are O(1) because when removing an element from the end of the array the indices do not need to be remapped.

Linked lists are better for Queues because removing items from the beginning of linked lists is 0(1) because the all of the pointers do not need to be remapped using the head pointer. 


Stacks and queues are generally inefficient for lookups.