# Midterm 1 Notes
## Differential Equations with Boundary Value Problems - Polking (2nd Ed.)
## Section 2.1: First-Order Equations
### Show that [equation] is a solution of differential equation, initial value
1. Given y(t) = exp1 and y' = exp2.
2. Plug exp1 into equation for y'
3. Find derivative of exp1, verify it is the same as the expression resulting from step 2
4. Verify initial value satisfies y(t), if applicable
5. Interval of existence is longest defined interval containing the given t value
## Section 2.2: Separable Functions
* F(x,y) is separable if it can be expressed as a product of x's and y's
### [Solving Separable Differential Equations](https://www.youtube.com/watch?v=nNHlSB6b1HU)
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
   * Set LHS to x(dv/dx)+v, perform separation of variables and solve
### [Solving Arbitrary Linear Equations with the Integrating Factor](https://www.youtube.com/watch?v=eWLgWazTc-0)
1. Given equation in the form x' = ax = f
2. Rewrite as x' - ax = f
3. Calculate integrating factor u(x) = e<sup>-∫a(t)dt</sup> (disregard the + C)
4. Multiply both sides of the original equation by the integrating factor
5. Integrate this to obtain u(x)x(t) = ∫u(t)f(t)dt + C
6. Solve for x(t)
### [Solving Arbitrary Linear Equations with Variation of Parameters](https://www.youtube.com/watch?v=YNrJ9LA3Kxk)
1. Rewrite as homogenous (equals zero)
   * For example, rewrite y' + 2xy = 2x as y'<sub>h</sub> + 2xy<sub>h</sub> = 0
2. Separate homogenous equation
3. Integrate both sides, solve for y<sub>h</sub> (disregard the + C)
4. Set y = u * y<sub>h</sub>
5. Take derivative, y'. Plug your y' and the y found in step 4 into the original function
6. Separate into u and x sides, integrate each side, solve for u
7. Plug solved u into equation from step 4 to get y
## Section 2.5: Mixing Problems
### [Solving Using First-Order Separable Differential Equations](https://www.youtube.com/watch?v=6wk9zWa-Fww)
* Want, for example, amount of salt in tank ofter t minutes
* Set A(t) = amount of salt after t minutes
* Set dA/dt = (rate in) - (rate out)
  * More generally, dA/dt = (concentration that enters container)(rate of flow) - (concentration out)(rate of flow out)
    * Concentration out = A(t)/ volume of container
* Simplify for dA/dt = expression with A
* Separate; get A on one side and dt on the other
* Integrate both sides and solve for A as a function of t
* Plug in initial value, for example A(t) = 15 "the amount of salt at time 0 was 15" to find C
* Write the newly discovered function for A(t)
## Section 2.6: Exact Differential Equations
* Exact differential equation: we have a function of (x,y) and a function of (x,y) times y' equal to zero
  * M(x,y) + N(x,y)y' = 0
  * If we take the derivative of M with respect to y and N with respect to x, they are equal: M<sub>y</sub>(x,y) = N<sub>x</sub>(x,y)
