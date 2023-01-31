**Abstract Methods:** Similar to a method in an interface. Subclasses must implement the method.
- Have no method bodies and use "abstract": `public abstract void draw() {`

**Abstract Classes:** A class with abstract methods `public abstract class Shape {`
- Objects of an abstract class can't be instantiated
	-- Non-abstract subclasses can be instantiated (and referred to by a super class)

Ex:
```
1 public abstract class AbstractProgression { 
2 protected long current; 
3 public AbstractProgression( ) { this(0); } 
4 public AbstractProgression(long start) { current = start; } 
5 
6 public long nextValue( ) { // this is a concrete method 
7 long answer = current; 
8 advance( ); // this protected call is responsible for advancing the current value 
9 return answer; 
10 } 
11 
12 public void printProgression(int n) { // this is a concrete method 
13 System.out.print(nextValue( )); // print first value without leading space 
14 for (int j=1; j < n; j++) 
15 System.out.print(" " + nextValue( )); // print leading space before others 
16 System.out.println( ); // end the line 
17 } 
18 
19 protected abstract void advance( ); // notice the lack of a method body 
20 }
```