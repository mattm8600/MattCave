**Throw:** Generates an exception
- Note: only use exceptions for rare and incorrect events
- Ex: `throw new exceptionType(params);`

**Throws:** Declares that a method may be thrown in a method signature
- Ex: `public static int parseInt(String s) throws NumberFormatException`
	– If multiple exceptions are thrown use commas
- Use when you want to propagate the error to the Caller instead of dealing with it locally