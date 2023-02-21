**Euler’s Method** is the simplest and least accurate of the [[Numeric Methods]]. But it can be done by hand, which is why we get tested on it.

### Suppose we have a differential equation $\frac{dy}{dt} =f(t,y)$
Using the definition of a derivative:
## $Y'(t)=\lim \limits_{h\to0}=\frac{Y(t-h)-Y(t)}{h}$
- Aka we can approximate $Y’(t)$ (which is $\frac{dy}{dt})$ with a small enough h (called the **step**)

Algebraically manipulate this relationship to get:
## $Y(t+h)\approx Y(t)+hY'(t)$
- Now we can go step by step using $t_n =t_I +nh$

### Example: $\frac{dy}{dt} = t^2+y^2$, $y(0)=1$, find $y(.2)$ using $h=.1$
For step 0:
### $y_0 = 1$ and $f_0 =0^2+1^2=1$
then plug these numbers in to find y and f for step 1:
### $y_1 = y_0f_0= 1+ (.1)(1) =1.1$
### $f_1 = $