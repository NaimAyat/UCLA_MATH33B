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
* Equation for motion of a spring: my'' + μy' + ky = F(t) where m = mass, μ = damping constant, k = spring constant, F(t) = external force
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
