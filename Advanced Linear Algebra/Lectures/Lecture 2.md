**Date: 1/18/2024**
<hr>
### Systems of Linear Equations
A *system of linear equations* is a finite set of linear equations each with the same variables.
 - All variables must be of polynomial degree 1.
 - A *solution* to a system is a set of solutions that satisfy the system completely.
#### Augmented Matrix Representation
The system of linear equations can be represented as a coefficient matrix with an augmented output vector appended to the right.
$$\begin{cases}1x_1+1x_2+1x_3=2\\2x_1-3x_2+5x_3=11\\-x_1-x_2+4x_3=2\end{cases} \implies \left[\begin{array}{ccc|c}1&1&1&2\\2&-3&5&11\\-1&-1&4&1\end{array}\right]$$
<hr>
### Matrix Properties
#### Row-Echelon Form (REF)
A matrix is in *row-echelon form* if it satisfies the following conditions:
1) All zero rows appear at the bottom triangle.
2) In each non-zero row, the 1st non-zero entry is in a column left of any leading entry below it.
#### Reduced Row-Echelon Form (RREF)
A matrix is in *reduced row-echelon form* if it satisfies the following conditions:
1) Satisfies the conditions for Row-Echelon Form.
2) All leading entries in each row must be $1$.
3) Any column containing a leading 1 must have zeros elsewhere.
#### Rank / Rank Theorem
The *rank* of a matrix is the number of non-zero rows in the Row-Echelon Form.

**Theorem:** Let $A$ be the coefficient matrix of a system of linear equations with $n$ variables.
If the system is *consistent* (at least 1 solution), then:
$$\mathrm{Number\ of\ Free\ Variables} = \mathrm{Columns}-\mathrm{Rank}(A)$$
#### Homogeneity / Homogeneity Theorem
A system of linear equations is *homogenous* if the constant term in each equation is 0. For an augmented matrix, that means that right of the bar is the $0$ vector.

**Theorem:** If $[A|0]$ is a homogenous system of *m* linear equations with *n* variables and $m\lt n$, then the system has infinitely many solutions (at least 1 free parameter).

<hr>
### Matrix Operations
#### Elementary Row Operations
In solving augmented matrices, an *elementary row operation* is an operation that allows for the following set of matrix operations. 
1) Exchanging (interchange) rows.
2) Multiplication of any non-zero constant.
3) Multiple of 1 row and add it to another.
Elementary Row Operations can also be expressed as a matrix that can multiply an original matrix for the same effect. This is useful in LU factorization and in inverse matrix calculations.
#### Gauss-Jordan Elimination Process
The *Gauss-Jordan elimination process* is a process for reduction of a matrix to Reduced Row-Echelon Form and solving for the solution vector in terms of the free variables.
1) Write the augmented matrix of a system of linear equations.
2) Obtain the Reduced Row-Echelon Form of the augmented matrix.
3) If the system is consistent, then solve for leading variables in terms of free variables.

<hr>
#### Span / Spanning Theorem
The *span* of a set of vectors the the space covered by a linear combination of the set of vectors.

**Theorem:** If $s = \{v_1, v_2, v_3,\dots\}$ is a set of vectors in $\mathbb{R}^n$, then the set of linear combinations of the vectors $s$ is called the *span* of the vectors. If Span($s$) = $\mathbb{R}^n$, then $s$ is a spanning set for $\mathbb{R}^n$.

<hr>
### Homework
Section 2.1: 26
Section 2.2: 26, 28, 34
Section 2.3: 4, 12, 28
Section 2.4: 4
Section 3.1: 6, 8
Section 3.2: 6, 10, 14

