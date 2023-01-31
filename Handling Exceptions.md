**Definition:** Program performing an action in response to a detected error
- Ex: Print error message, terminate program, request new input, retry operation
	– You can exit the program by using `System.exit(-1);`

Informing the Caller - Throw an exception for the caller to deal with
- Or handle exceptions locally:
Ex:
```
void g() {
if (seomthing bad happens)
	throw new ExceptionType();
}

void f()  {
try {
g();
} catch (ExceptionType e) {
  *** Do something ***
	}
}
```

Java Exceptions: Either Checked or Unchecked:
- Checked Exceptions → Must be handled by the program
- Unchecked Exceptions → Serious errors that programs typically don’t handle
- Examples: IOException, IllegalArgumentException, NullPointerException

**Try Block:** Tries running statements that may throw an exception
**Catch Block:** Specifies an exception type and code to be used when the exception is thrown
- A try block can have multiple Catch Blocks for different exceptions
**Finally Block:** Placed after try and catch blocks - used to cleanup code executed by catch blocks
- ALWAYS EXECUTED