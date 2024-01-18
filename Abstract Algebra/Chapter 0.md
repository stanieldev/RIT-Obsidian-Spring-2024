**Date: 1/17/2024**

Abstract Algebra: Groups and Rings (second semester)

Review Topics
 - Set Theory Basics
 - Properties of Integers
 - Modular Arithmetic




### Set Theory
#### Mathematical Logic
Statements who are Truth or False.
#### Negation
The "not" of a statement ($\not P$).
#### Conjunction
The "and" of a statement ($P\wedge Q$).
#### Disjunction
The "or" of a statement ($P\carot Q$).
#### Implication
Statements where $P$ implies $Q$ ($P\implies Q$).
$P$ is a *hypothesis*, $Q$ is a *conclusion*.
#### Equivalent
Statements where $P$ if-and-only-if (iff) $Q$ ($P\iff Q$).
$(P \iff Q) = (P \implies Q) \wedge (Q \implies P)$
#### Contrapositive
For all statements, contrapositive follows:
$P \implies Q$ is the implication $\not Q \implies \not P$
#### Contradiction
When a proposition leads to a conflict in its conclusion.
#### Open Sentence
An open sentence is a sentence that contains one or more variables.
$P(x) = \ 'x \gt 7'$ depends on a variable $x$.
#### Existential Quantifiers
If there exists something, written as $\exists$.
For a unique existential qualifier, use $\exists!$.
Uniqueness sometimes will occur in the class.
#### Universal Qualifier
For all of a certain variable, written as $\forall$.
#### Element Of (In)
Where a value is in a set S ($x\in S$).
#### Subset
A set that is a selection of objects from a parent set.
$A \subset B$ for a non-equal subset, $A \psubset B$ for a subset that may be identical to its parent.
#### Union
$A\union B = \{x|x\in A \mathrm{\ or\ } x\in B \}$
#### Intersection
$A\intersect B = \{x|x\in A \mathrm{\ and\ } x\in B \}$
#### Cardinality
Denoted $|A|$ is the quantity of unique elements in a set.
#### Set Equality
$A = B$, if $A \psubset B$ and $B \psubset A$
#### Disjointness
$A$ and $B$ are disjoint if $A \intersect B = \varnothing$
#### Complement
The Complement of $A$ in $B$, written $B-A$ or $A^c$
$B-A = \{x\in B | x\notin A\}$ or $B \backslash A$.
#### Cartesian Product
$A \times B = \{(a,b) | a\in A, b\in B\}$

### Properties of Sets
Sets do not care about ordering and do not repeat elements.

#### Proposition: Let $A$, $B$, and $C$ are sets. Then:
(1) $\varnothing \intersect A = \varnothing$ and $\varnothing \union A = A$.
(2) $A\intersect B \psubset A$ and $A\intersect B \psubset B$.
(3) $A\psubset A \union B$ and $B\psubset A \union B$.
(4) $A \union B = B \union A$ and $A \intersect B = B \intersect A$. (Communitive)
(5) $A \union (B \union C) = (A \union B) \union C$ and $A \intersect (B \intersect C) = (A \intersect B) \intersect C$ (Associativity)
(6) $A \union A = A \intersect A = A$
(7) $A \psubset B \implies A \union C \psubset B \union C \mathrm{\ and \ } A \intersect C \psubset B \intersect C$
#### Distribution Rules
(1) $A \intersect (B \union C) =  (A \intersect B) \union (A \intersect C)$
(1.a) Show $A \intersect (B \union C) \psubset (A \intersect B) \union (A \intersect C)$
	Let $x \in A \intersect (B \union C)$, then $x\in A$ and $x \in (B \union C)$
	So $x\in A$ and ($x\in B$ or $x \in C)
	So $x \in (A\intersect B)$ or $x \in (A\intersect C)$...
	Thus $x \in (A \intersect B) \union (A \intersect C)$
(2) $A \union (B \intersect C) =  (A \union B) \intersect (A \union C)$


### Mathematical Induction
Proving the k+1 step and an initial condition to solve a problem.

#### Binary Relations
A binary relation on a set $A$ is a subset, denoted $R$, of $A \times A$. If $(a,b)\in R$, then we write $_aR_b$.
Example: If A is a set of all humans, then "is a parent of" is a binary relation.
For $A = \mathbb{Z}$, then $\lt, \le, \gt, \ge$, are binary relations.
If $A=\mathbb{R}^n$, then orthogonality is a binary relation.
#### Equivalence Relation
*Reflexive* if $_aR_a$ for all $a\in A$.
*Symmetric* if $_aR_b \implies _bR_a$ for all $a,b\in A$.
*Transitive* if $_aR_b$ and $_bR_c$ $\implies _bR_a$ for all $a,b,c\in A$.
