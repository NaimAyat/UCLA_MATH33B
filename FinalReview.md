# Section 9.5
## Finding Eigenvalues and Eigenvectors
* To find eigenvalues of A, compute det(A) and set = 0. Eigenvalues are roots.
  * [To compute det(A)](https://www.youtube.com/watch?v=V3e7m-qFDFU)
* To find eigenvectors, compute Null(A-λI) for each eigenvalue λ
  * [To compute nullspace](https://www.youtube.com/watch?v=bqBacABVCeQ)
* Check if the eigenvectors are independent by combining them into a matrix B and ensuring det(B) = nonzero
## Solutions to Differential Equations
### Real, Distinct Eigenvalues
* y(t) = C<sub>1</sub>e<sup>λ<sub>1</sub>t</sup>v<sub>1</sub> + C<sub>2</sub>e<sup>λ<sub>2</sub>t</sup>v<sub>2</sub> + ... + C<sub>n</sub>e<sup>λ<sub>n</sub>t</sup>v<sub>n</sub>
### Complex, Distinct Eigenvalues
* Use Euler's Identity e<sup>it</sup> = cost + isint
* y(t) = c<sub>1</sub>(real part of Euler)+c<sub>2</sub>(imaginary part of Euler)
    * Where roots have the form λ = α ± iβ
# Section 9.6
## Exponential of a Matrix
* e<sup>A</sup> = I + A + A<sup>2</sup>/(2!) + A<sup>3</sup>/(3!) + ...
