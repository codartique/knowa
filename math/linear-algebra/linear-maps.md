# Linear Maps

A $k$-linear map is a morphism in $\mathsf{Vect}_k$, that is a
homomorphism of vector spaces, often one suppresses the mention of $k$.

In elementary terms, a $k$-linear map between $k$-vector spaces $U$ and
$V$ is a function $T: U \to V$ such that
$$T(ru + v) = rT(u) + T(v), \forall u, v \in U.$$

One can check that $\mor(U, V)$ itself forms a $k$-vector space
(actually an algebra, with map composition as multiplication), which is
also denoted as $\mathcal{L}(U, V)$.

Fixing bases $\{u_1, \dots, u_n\}$ of $U$ and $\{v_1, \dots, v_n\}$ of
$V$, there exists a unique linear map $T: U \to V$ such that
$$T u_j = v_j, \quad j = 1, \dots, n.$$

## Kernel and Images

For $T: U \to V$,

$\ker T = \{Tu = 0 \mid u \in U\}, \quad \im T = T(U)$.

$\ker T$ is a subspace of $U$, and $\im T$ is a subspace of $V$.

$T$ is injective iff $\ker T = 0$. $T$ is surjective iff $\im T = W$.

Suppose $\dim V < \infty$ and $T: V \to W$, then
$$\dim V = \dim \ker T + \dim \im T.$$

- $\dim U > \dim V \Rightarrow T$ is not injective.

- $\dim U < \dim V \Rightarrow T$ is not surjective.

A homogeneous system of linear equations with more variables than
equations has nonzero solutions.

An inhomogeneous system of linear equations with more equations than
variables has no solution for some choice of the constant terms.

A linear map $T: U \to V$ is said to be *invertible* if there exists a
linear map $S: V \to U$ such that $ST = \id_U, TS = \id_V$.

An invertible linear map is also called a linear *isomorphism*, two
vector spaces are *isomorphic* if a linear isomorphism exists between
them.

The inverse is unique.

Invetible is equivalent to bijective.

Two finite-dimensional vector spaces over the same field are isomorphic
if and only if they have the same dimension.

## Operators

A linear map from a vector space to itself is called an *operator*.

The set of all operators on $V$ is denoted as $\mathrm{end} (V)$, or
$\mathcal{L}(V)$.

Suppose $T \in \mathrm{end} (V)$, then the following are equivalent:

-   $T$ is injective,

-   $T$ is surjective,

-   $T$ is invertible.

Suppose we have a quotient space $V/U$, the *quotient map* is the linear
map $$\pi : V \to V/U; v \mapsto v + U.$$

Each linear map $T: U \to V$ induces a linear isomorphism
$\tilde{T}: U/\ker T \to \im T$, which we now define.

## Duality

A *linear functional* on $V$ is a linear map from $V$ to $k$.

The *dual space* of $V$, denoted as $V^\ast$, is $\hom(V, k)$.

If $\{v_1, \dots, v_n\}$ is a basis of $V$, then the dual basis of
$\{v_1, \dots, v_n\}$ is the list $\{\varphi_1, \dots, \varphi_n\}$ of
elements of $V^\ast$, where each $\varphi_j$ is the linear functional on
$V$ such that
$$\varphi_j (v_k) = \begin{cases} 1, & k = j, \\ 0, & k \neq j. \end{cases}$$

Dual basis is a basis of the dual space, suppose $V$ is
finite-dimensional. Then the dual basis of a basis of $V$ is a basis of
$V^\ast$.

If $T \in \hom(U, V)$, then the *dual map* of $T$ is the linear map
$T^\ast \in \hom(V^\ast, U^\ast)$ defined by
$T^\ast(\varphi) = \varphi \circ T$ for $\varphi \in W^\ast$.

-   $(S + T)^\ast = S^\ast + T^\ast$ for all $S, T \in \hom(U, V)$.

-   $(rT)^\ast = r T^\ast$ for all $r \in k$ and all $T \in \hom(U, V)$.

-   $(ST)^\ast = T^\ast S^\ast$ for all $T \in \hom(U, V)$ and all
    $S \in \hom(V, W)$.

## Kernel and Image of a Dual Map

For $U \subseteq V$, the *annihilator* of $U$, denoted $U^0$, is defined
by
$$U^0 = \{ \varphi \in V^\ast \mid \varphi(u) = 0, \forall u \in U \}.$$

The annihilator is a subspace.

Suppose $V$ is finite-dimensional and $U$ is a subspace of $V$. Then
$$\dim U + \dim U^0 = \dim V.$$

-   $\ker T^\ast = (\im T)^0$;
    $\dim \ker T = \dim \ker T + \dim W - \dim V$.

-   $\im T^\ast = (\ker T)^0$; $\dim \im T^\ast = \dim \im T$.

-   $T$ injective is equivalent to $T^\ast$ surjective,

-   $T$ surjective is equivalent to $T^\ast$ injective.
