# Lecture 1: April 2, 2018
## Logistics
* Professor Niccolò Ronchetti
* niccronc [at] math.ucla.edu
* Midterm 1: April 27 (in-lecture)
* Midterm 2: May 18 (in-lecture)
* Final: June 13 (3pm-6pm)
* HW due every Friday, beginning in Week 2
## Differential Equations
* Equations with an unknown; the unknown is a function
* Both the function and its derivatives appear in the equation
* Example: f = f' has the solution f(x) = Ce<sup>x</sup> for any real number constant C

**Definition**: *Ordinary differential equations (ODE)* are equations involving an unknown function and its derivatives. f(x) is the unknown function, x is the independent variable.

**Definition**: We call the order of an ODE "the highest derivative that appears". For example, f'' = f has order 2. Hyperbolic sin and hyperbolic cos are solutions.

* f = f(x) will always be a function mapping from fI -> R, where I is an interval

**Definition**: To get the *normal form of an ODE*, algebraically solve for the highest derivative.
  * Example: xy'-y=x<sup>2</sup>sinx. The independent variable is x; the unknown function is y (also may be written as y(x)). Solving for y', we get the normal form y'=xsinx+(y/x)
  
**Definition**: A solution to an ODE is a functon f=f(x) or y=y(x) which satisfies the equation for any x in the interval which is the domain of f

* Question: How do we know we've found a solution to a diff eq? Answer: plug it back into the original equation.
  * Example: Verify that y=-xcosx is a solution for xy'-y=x<sup>2</sup>sinx. Left side: xy'-y=x(-cosx+sinx)-(-xcosx)=x<sup>2</sup>sinx

**Definition**: For an ODE, we have a *general solution*: many solutions depending on one or more constants. Assigning a value to the constant(s) produces a *particular solution*
  * Example: The general solution to xy'=y+x<sup>2</sup>sinx is y(x)=Cx-xcosx, where C is any real number constant. Plotting solutions for various C values shows that all solutions intersect at the origin, since the normal form is not continuous at x=0.
  
* Question: How do we pick a value for C in the general solution?

**Definition**: A *first-order ODE* y'=f(y,x) with an *initial condition* y(x<sub>0</sub>)=y<sub>0</sub> is called an *initial value problem (IVP)*. A solution to an IVP is a function y=y(x) that satisfies the ODE and the initial condition.

* Example: Solve the IVP: xy'-y=x<sup>2</sup>sinx for the initial condition y(π)=2π. Take the general solution y(x)=Cx-xcosx, plug in x<sub>0</sub> and y<sub>0</sub>. 2π=y(π)=Cπ-πcosπ=(C+1)π. Solve for C to yield C=1.

* Note that choosing an initial condition y(x<sub>0</sub>)=y<sub>0</sub> corresponds to choosing a solution curve by fixing a point the graph
