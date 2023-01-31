**Definition:** A symmetric matrix is a matrix A such that $A^T = A$ 
- Matrix has to be square

Ex:
![[Pasted image 20221218195858.png]]
^ First row and column are the same, symmetrical about diagonal for the rest

If $A$ is symmetric, then any two eigenvectors from different eigenspace are orthogonal
- Easy to find orthonormal basis of an eigenspace

An $n \times n$ matrix $A$ is orthogonally diagonalizable iff $A$ is a symmetric matrix.

### Orthogonal [[Diagonalization]]
#### $A = PDP^T = PDP^{-1}$
- This only works if A is a symmetric matrix.

### Spectral Theorem of Symmetric Matrices:
An $n \times n$ symmetric matrix $A$ has the following properties:
1. $A$ has $n$ real eigenvalues, counting multiplicities
2. The dimension of the eigenspace for each eigenvalue $\lambda$ equals the multiplicity of $\lambda$ as a root of the characteristic equation
3. The eigenspaces are mutually orthogonal, in the sense that eigenvectors corresponding to different eigenvalues are orthogonal
4. $A$ is orthogonally diagonalizable