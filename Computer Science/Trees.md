**Definition:** Self-referential data structures
	– One to many relationship between elements

Tree Terminology:
- Root → Element with no parent
- Leaf → Element with no children
- Interior Elements → Elements with children
![[Pasted image 20221213154247.png]]

Subtree - An element and all of its descendants

Depth - A measure of an element’s distance from the root
Height - Maximum depth of the tree

Perfect Tree Shape: has exactly 2^(h+1) -1 elements (where h is height)
![[Pasted image 20221213161017.png]]
Complete Tree Shape: Complete tree - Is a perfect tree up to level h-1, where leaves are as far left as possible
![[Pasted image 20221213161102.png]]


| Operation          | Balanced Tree | Degenerate Tree |
| ------------------ | ------------- | --------------- |
| Search / Lookup    | $O(log(n))$   | $O(n)$          |
| Lookup + Insertion | $O(log(n))$   | $O(n)$          |
| Lookup + Deletion  | $O(log(n))$   | $O(n)$          |
