**Efficiency Definition:** How many resources are used by an algorithm

Asymptotic Analysis: Mathematically analyze efficiency and express its running time as a function of input size
- The best way to measure efficiency

**Big-O Notation:** Represents the upper bound on the number of operations performed by an algorithm

Complexity Categories from most efficient to least efficient
| Complexity | Name        | Examples                  |
| ---------- | ----------- | ------------------------- |
| O(1)       | Constant    | Add elt. to front of list |
| O(log(n))  | logarithmic |                           |
| O(n)       | Linear      | Max of unordered array    |
| O(nlog(n)) | n log n     |                           |
| O(n^2)     | quadratic   | 2D matrix addition        |
| O(n^3)     | Cubic       | 2D matrix multiplication  |
| O(n^k)     | Polynomial  |                           |
| O(k^n)     | Exponential |                           |
| O(n!)      | factorial   | Stupid sort               |
| O(n^n)     | n to the n  |                           |

The highest complexity category determines the complexity for large numbers of data sets
- Ex: $T(n) = .5nlog(n) + 10n$ is approximately $O(nlog(n))$

Crucial Section - Section of code that dominates the overall execution time (highest complexity)

## Examples:

### Example 1
```
A
for(i=0, i < n; i++) {
	B
}
C
```
Execution: A → once, B → N, C → once
$T(n) = 1 + N + 1 = N+2$
$O(n)$

### Example 2
```
A
for(i = 0; i < n; i++) {
	B
	for(k = 0; j<n; j++) {
	C
	}
}
D
```
Execution: A → Once, B→ n, c→ n^2, D → Once
$T(n) = 1 + n + n^2 + 1 = n^2 + n  + 2$
$O(n^2)$

### Example 3
```
for(int i=0; i<n; i++) {
	for(j=0; j<n; j++) {
	A
	}
for(i=0; i<n; i++) {
	for(j=0; j<n; j++) {
	B
	}
}
}
```
Execution: A→ n^2, B → n^2
$T(n) = n^2 + n^2 = 2n^2$
$O(n^2)$

### Example 4
```
A
for(i=0; i<n; i++) 
	for(j=0; j<10000; j++)
```
Execution: A→ once, B→ 10000n
$T(n) = 1 + 10000n$
$O(n)$

### Example 5
```
k = 1 //A
while(k < n) {
k = 2*k; //B
}
C
}
```
Execution: A → Once, B→ log(n), c→ Once
$T(n) = 1+ log(n) + 1 = log(n) +2$
$O(log(n))$
- Note: Log is computer science is usually log base 2

### Example 6
```
void f(int[] arr, int pos) {
if (pos>= arr.length)
	A
else
	B + f(arr,pos+1)
}
```
Execution: A → Once, B→ n-1, Recursive Call → n-1
$T(n) = 1 + n-1 + n-1 = 2n-1$
$O(n)$
- Note count recursive calls as an operation too

## Types of Case Analysis
Best Case - Smallest # of operations required
- Ex: if an element searched for happens to be the first element
- Not useful
Worst Case - Largest # of operations required
- Ex: if an element searched for happens to be last element
Average Case - # of operations for typical case 
- Average Case -Average among all possible cases assuming they have the same likelihood
- Expected Case - Weight ed average over all possible cases based on the likelihood of each