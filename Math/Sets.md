**Definition:** A data type where elements have no relationship between them
- Sets are just a collection of elements without order or duplicates

Java has a set interface, but there are three common Java classes that implement it
#### Methods:
- `boolean add(E element)` → Inserts an element into the set
- `boolean contains(Object o)` → Tests whether o is in the current object set
- `boolean remove(Object element)` → Deletes object, returning true if successful
- `int size()` → Returns # of elements in set
- `void clear()` → Removes all elements from set
- `boolean isEmpty()` → Returns true if the set is empty
- `Iterator<E> iterator()` → Returns an iterator reference for the set
- `boolean addAll(Collection<> extends E> c)` → Adds all of Cs elements to current object set
- `boolean containsAll(Collection<?> c)` → Returns true if all of Cs elements are in the set

### Common Java Sets
- HashSet → A set that using hashing, requiring the elements implement the hashCode() method
	– Iteration of elements is in no predictable order
- LinkedHashSet → A hash set that orders elements in the order they were added
	– Also has an internal doubly linked list
	– requires more memory than HashSet
- TreeSet → Uses a binary search tree to store elements
	– Elements are iterated in increasing order


