---
aliases: inverse
tags: specialist
---

# Identity and inverse matrices

## The identity matrix

The identity [[Matrices|matrix]] is a square matrix with 1s along its top-to-bottom diagonal and all other elements being 0. The 2x2 and 3x3 identity matrices are

$$I_{2\times 2}=\left[\begin{matrix}1 & 0 \\ 0 & 1\end{matrix}\right] $$ $$ I_{3 \times 3} = \left[\begin{matrix}1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{matrix}\right]$$

The identity matrix has the interesting property of returning the other input of a [[Matrix operations#Matrix multiplication|matrix multiplication]], or

$$AI = A $$ $$ IA = A$$

## The inverse of a matrix

Notated as $A^{-1}$, the inverse $A^{-1}$ of a matrix $A$ is the matrix which, when multiplied by $A$, returns the identity matrix $I$. Put simply,

$$A \cdot A^{-1} = I$$

To find the inverse of a matrix, let us define an arbitrary 2x2 matrix $A$ and its inverse $A^{-1}$as

$$A = \left[\begin{matrix}a & b \\ c & d\end{matrix}\right] $$
$$ A^{-1} = \left[\begin{matrix}p & q \\ r & s\end{matrix}\right]$$

By the definition above:

$$A \cdot A^{-1} = I $$
$$ \left[\begin{matrix}a & b \\ c & d\end{matrix}\right] \cdot  \left[\begin{matrix}p & q \\ r & s\end{matrix}\right] = \left[\begin{matrix}1 & 0 \\ 0 & 1\end{matrix}\right]$$

To find the inverse of a matrix, find its determinant $\det A$ where

$$\det A=\frac{1}{ad-bc}$$

$A^{-1}$ is then

$$A^{-1}=\det A\left[\begin{matrix}d & -b \\ -c & a\end{matrix}\right] \\ =\frac{1}{ad-bc} \left[\begin{matrix}d & -b \\ -c & a\end{matrix}\right]$$

A matrix must satisfy two conditions to have an inverse:

1. That the matrix is square
2. That the matrix's determinant is not equal to zero
