# Inner Product Spaces

An *inner product* is a map
$\langle \cdot , \cdot \rangle : V \times V \to k$ which satisfies

-   **conjugate symmetry**:
    $\langle x, y \rangle = \overline{\langle y, x \rangle}$;

-   **linear in the first argument**:
    $\langle ax + by, z \rangle = a \langle x, z \rangle + b \langle y, z \rangle$;

-   **positive-definiteness**: $\langle x, x \rangle \geq 0$, the
    equality holds only if $x = 0$.

The inner product hereby induces a *norm*
$$\| \cdot \| : x \mapsto \sqrt{\langle x, x \rangle},$$ and moreover a
metric $d(x, y) = \| x - y \|$.

Two vectors $u, v \in V$ are called *orthogonal* if
$\langle u, v \rangle = 0$.

## Orthonormal Bases
