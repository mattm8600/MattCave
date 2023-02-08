**Nonhomogeneous ODEs** are a subset of [[Linear ODE]]s

These start with the first order Linear ODE form:
## $\frac{dy}{dt} + a(t)y = f(t)$

The key to solving these equations is to set up a multiplication rule derivative like this:
## $\frac{d}{dt}(e^{A(t)}y) = e^{A(t)}f(t)$
where $A'(t) = a(t)$

Then you can integrate that explicitly to solve for y:
## $e^{A(t)}y = \int e^{A(t)}f(t)$
and then divide by y

Note that $e^{A(t)}$ is called the integrating factor

