---
id: def-euler-prime-obstruction-count
kind: definition
title: The obstruction at a prime congruent to 3 modulo 4
status: draft
domain: mathematics
deps:
  - def-euler-prime-classes
  - def-euler-mixed-four-square-representations
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - math:def-subset-and-proper-subset
  - math:def-countable
  - math:def-finite-cardinality
  - math:thm-subset-of-a-finite-set
formulation_deps:
  - def-euler-prime-classes
  - def-euler-mixed-four-square-representations
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - math:def-subset-and-proper-subset
  - math:def-countable
  - math:def-finite-cardinality
argument_deps:
  - def-euler-mixed-four-square-representations
  - math:def-divides-in-z
  - math:def-subset-and-proper-subset
  - math:thm-subset-of-a-finite-set
  - math:def-finite-cardinality
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  def-euler-mixed-four-square-representations: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-countable: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §2, definition of the exceptional sets following (2.2)
dependency_level: 2
---

## Definition

Write $\mathbb Z$ for the integers, and fix a positive integer $n$, meaning $n>0$. For integers $d$ and $a$, write $d\mid a$ if $a=dq$ for some $q\in\mathbb Z$. In that case $d$ divides $a$ and is called a divisor of $a$. An integer $p$ is prime if $p>1$ and its only positive divisors are $1$ and $p$. Fix $p\in\mathcal P_3$, the set of primes congruent to $3$ modulo $4$, where this congruence means $4\mid(p-3)$.

The set $\mathcal R_{\mathrm{mix}}(n)$ consists of ordered quadruples $(x_1,x_2,x_3,x_4)$ of integers with $x_1^2+x_2^2+x_3^2+x_4^2=n$, where $x_i^2=x_i\cdot x_i$, and with one even and one odd coordinate in each of the pairs $(x_1,x_2)$ and $(x_3,x_4)$. An even integer has the form $2k$ and an odd integer has the form $2k+1$, for an integer $k$. Entries may be negative, zero, or positive. Two quadruples are equal exactly when their entries agree in all four positions.

Let $E_p(n)$ be the exceptional set at $p$, meaning the subset of $\mathcal R_{\mathrm{mix}}(n)$ consisting of the quadruples for which $p\mid x_1$ and $p\mid x_2$, or $p\mid x_3$ and $p\mid x_4$. Here “or” includes the case where both pairs satisfy the divisibility test.

A set is finite if its elements can be listed in $k$ positions for some $k\in\{0,1,2,\ldots\}$, with each element listed exactly once. For a finite set $S$, write $|S|$ for its cardinality, the number of elements of $S$. Define the obstruction count $b_p(n)=|E_p(n)|$. A quadruple satisfying both divisibility tests contributes once.

## Definition references

[[def-euler-prime-classes]]

[[def-euler-mixed-four-square-representations]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-divides-in-z]]

[[math:def-prime]]

[[math:def-congruence-modulo-an-integer]]

[[math:def-subset-and-proper-subset]]

[[math:def-countable]]

[[math:def-finite-cardinality]]

## Facts & Assumptions

[F1] For each positive integer $n$, $\mathcal R_{\mathrm{mix}}(n)$ is a well-defined finite set of ordered integer quadruples. [[def-euler-mixed-four-square-representations]]

[F2] For any integers $d$ and $a$, the condition $d\mid a$ means that there exists an integer $q$ with $a=dq$. This definition applies to zero and negative coordinates as well. [[math:def-divides-in-z]]

[F3] A fixed condition on the elements of a given set selects a unique subset whose elements are exactly the elements satisfying the condition. [[math:def-subset-and-proper-subset]]

[F4] Every subset of a finite set is finite. [[math:thm-subset-of-a-finite-set]]

[F5] A finite set has a unique cardinality, given by the number of its distinct elements. [[math:def-finite-cardinality]]

## Justification

**Given:** A positive integer $n$ and a prime $p\in\mathcal P_3$.

**Goal:** Show that the exceptional set and its count are defined uniquely, with a single contribution from each qualifying quadruple.

1.1 For each element of $\mathcal R_{\mathrm{mix}}(n)$, all four coordinates are integers, so integer divisibility applies to each coordinate. The condition that at least one of the two pairs has both entries divisible by $p$ therefore selects a unique subset of $\mathcal R_{\mathrm{mix}}(n)$, namely $E_p(n)$. [given, F1, F2, F3]

2.1 Since $\mathcal R_{\mathrm{mix}}(n)$ is finite, its subset $E_p(n)$ is finite. It has a unique cardinality, so $b_p(n)$ is defined uniquely. The membership condition includes a quadruple whenever either pair qualifies, including when both qualify. The count gives one contribution to each distinct element of $E_p(n)$. [F1, F4, F5, step 1.1] ∎
