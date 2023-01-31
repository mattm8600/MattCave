**Definition:** Transforming a key into another value (typically an index in a hash table)


Hash function → A function that makes a key to an integer
	– Value produced is called a hash code
Compression function → Makes the hash code into an index of a hash table
Ex:
```
hashFunction(UID) = UID;
compressionFunction(n) = n % 4
```

Collisions → When multiple keys hash to the same location on a hash table
How to Handle collisions:
1. Bucket or Chained Hashing:
	– Each element of hash table stores a collection of values that have the same index
2. Linear Probing:
	– When there is a collision, put the element in the next empty element
	– When an element is deleted put a “defunct” value, or else anything hashed past it won’t be found
	– Lookup must keep examining situations until it finds the value or an empty index
3. Double Hashing:
	– If there’s a second collision, run a second hash function that tells you how far over to check for the next open spot
	– If you run into defunct, keep going until there’s an empty spot (check for duplicate) then put in delete

Properties of a good Hash Function:
1. Scatters values as uniformly as possible
2. Is not expensive to compute

Hash Function Examples:
- Choose a subset of digits of key
- Square the key and perform digit selection on result
- Move some of the bits from the left of key to the right
- (For non integer types) treat the bits of the key as integers

Clustering - When the hash function outputs the same elements and the hash table becomes less efficient

NOTE: Choose a prime number for hash table sizes so probing can shift through elements well