The **Gran-Schmidt Process** is a simple algorithm for producing an orthogonal basis for any subspace of $\mathbb{R}^n$

You basically take a bunch of orthogonal projections over and over

**Definition**: given a basis $\{x_1,...,x_p \}$ for a nonzero subspace $W$ of $\mathbb{R}^n$, define
#### $v_1 = x_1$
#### $v_2 = x_2 - \frac{x_2 \cdot v_1}{v_1 \cdot v_1} \vec v_1$
#### $v_3 = x_3 -\frac{x_3 \cdot v_1}{v_1 \cdot v_1} \vec v_1 - \frac{x_3 \cdot v_2}{v_2 \cdot v_2} \vec v_2$

Repeat this process for as many dimensions as there are  in the [[Orthogonal Sets]]]:
![[Pasted image 20221218195247.png]]

- QR factorization is a factorization that can give you the orthonormal basis for the [[Column Space]] of a matrix