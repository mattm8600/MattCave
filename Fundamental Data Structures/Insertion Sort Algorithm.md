**Approach:** Sorted part of the array on the left, unsorted is on the right. Every step adds the first unsorted element into the sorted part (all elements greater than it are shifted one index over)

Ex:
![[Pasted image 20221213190016.png]]

Code:
```
void insertionSort(int[] a) {
	int i,j,x;
	for(i=1; i<a.length;i++) { //Iterate through the unsorted elements of the array
		x = a[i]; // set our current value to sort
		j = i; // Reset index
		while(j > 0; && x < a[j-1]) { //While element is less than preceding element
		a[j] = a[j-1]; //swap the elements
		j--; // then check if element is less than element before preceding element
		}
		a[j] = x; //Set the element at the spot it ends up
	}
}
```

Trace:
1. We go through the unsorted elements of the array
2. We continually check if the element is less than the one preceding it
3. Place element after an element that it is greater than or first element
4. Repeat with all unsorted sections of array
