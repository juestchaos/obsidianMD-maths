---
aliases: 
tags: specialist
---

Links: [[Matrices]]

# Leslie matrices

A Leslie matrix is a matrix $L$ which is used to model the different age groups of a population over time.

Let us define a column matrix $P_0$ which contains the initial populations of the three age groups of a population of koalas, 0 - <3 years, 3 - <6 years and 6 - 9 years, the population of the first group expressed as $p_1$, the second as $p_2$ etc.

$$ P_0 = \begin{bmatrix} p_1 \\ p_2 \\ \vdots \\ p_n\end{bmatrix}$$

Let us now define a Leslie matrix $L$ using the following information:

- $c_n$, the average number of children a member of age group $n$ will have in the time period
- $s_n$, the average number of members of group $n$ who will survive the time period and become members of group $n+1$

$$ L = \begin{bmatrix}
c_1 & c_2 & c_3 &\cdots & c_n \\
s_1 & 0 & 0 & \cdots &  0 \\
0 & s_2 & 0 & \cdots & 0 \\
0 & 0 & s_3 & \cdots & 0\\
\vdots & \vdots & \vdots &\ddots & 0 \\
0 & 0 & \cdots & s_n & 0
\end{bmatrix} $$

To find the population matrix $P_1$ after the first period, simply multiply the Leslie matrix by $P_0$:

$$ P_1 = LP_0 $$

In doing this, the first row of the Leslie matrix (the birth rates of the different age groups) is multiplied by the populations of the different groups to find the number of members of the youngest age group. Each group is then multiplied by only its survival rate, to find its population in the next age group in the next time period. Note that the Leslie matrix assumes the death rate of the highest age group is 100%.

To find the the population after two periods $P_2$:

$$ P_2 = LP_1 $$

This gives the [[Recursion|recursive]] definition of the population after $k$ periods as

$$ P_k = LP_{k-1}$$

However, since this is just repeated multiplication by $L$, this can also be expressed as

$$ P_k = L^kP_0 $$
