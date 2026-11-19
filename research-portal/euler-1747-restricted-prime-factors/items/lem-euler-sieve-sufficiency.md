---
id: lem-euler-sieve-sufficiency
kind: lemma
title: A union bound suffices for admissible summands
status: published
domain: mathematics
deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-classes
  - math:def-divides-in-z
  - def-euler-prime-obstruction-count
  - math:def-finite-cardinality
  - math:def-sum-over-a-finite-index-set
  - math:def-rationals
  - math:def-rat-operations
  - math:def-rat-order
  - math:thm-rat-ordered-field
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:thm-int-ordered-ring
  - lem-square-residue-parity
  - math:lem-divisor-bound
  - math:def-int-abs
  - math:def-subset-and-proper-subset
  - math:thm-subset-of-a-finite-set
  - math:def-nat-order
  - math:lem-nat-order-is-membership
  - math:thm-nat-linear-order
  - math:def-indexed-family
  - lem-euler-mixed-four-square-count
  - lem-finite-obstruction-cover-bound
  - lem-euler-unobstructed-pair-sums
  - math:def-natural-numbers
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:def-cartesian-product
  - math:def-power-set
  - math:def-axiom-schema-of-separation
  - math:thm-the-characterising-property-of-ordered-pairs
formulation_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - def-euler-four-square-representations
  - def-euler-mixed-four-square-representations
  - def-euler-prime-classes
  - math:def-divides-in-z
  - def-euler-prime-obstruction-count
  - math:def-finite-cardinality
  - math:def-sum-over-a-finite-index-set
  - math:def-rationals
  - math:def-rat-operations
  - math:def-rat-order
  - math:thm-rat-ordered-field
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
argument_deps:
  - math:thm-int-ordered-ring
  - def-euler-mixed-four-square-representations
  - def-euler-prime-classes
  - math:def-divides-in-z
  - def-euler-prime-obstruction-count
  - lem-square-residue-parity
  - math:lem-divisor-bound
  - math:def-int-abs
  - math:def-subset-and-proper-subset
  - math:thm-subset-of-a-finite-set
  - math:def-finite-cardinality
  - math:def-nat-order
  - math:lem-nat-order-is-membership
  - math:thm-nat-linear-order
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:thm-rat-ordered-field
  - math:def-indexed-family
  - math:def-sum-over-a-finite-index-set
  - lem-euler-mixed-four-square-count
  - lem-finite-obstruction-cover-bound
  - lem-euler-unobstructed-pair-sums
  - math:def-int-operations
  - math:def-natural-numbers
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:def-cartesian-product
  - math:def-power-set
  - math:def-axiom-schema-of-separation
  - math:thm-the-characterising-property-of-ordered-pairs
dependency_roles:
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  def-euler-four-square-representations: mathematical-premise
  def-euler-mixed-four-square-representations: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  def-euler-prime-obstruction-count: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:def-rationals: mathematical-premise
  math:def-rat-operations: mathematical-premise
  math:def-rat-order: mathematical-premise
  math:thm-rat-ordered-field: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  lem-square-residue-parity: mathematical-premise
  math:lem-divisor-bound: mathematical-premise
  math:def-int-abs: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:thm-nat-linear-order: mathematical-premise
  math:def-indexed-family: mathematical-premise
  lem-euler-mixed-four-square-count: mathematical-premise
  lem-finite-obstruction-cover-bound: mathematical-premise
  lem-euler-unobstructed-pair-sums: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-function: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-power-set: mathematical-premise
  math:def-axiom-schema-of-separation: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §2, equation (2.3), and p. 7, §6, application of (2.2) and (2.3)
dependency_level: 4
---

## Statement

Let $m$ be a positive odd integer, so $m>0$ and $m=2k+1$ for some integer $k$. Put $n=2m$. Let $\mathcal R(n)$ be the set of ordered integer quadruples $(x_1,x_2,x_3,x_4)$ with $x_1^2+x_2^2+x_3^2+x_4^2=n$, where $x_i^2=x_i\cdot x_i$. Each coordinate may be zero, positive or negative. Define $R(n)=|\mathcal R(n)|$, where $|S|$ denotes the number of elements of a finite set $S$, each counted once. Let $\mathcal R_{\mathrm{mix}}(n)$ consist of the quadruples in $\mathcal R(n)$ with one even and one odd entry in each of $(x_1,x_2)$ and $(x_3,x_4)$. An even integer has the form $2k$ for an integer $k$.

