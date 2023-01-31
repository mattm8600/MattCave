**Definition:** A set of keys which each have values. The key is used to look up, modify, or delete their associated value.
![[Pasted image 20221213174739.png]]
- Keys HAVE to be unique, values do not.
- Different keys can map to the same value

### Methods:
- `V put(K key, V value)` → Inserts key into map with its corresponding value. 
	– If key is already in map, it replaces value
- `V get(Object key)` → Returns value associated with the key in the object map
- `V remove(Object key)` → Removes key and its associated value
- `boolean isEmpty()` → self-explanatory
- `int size()` → Returns the number of key/value pairs in the map
- `void clear()` → Removes all key/value pairs
- `boolean containsValue(Object value)`  → Returns true if the value is in the map
- `boolean containsKey(Object key)` → Same thing but for key
- `Set<k> keySet()` → Returns a set of all the keys
- `Collection<V> values` → Returns a collection of the values

### Three Map Classes in Java
- HashMap → Implements a map using hashing
	– Elements must implement hashCode()
- LinkedHashMap → HashMap that supports ordering of elements in the order they were added
- TreeMap - Elements are iterated over in increasing order of keys