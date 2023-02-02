A **linear equation** takes the form of $a_1x_1 + a_2x_2 + … + a_nx_n = b$
- x is variables, $a_n$ is their coefficients

A **system of linear equations** is a set of linear equations, either has…
1. No solution (System is **Inconsistent**)
2. One solution (System is **Consistent**)
3. Infinitely many solutions (System is **Consistent**)

To solve systems of linear equations, use row reductions in the matrix
1. Replace one row by the sum of itself and a multiple of another row
2. Interchange two rows
3. Multiply all entries in a row by a nonzero constant
- If two linear systems are row equivalent (aka the same after row operations) then they have the same solution set



## Solutions of Linear Systems:
When a system has an infinite number of solutions, you can parameterize it by a few variables:
- Basic Variable → A variable that corresponds to a pivot column (depends on the free variables)
- Free Variable → A variable that can be an infinite number of solutions

Ex:
![[Pasted image 20221217174206.png]]     becomes      ![[Pasted image 20221217174215.png]] 
- $x_1, x_2$ are **basic variables** (have a pivot in their column)
- $x_3$ is a **free variable** (no pivot) and can make a different solution with any value