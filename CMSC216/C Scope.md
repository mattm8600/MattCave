**Scope** is the visibility of a variable in a program

### Types of Scope:
- Block Scope → Visibility within a code block (or nested code blocks)
- File Scope → Identifiers outside of code blocks have scope across the whole file
- Prototype Scope → Applies only to argument names in prototypes 
	– (don’t use the same name in the same prototype)


Question: What if you have two things of the same name in different files?
### Types of Linkage
- Internal Linkage → All Declarations within one source file refer to one entity
- External Linkage → All Declarations across source files refer to one entity
- None → All declarations are individual

Ex:
![[Pasted image 20230305223623.png]]
- b, c, and f are external (Global variable or function name)
- Everything else has no linkage (a, d, g)

### Switching Linkage
- `static` keyword → Gives something with external linkage internal linkage
- `extern` keyword → Gets access to an entity defined somewhere else
	–  You need to use it when declaring a variable in a different scope to access it from another file

### Storage
- Automatic Storage → Remains in memory only while it is in scope
- Static Storage → Remains in memory while the program is executing