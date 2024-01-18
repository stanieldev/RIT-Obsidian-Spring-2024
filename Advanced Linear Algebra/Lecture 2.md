A system of linear equations is a finite set of linear equations each with the same variables.
All variables must be of polynomial degree 1.

Solution -> A set of solutions that satisfy the system of linear equations.
Solutions sometimes don't have solutions.
Some have infinitely many solutions.

A description can be written as an augmented matrix. Example:
$$\begin{bmatrix}1&1&1&|\ 2 \ \\2&-3&5&|11\\-1&-1&4&| \ 1 \ \end{bmatrix}$$
Def : A matrix is in Row-Echelon Form (REF) if it satisfies
1) All zero rows appear at the bottom.
2) In each non-zero row, the 1st non-zero entry is in a column left of any leading entry below it.

Elementary Row Operations:
1) Exchanging (interchange) rows.
2) Multiplication of any non-zero constant.
3) Multiple of 1 row and add it to another.
Note: Remember to show steps based on elementary row operations.

Def : The rank of a matrix is the number of non-zero rows in the REF.


Rank Theorem : Let $A$ be the coefficient matrix of a system of linear equations.
Sps. you start with $n$ variables.
If the system is *consistant* (at least 1 solution), then the number of free variables = number of columns - rank(A).

Reduced Row Echelon Form (RREF):
1) Obtain REF.
2) The leading entry of each row must be 1.
3) Any column containing a leading 1 must have zeros elsewhere in the zeros.

Gauss-Jordan Elimination Process:
1) Write the augmented matrix of a system of linear equations.
2) Obtain the RREF of the augmented matrix.
3) If the system is consistent, then solve for leading variables in terms of free variables.

### **EXAMPLE**: Pg. 80, #30
$$\begin{bmatrix}-1&3&-2&4&| \ \ \  0 \ \ \\2&-6&1&-2&|-3\\1&-3&4&-8&| \ \ \  2 \ \  \end{bmatrix}$$
Add R3 and R1 to R3
$$\begin{bmatrix}-1&3&-2&4&| \ \ \  0 \ \ \\2&-6&1&-2&|-3\\0&0&2&-4&| \ \ \  2 \ \  \end{bmatrix}$$
R1 -> 2R2
$$\begin{bmatrix}-2&6&-4&8&| \ \ \  0 \ \ \\2&-6&1&-2&|-3\\0&0&2&-4&| \ \ \  2 \ \  \end{bmatrix}$$Add R2 and R1 to R2
$$\begin{bmatrix}-2&6&-4&8&| \ \ \  0 \ \ \\0&0&-3&6&|-3\\0&0&2&-4&| \ \ \  2 \ \  \end{bmatrix}$$
R2 -> R2 / 3, R3 -? R3/2
$$\begin{bmatrix}-2&6&-4&8&| \ \ \  0 \ \ \\0&0&-1&2&|-1\\0&0&1&-2&| \ \ \  1 \ \  \end{bmatrix}$$Add R3 and R2 to R3
$$\begin{bmatrix}-2&6&-4&8&| \ \ \  0 \ \ \\0&0&-1&2&|-1\\0&0&0&0&| \ \ \  0 \ \  \end{bmatrix}$$
R3 -> R3/4, 2R3+R2->R2, 8R3+R1->R1
$$\begin{bmatrix}-2&6&-4&0&| \ \ \  0 \ \ \\0&0&-1&2&|-1\\0&0&0&0&| \ \ \  0 \ \  \end{bmatrix}$$
R2 -> -R2, R1 -> -R1/2
$$\begin{bmatrix}1&-3&2&0&| \ \ 0\\0&0&1&-2&| \ \ 1\\0&0&0&0&| \ \ 0   \end{bmatrix}$$
R1 - 2R2 -> R1
$$\begin{bmatrix}1&-3&0&0&|-2\\0&0&1&-2&| \ \ \ 1\ \ \\0&0&0&0&| \ \ \ 0 \ \   \end{bmatrix}$$
4 Columns (n=4), Rank 2.
The # of free variables is n - rank = 2.
So the solution vector comes to:
$$\vec{x}=\begin{bmatrix}3s-2\\s\\2t+1\\t\end{bmatrix}$$
### Homework
Section 2.1: 26
Section 2.2: 26, 28, 34
Section 2.3: 4, 12, 28
Section 2.4: 4




DEF : A system of linear equations is *homogenous* if the constant term in each equation is 0.

Theorem: If $[A|0]$ is a homogenous system of *m* linear equations with *n* variables and $m\lt n$, then the system has infinitely many solutions (at least 1 free parameter).

DEF : If $s = \{v_1, v_2, v_3,\dots\}$ is a set of vectors in $\mathbb{R}^n$, then the set of linear combinations of the vectors $s$ is called the *span* of the vectors. If Span($s$) = $\mathbb{R}^n$, then $s$ is a spanning set for $\mathbb{R}^n$.

### EXAMPLE: Pg. 98, #11
$$\mathrm{Span}\left(\begin{bmatrix}1\\0\\1\end{bmatrix}, \begin{bmatrix}1\\1\\0\end{bmatrix}, \begin{bmatrix}0\\1\\1\end{bmatrix}\right)$$
A vector can be represented by the augmented matrix:
$$\begin{bmatrix}1&1&0&|\ \ \ a\\0&1&1&| \ \ \ b\\1&0&1&| \ \ \ c\end{bmatrix}$$
After RREF:
$$\begin{bmatrix}1&0&0&|\ \ \ \dfrac{2a-b+c}{2} \ \\0&1&0&| \ \ \ \ \dfrac{a+b-c}{2} \ \ \\0&0&1&| \ \ \dfrac{-a+b+c}{2} \ \end{bmatrix}$$
Meaning there is a unique solution in this basis, therefore the vector spans $\mathbb{R}^n$.
