
### Inner Products
Used to define "length" and "distance" in vector spaces other than $\mathbb{R}^n$.

Def : A *inner product* on a vector space $V$ is an operator that assigns to every pair a vectors $u,v\in V$ a real number $\langle u,v\rangle$ such that the following properties hold for $u,v,w\in V$ and $c\in\mathbb{R}$.
1) $\langle u,v\rangle=\langle v,u\rangle$
2) $\langle u,v+w\rangle=\langle u,v\rangle+\langle u,w\rangle$
3) $\langle cu,v\rangle = c\langle u,v\rangle$
4) $\langle u,u\rangle = ||u||^2 \ge 0$
5) $\langle u,u\rangle=0\iff u=0$

Properties :
1) $\langle u+v,w\rangle=\langle u,w\rangle+\langle v,w\rangle$
2) $\langle u,cv\rangle = c\langle u,v\rangle$
3) $\langle u,0\rangle = \langle 0,u\rangle = 0$

Definition :
1) Length (or more generally, the norm) of $v$ is $||v||=\sqrt{\langle v,v\rangle}$
2) Distance between $u$ and $v$ is $||u-v||=\sqrt{\langle u-v,u-v\rangle}$
3) $u$ and $v$ are orthogonal when $\langle u,v\rangle=0$.

Pythagoras' Theorem : $u,v$ are orthogonal iff $||u+v||^2 = ||u||^2 + ||u||^2$.

Cauchy-Schwartz Inequality : $|\langle u,v\rangle| \le ||u||\cdot||v||$

Triangle Inequality: $||u+v|| \le ||u|| + ||v||$



