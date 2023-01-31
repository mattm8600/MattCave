**Definition:** Writing code that can be used with different types of data

**Generic Classes:** Putting one or more “type” variables in name
Ex: `class MyGeneric<E> {`
- Provides abstraction over types
-  You can limit the types that go into the class by using the extends keyword
	–Ex: ` class MyGeneric2<t extends Vehicle> {` // Only a Vehicle or Vehicle subclass can be used
- Usually can’t put an array into a Generic class

**Using a Generic Class:** Must give an actual type for each type variable
- Wildcard Type Parameters - Represents an unknown type (used to soften restrictions on params)
	– Ex: `ArrayList<?>` is an arrayList with any type
	– `ArrayList<? extends Vehicle>` arrayList with a vehicle or subclass of Vehicle
	– `ArrayList<? super vehicle` arrayList with a vehicle or superclass of Vehicle
		– Just adds some more flexibility in what can be inputted into generic method

**Instantiating Generic Class:** 
`Generic<Integer> m = new Generic<>();`

Ex:
```
public class Portfolio<T> { 
T[ ] data; 
public Portfolio(int capacity) { data = new T[capacity]; 
// illegal; compiler error 
data = (T[ ]) new Object[capacity]; // legal, but compiler warning 
}
public T get(int index) { return data[index]; } 
public void set(int index, T element) { data[index] = element; } }
```

Advantages:
- Reduces duplicative code
- You can only add objects of the correct type to a Generic Class
- Elements returned from a Generic class are checked at Compile Time not Run Time