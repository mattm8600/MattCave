**Definition:** A class defined inside the scope of another class
- Can directly access all fields and method from outside class and vice versa
- Inner class has an association to the object of its outer class
	– Must be Instantiated with an outer class object

Ex: Literally just any class declared inside another class

Use Cases:
- Private Helper Classes
- Their automatic link to outer class (everything in inner is tied to outer)

Instantiation:
- Inside class: `a = new InnerClass()`
- Outer class: `a = b.new InnerClass()` where b is outer class

- Static nested class is a static inner class
	– Has no link to outer class instance
	– Can only access static fields and methods of outer class

Static objects can return an instance to their outer class
```
public OuterClass getOuter() {
	return OuterClass.this;
}
```
