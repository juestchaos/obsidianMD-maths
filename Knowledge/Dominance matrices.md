Links: [[Matrices]]

# Dominance Matrices

A dominance matrix is used to represent the ranking of competitors in a competition where not all competitors have had the opportunity to play each other. Take for example a competition with four teams; A, B, C and D, where
- A beat B and C
- B beats D
- D beats C

From this, the ranking of the four teams is not clear, since B and D have both won one game each. To clarify this, we create a [[Matrices|matrix]] where a 1 indicates that the team with that row beat the team with that column. 
$$ D = \begin{bmatrix} 
0 & 1 & 1 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 0 & 0 \\
0 & 0 & 1 & 0
\end{bmatrix} $$

Using this, we can calculate a 'score' for each team by adding up the elements in their row:
$$ D = \begin{bmatrix} 
0 & 1 & 1 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 0 & 0 \\
0 & 0 & 1 & 0
\end{bmatrix} \ \begin{matrix} 2 \\ 1 \\ 0 \\ 1\end{matrix}$$

While this allows us to see that clearly A is the strongest team and C the weakest, there is no way of distinguishing between B and D. To determine this, we multiply the matrix $D$ by itself, and the row sums of this matrix $D^2$ are the 'second-hand' wins for each team.

We can then simply add up these matrices, as well as any higher powers of $D$ required to break further ties, to find a final dominance matrix from which to determine rankings. Optional weightings can also be applied at this step, if a 'second-hand' win isn't considered as valuable.
$$ M = D + a_1D^2 + \cdots + a_mD^n $$