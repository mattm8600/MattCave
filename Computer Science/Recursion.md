**Definition:** Recursion is a strategy to solve problems where a method calls itself
Approach:
- If a problem is trivial, solve it directly → Base Case
- Otherwise break it into smaller instances of the same problem, and call the algorithm again to solve each instance
	– Then combine the solutions in a way that solves original problem

**Advantages:**
- Natural for backtracking searches
- May be simpler than iteration depending on the problem
**Disadvantage:** Usually less efficient than iterative (overhead of recursive method calls)

Each method invocation gets its own stack space (i.e. its own local variables)

Many problems require recursive helper methods
→ Strategy: Have the original method set up the recursion
	→ Then helper method contains arguments needed at each recursive step

Ex: Compute sum of an array of integers:
```
2 public static int linearSum(int[ ] data, int n) { 
3 if (n == 0) //Base Case
4 return 0; 
5 else 
6 return linearSum(data, n−1) + data[n−1]; //Recursive Step
7 }
```
NOTE: A lot of times you can “store” the result by just returning a value with the return statement 
- Ex: return methodCall() + 1

Forms of Recursion:
- Tail recursion - Recursive call is the very last thing performed
- Non-Tail Recursion - Recursive call is not performed last in the method

WARNING: Avoid calling the recursive call excessively, it will make your algorithm inefficient