What happens when a function is compiled?
1. Generates code to pass arguments and call function
2. Code to receive values passed back by function

## Function Prototypes
**Prototypes** give the compiler information about the function name, arguments, and return value
- Note: You don’t *need* a prototype if the function is defined before it is called

Include prototypes at the beginning of a source file or [[Header File]]
- Also acts as a check to see if your prototype isn’t mistyped


When a function has no prototype - C assumes the return type is an integer

## Function Arguments
All function arguments are passed in via *call by value*
- Function gets a copy of the argument value

If an array name is an argument, the function will change the values of the array
- Value of array name is a pointer (array names are basically [[Pointers]])
- Subscript is a form of indirection that access an element using [[Pointer Arithmetic]]



