---
id: lem-euler-obstructing-prime-square-tail
kind: lemma
title: "Lemma 5.2: Reciprocal-square tail of the obstructing primes"
status: published
domain: mathematics
proof_strategy: direct
deps:
  - def-euler-prime-classes
  - math:def-complete-ordered-real-field
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-field
  - math:def-integer-power
  - math:def-natural-numbers
  - math:def-sequence
  - math:def-finite-sum
  - math:def-series
  - math:def-real-limit
  - def-euler-obstructing-prime-residue-count
  - lem-euler-obstructing-prime-residue-inclusion
  - lem-euler-residue-reciprocal-square-tail
  - math:lem-of-inverse-positive
  - math:lem-nat-embeds-int
  - math:lem-finite-sum-laws
  - math:thm-nonnegative-series-bounded-partial-sums
  - math:def-nat-order
  - math:def-rationals
  - math:lem-limit-of-tail
formulation_deps:
  - def-euler-prime-classes
  - math:def-complete-ordered-real-field
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-field
  - math:def-integer-power
  - math:def-natural-numbers
  - math:def-sequence
  - math:def-finite-sum
  - math:def-series
  - math:def-real-limit
  - math:def-nat-order
  - math:def-rationals
  - math:lem-nat-embeds-int
argument_deps:
  - def-euler-prime-classes
  - def-euler-obstructing-prime-residue-count
  - lem-euler-obstructing-prime-residue-inclusion
  - lem-euler-residue-reciprocal-square-tail
  - math:def-complete-ordered-real-field
  - math:def-field
  - math:def-integer-power
  - math:lem-of-inverse-positive
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:def-sequence
  - math:def-finite-sum
  - math:def-series
  - math:lem-finite-sum-laws
  - math:thm-nonnegative-series-bounded-partial-sums
  - math:def-nat-order
  - math:lem-limit-of-tail
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  math:def-complete-ordered-real-field: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-field: mathematical-premise
  math:def-integer-power: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-sequence: mathematical-premise
  math:def-finite-sum: mathematical-premise
  math:def-series: mathematical-premise
  math:def-real-limit: mathematical-premise
  def-euler-obstructing-prime-residue-count: mathematical-premise
  lem-euler-obstructing-prime-residue-inclusion: mathematical-premise
  lem-euler-residue-reciprocal-square-tail: mathematical-premise
  math:lem-of-inverse-positive: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-finite-sum-laws: mathematical-premise
  math:thm-nonnegative-series-bounded-partial-sums: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:def-rationals: mathematical-premise
  math:lem-limit-of-tail: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 6, Lemma 5.2, equation (5.3) and the sentence following the
        partial-summation display
dependency_level: 3
---

## Statement

Use the real numbers with the integers included so that order and arithmetic are preserved. Let $\mathcal P_3$ be the set of primes congruent to $3$ modulo $4$. An integer $p$ is prime if $p>1$ and its only positive divisors are $1$ and $p$. A positive divisor of $p$ is an integer $d>0$ with $p=dq$ for some integer $q$. Congruence to $3$ modulo $4$ means that $p-3=4q$ for some integer $q$.

For every real cutoff $P\ge3$, the series converges and satisfies
$$\sum_{\substack{p>P\\p\in\mathcal P_3}}\frac{1}{p^2}\le\frac{2}{15P}+\frac{2}{P^2}.$$

Here $x^2=x\cdot x$, and $a/b$ is the product of $a$ and the reciprocal of the nonzero real number $b$. Identify each natural number with its image under the order-preserving embedding into the integers. To form the series, take the sequence of real terms indexed by the natural numbers $0,1,2,\ldots$, using $1/k^2$ at index $k$ when $k>P$ and $k\in\mathcal P_3$, and zero otherwise. The $n$th partial sum adds the terms with $k<n$, starting at zero. The series converges to $L$ if these partial sums have limit $L$. This means that for every rational $\varepsilon$ whose real image $\widehat\varepsilon$ is positive, there is a natural number $N$ such that for every natural $n\ge N$ the $n$th partial sum differs from $L$ by less than $\widehat\varepsilon$ in absolute value. The absolute value of a real number is the number itself when nonnegative and its negative otherwise.

## Statement references

[[def-euler-prime-classes]]

[[math:def-complete-ordered-real-field]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-prime]]

[[math:def-divides-in-z]]

[[math:def-congruence-modulo-an-integer]]

[[math:def-field]]

[[math:def-integer-power]]

[[math:def-natural-numbers]]

[[math:def-sequence]]

[[math:def-finite-sum]]

[[math:def-series]]

[[math:def-real-limit]]

[[math:def-nat-order]]

[[math:def-rationals]]

[[math:lem-nat-embeds-int]]

## Facts & Assumptions

