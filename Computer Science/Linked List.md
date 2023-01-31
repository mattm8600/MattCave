**Definition:** A list linked together by references to the next node
![[Pasted image 20221213114659.png]]

Advantages of a List:
- Elements can be easily inserted or removed compared to array implementation
Disadvantages of a List:
- Doesn’t have indexing (must traverse from head)
- Requires more memory space than array implementation

- Typical Implementation: Use node [[Inner Classes]]
```
public class SinglyLinkedList { 
2 private Node head; 
3 private static class Node { 
4 private E element; // reference to the element stored at this node 
5 private Node next; // reference to the subsequent node in the list 
6 public Node(E e, Node n) { 
7 element = e; 
8 next = n; 
9 } 

}
```


Linked List Insertion (after current):
1. Create a new element temp
2. Set temp.next to current.next
3. Set current.next to temp

Linked List Deletion (item at current):
1. find prev such that prev.next = current
2. set prev.next to current.next

NOTE: For insertion and deletion, there are special cases such as:
- Empty Lists
- Beginning of List
- End of List

Ordered Lists - Need to iterate through list until insertValue is larger than current

Linked List Variations:
- Circularly-Linked Lists - The tail points to the head, good for cyclical iterations
- Dummy-head node - Put an empty node at the beginning and/or end of the list
	– Eliminates some special cases such as checking if the list is null
- Doubly-Linked Lists - There are next and previous references for every node
	– Advantages: Easy to find succeeding / preceding elements
	– Disadvantages: Extra work to maintain references, more memory per node