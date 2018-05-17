# Midterm 2
## Section 4.1
* Linear second-order differential equations are of the form a(x)y'' + b(x)y' + c(x)y = d(x)
* Homogenous second-order differential equations are of the form a(x)y'' + b(x)y' + c(x)y = 0
### [Wronskian](https://www.youtube.com/watch?v=zw9rkAD3BEI)
```
                |  f_1   f_2  |
W (f_1, f_2) =  |             |
                |  f_1'  f_2' |
```
* If W = nonzero for some value of x on the interval, the functions are linearly independent and form a fundamental set of solutions
## Section 4.3
### Characteristic Equation
* Characteristic equation of y'' + py' + qy = 0 is λ<sup>2</sup> + pλ + q = 0
* Roots of characteristic equation are given by λ = [-p ± √(p<sup>2</sup>-4q)]/2
  * Two distinct real roots if p<sup>2</sup>-4q > 0
  * Two distinct complex roots if p<sup>2</sup>-4q < 0
  * One repeated real root if p<sup>2</sup>-4q = 0
#### [Using Characteristic Equation to Solve Differential Equation](https://www.youtube.com/watch?v=soU-zRdpsoA)
* Solve λ<sup>2</sup> + pλ + q = 0
  * If roots (r) are distinct (r<sub>1</sub>, r<sub>2</sub>): y = c<sub>1</sub>e<sup>r<sub>1</sub>x</sup> + c<sub>2</sub>e<sup>r<sub>2</sub>x</sup>
  * If roots are repeated (r): y = c<sub>1</sub>e<sup>rx</sup> + c<sub>2</sub>xe<sup>rx</sup>
  * If roots are distinct and complex: y = e<sup>αx</sup>(c<sub>1</sub>cos(βx)+c<sub>2</sub>sin(βx))
    * Where roots have the form λ = α - iβ
## Section 4.4
### Harmonic Motion
* Equation for motion of a spring: my'' + μy' + ky = F(t) where m = mass, μ = damping constant, k = spring constant = mg/x, F(t) = external force
* Unforced harmonic motion: x'' + 2cx' + w<sub>0</sub><sup>2</sup>x = 0
  * c = damping constant = μ/2m
  * W = angular frequency = sqrt(k/m)
### Simple Harmonic Motion
* x'' + w<sub>0</sub><sup>2</sup>x = 0 with characteristic equation λ<sup>2</sup> + w<sub>0</sub><sup>2</sup> = 0
  * Characteristic roots λ = ±iw<sub>0</sub>
  * General solution x(t) = acosw<sub>0</sub>t + bsinw<sub>0</sub>t where a and b are constants
### Amplitude and Phase Angle
* A general solution to x'' + w<sub>0</sub><sup>2</sup>x = 0 can also be written in terms of amplitude and phase angle:
  * x(t) = Acos(w<sub>0</sub>t - ϕ)
  * Given vector elements a and b, we can compute A and ϕ: 
    * A = sqrt(a<sup>2</sup>+b<sup>2</sup>)
    * ϕ = arctan(b/a) if a > 0; arctan(b/a) + π if a < 0 and b > 0; arctan(b/a) - π if a < 0 and b < 0
### Damped Harmonic Motion
* c > 0 in x'' + 2cx' + w<sub>0</sub><sup>2</sup>x = 0
  * Characteristic equation is λ<sup>2</sup> + 2cλ + w<sub>0</sub><sup>2</sup> = 0
  * Roots are λ = -c ± sqrt(c<sup>2</sup> - w<sub>0</sub><sup>2</sup>)
1. c < w<sub>0</sub> is underdamped. Distinct complex roots.
   * General solution: x(t) = e<sup>-ct</sup>[C<sub>1</sub>coswt + C<sub>2</sub>sinwt] where w = sqrt(w<sub>0</sub><sup>2</sup> - c<sup>2</sup>)
2. c > w<sub>0</sub> is overdamped. Distinct real roots.
   * General solution: x(t) = C<sub>1</sub>e<sup>λ<sub>1</sub>t</sup> + C<sub>2</sub>e<sup>λ<sub>2</sub>t</sup> 
