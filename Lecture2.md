# Lecture 1: April 4, 2018
## Initial Value Problems
* y' = f(y, x)
  * y<sub>0</sub> = y(x<sub>0</sub>)
  * x = independent variable
  * y = unknown function
  * f(y, x) = expression involving x and y
## Interval of Existence
* Question: What is the domain of a solution to an ODE?
* Fact: This domain must be on interval (possibly (-inf, inf) on (-inf, 3)) because y(x) is differentiable, therefore continuous
* Definition: We call the *interval of existence* the longest interval on which a solution y(x) to an ODE (or to an IVP) is defined
* Example: y' = y/x + xsinx f(y,x)
  * The general solution is y(x) = Cx - xcosx for any constant C
  * What is the interval of existence of y(x) = 3x - xcosx? 
    * Answer: (-inf, inf). This is the same for any value of C.
* Example: Consider y' + 2xy<sup>2</sup> = 0, y' = -2xy<sup>2</sup>
  * Show that y(x) = 1/(x<sup>2</sup> + C) is a general solution
    * Find the derivative of the general solution, plug into differential equation
    * y'(x) = -2x / (x<sup>2</sup> + C)<sup>2</sup> so y' + 2xy<sup>2</sup> = -2x / (x<sup>2</sup> + C)<sup>2</sup> + 2x / (x<sup>2</sup> + C)<sup>2</sup> = 0. Hence, general solution is correct
* Example: Solve the IVP y' + 2xy<sup>2</sup> = 0, y(0) = 1.
  * Plug in y(0) = 1 into the general solution and solve for C
  * 1 = y(0) = 1/C -> C = 1
  * Solution to IVP is y(x) = 1/x<sup>2</sup> + 1, with interval of existence (-inf, inf)
