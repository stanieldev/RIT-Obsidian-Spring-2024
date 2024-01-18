### Properties of Sets
Repeat elements in a set are disallowed.
#### Empty set
$\varnothing \cap A = \varnothing$ and $\varnothing \cup A = A$.
#### Intersection-Subset
$A\cap B \subseteq A$ and $A\cap B \subseteq B$.
#### Union-Subset
$A\subseteq A \cup B$ and $B\subseteq A \cup B$.
#### Commutivity
$A \cup B = B \cup A$ and $A \cap B = B \cap A$.
#### Associativity
$A \cup (B \cup C) = (A \cup B) \cup C$ and $A \cap (B \cap C) = (A \cap B) \cap C$
#### Self-Referential
$A \cup A = A \cap A = A$
#### ???
$A \subseteq B \implies A \cup C \subseteq B \cup C \mathrm{\ and \ } A \cap C \subseteq B \cap C$
### Intersection on Union
$A \cap (B \cup C) =  (A \cap B) \cup (A \cap C)$
#### Union on Intersection
$A \cup (B \cap C) =  (A \cup B) \cap (A \cup C)$


### Set Connectives
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
$A \subset B$ for a non-equal subset, $A \subseteq B$ for a subset that may be identical to its parent.
#### Union
$A\cup B = \{x|x\in A \mathrm{\ or\ } x\in B \}$
#### Intersection
$A\cap B = \{x|x\in A \mathrm{\ and\ } x\in B \}$
#### Cardinality
Denoted $|A|$ is the quantity of unique elements in a set.
#### Set Equality
$A = B$, if $A \subseteq B$ and $B \subseteq A$
#### Disjointness
$A$ and $B$ are disjoint if $A \cap B = \varnothing$
#### Complement
The Complement of $A$ in $B$, written $B-A$ or $A^c$
$B-A = \{x\in B | x\not\in A\}$ or $B \backslash A$.
#### Cartesian Product
$A \times B = \{(a,b) | a\in A, b\in B\}$


### Set Relations (Mappings)
#### Binary Relations
A binary relation on a set $A$ is a subset, denoted $R$, of $A \times A$. If $(a,b)\in R$, then we write $_aR_b$.
Example: If A is a set of all humans, then "is a parent of" is a binary relation.
For $A = \mathbb{Z}$, then $\lt, \le, \gt, \ge$, are binary relations.
If $A=\mathbb{R}^n$, then orthogonality is a binary relation.
#### Equivalence Relation
*Reflexive* if $_aR_a$ for all $a\in A$.
*Symmetric* if $_aR_b \implies _bR_a$ for all $a,b\in A$.
*Transitive* if $_aR_b$ and $_bR_c$ $\implies _bR_a$ for all $a,b,c\in A$.
