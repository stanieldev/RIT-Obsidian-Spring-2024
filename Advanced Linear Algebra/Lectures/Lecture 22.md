Sec 7.2 Norm

Inner product introduces "length" and "distance"
But there are versions that don't depend on the inner product.

Def : A *norm* on a vector space is a mapping that assigns a real number $||v||$ to each vector $v$, called the norm of $v$, that satisfies:
1) $||v||\ge 0$
2) $||v||=0 \iff v=0$
3) $||cv||=c||v||$
4) $||u+v||\le||u||+||v||$

A vector space with a norm is called a *normed linear space*.


The p-th norm can be defined on $\mathbb{R}^n$ to be:
$$||v||_p=(v_1^p+v_2^p+\dots+v_n^p)^{1/p}$$
**The metric space**
Let $d$ be a distance function on a normed linear space $V$.
Then the following are true:
1) $d(u,v)\ge0$
2) $d(u,u)=0$
3) $d(u,v)=d(v,u)$
4) $d(u,w) \le d(u,v)+d(v+w)$
A function $d$ that satisfies the above is called a *metric*
and a vector space with a metric is called a *metric space*.