For integers $d,z$, write $d\mid z$ if $z=dq$ for some integer $q$. A prime is an integer $p>1$ whose only positive divisors are $1$ and $p$. Write $p\equiv r\pmod 4$ when $4\mid(p-r)$. Let $\mathcal P_3$ be the set of primes congruent to $3$ modulo $4$. For $p\in\mathcal P_3$, let $E_p(n)$ be the set of quadruples in $\mathcal R_{\mathrm{mix}}(n)$ for which $p$ divides both entries of at least one of the two pairs. Define $b_p(n)=|E_p(n)|$.

The set of primes $p\in\mathcal P_3$ with $E_p(n)$ nonempty is finite. The sum $\sum_{p\in\mathcal P_3}b_p(n)$ adds the counts over those primes, with value $0$ if there are none. If
$$\sum_{p\in\mathcal P_3}b_p(n)<\frac23 R(n),$$
then $n\in\mathcal A+\mathcal A$. Here $\mathcal A$ consists of the admissible integers, meaning the positive integers whose prime divisors are all congruent to $1$ modulo $4$, and $\mathcal A+\mathcal A$ consists of the integers $a+b$ with $a,b\in\mathcal A$. The inequality is between rational numbers, with each count identified with its value as a rational of denominator $1$.

## Statement references

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[def-euler-four-square-representations]]

[[def-euler-mixed-four-square-representations]]

[[def-euler-prime-classes]]

[[math:def-divides-in-z]]

[[def-euler-prime-obstruction-count]]

[[math:def-finite-cardinality]]

[[math:def-sum-over-a-finite-index-set]]

[[math:def-rationals]]

[[math:def-rat-operations]]

[[math:def-rat-order]]

[[math:thm-rat-ordered-field]]

[[math:lem-nat-embeds-int]]

[[math:lem-int-embeds-rat]]

## Facts & Assumptions

[F1] Integer addition and multiplication are associative and commutative, and multiplication distributes over addition. The integer order is total and adding the same integer to both sides of an inequality preserves it. [[math:thm-int-ordered-ring]]

[F2] For any positive integer $u$, the finite set $\mathcal R_{\mathrm{mix}}(u)$ has the stated square-sum condition and one even and one odd entry in each specified pair. For $p\in\mathcal P_3$, the stated divisibility test determines a unique subset $E_p(u)$ of $\mathcal R_{\mathrm{mix}}(u)$ and a unique count $b_p(u)$. Each $p\in\mathcal P_3$ is a prime and hence greater than $1$. Integer divisibility means that $d\mid z$ exactly when $z=dq$ for some integer $q$. [[def-euler-mixed-four-square-representations]] [[def-euler-prime-obstruction-count]] [[def-euler-prime-classes]] [[math:def-divides-in-z]]

[F3] For integers $x,y$ with one even and one odd entry, the sum $x^2+y^2$ is positive. [[lem-square-residue-parity]] If $d\mid v$ for integers $d,v$ with $v\ne0$, then $|d|\le |v|$. [[math:lem-divisor-bound]] For every nonnegative integer $a$, its integer absolute value satisfies $|a|=a$. [[math:def-int-abs]]

[F4] Specifying a membership condition on a set defines the subset consisting of the elements that satisfy it. Every subset of a finite set is finite. The cardinality $|S|$ of a finite set $S$ is its uniquely determined number of elements, which is a natural number. A bijection, meaning a one-to-one correspondence onto its target, transports finiteness. [[math:def-subset-and-proper-subset]] [[math:thm-subset-of-a-finite-set]] [[math:def-finite-cardinality]]

