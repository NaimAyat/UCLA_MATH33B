# Second Order Differential Equations
## Linear Dependence / Independence
### [Wronskian](https://www.youtube.com/watch?v=zw9rkAD3BEI)
```
                |  f_1   f_2  |
W (f_1, f_2) =  |             |
                |  f_1'  f_2' |
```
* If W = nonzero for some value of x on the interval, the functions are linearly independent
## [Homogenous Second Order Linear Differential Equations](https://www.youtube.com/watch?v=soU-zRdpsoA)
* Take form P(x)y'' + Q(x)y' + R(x)y = G(x)
* Focus on: ay'' + by' + cy = 0
* Solve ar<sup>2</sup> + br + c = 0
  * If roots are distinct (r<sub>1</sub>, r<sub>2</sub>): y = c<sub>1</sub>e<sup>r<sub>1</sub>x</sup> + c<sub>2</sub>e<sup>r<sub>2</sub>x</sup>
  * If roots are repeated (r): y = c<sub>1</sub>e<sup>rx</sup> + c<sub>2</sub>xe<sup>rx</sup>
  * If roots are distinct and complex: y = e<sup>αx</sup>(c<sub>1</sub>cos(βx)+c<sub>2</sub>sin(βx))
