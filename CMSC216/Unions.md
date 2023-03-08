**Def:** Similar to [[Structures]], but all members of the union refer to the *same location* in memory

**Usage:** Create a structure with an enum for which data is selected and then a union with said data
- Allows you to store multiple different types and also know what's stored there

Memory is stored inefficiently - takes up the size of the biggest member

### Initialization:
```c
union {
	int a;
	float b;
	char c[4];
} x
```

