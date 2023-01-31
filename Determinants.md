**Determinants** are scalar values that are a function of the entries of a *square* matrix

## Ways to solve for determinants
1. Cofactor Expansion → Basically the same as a 3d cross product except you can do it across any row or column
	– Ex:
	![[Pasted image 20221218145350.png]]

The signs alternate in cofactor expansion between positive and negative
![[Pasted image 20221218145532.png]]
- Cofactor expansion can be really useful when there are a bunch of zeros in the matrix


2. Determinant of a 2d matrix:
	– Equals $ad-bc$ where $\begin{bmatrix} a & b \\ c & d \end{bmatrix}$

3. If $A$ is a triangular matrix, then $detA$ is the product of the entries on the main diagonal of $A$

4. You can row reduce a matrix into a triangular matrix then use (3) to find determinant
	– Row reductions change the determinant:
	- If a multiple of one row of $A$ is added to another row to produce matrix $B$ then $det B = det A$
	- If two rows of $A$ are interchanged to produce matrix B then
		$det B = -det A$
	- If one row of $A$ is multiplied by $k$ to produce $B$ then
		$det B = k detA$
	Ex:
	![[Pasted image 20221218150133.png]]


### ### A square matrix $A$ is invertible iff $det A \neq 0$
See [[Inverse of a Matrix]]


## Other Operations and Determinants
Taking the transpose of a (square) matrix also change its determinant
#### If $A$ is an $n \times n$ matrix, then $det A^T = det A$
- ^ Ex: if n is 1, the determinants are obviously equal

Multiplying matrices doesn’t change its determinant either
### If $A$ and $B$ are $n \times n$ matrices, then $det AB = (det A)(det B)$
