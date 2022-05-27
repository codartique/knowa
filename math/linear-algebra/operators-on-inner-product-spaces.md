# Operators on Inner Product Spaces

## Positive Operators and Isometries

An operator $T \in \mathcal{L}(V)$ is called *positive* if $T$ is
self-adjoint and $\langle Tv, v \rangle \geq 0$ for all $v \in V$.

An operator $R$ is called a *square root* of an operator $T$ if
$R^2 = T$.

Let $T \in \mathcal{L}(V)$. Then the following are equivalent:

-   $T$ is positive;

-   $T$ is self-adjoint and all the eigenvalues of $T$ are nonnegative;

-   $T$ has a positive square root;

-   $T$ has a self-adjoint square root;

-   there exists an operator $R \in \mathcal{L}(V)$ such that
    $T = R^\ast R$.

Every positive operator on $V$ has a unique positive square root.

### Isometries

As an inner product $\langle \cdot , \cdot \rangle$ induces a norm
$\| \cdot \|$, and moreover a metric $d(\cdot, \cdot)$.

An *isometry* is a map between metric spaces $f: X \to Y$ such that
$$d_X(x, y) = d_Y(f(x), f(y)).$$

In our settings, it is equivalent to preserves norms,
$\| Sv \| = \| v \|$.

Suppose $S \in \mathcal{L}(V)$. Then the following are equivalent:

1.  $S$ is an isometry;

2.  $\langle Su, Sv \rangle = \langle u, v \rangle$ for all
    $u, v \in V$;

3.  $\{Se_1, \dots, Se_n\}$ is orthonormal for every orthonormal set of
    vectors $\{e_1, \dots, e_n\}$ in $V$;

4.  there exists an orthonormal basis $\{e_1, \dots, e_n\}$ of $V$ such
    that $\{Se_1, \dots, Se_n\}$ is orthonormal;

5.  $S^\ast S = I$;

6.  $S S^\ast = I$;

7.  $S^\ast$ is an isometry;

8.  $S$ is invertible and $S^{-1} = S^\ast$.

Moreover, when $k = \CC$,

1.  There is an orthonormal basis of $V$ consisting of eigenvectors of
    $S$ whose corresponding eigenvalues all have absolute value $1$.

## Polar Decomposition and Singular Value Decomposition

Suppose $T \in \mathcal{L}(V)$, then there exists an isometry
$S \in \mathcal{L}(V)$ such that $$T = S \sqrt{T^\ast T}.$$

The Polar Decomposition states that each operator on V is the product of
an isometry and a positive operator. Thus we can write each operator on
V as the product of two operators, each of which comes from a class that
we can completely describe and that we understand reasonably well.

Specifically, consider the case $k = \CC$, and suppose
$T = S \sqrt{T^\ast T}$ is a Polar Decomposition of an operator
$T \in \mathcal{L}(V)$, where $S$ is an isometry. Then there is an
orthonormal basis of $V$ with respect to which $S$ has a diagonal
matrix, and there is an orthonormal basis of $V$ with respect to which
$\sqrt{T^\ast T}$ has a diagonal matrix. Warning: there may not exist an
orthonormal basis that simultaneously puts the matrices of both $S$ and
$\sqrt{T^\ast T}$ into these nice diagonal forms. In other words, $S$
may require one orthonormal basis and $\sqrt{T^\ast T}$ may require a
different orthonormal basis.

### Singular Value Decomposition

Suppose $T \in \mathcal{L}(V)$. The *singular values* of $T$ are the
eigenvalues of $\sqrt{T^\ast T}$, with each eigenvalue $\lambda$
repeated $\dim E(\lambda, \sqrt{T^\ast T})$ times.

Suppose $T \in \mathcal{L}(V)$ has singular values $s_1, \dots, s_n$.
Then there exist orthonormal basis $e_1, \dots, e_n$ and
$f_1, \dots, f_n$ of $V$ such that
$$Tv = s_1 \langle v, e_1 \rangle f_1 + \dots + s_n \langle v, e_n \rangle f_n$$
for every $v \in V$.

Suppose $T \in \mathcal{L}(V)$. Then the singular values of $T$ are the
nonnegative square roots of the eigenvalues of $T^\ast T$, with each
eigenvalue repeated $\dim E(\lambda, T^\ast T)$ times.

## Operators on Complex Vector Spaces

Suppose $T \in \mathcal{L}(V)$, then
$\ker T \subseteq \ker T^2 \subseteq \cdots \subseteq \ker T^k \subseteq \ker T^{k+1} \subseteq \cdots$.
This chain of containing will eventually stablize as

For the above $T$, suppose $m \in \ZZ_+$ such that
$\ker T^m = \ker T^{m+1}$. Then
$$\ker T^m = \ker T^{m+1} = \ker T^{m+2} = \cdots .$$

and for $m = \dim V$, there is always $\ker T^{m} = \ker T^{m}$.

It is not true generally that $V = \ker T \oplus \im T$, but an
alternative is

Suppose $T \in \mathcal{L}(V)$. Let $n = \dim V$. Then
$$V = \ker T^n \oplus \im T^n.$$

Suppose $T \in \mathcal{L}(V)$ and $\lambda$ is an eigenvalue of $T$. A
vector $v \in V$ is called a *generalized eigenvector* of $T$
corresponding to $\lambda$ if $v \neq 0$ and $$(T - \lambda I)^j = 0$$
for some positive integer $j$.

Suppose $T \in \mathcal{L}(V)$ and $\lambda \in k$. The *generalized
eigenspace* of $T$ corresponding to $\lambda$, denoted $G(\lambda, T)$,
is defined to be the set of all generalized eigenvectors of $T$
corresponding to $\lambda$, along with the $0$ vector.

Suppose $T \in \mathcal{L}(V)$ and $\lambda \in k$. Then
$G(\lambda, T) = \ker (T - \lambda I)^{\dim V}$.

Let $T \in \mathcal{L}(V)$. Suppose $\lambda_1, \dots, \lambda_m$ are
distinct eigenvalues of $T$ and $v_1, \dots, v_m$ are corresponding
generalized eigenvectors. Then $v_1, \dots, v_m$ is linearly
independent.

Suppose $N \in \mathcal{L}(V)$ is nilpotent. Then $N^{\dim V} = 0$.

Suppose $N$ is a nilpotent operator on $V$. Then there is a basis of $V$
with respect to which the matrix of $N$ has the form
$$\begin{pmatrix} 0 & & \ast \\ & \ddots & \\ 0 & & 0 \end{pmatrix};$$
here all entries on and below the diagonal are $0$\'s.