[F5] Use the additive order on the natural numbers, whose strict part $a<b$ means $a\le b$ and $a\ne b$. [[math:def-nat-order]] The additive order is total. [[math:thm-nat-linear-order]] The natural number $N$, viewed as a set, consists of exactly the natural numbers $j<N$. [[math:lem-nat-order-is-membership]] The set $N$ is finite and has cardinality $N$. [[math:def-finite-cardinality]]

[F6] The map $\iota$ from the natural numbers to the integers is one-to-one, preserves order, and takes precisely the integer values at least $0$. The map from the integers to the rationals sending $k$ to $k/1$ is one-to-one and preserves order. [[math:lem-nat-embeds-int]] [[math:lem-int-embeds-rat]] The rational order is well defined on classes because comparison is independent of the representatives with positive denominators. [[math:thm-rat-ordered-field]]

[F7] An indexed family is a function whose domain is the index set. A sum of natural numbers over finitely many indices is obtained by listing the indices once each and adding their corresponding terms. Its value is independent of the listing, and the empty sum is zero. [[math:def-indexed-family]] [[math:def-sum-over-a-finite-index-set]]

[F8] For $u=2m$ with $m$ positive and odd, $|\mathcal R_{\mathrm{mix}}(u)|=\frac23 R(u)$ with the counts viewed in the rationals. [[lem-euler-mixed-four-square-count]]

[F9] For a finite set $S$ and a family of subsets $(B_j)_{j\in I}$ of $S$ with only finitely many indices $j$ for which $B_j$ is nonempty, if $\sum_{j\in I}|B_j|<|S|$, then some element of $S$ lies in none of the $B_j$. The sum ranges over the indices of nonempty subsets, and the comparison is in the natural numbers. [[lem-finite-obstruction-cover-bound]]

[F10] For positive $u$, a quadruple in $\mathcal R_{\mathrm{mix}}(u)$ outside every $E_p(u)$ yields $a=x_1^2+x_2^2$ and $b=x_3^2+x_4^2$ in $\mathcal A$ with $a+b=u$. [[lem-euler-unobstructed-pair-sums]]

[F11] Separation forms the subset of a given set whose members satisfy a specified condition. A Cartesian product consists of all ordered pairs with first coordinate in its first factor and second coordinate in its second factor. Two ordered pairs are equal exactly when their corresponding coordinates agree. The power set of a set consists of all its subsets. A subset of a product is the graph of a function from its first factor to its second when each input has exactly one output. Such a function is a bijection if it is one-to-one and onto its target. [[math:def-axiom-schema-of-separation]] [[math:def-cartesian-product]] [[math:thm-the-characterising-property-of-ordered-pairs]] [[math:def-power-set]] [[math:def-function]] [[math:def-injection-surjection-bijection]]

[F12] Write $\mathbb N$ for the set of natural numbers. In the von Neumann naturals, $0=\varnothing$ and $1=\{0\}$. The map $\iota$ sends $k$ to $[(k,0)]$, and the integer constants $0$ and $1$ are $[(0,0)]$ and $[(1,0)]$, respectively. [[math:def-natural-numbers]] [[math:lem-nat-embeds-int]] [[math:def-int-operations]]

## Proof

**Given:** A positive odd integer $m$ and $n=2m$. For the implication, assume the stated strict inequality.

**Goal:** Show that the obstruction counts form a finite sum and that the strict inequality implies $n\in\mathcal A+\mathcal A$.

1.1 Since $0<m$, adding $m$ gives $m<m+m=2m=n$, so $n>0$. [given, F1]

1.2 On the natural numbers use the strict part of the additive order in F5. A one-to-one order-preserving map from a totally ordered set preserves strict inequalities because distinct inputs have distinct images. It also reflects strict inequalities, since if $a\ge b$ then the image of $a$ is at least the image of $b$. Apply this observation to $\iota$ and to the map from the integers to the rationals in F6. [F1, F5, F6]

2.1 In the natural numbers $0\in1$, since $1=\{0\}$. Thus $0<1$ in the natural order by F5. The map $\iota$ preserves strict order by Step 1.2 and sends the natural $0$ and $1$ to the integer $0$ and $1$ by F12. Hence $0<1$ in the integers. [F5, F12, step 1.2]

