This is an interface that allows you to iterate through the elements of a custom data type
- Already integrated into [[Collections]]

NOTE: The first time you call next it returns the first element

Interface:
```
public interface Iterator<E> {
boolean hasNext();
E next();
void remove(); //Optional
}
```

- Allows you to move through objects without knowing internal representation

- Calling an iterator
```
ArrayList<Car> myCars = new ArrayList<Car>();
Iterator<Car> iter = myCars.iterator();
```

Typical Iteration using iterator
```
while(hasNext())
{
doSomething(next())
}
```

