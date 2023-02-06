**Definition:**  [[Linked List]] that use subclasses to represent an empty or nonempty list

Ex:
```
interface list {
NonemptyList insert(Object data);
}

class EmptyList implements List {
NonEmptyList insert(Object data);
}

class NonEmptyList implements List {
Object data;
private List next; //Can refer to either empty or nonempty list object
NonEmptyList insert(Object Data);
}

```

^This example uses EmptyList to represent an empty or end of list rather than null
- No null checks needed