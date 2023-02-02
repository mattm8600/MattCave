The **inverse** of an $n \times n$ matrix A satisfies this equation:
## $A^{-1}A = I$
or
## $AA^{-1} = I$
where $I$ is the [[Identity Matrix]]

- If the matrix isn’t square you can’t take the inverse of it
- A matrix is **invertible** if there is a matrix C where $AC = I$
	– If there is no inverse it is called a *singular matrix*

A matrix is invertible iff $det A \neq 0$

If the matrix is invertible, then the solution for $A \vec x = \vec b$ has the solution $A^{-1}\vec b$

## To find the inverse of a matrix
1. Create an augmented matrix $\begin{bmatrix} A & I \end{bmatrix}$
2. Use elementary row reduction until $A$ becomes $I$
3. Your result is: $\begin{bmatrix} I & A^{-1} \end{bmatrix}$

Ex:
![[Pasted image 20221218140310.png]]
