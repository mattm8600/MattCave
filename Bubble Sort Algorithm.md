**Approach:** Repeated sweep through shrinking portions of the list elements remaining to be sorted
	– Swap an element x with the element following it if x is larger

Ex:
![[Pasted image 20221213184010.png]]

Bubble Sort Code:
```
void bubbleSort(int[] a) {
int outer, inner;
for(outer = a.length-1; outer > 0; outer--) {  //Create each unsorted section
	for(inner = 0; inner < outer; inner++) { //Iterate through unsorted section
		if(a[inner] > a[inner+1]) { //If a value is out of order...
		swap(a, inner, inner+1) // Swap it with the next element
		}
	}
}

}
```
Trace:
1. Start with the whole array and if an element is greater than the next element, swap them
	– The greatest element should now be at the end
2. Iterate through the remaining unordered section (everything except the last element)
	– Put that greatest element at the end
3. Repeat until the entire array is sorted
