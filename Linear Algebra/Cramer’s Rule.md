**Cramer’s Rule** uses [[Determinants]] to solve a linear system.

**Definition:** Let $A$ be an invertible (see [[Inverse of a Matrix]]) $n \times n$ matrix. For any $\vec b$ in $\mathbb{R}^n$, the unique solution of $A \vec x = \vec b$ has entries given by: $$x_i = \frac{detA_i(\vec b)}{det A}$$
where $A_i(\vec b) = [a_1 ... \vec b ... a_n]$ . $i$ signifies the column that $\vec b$ replaces

Ex:
![[Pasted image 20221218151747.png]]
![[Pasted image 20221218151755.png]]

NOTES:
- Probably useful when you can’t use matrix inverse to solve a problem
- Not very efficient for large matrices (you would row reduce a bunch of times instead of just once)