# Eigenvalues, Eigenvectors and Invariant Spaces {#sec:eigenvalues_eigenvectors_and_invariant_spaces}

Suppose $T \in \mathrm{end} (V)$. A subspace $U$ of $V$ is called
*invariant* under $T$ if $T(U) \subseteq U$.h

## Eigenvalues and Eigenvectors {#sub:eigenvalues_and_eigenvectors}

Suppose $T \in \mathrm{end} (V)$. A number $\lambda$ is called an
eigenvalue of $T$ if there exists $v \in V$ such that $v \neq 0$ and
$Tv = \lambda v$.

We also have $\lambda$ being an eigenvalue of $T$ if and only if
$T - \lambda I$ is not invertible ( or injective, or surjective, which
are equivalent by
\[\[#thm:injectivity~isequivalenttosurjectivityinfinitedimension~\]\[Theorem
[\[thm:injectivity~isequivalenttosurjectivityinfinitedimension~](#thm:injectivity_is_equivalent_to_surjectivity_in_finite_dimension)\]\]\]
)

Suppose $T \in \mathrm{end} (V)$ and $\lambda$ is an eigenvalue of $T$.
A vector $v \in V$ is called an *eigenvector* of $T$ corresponding to
$\lambda$ if $v \neq 0$ and $Tv = \lambda v$.
($v \in \ker (T - \lambda I)$)

Eigenvectors of a linear map corresponding to distinct eigenvalues are
linearly independent.

Suppose $V$ is finite-dimensional. Then each operator on $V$ has at most
$\dim V$ distinct eigenvalues.

### Restriction and Quotient Operators

If $T \in \mathrm{end} (V)$ and $U$ is a subspace of $V$ invariant under
$T$, then $U$ determines two other operators $T|_U \in \mathrm{end} (U)$
and $T/U \in \mathrm{end} (V/U)$ in a natural way, as defined below.

Suppose $T \in \mathrm{end} (V)$ and $U$ is a subspace of $V$ invariant
under $T$.

-   The *restriction operator* $T|_U \in \mathrm{end} (U)$ is defined by
    $T|_U (u) = T u$, for $u \in U$.

-   The *quotient operator* $T/U \in \mathrm{end} (V/U)$ is defined by
    $(T/U)(v + U) = Tv + U$ for $v \in V$.

### Existence of Eigenvalues {#ssub:existence_of_eigenvalues}

As a result of the Fundamental Theorem of Algebra.

Every operator on a finite-dimensional, nonzero, complex vector space
has an eigenvalue.

### eigenspace

Suppose $T \in \mathrm{end} (V)$ and $\lambda \in k$. The eigenspace of
$T$ corresponding to $\lambda$, denoted $E(\lambda, T)$, is defined by
$$E(\lambda, T) = \ker (T - \lambda I).$$ In other words,
$E(\lambda, T)$ is the set of all eigenvectors of $T$ corresponding to
$\lambda$, along with the $0$ vector.