3. c = w<sub>0</sub> is critically damped. Double root λ = -c.
   * General solution: x(t) = C<sub>1</sub>e<sup>-ct</sup> + C<sub>2</sub>te<sup>-ct</sup> 
## Section 4.5
* Inhomogenous equations have the form y'' + p(t)y' + q(t)y = f(t)
### [Method of Undetermined Coefficients](https://www.youtube.com/watch?v=_U8Y5z-kVvI)
* Works only when p(t) and q(t) are constants in y'' + p(t)y' + q(t)y = f(t)
* f(t) is the forcing term, y<sub>p</sub>(t) is the trial solution
  * f(t) = e<sup>rt</sup>, y<sub>p</sub>(t) = ae<sup>rt</sup>
  * f(t) = coswt or sinwt, y<sub>p</sub>(t) = acostwt + bsinwt
  * f(t) = P(t), y<sub>p</sub>(t) = p(t); P is a polynomial and p is a polynomial of the same degree
  * f(t) = P(t)coswt or P(t)sinwt, y<sub>p</sub>(t) = p(t)coswt + q(t)sinwt; P is a polynomial, p & q are polynomials of same degree
  * f(t) = e<sup>rt</sup>coswt or e<sup>rt</sup>sinwt, y<sub>p</sub>(t) = e<sup>rt</sup>[acoswt + bsinwt]
  * f(t) = e<sup>rt</sup>P(t)coswt or e<sup>rt</sup>P(t)sinwt, y<sub>p</sub>(t) = e<sup>rt</sup>[p(t)coswt + q(t)sinwt]
1. Given y'' + py' + qy = f(t)
2. Solve complimentary function y'' + p(t)y' + q(t)y = 0 by getting roots of λ<sup>2</sup> + pλ + q = 0
3. Using the roots, get an equation for y<sub>c</sub>(t)
4. Come up with a particular solution y<sub>p</sub>(t)
   * For example, if f is x<sup>2</sup> choose y<sub>p</sub>(t) = Ax<sup>2</sup> + Bt + C 
5. Get first and second derivatives of y<sub>p</sub>(t). Plug them into original inhomogenous equation and solve for the undetermined coefficients of y<sub>p</sub>(t)
6. General solution of the inhomogenous equation: y(t) = y<sub>p</sub>(t) + y<sub>c</sub>(t)
## Section 4.6
### Variation of Parameters
* Solve y'' + p(t)y' + q(t)y = g(t) given a fundamental set of solutions {y<sub>1</sub>, y<sub>2</sub>} of the associated homogenous equation y'' + p(t)y' + q(t)y = 0
1. Find fundamental set of solutions to the associated homogenous equation y'' + py' + qy = 0
2. Form y<sub>p</sub> = v<sub>1</sub>y<sub>1</sub> + v<sub>2</sub>y<sub>2</sub> where "y"s are the fundamental solutions and "v"s are functions to be determined
3. Find v<sub>1</sub> and v<sub>2</sub>
   * Method 1: 
      * v<sub>1</sub>(t) = ∫ [ (-y<sub>2</sub>gdt) / (y<sub>1</sub>y'<sub>2</sub> - y'<sub>1</sub>y<sub>2</sub>) ] 
      * v<sub>2</sub>(t) = ∫ [ (y<sub>2</sub>gdt) / (y<sub>1</sub>y'<sub>2</sub> - y'<sub>1</sub>y<sub>2</sub>) ] 
   * Method 2:
      * Solve the system of equations v'<sub>1</sub>y<sub>1</sub> + v'<sub>2</sub>y<sub>2</sub> = 0; v'<sub>1</sub>y'<sub>1</sub> + v'<sub>2</sub>y'<sub>2</sub> = g(t)
      * Integrate to get v<sub>1</sub> and v<sub>2</sub>
4. Write the particular solution y = v<sub>1</sub>y<sub>1</sub> + v<sub>2</sub>y<sub>2</sub>
