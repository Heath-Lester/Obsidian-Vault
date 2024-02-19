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

https://visualgo.net/en/heap

| Method | O |
| ---- | ---- |
| lookup | O(log n) |
| insert | O(log n) |
| delete | O(log n) |
### Binary Search Tree Rules

- All increasing values are placed to the right
- All nodes can only have up to two children

```
    101
   /   \
  33   105
 / \   /  \
9  37 104 144  
```


Find 104:
1. 104 > 101; go right
2. 104 < 105; go left
3. 104 == 104; done


## Unbalanced Search Trees

An unbalanced search tree are is when a search trees structure starts to fall outside of a compete, full, or perfect binary structure. The long limbs of a search tree essentially start to function as a linked list once sequential numbers continue to be inserted into the tree.

```
     60
    /  \
   30   72
  / \     \
 14  51   73
 /   /      \
1  38       78
    \         \
    44        85
                \
                86
                  \
                  90
                    \
                    99
```

Because of this the time complexity starts to become closer to O(n) meaning that in order for a search tree to be optimally efficient, it must be balanced. While Binary trees are not the fastest for data structures, they are fast and consistent for a variety of methods.

|Method|O|
|---|---|
|lookup|O(n) |
|insert|O(n) |
|delete|O(n) |

## Tries

A Trie is a specialized and non-binary tree that, under normal circumstances can outperform most search trees.

These tree are commonly used for auto suggestions or auto complete.

```
         HEAD (Empty)
     /  /  \   \
    A   D    N   Z
   / \  |   / \   \
  R   S O  E   O   E
 /      |  |   |    \
E       T  W   T     N
           |
           S
```

The variable used in complexity measurement of a Trie is l for lenth.

|Method|O|
|---|---|
|lookup|O(l) |
|insert|O(l) |
|delete|O(l) |
