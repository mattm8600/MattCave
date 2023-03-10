Previously, we have found out how to calculate the shear force on a beam
To find the direct shear stress we follow this equation

## Formula:
# $\tau=\frac{VQ}{Ib}$
where:
- $V$ is the shear force (from shear force diagram)
- $I$ is the moment of inertia of entire cross-section
- $b$ = width of cross-section at shear line
- $Q$ is the first moment of area above/below shear line
	–> $Q=\int \tilde{y} da = \sum{\tilde{y}_iA_i}$

$\tilde{y}$ is the distance from the centroid of the entire cross-section to the centroid of part $i$
$Q_{max}$ is always at the centroid

### Shear Line
You draw the shear line depending on where you want to find the shear stress at
- For max stress of an object draw shear line at centroid
Here are two other examples of shear lines not at the centroid:
![[Pasted image 20230308143621.png]]
![[Pasted image 20230308143629.png]]
- Note for the second case, the thickeness is 10 because the height of that section is 10


### Notes:
- $\tau = 0$ at top and bottom edges
- $\tau_{max}$ is usually at the centroid
- If choosing between places to find $\tau_{max}$ use the smallest thickness

### Steps:
1. Find reactions and V/M Diagram
2. Draw shear line
3. Find $\tilde{y}$ of each component (Distance from centroid to the furthest edge of part) 
4. Calculate and sum $Q$
5. Find $b$, $V$ for the section you are looking at
6. Plug and chug

