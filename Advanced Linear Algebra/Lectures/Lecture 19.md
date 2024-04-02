Homework #11:
6.5 : 3,4,7,8,10,11,16,17,21,22


Sec 6.5: Kernel and Range

Def : The *kernel* of a linear transformation $T: V\rightarrow W$ is the set of all vectors in $V$ that are mapped to 0 in $W$. I.e. $\mathrm{ker}(T)=\left\{v\in V \ | \ T(v)=0\right\}$.

Def : The *range* of $T$ is the set of all vectors in $W$ that are images of vectors in $V$ under $T$.
I.e. $\mathrm{range}(T)=\left\{w\in W \ | \ w = T(v)\right\}$


Example : Given $A_{m\times n}$, defined as $T:\mathbb{R}^n\rightarrow\mathbb{R}^m$ by $T(\vec{v})=A\vec{v}$.
 - $\mathrm{ker}(T) = \mathrm{null}(A)$.
 - $\mathrm{range}(T)=\mathrm{col}(A)$


Theorem : If $T:V\rightarrow W$ is a linear transformation:
- $\mathrm{ker}(T)$ is a subspace of $V$
- $\mathrm{range}(T)$ is a subspace of $W$

Def : Let $T:V\rightarrow W$ be a linear transformation.
 - $\mathrm{rank}(T) = \mathrm{dim}(\mathrm{range}(T))$
 - $\mathrm{nullity}(T) = \mathrm{dim}(\mathrm{ker}(T))$

Theorem : Let $T:V\rightarrow W$ be a linear transformation from a finite-dimensional vector space $V$ into a vector space $W$.
 - $\mathrm{rank}(T) + \mathrm{nullity}(T) = \mathrm{dim}(V)$


Ex: $T:\mathbb{P}_2\rightarrow\mathbb{P}_3$ defined by $T(a+bx+cx^2)=ax+bx^2+cx^3$
 - $\mathrm{nullity}(T) = 0$
 - $\mathrm{rank}(T) = 3$
 - $\mathrm{dim}(V) = \mathrm{dim}(\mathbb{P}_2) = 3$

Def : A linear transform $T:V\rightarrow W$ is injective (1-to-1) iff $T$ maps distinctive vectors in $V$ to distinctive vectors in $W$.
 - $u\ne v \implies T(u)\ne T(v)$
 - $T(u)=T(v) \implies u=v$   (contrapositive)

Def : A linear transform $T:V\rightarrow W$ is surjective (onto) iff $\forall w\in W, \exists v\in V \ | \ w=T(v)$.
 - $\mathrm{range}(T)=W$



## Mapping Qualities

A map $f$ is **injective** $\iff \forall v\in V,\ \exists! \ w\in W \ | \ w=f(v)$.
 - $\forall a,b\in V,\ f(a)=f(b) \implies a=b$
 - $\forall a,b\in V,\ a\ne b \implies f(a)\ne f(b)$

A map $f$ is **surjective** $\iff \forall w\in W,\ \exists v\in V \ | \ f(v)=w$.

A map $f$ is **bijective** $\iff \forall w\in W,\ \exists!\ v\in V \ | \ f(v)=w$.
 - $f$ is Bijective  $\iff$ $f$ is Injective $\wedge$ $f$ is Surjective.





Def : A linear transformation is an isomorphism if T is Bijective.






