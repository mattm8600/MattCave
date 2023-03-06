**C Mechanism** that lets you define new names for various data types
- Is able to handle pointer types

Ex: 
### `typedef char *ptr_to_char`
- Declares identifier `ptr_to_char` to be a new name for a pointer to a character

Using typedefs for complex declarations can reduce errors
- Note:  `#define` doesn’t let you handle pointers