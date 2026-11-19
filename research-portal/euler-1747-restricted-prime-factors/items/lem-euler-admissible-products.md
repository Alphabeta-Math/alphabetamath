---
id: lem-euler-admissible-products
kind: lemma
title: Products and congruence of admissible integers
status: published
domain: mathematics
proof_strategy: direct
deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-monoid-finite-product
  - math:thm-int-ordered-ring
  - math:thm-euclids-lemma
  - math:lem-units-of-z
  - math:thm-fundamental-theorem-of-arithmetic
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
  - math:thm-generalised-associativity
  - math:thm-induction-principle
  - math:lem-congruence-respects-integer-arithmetic
  - math:def-natural-numbers
  - math:def-nat-order
  - math:lem-nat-order-is-membership
  - math:lem-nat-nonzero-is-successor
  - math:def-symmetric-group
formulation_deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-monoid-finite-product
  - math:def-natural-numbers
  - math:def-nat-order
argument_deps:
  - def-euler-prime-classes
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-monoid-finite-product
  - math:thm-int-ordered-ring
  - math:thm-euclids-lemma
  - math:lem-units-of-z
  - math:thm-fundamental-theorem-of-arithmetic
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
  - math:thm-generalised-associativity
  - math:thm-induction-principle
  - math:lem-congruence-respects-integer-arithmetic
  - math:def-natural-numbers
  - math:def-nat-order
  - math:lem-nat-order-is-membership
  - math:lem-nat-nonzero-is-successor
  - math:def-symmetric-group
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-euclids-lemma: mathematical-premise
  math:lem-units-of-z: mathematical-premise
  math:thm-fundamental-theorem-of-arithmetic: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:thm-generalised-associativity: mathematical-premise
  math:thm-induction-principle: mathematical-premise
  math:lem-congruence-respects-integer-arithmetic: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:lem-nat-nonzero-is-successor: mathematical-premise
  math:def-symmetric-group: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, §1, definition of admissible summands and Euler formulation; p.
        1, Lemma 2.1, scaling step
dependency_level: 2
---

## Statement

Write $\mathbb Z$ for the integers. An integer $a$ is **admissible** if $a>0$ and every prime divisor $p$ of $a$ satisfies $p\equiv1\pmod4$. Write $\mathcal A$ for the set of admissible integers. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Here a positive integer is one greater than $0$, and $d\mid a$ means $a=dq$ for some $q\in\mathbb Z$. A prime divisor of $a$ is a prime $p$ with $p\mid a$. The notation $x\equiv1\pmod4$ means $4\mid(x-1)$.

A finite list of length $r\in\mathbb N$ has one entry for each natural number $i<r$, with $\mathbb N$ including $0$. Every finite product of members of $\mathcal A$ belongs to $\mathcal A$, with the product formed by starting at $1$ and multiplying the entries in order. In particular the product of no entries is $1$. Every member of $\mathcal A$ is congruent to $1$ modulo $4$.

## Statement references

[[def-euler-prime-classes]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-prime]]

[[math:def-divides-in-z]]

[[math:def-congruence-modulo-an-integer]]

[[math:def-monoid-finite-product]]

[[math:def-natural-numbers]]

[[math:def-nat-order]]

## Facts & Assumptions

[F1] The defining condition for membership in $\mathcal A$ is positivity together with congruence to $1$ modulo $4$ for each prime divisor ([[def-euler-prime-classes]]). We use the integers, their addition and multiplication, and their order, with positivity defined by $a>0$ ([[math:def-integers]], [[math:def-int-operations]], [[math:def-int-order]]).

[F2] Divisibility $d\mid a$ means $a=dq$ for an integer $q$. A prime $p$ satisfies $p>1$, and a prime divisor is a prime that divides the given integer ([[math:def-divides-in-z]], [[math:def-prime]]). The congruence $x\equiv y\pmod4$ means $x-y=4q$ for some integer $q$ ([[math:def-congruence-modulo-an-integer]]).

[F3] Products of positive integers are positive. Integer multiplication is associative and commutative, with identity $1$ and $4\cdot0=0$ ([[math:thm-int-ordered-ring]]). The integer divisors of $1$ are exactly $1$ and $-1$ ([[math:lem-units-of-z]]).

[F4] Euclid's lemma states that if $p$ is prime and $x,y$ are integers with $p\mid xy$, then $p\mid x$ or $p\mid y$ ([[math:thm-euclids-lemma]]).

[F5] Every integer $c\ge1$ is a product of a finite list of primes ([[math:thm-fundamental-theorem-of-arithmetic]], existence clause). Positive integers are at least $1$: each nonnegative integer corresponds to a natural number with $0$, $1$, and order preserved, and no natural number lies strictly between $0$ and $1$ ([[math:lem-nat-embeds-int]], [[math:lem-nat-discrete]]).

