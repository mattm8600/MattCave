**Approach:** Sort sublists from greatest to lowest and then merge them into a result list
- Uses [[Recursion]]

Ex:
![[Pasted image 20221213214055.png]]

Code:
```
void mergeSort(int[] a, int x, int y) {
	int mid = (x+y)/2;

	if(x != y) {
		mergeSort(a,x,mid);
		mergeSort(a,mid+1, y);
		merge(a,x,y,mid);
	}
}

void merge(int[] a, int x, int y, int mid) {
	int j=0, left = x, right = mid + 1;
	int[] tmp = new int[a.length];
	
	while(left <= mid || right <= y) {
		if(right > y || left <= mid && a[left] < a[right])) {
			tmp[j++] = a[left++];
		}
		else {tmp[j++] = a[right++]; }
	}
	for(j=0; j < y - x + 1; j++) {
		a[x+j] = tmp[j];
	}
}
```

Trace:
1. Continuously divide the array in half until we are left with individual items
2.  Sort pairs of elements into smaller sorted lists
3. 