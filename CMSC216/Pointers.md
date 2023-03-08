Remember from [[C Operators]] that the `&` operator returns the memory address:
- Initialize pointers by making them point to the memory address
- Ex: `float *e = &c` ← Points to c

### Dereference Operator
Following a pointer to the location it points to → **dereferencing**
- Use the `*` operator
Be careful representing pointers with arrows
- They are only pointing to the value when dereferenced - Otherwise they just point to their memory address
- Arrow points to the **location**, not the value at the location
- You can only dereference pointer data types
- The dereference operator goes from right to left


### Mistake: Pointer points to no memory location
![[Pasted image 20230307013857.png]]
- Creates pointer `a`, and stores 12 to the location that `a` points to
	– `a` has no memory address!!! This will fail

### Null Pointer
**Null pointers** don’t point to anything
- Specifies when a pointer doesn’t point to anything
- You can also return pointers pointing to null if something wasn’t found (for example)

### Pointers to Pointers
You can point pointers to pointers
![[Pasted image 20230307014759.png]]
	– Pointer points to where the pointer is stored in memory
	– Equivalent to `*(*c)`
	– `*c` takes us to location where c points (variable b)
	– `**c` takes us to where b points which is variable a

### Constant Pointers
You can declare a constant pointer by following this syntax:
`type * const ptr`
- Note that dereference operator operates from right to left
- Therefore since `const ptr` is to the right it makes a constant pointer
Note:
`type const * ptr` → This is a pointer pointing to a constant variable