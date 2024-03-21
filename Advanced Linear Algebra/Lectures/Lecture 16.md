**Date: 3/19/2024**



Homework #9
Sec 6.1 :  2-10, 26-40  Evens
Sec 6.2 :  2-8, 18-24    Evens

**Vector Spaces**
Def : Let $V$ be a set on which addition and scalar multiplication are defined.
	If for all $u,v,w \in V$ and for all $c, d\in \mathbb{R}$.
1) $u+v \in V$                             (closure)
2) $u+v=v+u$                       (addition commutativity)
3) $u+(v+w)=(u+v)+w$   (addition associativity)
4) $\vec{0} \in V$, $\vec{0}+u=u$                  (addition identity)
5) $u+(-u)=\vec{0}$                       (additive inverse)
6) $c\cdot u\in V$
7) $c(u+v)=cu+cv$               (scalar multiplication distributive)
8) $(c+d)u = cu+cd$               (distributive)
9) $c(du) = (cd)u$                      (product)
10) $1\cdot u = u$                            (multiplicative identity)

Ex: $(\mathbb{R}, +, \times)$ is a vector space.
Ex: $\left(\mathbb{R}^2, +, \times\right)$ is a vector space.
Ex: $\left(\mathbb{R}^n, +, \times\right)$ is a vector space.
Ex: The set of all matrices $A\in \mathbb{R}^{2\times3}$ is also a vector space.
Ex: $\mathbb{P}_2$ is the set of all polynomials of degree 2 or less.
Ex: $F$ is the set of all real-valued functions $f:\mathbb{R}\rightarrow\mathbb{R}$.
Ex: $\mathbb{Z}$ is the set of all integers.


Theorem : Let $V$ be a vector space, $u\in V$, and $c\in\mathbb{R}$.
1) $0\cdot u = 0$
2) $u\cdot0 = 0$
3) $(-1)u=-u$

Def : A subset $W$ of a vector space $V$ is a subspace of $V$ if $W$ is a vector space under the same operations.

Theorem : Let $V$ be a vector space and $W \subset V, W\ne\emptyset$ is a subspace of $V$ iff:
1) If $u,v \in W$, then $u+v\in W$.
2) If $u\in W$, then $c\cdot u\in W$.


Ex: The set $\mathbb{P}_n\subset\mathbb{P}$ and satisfies above, therefore $\mathbb{P}_n$ is a subspace of $\mathbb{P}$.

Ex: Let $W$ be the set of all symmetric matrices. $W\subset\mathbb{R}^{n\times n}$.
	The above is satisfied, so $W$ is a subspace of $\mathbb{R}^{n\times n}$.

Ex: Set of vectors of the form $\langle a,b,-b,a\rangle$. Is it, in fact, a vector space as well.

Ex: The set of polynomials of the form $a+bx-bx^2+ax^3$ is a subspace of $\mathbb{R}^4$.
	This set is isomorphic to the above, and so is also a vector space.

Theorem : If $B$ is a basis for a vector space $V$, then for every $u\in V$, there is a unique way to write $u$ as a linear combination of the basis vectors in $B$.

