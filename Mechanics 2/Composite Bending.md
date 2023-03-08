You can strengthen the [[Bending Stress]] (also [[Direct Shear Stress]] but we don’t get into that) by reinforcing a beam with a stronger material
- We model this in our calculations by scaling the original cross-section as if it were the new material

## Formula:
# $\sigma = -\frac{Mc}{nI}$
- $n$ is the conversion factor
- All other variables are the same as [[Bending Stress]]

## Conversion Factor
The ratio between both material’s modulus of elasticities
# $n_i =\frac{E_{chosen}}{E_i}$
- Usually make all $n$ values larger than one
- Calculate for each separate material

## Steps:
1. Calculate conversion factors turning all materials into one with the greatest elasticity
2. Convert the cross-section by dividing the **WIDTH** of each material by $n$
3. Calculate a new centroid (if vertically asymmetrical) and a new moment of inertia
4. Calculate C values for each material
	– Distance from centroid of beam to the farthest edge of material
5. Plug and chug into composite bending formula
