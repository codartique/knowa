# Matrices, Representations of Linear Maps {#sec:matrices}

A *matrix* is an $2$-dimensional array of scalars with perscribed rows
and columns. A matrix with $m$ rows and $n$ columns is called a
$m$-by-$n$ matrix, and is usually written
$$A = \begin{bmatrix} a_{11} & \cdots & a_{1n} \\ \vdots & \ddots & \vdots \\ a_{m1} &\cdots & a_{mn} \end{bmatrix}.$$
The set of all $m$-by-$n$ matrices of entries in $k$ is denoted as
$M_{m\times n}(k)$. A matrix can also be written blockwise, in its
submatrices
$$A = \begin{bmatrix} A_{11} & \cdots & A_{1q} \\\\ \vdots & \ddots & \vdots \\\\ A_{p1} & \cdots & A_{pq} \end{bmatrix}$$

## Basic Operations

Matrices with entries in some field forms an algebra over that field.

-   Matrix addition and scalar multiplication are defined entrywise.

-   Suppose $A$ is a $m$-by-$n$ matrix and $B$ is a $n$-by-$p$ matrix,
    the multiplication $AB$ is defined such that
    $$(AB)_{ij} = \sum_{r=1}^n a_{ir}b_{rj}.$$ Notice that the
    multiplication is not commutative.

-   Transposition The *transposition* of a matrix $A$ is
    $(A^\top)_{ij} = A_{ji}$.

### Special Matrices

upper-triangular matrix lower-triangular matrix diagonal matrix

## Matrices as Linear Maps

Matrix of a linear map $M(T)$. When bases are fixed, the linear map $T$
can be represented via a matrix $M$ by letting $Tv_k = \sum M_{ik}w_i$

Suppose $\dim U = n, \dim V = m$, then
$\hom(U, V) \cong k^{m \times n}$.

## Linear Maps Thought of as Matrix Multiplication

In what follows we fix a basis $\{v_1, \dots, v_n\}$ of $V$.

Suppose $v \in V$ such that $v = \sum_i c_iv_i$, the *matrix of $v$*
with respect to basis $\{v_1, \dots, v_n\}$

## Matrices as Bilinear Forms
