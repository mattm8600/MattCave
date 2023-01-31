**Definition:** Diagonalization is a useful factorization of a matrix A following the form:
## $A = PDP^{-1}$
where D is a diagonal matrix

You can find $A^k$ easily by diagonalizing it and then doing $A^k = PD^kP^{-1}$

### Diagonalization Theorem:
An $n \times n$ matrix $A$ is diagonalizable if and only if $A$ has $n$ linearly independent eigenvectors
- The **columns** of $P$ are eigenvectors
- The Diagonal entries of D are eigenvalues corresponding with $P$

You can have eigenvalues with multiplicity greater than 1, but you still need n independent eigenvectors

#### Diagonalization Steps:
1. Find the eigenvalues of A (See [[Eigenvalues and Eigenvectors]])
2. Find the linearly independent eigenvectors of A
3. Construct $P$ and $P^{-1}$ from the vectors in (2)
4. Make D from eigenvalues (in same order as $P$)

