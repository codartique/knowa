# Limits

Recall that in categorical language, a limit captures the essentials of
constructions such as products, pullbacks and inverse limits, and is
defined as a cone of a diagram satisfying a particular universal
property.

Meanwhile, the limit of a sequence described here generalize very well
in point-set topology to the idea of the limit of a filter.

## The Limit of a Sequence

As a special case of functions, a **sequence** is nothing more than a
function over $\mathbb{N}$. The limit of a sequence is defined solely at
the point $\infty$, as only around $\infty$ there is a well-defined
notion of neighborhood filter (the subset $\mathbb{N}$ has only one
limit point under the inherited topology from
$\mathbb{R} \cup \{ \infty \}$).

The usual definition utilizes the $\varepsilon$ - $N$ language,

<div class="definition">
A sequence $\{ a_n \}$ is said to converge to $A$, if
$\forall \varepsilon > 0$, $\exists N > 0$ such that if $n > N$, then
$d(a_n, A) < \varepsilon$.
</div>

### Properties of Sequential Limits

Topological properties

<div class="theorem">

-   Any neighborhood of the limit contains all but finitely many terms
    of the sequence.
-   The limit is unique.
-   A convergent sequence is bounded.

</div>

Compatible with arithmetic operations

<div class="theorem">

-   $\lim x_n + y_n = \lim x_n + \lim y_n$
-   $\lim x_n \cdot y_n = \lim x_n \cdot \lim y_n$

</div>

Inequalities

<div class="theorem">
-   Let $\{x_n\}, \{y_n\}$ be two convergent sequence with
    $\lim x_n = A, \lim y_n = B$. If $A < B$, then
    $\exists N \in \mathbb{N}$ such that $x_n < y_n$ for all $n \geq N$.
-   Suppose $\{x_n\}, \{y_n\}, \{z_n\}$ are sequences such that
    $x_n \leq y_n \leq z_n$ if $n \geq N$ for some $N \in \mathbb{N}$
    and $\lim x_n = \lim z_n =: A$, then $\lim y_n = A$.
</div>

### Subsequences

<div class="definition">
Given a sequence $\{x_n\}$, consider an increasing sequence $\{n_k\}$ of
natural numbers. Then the sequence $\{x_{n_k}\}$ is called a
*subsequence* of $\{x_n\}$ and its limit is called a *subsequential
limit* of $\{x_n\}$.
</div>

### Inferior and Superior Limits

### Numerical Series

<div class="definition">
Given a sequence $\{a_n\}$, A *series* is a formal sum $\sum_{n=1}^\infty a_k$. With $\{a_n\}$ we associate a sequence of *partial sums* $\{s_n\}$ where $s_n := \sum_{k=1}^{n} a_k$. if $\{s_n\}$ converges to $s$, we say that the series converges, and write $$\sum_{n=1}^\infty a_n = s.$$
</div>

<div class="theorem">
The series converges iff $\forall \varepsilon > 0$,
$\exists N \in \mathbb{N}$ such that $\forall m \geq n \geq N$ imply
$\left| \sum_{k=n}^m a_k \right| < \varepsilon$.
</div>

<div class="corollary">
A necessary condition for the series to converge is $a_n \to 0$ as
$n \to \infty$.
</div>

#### Series of Nonnegative Terms

<div class="theorem">
A series of nonnegative terms converges iff its partial sums form a
bounded sequence.
</div>

<details class="proof">
<summary>Proof</summary>
As the partial sums form a monotonic non-decreasing sequence. Then by [Monotone Convergence Theorem](#7B6EF184-23B7-47F2-9FC6-46AF4C754638).
</details>

<div class="theorem">
A monotonic non-increasing series $\sum_{n=1}^\infty a_n$ converges
iff the series $\sum_{k=0}^\infty 2^k a_{2^k}$ converges.
</div>

Examples

<div class="example">

-   (geometric series) $\sum_{n=0}^\infty x^n = \frac{1}{1-x}$ if $0 \leq x < 1$, and diverges if $x \geq 1$.

-   ($p$-series) $\sum n^{-p}$ converges if $p > 1$ and diverges if $p \leq 1$.

-   ($p$-logarithmic series) $\sum_{n=2}^\infty \frac{1}{n(\log n)^p}$ converges if $p > 1$, and diverges if $p \leq 1$.

</div>

#### The number $e$

<div class="definition">
$e := \sum_{n=0}^\infty \frac{1}{n!}$.
</div>

<div class="theorem">
$\lim_{n\to\infty} (1 + \frac{1}{n})^n = e$
</div>

<div class="theorem">
$e$ is irrational.
</div>

#### Absolute Convergence

<div class="definition">
A series $\sum a_n$ is said to *converge absolutely* if the series
$\sum |a_n|$ converges.
</div>

<div class="theorem">
If a series converges absolutely, then it converges.
</div>

#### Convergence Tests

Comparison test
	
Root test
		
Ratio test

#### Operations on Series

-   Summation by parts
-   Addition and Multiplication
-   Rearrangements

## The Limit of a Function

Limits of functions are a special case of limits of filters.

<div class="definition">
$L$ is a limit of $f$ approaching $c$ iff $L$ is a limit of
$f(\mathring{\mathcal{N}}_c)$.
</div>

In an metrizable space, the definition can be reworded into the usual
$\varepsilon$ - $\delta$ language.

<div class="definition">
A function $f$ is said to converge to $A$ at $x_0$, if
$\forall \varepsilon > 0$, $\exists \delta > 0$ such that if
$d(x, x_0) < \delta$, then $d(f(x), L) < \varepsilon$.
</div>
