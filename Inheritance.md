
- **Definition:** Inheritance is organizing structural components of a package in a hierarchical fashion
- **Application:** Extend a class from another in Java to inherit all methods from the super class class
``` class SubClass extends SuperClass ```
	--  Adds different methods and fields in addition to the super class'

- NOTE: Java only allows one super class for a class
	-- All classes automatically inherit from Object Class

- Constructors are NEVER inherited in Java
-- Subclass constructor implicitly calls its super class' default constructor
-- To use the super class constructor use:
	` Super(param1, param2); `
	-- Super can also be used to call a super class version of a method

- Polymorphism - Super class objects can refer to any subclass object
	-- Ex: Vehicle is a super class, Car and Bus and Bike are subclasses
```   
Vehicle v = new Vehicle();
Car c = new Car();

v = c;  // Valid, a super class object can refer to a subclass reference
v = new Car(); // Also valid
c = v; //Not valid, subclasses can't refer to superclass objects
c = new Vehicle(); //Also not valid 
```

- `reference instanceof Class` - Returns true if the object the reference is referring to is of type class name
- `ref.getClass()` - returns a reference to a class that can be compared with other classes
⇾ Using instanceof or getClass() is poor design, just overload methods instead

- Super classes (even if referring to subclass) can only reference things visible to the super class
	-- Subclasses can't directly access super class private fields

- Method Overriding - Using the same method name / signature as a super class method
	-- Java uses the subclass method whenever applicable
	-- An overridden method can't have a more restrictive access type
	-- Class inherits a method from the nearest super class when overridden

- Final Keyword - Cannot be extended (applies to classes, methods, fields)

You can only downcast a superclass to a subclass if it is a subclass object with a superclass reference
Ex:
```
Instrument y = new Piano();
(Piano y).play() //Valid
Instrument x = new Instrument();
(Piano x).play() //Invalid
```

Super Class Reference to a subclass:
- Can use overwritten subclass objects
- Cannot use different subclass methods without casting