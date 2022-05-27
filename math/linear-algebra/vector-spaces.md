# Vector Spaces

## Definition and Examples

A *vector space* $V$ over a field $k$ is a $k$-module, i.e., an abelian
group admits a linear ring action by elements of $k$, which can then be
characterized by the following axioms:

-   $V$ is an abelian group:

    1.  $v + w = w + v$.

    2.  $(v + w) + u = v + (w + u)$.

    3.  $\exists 0 \in V, 0 + v = v + 0 = v$.

    4.  $\forall v \in V, \exists - v, v + (- v) = (- v) + v = 0$.

-   $V$ admits a linear ring action by elements of $k$:

    1.  $1 \cdot v = v$.

    2.  $(r + s)v = rv + sv$.

    3.  $r(sv) = (rs)v$.

    4.  $r(v + w) = rv + rw$.

-   real and complex coodinate space $\RR^n, \CC^n$.

-   $k^S := \{f: S \to k\}$.

## Subspaces

A subset $U \subseteq V$ is called a *subspace* of $V$ if $U$ is also a
vector space.

The easiest way is to check that

-   $U$ is a subgroup,

-   $U$ is closed under scalar multiplication.

### Sums, Products and Quotients

The sum of two vector spaces is valid as long as there is a valid
definition of addition over their elements, in such case we shall assume
they are both subspaces of some larger vector space.

The sum of two vector space $V, W$ is defined as
$$V + W := \{v + w \mid v \in V, w \in W \}$$

The sum of $V, W$ is called a *direct sum* if $V + W \cong V \times W$.
An equivalent criterion is
$\forall u \in V + W, \exists ! v \in V, w \in W$ such that $u = v + w$.
In this case the sum is denoted as $V \oplus W$.

Condition for direct sum: iff $0 = \sum 0_i$ where $0_i$ refers to the
zero element in each addend.

The product of vector spaces is defined to be the Cartesian product of
the ground sets while addition and scalar multiplication are defined
componentwise. The product is also a vector space.

*Cartesian product* usually means that you are just talking about sets
with no additional structure. *Direct product* usually means you have
some sort of algebraic structure on each set and are considering the
Cartesian product to have the same algebraic structure defined
coordinatewise.

For finitely many vector spaces, direct sum and product are equivalent,
but for infinitely many vector spaces, direct sum is undefined.

The *quotient* of a vector space by a subspace is the vector space whose
elements are cosets (or affine subset) $v + U = \{v + u \mid u \in U\}$.
The addition and scalar multiplication are defined as

-   $(v + U) + (w + U) = (v + w) + U$,

-   $r(v + U) = (rv) + U$.

for $v, w \in V$ and $r \in k$.

## Span and Linear Independence

In $V$ over $k$,

A *linear combination* of vectors $v_1, \dots, v_n$ is a vector
$$a_1 v_1 + \dots + a_n v_n$$ with $a_1, \dots, a_n \in k$.

The set of all linear combinations of a set of vectors is called the
*span* of them, denoted $\spn \{v_1, \dots, v_n\}$.
$\spn \emptyset = \{0\}$.

If $\spn\{v_1, \dots, v_n\} = V$, we say $v_1, \dots, v_n$ spans $V$.

Span is the smallest containing subspace.

A set of vectors $v_1, \dots, v_n$ is called *linearly independent* if
the only choice of scalars annihilates $a_1v_1 + \cdots + a_nv_n$ is the
trivial one, i.e., $c_1 = \cdots = c_n = 0$.

The empty set $\emptyset$ is declared to be linearly independent.

## Bases and Dimension

A *basis* of $V$ is a linearly independent set of vectors spanning $V$.

Suppose $U$ is a subspace of $V$. Then $U$ has a complement $W$ in the
sense of direct sum such that $V = U \oplus W$.

All bases of a vector space have the same cardinality, which is called
the *dimension* of the vector space.

If $U_1, U_2$ are subspaces, then
$\dim (U_1 + U_2) = \dim U_1 + \dim U_2 - \dim (U_1 \cap U_2)$

$\dim (\bigtimes_{i=1}^m V_i) = \sum_{i=1}^m \dim V_i$.

Suppose $V$ is finite-dimensional and $U$ is a subspace of $V$. Then
$$\dim (V/U) = \dim V - \dim U.$$
