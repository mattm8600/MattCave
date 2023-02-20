**Autonomous Ordinary Differential Equations** are when $f(t)$ is constant
## $\frac{dy}{dt} = g(y)$
- The function only depends on $y$

### There are two ways to find solutions:
1. *General solution* → Solve the separable differential equation
	- These usually are implicit solutions, so turn them into [[Explicit ODE]]s
2. *Stationary solutions* → when $g(y)=0$
	- Think about it: These are valid solutions as well
	- Most likely going to be an undefined point

## Ex 1: $\frac{dy}{dt}=y^2$
Stationary Solution: $y=0$ 
### $dt = \frac{dy}{y^2}$
### $t = \int{\frac{1}{y^2}dy}=-\frac{1}{y}+c$
- This is an implicit solution we want y in terms of t
Use algebra → $y=\frac{1}{c-t}$
