**Approach:** Sorts keys with values over range 0…k
1. Count occurrences of each key
2. Calculate # of keys that are less than or equal to each key
3. Place keys in sorted location using # of keys counted -1
![[Pasted image 20221214001342.png]]

Code:
```
void countSort(int[] a, int k) { //k is last value of k
	int[] b = new int[a.length],  //create temp array of all counts
			c = new int[k+1];

	int i;
	for(i=0; i<k; i++) { //initialize temp array
		c[i] = 0;
	}
	for(i=0; i<=k; i++) { //count # of keys
		c[a[i]]++;
	}

	for(i=1; i<= k; i++) { //count the # of keys <= value i
		c[i] = c[i] + c[i-1];
	}

	for(i= a.length-1; i >= 0; i--) { //move keys to proper location
	b[c[a[i]]-1] = a[i];
	c[a[i]]--;
	}

	for(i=0; i<a.length; i++) { //copy sorted list to a
	a[i] = b[i];
	}
}
```
