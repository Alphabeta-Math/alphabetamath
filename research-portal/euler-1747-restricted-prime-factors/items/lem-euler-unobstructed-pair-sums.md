---
id: lem-euler-unobstructed-pair-sums
kind: lemma
title: Unobstructed mixed pairs give admissible summands
status: published
domain: mathematics
deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - lem-square-residue-parity
  - def-euler-mixed-four-square-representations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - def-euler-prime-classes
  - def-euler-prime-obstruction-count
  - math:thm-int-ordered-ring
  - lem-euler-nonsplit-square-obstruction
formulation_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - lem-square-residue-parity
  - def-euler-mixed-four-square-representations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - def-euler-prime-classes
  - def-euler-prime-obstruction-count
argument_deps:
  - math:thm-int-ordered-ring
  - def-euler-mixed-four-square-representations
  - lem-square-residue-parity
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - def-euler-prime-classes
  - def-euler-prime-obstruction-count
  - lem-euler-nonsplit-square-obstruction
dependency_roles:
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  lem-square-residue-parity: mathematical-premise
  def-euler-mixed-four-square-representations: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  def-euler-prime-obstruction-count: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  lem-euler-nonsplit-square-obstruction: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §2, conclusion immediately preceding (2.3)
dependency_level: 3
---

## Statement

Write $\mathbb Z$ for the integers. Let $n$ be a positive integer, meaning $n>0$. Write $z^2=z\cdot z$ for the square of an integer $z$. An integer is even if it has the form $2k$ and odd if it has the form $2k+1$, with $k$ an integer.

The set $\mathcal R_{\mathrm{mix}}(n)$ consists of ordered quadruples $(x_1,x_2,x_3,x_4)$ of integers with $x_1^2+x_2^2+x_3^2+x_4^2=n$ and one even and one odd entry in each of the pairs $(x_1,x_2)$ and $(x_3,x_4)$.

Write $d\mid s$ if $s=dq$ for some integer $q$. In that case $d$ is a divisor of $s$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Write $p\equiv r\pmod4$ if $4\mid(p-r)$. Let $\mathcal P_3$ be the set of primes congruent to $3$ modulo $4$, and let $\mathcal A$ be the set of positive integers whose prime divisors are all congruent to $1$ modulo $4$.

For $p\in\mathcal P_3$, let $E_p(n)$ be the exceptional set consisting of the quadruples in $\mathcal R_{\mathrm{mix}}(n)$ for which $p$ divides both entries of at least one of the two specified pairs. If $(x_1,x_2,x_3,x_4)$ belongs to $\mathcal R_{\mathrm{mix}}(n)$ and lies outside $E_p(n)$ for every $p\in\mathcal P_3$, then $a=x_1^2+x_2^2$ and $b=x_3^2+x_4^2$ are positive odd integers in $\mathcal A$ and $a+b=n$.

## Statement references

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[lem-square-residue-parity]]

[[def-euler-mixed-four-square-representations]]

[[math:def-divides-in-z]]

[[math:def-prime]]

[[math:def-congruence-modulo-an-integer]]

[[def-euler-prime-classes]]

[[def-euler-prime-obstruction-count]]

## Facts & Assumptions

[F1] Integer addition and multiplication are associative, and multiplication distributes over addition. [[math:thm-int-ordered-ring]]

[F2] A quadruple in $\mathcal R_{\mathrm{mix}}(n)$ has the indicated sum of four squares and one even and one odd entry in each specified pair. [[def-euler-mixed-four-square-representations]]

[F3] Every integer is even or odd, and these two possibilities are disjoint. If $u,v$ are integers of opposite parity, meaning one is even and one is odd, then $u^2+v^2$ is positive and odd. [[lem-square-residue-parity]]

[F4] The condition $p\mid s$ gives $s=pq$ for some integer $q$. The equality $p=4t+r$ with integer $t$ gives $p\equiv r\pmod4$. [[math:def-divides-in-z]] [[math:def-congruence-modulo-an-integer]]

[F5] A prime congruent to $3$ modulo $4$ belongs to $\mathcal P_3$. A positive integer belongs to $\mathcal A$ exactly when all its prime divisors are congruent to $1$ modulo $4$. [[def-euler-prime-classes]]

[F6] A quadruple of $\mathcal R_{\mathrm{mix}}(n)$ belongs to $E_p(n)$ if both entries of either specified pair are divisible by $p\in\mathcal P_3$. [[def-euler-prime-obstruction-count]]

[F7] For $p\in\mathcal P_3$ and any integers $u,v$, the condition $p\mid u^2+v^2$ implies $p\mid u$ and $p\mid v$. [[lem-euler-nonsplit-square-obstruction]]

## Proof

**Given:** A positive integer $n$ and a quadruple in $\mathcal R_{\mathrm{mix}}(n)$ outside $E_p(n)$ for every $p\in\mathcal P_3$.

**Goal:** Show that both specified sums $a,b$ are positive odd integers in $\mathcal A$ and that $a+b=n$.

1.1 Each of the two specified pairs has one even and one odd entry by membership in $\mathcal R_{\mathrm{mix}}(n)$. Hence both $a$ and $b$ are positive and odd. The four squares sum to $n$, and associativity groups them as $a+b$, so $a+b=n$. [given, F1, F2, F3]

1.2 Fix $p\in\mathcal P_3$ and take $(u,v)$ to be either specified pair. If $p\mid u^2+v^2$, then $p\mid u$ and $p\mid v$. This places the quadruple in $E_p(n)$, contrary to the given avoidance condition. Thus neither $a$ nor $b$ has any prime divisor in $\mathcal P_3$. [given, F6, F7]

2.1 Let $s$ be either $a$ or $b$ and let $p$ be any prime divisor of $s$. Write $s=pq$ with $q$ an integer. If $p=2k$, associativity gives $s=2(kq)$, making $s$ even. This contradicts the oddness of $s$ and the disjointness of the parity cases. Therefore $p$ is odd, so $p=2k+1$ for some integer $k$. [F1, F3, F4, step 1.1]

3.1 If $k=2t+1$, then $p=2(2t+1)+1=4t+3$. This gives $p\equiv3\pmod4$ and $p\in\mathcal P_3$, which Step 1.2 excludes. Thus $k$ is even, so $k=2t$ for some integer $t$. Then $p=4t+1$ and $p\equiv1\pmod4$. [F1, F3, F4, F5, step 1.2, step 2.1]

4.1 Every prime divisor of either $a$ or $b$ is therefore congruent to $1$ modulo $4$. This condition also holds for a summand with no prime divisors. Since both summands are positive, both belong to $\mathcal A$. Together with their oddness and $a+b=n$, this proves the claim. [F5, step 1.1, step 3.1] ∎
