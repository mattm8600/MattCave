**Definition:** Binary [[Trees]] are trees with at most **two** children per tree

Implementation:
```
public class Tree {

	private static class Node {
		private Object data;
		private Node left;
		private Node right;
	}

	private Node root = null;
}
```

Tree Traversal:
1. Pre-order Traversal - Processes node, then left, then right (Pre-order: Node first)
2. In-order Traversal - Processes left, then node, then right
3. Post-order Traversal - Visits left, then right, then node (Post-order: Node last)
4. Breadth-First Traversal - Visits based on how far away from root

Binary Search Tree: - Binary Tree with the properties:
- Left subtree < node
- Right subtree > node

Balanced BST - Most of the tree has two children per node:
![[Pasted image 20221213160517.png]]
Degenerate BST: Tree has mostly one child per node:
![[Pasted image 20221213160541.png]]
- You lose a lot of the BST’s efficiency when it becomes degenerate → Basically linked list



## Binary Search Tree Algorithms:
Binary Search Tree Look-up Algorithm:
- If v == node, we found value
- If v < node, search left subtree
- If v > node, search right subtree

Binary Tree Insertion:
- Search for x (value you are inserting)
- if x is not in tree, it finishes at node y
- if x < y, add a new leaf containing x as left child of y
- if x > y, add a new lead containing x as right child of y

Binary Search Tree Deletion:
- Perform search for x to be deleted (value you are deleting)
- if x is a leaf, remove x
- delete x, replace with largest value in left subtree OR smallest value in right subtree

Polymorphic Binary Search Tree - Instead of having null for leafs, make it point to an Empty Tree Object