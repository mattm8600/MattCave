A heap is a [[Binary Tree]] tree with two properties:
1. It’s complete (see [[Trees]]])
2. All elements are either greater than or less than root
	– Min heap: All elements are greater than or equal to its parent
	– Max heap: All elements are less than or equal to its parent



Properties:
- Height = $log(n) + 1$
- Smallest item of a min heap can be found at $O(1)$

## Heap Operations
Insertion
```
add X to the end of heap
while(X < parent's value)
	swap X with parent //keeps swapping up the tree until it is valid
```
getSmallest() - returns and removes the smallest value
```
get smallest value (root)
replace root with X at end of heap
while(X > either child's value)
	swap X with smaller child // X drops down tree
return original root
```

Array Heap Implementation:
- Use the following formulas to store the location of each value:
	– parent of i = floor(i(-1)/2)
	left child of i = 2i + 1
	right child of i = 2i + 

Finding Largest Element of Min Heap: You have to go through whole heap $O(n)$
– Smallest element is not $O(1)$ bc you need to swap a new element into its spot