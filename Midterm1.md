# Midterm 1 Notes
## Differential Equations with Boundary Value Problems - Polking (2nd Ed.)
## Section 2.1: First-Order Equations
### Show that [equation] is a solution of differential equation, initial value
1. Given y(t) = exp1 and y' = exp2.
2. Plug exp1 into equation for y'
3. Find derivative of exp1, verify it is the same as the expression resulting from step 2
4. Verify initial value satisfies y(t), if applicable
5. Interval of existence is longest defined interval containing the given t value
## Section 2.2: Seperable Functions
* F(x,y) is seperable if it can be expressed as a product of x's and y's
### [Solving Seperable Differential Equations](https://www.youtube.com/watch?v=nNHlSB6b1HU)
1. Remember: y' means dy/dx. Get rid of the denominator by multiplying both sides by dx.
2. Get x's on one side, y's on the other
3. Integrate y side w.r.t. dy
4. Integrate x side w.r.t. dx
5. Solve for y to get an explicit solution. If not possible, get an implicit solution.
## Section 2.4: Linear Equations
* Linear equation: the unknown function x and its derivative x' both appear alone and only to first order
### [Solving Homogeneous Linear Equations](https://www.youtube.com/watch?v=5mFjvDvTiTg)
1. Get the rhs in terms of (y/x)
2. Substitute v for y/x in the rhs
3. Use the equation dy/dx = x(dv/dx)+v.
   * Set LHS to x(dv/dx)+v, perform seperation of variables and solve
### [Solving Arbitrary Linear Equations with the Integrating Factor](https://www.youtube.com/watch?v=eWLgWazTc-0)
1. Given equation in the form x' = ax = f
2. Rewrite as x' - ax = f
3. Calculate integrating factor u(x) = e<sup>-∫a(t)dt<sup> (don't need the + C)
4. Multiply both sides of the original equation by the integrating factor
5. Integrate this to obtain u(x)x(t) = ∫u(t)f(t)dt + C
6. Solve for x(t)