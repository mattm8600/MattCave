**Compilation** converts source code to machine code that the processor can run
Basic flow:
- Source code converted to object code in compiler
- Object files (and any standard C libraries used) are combined into an executable using the linker

![[Pasted image 20230305192817.png]]

Phases of Compilation Process:
1. Preprocessor
	- Substitute text identifiers from `#define`
	- Reading / inserting the text files that from `#include`
2. Parse Meaning
	- Figure out meanings of statements
	- Throw warnings / errors if necessary
3. Generate Object Code
	- Generates preliminary form of object code
	- Not directly executable - needs to be linked (usually)

## C Filename Conventions
- Source files (.c) → Contain functions and commonly related definitions
- Header files (.h) → Contain only definitions

