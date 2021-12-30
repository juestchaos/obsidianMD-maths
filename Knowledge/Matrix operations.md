## Operations

### Addition

It's easy. Add the elements in the same position.

$$\left[\begin{matrix}3 & 4 \\ 1 & 2 \end{matrix}\right] + \left[\begin{matrix} 5 & -1 \\ -3 & 2\end{matrix}\right] = \left[\begin{matrix} 8 & 3 \\ -2 & 4 \end{matrix}\right]$$

Addition is not defined for matrices with different dimensions.

### Negation

Negate all the elements.

### Subtract

Subtract all the elements (negate then add).

### Multiplication

#### Scalar multiplication

It's easy, since it's repeated addition.

$$k\left[\begin{matrix}a & b \\ c & d \end{matrix}\right] = \left[\begin{matrix} ka & kb \\ kc & kd \end{matrix}\right]$$

This also holds for taking common factors out of matrices.

#### Matrix multiplication

To multiply two matrices, pairwise multiply the rows of the left matrix by the columns of the right.

$$\begin{aligned}\left[\begin{matrix} \textcolor{blue}{11} & \textcolor{red}{8} \\ \textcolor{green}{4} & \textcolor{purple}{3} \end{matrix}\right]\cdot \left[\begin{matrix} \textcolor{olive}{3} & \textcolor{orange}{-8} \\ \textcolor{brown}{-4} & \textcolor{aquamarine}{11}\end{matrix}\right] & = \left[\begin{matrix} (\textcolor{blue}{11}\cdot \textcolor{olive}{3} + \textcolor{red}{8} \cdot \textcolor{brown}{-4}) & (\textcolor{blue}{11} \cdot \textcolor{orange}{-8} + \textcolor{red}{8} \cdot \textcolor{aquamarine}{11}) \\ (4\cdot3 + 3\cdot -4) & (4 \cdot -8 + 3 \cdot 11)\end{matrix}\right] \\ & = \left[\begin{matrix} 1 & 0 \\ 0 & 1 \end{matrix}\right] \end{aligned}$$

This means matrix multiplication can only be performed if $A_n=B_m$, that is, matrix $A$ has the same number of columns as matrix $B$ has rows.

This also means that the output matrix $C$ will have the dimensions $C_{A_n \times B_m}$

More generally:

$$\left[\begin{matrix}a_{1,1} & a_{1,2}\end{matrix}\right]$$