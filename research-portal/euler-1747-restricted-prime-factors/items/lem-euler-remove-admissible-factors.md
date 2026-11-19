---
id: lem-euler-remove-admissible-factors
kind: lemma
title: Removing admissible factors from the decomposition problem
status: published
domain: mathematics
proof_strategy: direct
deps:
  - def-euler-prime-classes
  - lem-euler-odd-factor-split
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - lem-euler-admissible-products
  - math:thm-int-comm-ring
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
formulation_deps:
  - def-euler-prime-classes
  - lem-euler-odd-factor-split
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
argument_deps:
  - def-euler-prime-classes
  - lem-euler-odd-factor-split
  - lem-euler-admissible-products
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:thm-int-comm-ring
  - math:thm-int-ordered-ring
  - math:thm-division-algorithm-in-z
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  lem-euler-odd-factor-split: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  lem-euler-admissible-products: mathematical-premise
  math:thm-int-comm-ring: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, Lemma 2.1, statement and scaling step
dependency_level: 3
---

## Statement

Write $\mathbb Z$ for the integers. An integer is positive if it exceeds $0$. Write $d\mid x$ if $x=dq$ for some integer $q$. An integer $x$ is odd if $2$ does not divide $x$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself, and a prime divisor of $x$ is a prime $p$ with $p\mid x$. Write $x\equiv r\pmod4$ if $4\mid(x-r)$. Let $\mathcal P_3$ be the primes congruent to $3$ modulo $4$, and let $\mathcal A$ be the set of positive integers whose prime divisors are all congruent to $1$ modulo $4$. Members of $\mathcal A$ are called admissible.

Every positive odd integer $m$ has a factorization $m=gm_0$ with $g\in\mathcal A$ and $m_0$ a positive integer whose prime divisors all lie in $\mathcal P_3$. For every such factorization, $m_0$ is odd, $2m_0\ge2$, and $2m_0\equiv2\pmod4$. If $2m_0=a+b$ with $a,b\in\mathcal A$, then $2m=ga+gb$ with $ga,gb\in\mathcal A$.

Consequently, every positive integer $n\equiv2\pmod4$ is of the form $n=g(2m_0)$ with $g$ and $m_0$ as above. To prove that each such $n$ is a sum of two admissible integers, it suffices to prove that each $2u$ with $u$ positive and odd and every prime divisor of $u$ in $\mathcal P_3$ is a sum of two admissible integers.

## Statement references

[[def-euler-prime-classes]]

[[lem-euler-odd-factor-split]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-divides-in-z]]

[[math:def-prime]]

[[math:def-congruence-modulo-an-integer]]

## Facts & Assumptions

[F1] The definitions of $\mathcal A$ and $\mathcal P_3$ impose the prime divisor and congruence conditions in the Statement ([[def-euler-prime-classes]]). An integer $d$ divides $x$ exactly when $x=dq$ for some integer $q$ ([[math:def-divides-in-z]]), so $x\equiv r\pmod4$ exactly when $x-r=4q$ for some integer $q$ ([[math:def-congruence-modulo-an-integer]]).

[F2] Every positive integer $m$ that is not divisible by $2$ can be written $m=gm_0$, where $g\in\mathcal A$ and $m_0>0$ has all its prime divisors in $\mathcal P_3$ ([[lem-euler-odd-factor-split]]).

[F3] The product of two members of $\mathcal A$ is again in $\mathcal A$ ([[lem-euler-admissible-products]], finite product clause).

[F4] Integer addition and multiplication are commutative and associative, and multiplication distributes over addition. Subtraction adds the additive inverse ([[math:thm-int-comm-ring]]).

[F5] The integer order is total and compatible with addition, and products of positive integers are positive ([[math:thm-int-ordered-ring]]).

[F6] For integers $x,d$ with $d>0$, there are unique integers $q,r$ with $x=dq+r$ and $0\le r<d$. Every positive integer is at least $1$ by step 1.2 of the same supplier ([[math:thm-division-algorithm-in-z]]).

## Proof

**Given:** The sets $\mathcal A$ and $\mathcal P_3$ and the integer conventions in the Statement.

**Goal:** Establish the factorization and the rule for multiplying a decomposition by $g$, then deduce the reduction for every positive $n\equiv2\pmod4$.

1.1 Let $m$ be positive and odd. By [F2] there is a factorization $m=gm_0$ with $g\in\mathcal A$ and $m_0>0$ whose prime divisors all lie in $\mathcal P_3$. Fix any such factorization. If $2\mid m_0$, then $m_0=2t$ for some integer $t$ and hence $m=g(2t)=2(gt)$, contrary to the oddness of $m$. Thus $m_0$ is odd. [given, F1, F2, F4]

2.1 If $2m_0=a+b$ with $a,b\in\mathcal A$, the products $ga$ and $gb$ are admissible by [F3]. Commutativity, associativity and distributivity give $2m=2(gm_0)=g(2m_0)=g(a+b)=ga+gb$. [step 1.1, F3, F4]

2.2 Let $u$ be any positive odd integer. Divide $u$ by $2$ to obtain $u=2q+r$ with $0\le r<2$. Oddness excludes $r=0$. Since $r>0$, we have $r\ge1$. If $r>1$, then $r-1>0$ and therefore $r-1\ge1$, giving $r\ge2$. Thus $r=1$ and $2u=4q+2$, so $2u\equiv2\pmod4$. Also $u\ge1$ gives $2u=u+u\ge1+1=2$. This applies to $u=m_0$ in step 1.1. [F1, F4, F5, F6, step 1.1]

3.1 Now let $n>0$ satisfy $n\equiv2\pmod4$. Write $n=4q+2$ for an integer $q$, and set $m=2q+1$, so $n=2m$. If $m\le0$, then $n=m+m\le m\le0$, which is impossible. The expression $m=2q+1$ has remainder $1$ on division by $2$, so uniqueness excludes a remainder of $0$ and makes $m$ odd. Step 1.1 now gives $n=g(2m_0)$ with the required conditions on $g$ and $m_0$. [given, F1, F4, F5, F6, step 1.1, step 2.2]

4.1 Suppose every $2u$ with $u$ positive and odd and with every prime divisor of $u$ in $\mathcal P_3$ is a sum of two admissible integers. For the factorization from step 3.1, the integer $u=m_0$ satisfies these hypotheses. Take $2m_0=a+b$ with $a,b\in\mathcal A$. Step 2.1 gives $n=ga+gb$ with $ga,gb\in\mathcal A$. Since $n$ was arbitrary in the stated positive congruence class, this proves the reduction. [given, step 2.1, step 3.1] ∎