2.2 Set $S=\mathcal R_{\mathrm{mix}}(n)$, which is finite by F2. Separate inside $\mathcal P_3\times\mathcal P(S)$ the pairs $(p,T)$ for which $T=E_p(n)$, where $\mathcal P(S)$ is the power set of $S$. For each $p\in\mathcal P_3$, F2 gives exactly one such $T\subseteq S$, so the graph defines a function with domain $\mathcal P_3$. By F7 it is the indexed family $(E_p(n))_{p\in\mathcal P_3}$. [F2, F7, F11, step 1.1]

2.3 Fix any $p\in\mathcal P_3$ with $E_p(n)$ nonempty and take a quadruple in $E_p(n)$. Denote the two entries of a pair divisible by $p$ by $x,y$, and the other pair by $s,t$. The two sums $v=x^2+y^2$ and $w=s^2+t^2$ are positive because each pair has one even and one odd entry. The defining equation gives $v+w=n$. Adding $v$ to $0<w$ gives $v<n$. [F1, F2, F3, step 1.1]

3.1 By the definition of integer divisibility in F2, $x=pq$ and $y=pr$ for integers $q,r$. Thus $v=p[p(q^2+r^2)]$, so $p\mid v$. Since $p>1>0$ and $v>0$, F3 gives $|p|\le |v|$, with $|p|=p$ and $|v|=v$. Hence $0<p\le v<n$ for every $p\in\mathcal P_3$ with $E_p(n)$ nonempty. [F1, F2, F3, step 2.1, step 2.3]

4.1 By separation let $J$ be the subset of $\mathcal P_3$ with $E_p(n)$ nonempty. Let $N$ be the natural number with $\iota(N)=n$. By F5, the set $N$ is finite. Separate inside $N$ the subset $D$ of elements $j$ such that $\iota(j)\in J$. This subset of $N$ is finite. Keep from the graph of $\iota$ exactly the pairs whose first coordinate belongs to $D$. Each $j\in D$ has the unique output $\iota(j)\in J$, so the restricted graph defines a function $D\to J$. The function is injective by F6. Every $p\in J$ satisfies $0<p<n$ by Step 3.1, so F6 gives a unique natural $j$ with $\iota(j)=p$. By Step 1.2, $j<N$, so $j\in N$ by F5 and hence $j\in D$. Thus the function is onto $J$. This bijection from the finite set $D$ makes $J$ finite by F4. [F4, F5, F6, F11, step 1.1, step 1.2, step 3.1, step 2.2]

5.1 For each $p\in J$, F2 gives the unique natural number $b_p(n)=|E_p(n)|$. Keeping the pairs $(p,b_p(n))$ by separation inside $J\times\mathbb N$ gives a function $J\to\mathbb N$. Applying F7 to this function on the finite set $J$ yields the well-defined natural-number sum in the statement, including the value zero if $J$ is empty. [F2, F7, F11, F12, step 4.1]

6.1 Assume the strict inequality in the statement. The comparison takes place in the well-defined rational order of F6. Since $n=2m$ with $m$ positive and odd, F8 identifies its right-hand side with the count of $\mathcal R_{\mathrm{mix}}(n)$. Both sides are now images of natural numbers under the two maps of F6. By Step 1.2 the strict comparison holds between those natural numbers. [given, F6, F8, step 1.2, step 5.1]

7.1 Apply F9 to the finite set $S$ and the family $(E_p(n))_{p\in\mathcal P_3}$ from Step 2.2. Its nonempty members have indices exactly in the finite set $J$ from Step 4.1. The sum of their cardinalities is the natural-number sum from Step 5.1, which is strictly less than $|S|$ by Step 6.1. Hence there is a quadruple in $\mathcal R_{\mathrm{mix}}(n)$ lying outside $E_p(n)$ for every $p\in\mathcal P_3$. [F9, step 2.2, step 4.1, step 5.1, step 6.1]

8.1 By F10, the two pair sums of this quadruple lie in $\mathcal A$ and add to $n$. The definition of $\mathcal A+\mathcal A$ therefore gives $n\in\mathcal A+\mathcal A$. [F2, F10, step 7.1] ∎
