---
id: def-euler-prime-classes
kind: definition
title: Restricted prime factors and admissible summands
status: draft
domain: mathematics
deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-subset-and-proper-subset
  - def-author-1d5f34b9c027-integer-sumset
formulation_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-subset-and-proper-subset
  - def-author-1d5f34b9c027-integer-sumset
argument_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-subset-and-proper-subset
  - def-author-1d5f34b9c027-integer-sumset
dependency_roles:
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  def-author-1d5f34b9c027-integer-sumset: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, §1, first displayed definitions and Theorem 1.1
dependency_level: 1
---

## Definition

Write $\mathbb Z$ for the integers and call an integer positive when it is greater than $0$. An integer $d$ **divides** an integer $a$, written $d\mid a$, if $a=dq$ for some integer $q$. In that case $d$ is a **divisor** or **factor** of $a$. An integer $p$ is **prime** if $p>1$ and its only positive divisors are $1$ and $p$. A **prime divisor** of $a$ is a prime $p$ satisfying $p\mid a$. For integers $x,r$, write $x\equiv r\pmod 4$ when $4\mid(x-r)$.

The set $\mathcal P_3$ consists of the primes congruent to $3$ modulo $4$.

An integer is **admissible** if it is positive and every prime divisor is congruent to $1$ modulo $4$. Let $\mathcal A$ be the set of admissible integers. The condition on prime divisors is satisfied whenever a positive integer has no prime divisor.

The **sumset** $\mathcal A+\mathcal A$ consists of the integers $n$ of the form $n=a+b$ with $a,b\in\mathcal A$.

## Definition references

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-prime]]

[[math:def-divides-in-z]]

[[math:def-congruence-modulo-an-integer]]

[[math:def-subset-and-proper-subset]]

[[def-author-1d5f34b9c027-integer-sumset]]

## Justification

For a stated condition on the elements of a set, there is a unique subset consisting of exactly the elements satisfying that condition. Primality and congruence to $3$ modulo $4$ give a fixed membership condition on $\mathbb Z$, which defines a unique subset $\mathcal P_3$. Positivity and the implication from prime divisibility to congruence to $1$ likewise give a fixed membership condition on $\mathbb Z$, which defines a unique subset $\mathcal A$. In each case the subset contains exactly the integers satisfying the stated condition. Since $\mathcal A$ is a subset of $\mathbb Z$, the integer sumset construction applies with both input sets equal to $\mathcal A$ and gives exactly the stated membership condition for $\mathcal A+\mathcal A$.