[F6] For an integer list, the product at length $0$ is $1$, and at length $\sigma(j)$ it is the product of the first $j$ entries multiplied by the entry at index $j$ ([[math:def-monoid-finite-product]]). The value depends only on the entries of the list, so any extension to a family on $\mathbb N$ can be used. For integer multiplication, if $\pi$ is a permutation of the index set $r$, the list with entries $h_i=p_{\pi(i)}$ has the same product as $p$ ([[math:thm-generalised-associativity]], commutative case, applied to such extensions).

[F7] Induction proves a property for all lengths in $\mathbb N$ if the property holds at $0$ and passes from each $j$ to its successor $\sigma(j)$ ([[math:thm-induction-principle]]).

[F8] If integers $x,x',y,y'$ satisfy $x\equiv x'\pmod4$ and $y\equiv y'\pmod4$, then $xy\equiv x'y'\pmod4$ ([[math:lem-congruence-respects-integer-arithmetic]]).

[F9] The von Neumann naturals have $0=\varnothing$ and successor $\sigma(j)=j\cup\{j\}$ ([[math:def-natural-numbers]]), and for the natural order, $j<r$ means $j\le r$ and $j\ne r$ ([[math:def-nat-order]]). The indices of a list of length $r$ are the members of $r$, since $i<r$ is equivalent to $i\in r$. Also $j\le r$ is equivalent to $j\subseteq r$ ([[math:lem-nat-order-is-membership]]). Discreteness gives $j<r$ if and only if $\sigma(j)\le r$ ([[math:lem-nat-discrete]]). Every nonzero natural number is a successor ([[math:lem-nat-nonzero-is-successor]]).

[F10] A permutation of $r$ is a bijection $r\to r$. The identity and the transposition of any two distinct elements of $r$ are permutations ([[math:def-symmetric-group]]).

## Proof

**Given:** The set $\mathcal A$ of admissible integers as defined in the Statement.

**Goal:** Prove that every finite product of members belongs to $\mathcal A$ and that every member is congruent to $1$ modulo $4$.

1.1 Let $a,b\in\mathcal A$. Then $ab>0$. For any prime $p$ with $p\mid ab$, Euclid's lemma gives $p\mid a$ or $p\mid b$. In either case the admissibility of the factor it divides gives $p\equiv1\pmod4$. Thus $ab\in\mathcal A$. [F1, F2, F3, F4]

1.2 Let $c\in\mathcal A$. Since $c>0$, we have $c\ge1$, so take a prime list $p:r\to\mathbb Z$ with product $c$. For any $i<r$, the index set $r$ is nonempty, so $r=\sigma(s)$ for some $s\in\mathbb N$ and $s\in r$. Let $\pi$ exchange $i$ and $s$ and fix all other indices if $i\ne s$, and let it be the identity if $i=s$. Put $h_k=p_{\pi(k)}$ for $k<r$, so $h_s=p_i$. Extend both lists to $\mathbb N$ by setting entries outside $r$ equal to $1$. The product of $h$ equals $c$ by reordering, and the product recursion gives $c=d p_i=p_i d$, where $d$ is the product of the restriction of $h$ to $s$. Hence $p_i\mid c$, and admissibility gives $p_i\equiv1\pmod4$. [F1, F2, F3, F5, F6, F9, F10]

2.1 Induct on the natural length of lists with entries in $\mathcal A$. The empty product is $1$, which is admissible since it is positive and its only integer divisors are $1$ and $-1$, neither of which is prime. At length $\sigma(j)$, restrict any such list to $j$. The restricted product is admissible by the induction hypothesis, and multiplying it by the entry at index $j$ gives an admissible product by step 1.1. This proves closure for every finite length. [F1, F2, F3, F6, F7, F9, step 1.1]

3.1 For the prime list in step 1.2, induct on the property that if $j\le r$, then the product of the restriction of $p$ to $j$ is congruent to $1$ modulo $4$. The empty product is $1\equiv1\pmod4$ since $1-1=4\cdot0$. For the successor step it suffices to consider $\sigma(j)\le r$. Then $j<r$ by discreteness, so $j\le r$ and $p_j$ is an entry of the list. By the induction hypothesis the product through the first $j$ entries is congruent to $1$, and by step 1.2 so is $p_j$. The product recursion and compatibility of congruence with multiplication give the congruence at $\sigma(j)$. Taking $j=r$ gives $c\equiv1\pmod4$. [F2, F3, F6, F7, F8, F9, step 1.2] ∎
