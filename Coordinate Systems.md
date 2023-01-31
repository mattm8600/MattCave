The **coordinates of x relative to the basis $\beta$** are:
#### $[x]_\beta = \begin{bmatrix} b_1 \\ ... \\ b_n \end{bmatrix}$
Ex:
![[Pasted image 20221218160546.png]]

## Change of Coordinates Matrix
This matrix changes from one coordinate system to another.
To convert from standard coordinates to $\beta$:
#### $\vec x = P_\beta [x]_\beta$ where $P_\beta = \begin{bmatrix} b_1 b_2 ... b_n \end{bmatrix}$
- Coordinate mappings are one-to-one [[Linear Transformations]]
	– Called an **isomorphism** from $V$ onto $W$ (they are basically the same just different representations)

## Change of Bases Matrix
A more general version of the Change of Coordinates Matrix.
**Definition:** Let $\beta$ and $C$ be bases of a vector space. Then there is a unique $n \times n$ matrix $P_{C \leftarrow \beta}$ such that:
### $[\vec x]_C = P_{C \leftarrow \beta} [\vec x]_\beta$
### where $P_{C \leftarrow \beta} = \begin{bmatrix} [b_1]_C && [b_2]_C && ... && [b_n]_C \end{bmatrix}$
^ Matrix of $C$ coordinate vectors of the vectors in basis $\beta$ ($\beta$ in terms of $C$)

The inverse of the change of bases matrix goes the other way
Ex:
![[Pasted image 20221218163402.png]]

### Change of Bases - Linear Transformations:
You can do the same change of bases for a linear transformation:
![[Pasted image 20221218171623.png]]
where $M$ is called the **matrix for T relative to the bases $\beta$**

You can use [[Diagonalization]] for it too

