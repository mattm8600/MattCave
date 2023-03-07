Array Name → **Pointer Constant** to the address of the first element of array
- Ex: `int b[10]`, Array name is a constant pointer to an int

ARRAYS AND POINTERS ARE NOT THE SAME
- Array has defined number of elements
- Only when array name is used in expression that compiler generates pointer constant
	– Note: Pointer substitution does not occur with `sizeof` and `&`

Note: `c=&a[0];` and `c=a;`

## Array Subscripts
`array[subscipt] = *(array + (subscript) )`
- Subscripts do pointer addition to produce a pointer to the desired element


When you send an array name into a function:
- Copies the pointer value as the argument
- Subscripts perform indirection
- Compiler accepts pointer or array declaration as function parameters
	– `int fn(char *string)` or `int fn(char string[])`

### Initialization
`int vector[5] = {1,2,3,4,5}`
- Initializer needs to match the array size
- You can also exclude the array size in declaration, and it will size to initializer
`char message[] = "hello";` 
- You can declare a character array with a string initializer or normal initializer

