**Definition:** Refers to rearranging a list of elements in order, based on the key for each element
	– Really important →

Types of Sorting Algorithms:
- Comparison Sort → Only uses pairwise key comparisons
- Linear sort → Doesn’t use key comparisons
	– More efficient, but requires addition information

Sorting Algorithm Properties:
- Stable Sort → Preserves the original order of duplicate keys
- In-place → Only uses a constant amount of additional memory
- External sort → Sorts data that’s not all in memory at the same time

Different Sorting Algorithms:
- [[Bubble Sort Algorithm]]
- [[Selection Sort Algorithm]]
- [[Insertion Sort Algorithm]]
- [[Tree Sort Algorithm]]
- [[Heap Sort Algorithm]]
- [[Quicksort Algorithm]]
- [[Mergesort Algorithm]]
- [[Counting Sort]]
- [[Radix Sort]]

| Name      | Comparison Sort | Average Case Complexity | Worst Case Complexity | Can be in-place | Can be stable |
| --------- | --------------- | ----------------------- | --------------------- | --------------- | ------------- |
| Bubble    | [x]             | $O(n^2)$                | $O(n^2)$              | [x]             | [x]           |
| Selection | [x]             | $O(n^2)$                | $O(n^2)$              | [x]             | [x]           |
| Insertion | [x]             | $O(n^2)$                | $O(n^2)$              | [x]             | [x]           |
| Tree      | [x]             | $O(n^2)$                | $O(n^2)$              |                 |               |
| Heap      | [x]             | $O(nlog(n))$            | $O(n^2)$              | [x]             |               |
| Quick     | [x]             | $O(nlog(n))$            | $O(n^2)$              | [x]             |               |
| Merge     | [x]             | $O(nlog(n))$            | $O(nlog(n))$          |                 | [x]           |
| Counting  |                 | $O(n)$                  | $O(n)$                |                 | [x]           |
| Radix     |                 | $O(n)$                  | $O(n)$                |                 | [x]           |

