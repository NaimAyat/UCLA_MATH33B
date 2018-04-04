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
* Example: Solve the IVP y' + 2xy<sup>2</sup> = 0, y(0) = -1
  * Plug in: -1 = y(0) = 1/C -> C = -1, solution to IVP is y(x) = 1/(x<sup>2</sup>-1)
  * Which of (-inf, -1), (-1, 1), (1, inf) is the interval of existence?
    * We are forced to pick (-1, 1), since our curve has to go through 0
* The interval of existence of the solution to an IVP must contain the x-coordinate of the initial condition
## Direction Fields
* Suppose we are given y' = f(x,y) on ODE, call the solution y(x). y' is the slope of the tangent line to the solution curve: y(x)
  * Reverse the argument: y' = f(x,y) is the slope of the solution curve
* Example: y' = xy. Draw line segments whose slopes are given by f(x,y)
  * [Resulting direction field](images/april4-1.PNG)
  * The solution curves are tangent to these line segments, so "connecting the line sigments" gives a qualitative idea of the solution curves
### Euler's Method
* Use the direction field to ketch the graph of a particular solution IVP
* Let y' = yx + x<sup>2</sup> + y<sup>2</sup>, y(0) = 1. Start with (0,1), compute f(0,1) = 1. The tangent line to the particular solution is (y-1) = 1(x-0), y = x+1. Pick a small grid x-length (say 1)
  * Increase the x-coordinate by grid length, we get x = 0 + 1 = 1. Follow the tangent line until that point y = x + 1 = 2. Repeat. Compute f(1,2) = 2 + 1 + 4 = 7. Tangent line (y-2) = 7(x-1).  New x coordinate is now 1 + grid length = 2. Plug this point into tangent line, so y = 7(2-1) + 2 = 9. New point (2,9)
* Example: [y' = cos(πy) + 1](images/april4-2.PNG)
  * Horizontal solutions are *equilibrium* solutions
