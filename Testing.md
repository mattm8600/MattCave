
Types of Errors:
1. Compile-time Errors $\rightarrow$ Syntax errors or type mismatch problems
2. Runtime Errors $\rightarrow$ Operations that are illegal or impossible to execute (Exceptions)
3. Logic Errors $\rightarrow$ Your coding logic is wrong

Testing
- Coverage → How much code is executed by the test cases
	– Goal: Write the minimum set of tests that achieve acceptable coverage
	1. Line / Statement Coverage → Percentage of lines executed by tests
	2. Branch Coverage → Percentage of conditions executed by tests
	3. Path Coverage → Percentage of execution sequences executed by tests
	– Ex:
```
if(x)
a = 1;
if (y)
b = 2;
```
| Coverage Type | Minimal set of Tests              |
| ------------- | --------------------------------- |
| Statement     | ` x = true, y = true`             |
| Branch        | `(x = true, y = true), (x=false, y = false)` |
| Path          | `(x = true, y = true), (x = false, y = true), (x = true, y = false), (x = false, y = false)`              |                                  |
