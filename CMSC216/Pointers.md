Remember from [[C Operators]] that the `&` operator returns the memory address:
- Initialize pointers by making them point to the memory address
- Ex: `float *e = &c` ← Points to c

### Dereference Operator
Following a pointer to the location it points to → **dereferencing**
- Use the `*` operator
Be careful representing pointers with arrows
- They are only pointing to the value when dereferenced - Otherwise they just point to their memory address
- Arrow points to the **location**, not the value at the location


### Mistake: Pointer points to no memory location
![[Pasted image 20230307013857.png]]
- Creates pointer `a`, and stores 12 to the location that `a` points to
	– `a` has no memory address!!! This will fail

### Null Pointer
**Null pointers** don’t point to anything
- Specifies when a pointer doesn’t point to anything
- You