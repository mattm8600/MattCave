**Definition:** If A is an $m \times n$ matrix and B is an $n \times p$ matrix, then the product AB is the $m \times p$ matrix whose columns are $AB_p$
#### $AB = A[b_1, b_2 ... b_p] = [Ab_1 Ab_2 ... Ab_p]$
Ex:
![[Pasted image 20221218133510.png]]

The number of **columns** must match the number of **rows** to multiply the matrices
Ex: you can multiply a $3 \times 5$ matrix by a $5 \times 2$ matrix.
- The Last of the first must match the first of the second to multiply
- Creates a matrix of the rows of A and the columns of B (first x last overall)
	– Ex would have a $3 \times 2$ matrix

### $AB$ does NOT equal $BA$
- You might not be able to multiply them both ways based on the matrix sizes

### Actually Remembering how to Multiply Matrices
![[Pasted image 20221218200520.png]]
- Take the dot product of the rows of $A$ and the columns of $B$
- Then put the result in the row # of $A$ and column # of $B$