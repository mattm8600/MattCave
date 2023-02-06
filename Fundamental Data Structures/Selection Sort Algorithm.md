**Approach:** Repeatedly go through the list, swapping with the smallest element of the group
![[Pasted image 20221213184921.png]]

Code:
```
void selectionSort(int[] a) {
	int outer, inner, min;

	for(outer = 0; outer < a.length -1; outer ++) { //Create unsorted sections
		min = outer; //Default min to first value in unsorted
		for(inner = outer + 1; inner < a.length; inner++) { //Iterate through unsorted
			if(a[inner] < a[min]) { //Find the lowest value
			min = inner;
			}
		}
		swap(a,outer,min); //Swap first unsorted index with lowest value
	}
}
```
Trace:
1. Iterate through unsorted section, set first index to min
	– If an element in the unsorted section is less than min, set it to min
2. Swap the first unsorted element with min
3. Repeat for each iteration of the unsorted index