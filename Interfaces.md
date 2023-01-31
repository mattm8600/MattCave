**Definition:** An interface is a contract that a class implementing it must include
- Contains Constants, Method Signatures WITHOUT data or bodies
- You can include any number of interfaces in a class
- Use the `implements` keyword to use it with your class

- Ex:
```
/∗∗ Interface for objects that can be sold. ∗/ 
2 public interface Sellable { 
3 
4 /∗∗ Returns a description of the object. ∗/ 
5 public String description( ); 
6 
7 /∗∗ Returns the list price in cents. ∗/ 
8 public int listPrice( ); 
9 
10 /∗∗ Returns the lowest price in cents we will accept. ∗/ 
11 public int lowestPrice( ); 
12 }
```

```
public class Photograph implements Sellable { 
3 private String descript; // description of this photo 
4 private int price; // the price we are setting 
5 private boolean color; // true if photo is in color 
6 
7 public Photograph(String desc, int p, boolean c) { // constructor 
8 descript = desc; 
9 price = p; 
10 color = c; 
11 } 
12 
13 public String description( ) { return descript; } 
14 public int listPrice( ) { return price; } 
15 public int lowestPrice( ) { return price/2; } 
16 public boolean isColor( ) { return color; } 
17 }
```