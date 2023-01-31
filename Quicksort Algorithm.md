**Approach:** Partition the array and sort recursively
- Uses [[Recursion]]

Ex:
![[Pasted image 20221213204910.png]]

Code:
```
void quickSort(int[]a, int x, int y) {
	int pivotIndex;

	if(x<y) {
		pivotIndex = partitionList(a,x,y); //Sort first element, get it's index
		quickSort(a,x,pivotIndex-1); //Sort all the elements under it recursively
		quickSort(a,pivotIndex_1,y); // Sort all the elements after it recursively
	}
}

int partitionList(int[] a, int x, int y) {
	int left = x, right = y - 1, pivot = a[y];
	//Pivot is farthest right index, start at left and right ends (one before pivot)
	while (left <= right) { //When this is broken it means we are done with this run
		while(left<=right && a[left] <= pivot) {
			left++; //Go to the right until the value is greater than the pivot
		}
		while(left <= right && a[right] >= pivot) {
			right--; //Go to the left until the value is less than the pivot
		}
		if(left < right) { //Swap these values, elements less than will be on left
			swap(a,left,right); //and elements right than will be on right of left
		}
	}
	swap(a,left,y); //Swap the pivot and the left value aka put pivot in it's spot
	return left; //Return pivot's new location so it can run again on both sides of it
}
```

Trace:
1. Run `partitionList` with a pivot
2.  We swap all the values less and greater than the pivot, so they are on the left and right sides
3. Once our left and right pointers cross, it means that all the less than the pivot are on the left, all the greater than pivots are on the right
4. This means our pivot is now in the correct position!
5. Now run the same algorithm on the sublists to the left and right of the pivot
6. Concatenate all the results into one list