**Structures** are an *aggregate* data type → Holds more than one piece of data at a time (see [[C Data Types]])

**Definition:** A structure is a collection of values called members
- Similar to a class in Java with only fields

Structures are not arrays: Cannot use subscripts, name of structure is not replaced with pointer
- Structure variables are scalars
- Can be passed as arguments to functions, returned by functions, etc

### Declaration:
```c
struct {
	int a;
	char b;
	float c;
} x;
```
- Members can be arrays, pointers, simple types, structures

To make a structure declaration repeatable, use `typedef`
```c
typedef struct {
	int a;
	char b;
	float c;
} Simple;
```
- Include this at either the top of the file or the header file

### Accessing Members
- You can access members using `.` operator
- `->` operator - is used for pointing to a member of a structure


Structures store each member one after and another
- May have gaps in between due to Natural Alignment
- Total Structure memory doesn’t necessarily equal the sum of member’s storages

