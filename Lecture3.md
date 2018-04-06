# Lecture 3: April 6, 2018
## Section 2.2
### Separable Equations
* Goal: Solve a special type of ODE
* Example: y' = yxe<sup>3x</sup>. y = y(x) is the unknown function. 
  * We can isolate y and x on opposite sides of the equation
  * We think of y' = dy/dx
  * dy/dx = yxe<sup>3x</sup> → dy/y = xe<sup>3x</sup> dx
  * Now integrate ∫ dy/y = ∫ xe<sup>3x</sup>dx
  * ∫ dy/y = ln|y| + C<sub>1</sub>
  * ∫ xe<sup>3x</sup>dx = (xe<sup>3x</sup>/3) - (xe<sup>3x</sup>/9) + C<sub>2</sub>
  * Get ln|y| + C<sub>1</sub> = (xe<sup>3x</sup>/3) - (xe<sup>3x</sup>/9) + C<sub>2</sub>
  * C = C<sub>2</sub> - C<sub>1</sub>
  * Solve for y to get y = ±e<sup>C</sup>, y(x) = De<sup>((e<sup>3x</sup>/3)(x-(1/3))
* Definition: A *first order ODE* is called *separable* if its normal form can be written as y' = g(x)h(y) , y' = f(x,y). That is, the right side of the normal form is a product of two functions; one only in x, the other only in y. We separate x and y.
* General strategy to solve a separable equation: 
  1. Separate x and y in the normal form: that is, find g(x), h(y) such that y' = g(x)h(y)
  2. Think y' = dy/dx = g(x)h(y). Isolate x and y on opposite sides dy/h(y) = dx g(x)
  3. Integrate to get ∫ dy/h(y) = ∫ dx g(x)
  4. H(y) + C<sub>1</sub> = G(x) + C<sub>2</sub>, solve for y
* Example: y' = y + sinx
  * Want y + sin(x) = g(x)h(y). This is not possible; thus equation is not separable
 * Example: y' = y<sup>2</sup> - 4 = (y-2)(y+2)
   1. Let g(x) = 1, h(y) = (y-2)(y+2)
   2. dy/dx = (y-2)(y+2) isolate x and y on opposite sides: dy/[(y-2)(y+2)] = dx
   3. ∫ dy/[(y-2)(y+2)] = ∫ dx = x + C<sub>2</sub>
      * By partial fractions: ∫ dy/[(y-2)(y+2)] = (1/4)ln|y+2| + C<sub>1</sub> = (1/4)ln|(y-2)/(y+2)| + C<sub>1</sub>
   4. Solve (1/4)ln|(y-2)/(y+2)| + C<sub>1</sub> = x + C<sub>2</sub> for y
 