[F1] In the real ordered field, $1>0$, the order is transitive, and sums and products of positive numbers are positive ([[math:def-complete-ordered-real-field]]). Each nonzero real number has a unique reciprocal, and the reciprocal of a positive real number is positive ([[math:def-field]], [[math:lem-of-inverse-positive]]). The natural numbers identify in order with the nonnegative integers ([[math:lem-nat-embeds-int]]).

[F2] Let $D$ be the set of positive integers in the residue classes modulo $60$ represented by $7,11,19,23,31,43,47,59$. The class represented by $r$ consists of the integers $k$ for which $k-r=60q$ for some integer $q$ ([[def-euler-obstructing-prime-residue-count]]). Every $p\in\mathcal P_3$ with $p>3$ belongs to one of these classes ([[lem-euler-obstructing-prime-residue-inclusion]]).

[F3] For real $P\ge3$, the series of $1/k^2$ over the integers $k\in D$ with $k>P$ converges to a sum at most $2/(15P)+2/P^2$. Its $n$th partial sum $C_n$ adds the terms for natural indices $j<n$, using at index $j$ the term for the positive integer corresponding to the successor $j+1$ ([[lem-euler-residue-reciprocal-square-tail]]).

[F4] If $a_k\le b_k$ at every index $k<n$, then the finite sums satisfy $\sum_{k<n}a_k\le\sum_{k<n}b_k$ ([[math:lem-finite-sum-laws]], part 4).

[F5] A series of nonnegative real terms converges if its partial sums have a common real upper bound. In the convergent case its sum is the least upper bound of its partial sums, meaning the smallest real number that bounds them all from above ([[math:thm-nonnegative-series-bounded-partial-sums]], part 2).

[F6] If the first tail $(x_{n+1})$ of a real sequence $(x_n)$ converges to $T$, then $(x_n)$ converges to $T$ ([[math:lem-limit-of-tail]]).

[F7] For any real sequence $(u_j)$, its finite sums form the unique real sequence $(S_n)$ with $S_0=0$ and $S_{n+1}=S_n+u_n$ ([[math:def-finite-sum]]). The real field has additive identity $0$, so $0+0=0$ ([[math:def-field]]).

## Proof

**Given:** A real number $P\ge3$ and the prime class $\mathcal P_3$ from the Statement.

**Goal:** Prove convergence of the prime series and the bound $2/(15P)+2/P^2$.

1.1 Let $(a_k)$ be the sequence defining the prime series in the Statement. For each natural number $k$, put $b_k=1/k^2$ if $k>P$ and $k\in D$, and put $b_k=0$ otherwise. The terms are well-defined and nonnegative because a term using $1/k^2$ has $k>P\ge3>0$, so $k^2>0$ and its reciprocal is positive. In particular, $b_0=0$ because $0<P$. Write $B_n=\sum_{k<n}b_k$. [given, F1, F2, F7]

2.1 By the indexing in [F3], the term at index $j$ in the residue-class series is $b_{j+1}$. By [F7], $C_0=0$ and $B_0=0$. Since $b_0=0$, we have $B_1=B_0+b_0=0+0=0=C_0$. For every natural $n$, the two successor equations from [F7] give $C_{n+1}=C_n+b_{n+1}$ and $B_{(n+1)+1}=B_{n+1}+b_{n+1}$. Thus $(C_n)$ and $(B_{n+1})$ both satisfy the defining recursion for partial sums of $(b_{j+1})_{j\in\mathbb N}$. Uniqueness in [F7] gives $B_{n+1}=C_n$ for every natural $n$. [F3, F7, step 1.1]

2.2 If $k>P$ and $k\in\mathcal P_3$, then $k>3$ and [F2] gives $k\in D$, since $k$ is positive. Both terms then equal $1/k^2$. At every other index $a_k=0$ and $b_k\ge0$. This proves $0\le a_k\le b_k$ at every index, including zero. [given, F1, F2, step 1.1]

3.1 By [F3], $(C_n)$ converges to a real number $T\le2/(15P)+2/P^2$. Step 2.1 identifies $(C_n)$ with the first tail of $(B_n)$. By [F6], $(B_n)$ converges to $T$, so the series of $(b_k)$ has sum $T$. [F3, F6, step 2.1]

4.1 Write $A_n=\sum_{k<n}a_k$ for the prime partial sums. For each natural $n$, [F4] gives $A_n\le B_n$. The terms $b_k$ are nonnegative and their series converges to $T$, so [F5] gives $B_n\le T$. Hence $T$ is a common upper bound for all $A_n$. [F4, F5, step 3.1, step 2.2]

5.1 Since the terms $a_k$ are nonnegative and their partial sums are bounded above by $T$, [F5] gives convergence and identifies the sum as the least upper bound of the $A_n$. This sum is at most $T$, which is at most $2/(15P)+2/P^2$ by step 3.1. [F5, step 3.1, step 2.2, step 4.1] ∎
