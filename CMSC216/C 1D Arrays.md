Array Name → **Pointer Constant** to the address of the first element of array
- Ex: `int b[10]`, Array name is a constant pointer to an int

ARRAYS AND POINTERS ARE NOT THE SAME
- Array has defined number of elements
- Only when array name is used in expression that compiler generates pointer constant
	– Note: Pointer substitution does not occur with `sizeof` and `&`

Note: `c=&a[0];` and `c=a;`

## Array Subscripts
`array[subscipt] = `