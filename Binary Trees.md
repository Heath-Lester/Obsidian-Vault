Trees are a hierarchical structure built with nodes of different roles.

Trees are made up of different nodes:
- Root
- Parent
- Child
- Leaf
- Sibling
## Binary Trees

Binary Trees are trees with nodes that can only have up to two children. Additionally, each node can only have one parent.

```java
public class BinaryTreeNode {

	public int val;
	public BinaryTreeNode left;
	public BinaryTreeNode right;
	
	BinaryTreeNode() {}
		
	BinaryTreeNode(int val) {
		this.val = val;
	}
	
	BinaryTreeNode(int val, BinaryTreeNode left, BinaryTreeNode right) {
		this.val = val;
		this.left = left;
		this.right = right;
	}
	
}
```


## Perfect Binary Tree

https://www.baeldung.com/cs/full-vs-complete-vs-perfect-tree#perfect-binary-tree

A "perfect" binary tree is a binary tree where all leaf nodes *all* have the two children.
 - The numbers nodes are predicable as you descend down each level as they double each level down the tree.
 - The number of nodes on the last level is equal to the sum of all the of all the other nodes + 1.  An implication of this is that in any "perfect" binary tree, almost half of all nodes in the tree are in the bottom level.
 - All internal nodes have a degree of 2
 - All leaf nodes have a degree of 0

```
	    A
     /    \
    B      C
   / \    /  \
  D   E   F   G
 / \ / \ / \ / \  
H  I J K L M N  O
```

| Tree Property | Formula | Variable |
| ---- | ---- | ---- |
| # of Leaf Nodes | `n + 1` | n = internal nodes |
| # of nodes | `2^(h) - 1` | h = tree height |
| height of tree | `log(n + 1)/log(2)` | n = number of nodes |
 
## Complete Binary Tree

https://www.baeldung.com/cs/full-vs-complete-vs-perfect-tree#complete-binary-tree

A "complete" binary tree is a binary tree where all leaf nodes are filled from the left.

```
       A
     /    \
    B      C
   / \    / \
  D   E   F  G
 / \ / \ / \ | 
H  I J K L M N
```
## Full Binary Tree

https://www.baeldung.com/cs/full-vs-complete-vs-perfect-tree#full-binary-tree

A "full" binary tree is a binary tree is where all leaf nodes *either* have the maximum number of children or none.

```
       A
     /    \
    B      C
   / \    / \
  D   E   F  G
 / \ / \ / \  
H  I J K L M
```

## Binary Search Trees

| Method | O |
| ---- | ---- |
| lookup | O(log n) |
| insert | O(log n) |
| delete | O(log n) |
