**Linear Transformations** are [[The Matrix Equation]] except it’s not a linear combination:
- Has many applications, such as changing a vector from $\mathbb{R}^n$ to $\mathbb{R}^m$

#### Terminology (for $T : \mathbb{R}^n → \mathbb{R}^m$)
- $\mathbb{R}^n$ → Domain
- $\mathbb{R}^m$ → Co-Domain
- $T(x)$ is the **images** of $x$
- The set of all $T(x)$ is the **range** of T

## Matrix Transformations: $T(\vec x) = A \vec x$
Ex:
![[Pasted image 20221217184519.png]]

- $T(0) = 0$

### Onto:
- A mapping is **onto** if each $\vec b$ is an image of $T(x)$ 
 ![[Pasted image 20221217184913.png]]

### One to One:
- A mapping is **one-to-one** if each $\vec b$ is at MOST one image of $T(x)$
![[Pasted image 20221217221409.png]]


## Geometric Linear Transformations (for $\mathbb{R}^2$)
Reflection across an Axis:
#### $\begin{bmatrix} a & 0 \\ 0 & b \end{bmatrix}$
- If a is negative → Flips across the y-axis
- If b is negative → Flips across the x-axis
- If a != 1 → Horizontal contraction or expansion
- If b != 1 → Vertical contraction or expansion
^ To reflect across $y=x$ → Replace the 0s with 1s
	– To reflect across $y=-x$ → Replace the 0s with -1s

Rotation Matrix:
#### $\begin{bmatrix} cos\theta & -sin\theta \\ sin\theta & cos\theta \end{bmatrix}$
where theta is the angle to rotate **Counterclockwise**
