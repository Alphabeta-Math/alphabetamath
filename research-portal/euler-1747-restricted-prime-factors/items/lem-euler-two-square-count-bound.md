---
id: lem-euler-two-square-count-bound
kind: lemma
title: Uniform bound from the two-square formula
status: draft
domain: mathematics
deps:
  - math:thm-division-algorithm-in-z
  - def-euler-two-square-counts
  - math:def-integers
  - math:def-int-order
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-group-power
  - math:def-monoid-finite-product
  - math:def-p-adic-valuation
  - math:lem-p-adic-valuation-basic
  - lem-two-square-count-from-prime-exponents
  - math:thm-int-ordered-ring
  - math:def-int-operations
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
formulation_deps:
  - def-euler-two-square-counts
  - math:def-integers
  - math:def-int-order
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-group-power
  - math:def-monoid-finite-product
  - math:def-int-operations
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
argument_deps:
  - math:thm-division-algorithm-in-z
  - def-euler-two-square-counts
  - math:def-prime
  - math:def-divides-in-z
  - math:def-congruence-modulo-an-integer
  - math:def-group-power
  - math:def-monoid-finite-product
  - math:def-p-adic-valuation
  - math:lem-p-adic-valuation-basic
  - lem-two-square-count-from-prime-exponents
  - math:thm-int-ordered-ring
  - math:def-int-operations
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:def-integers
  - math:def-int-order
dependency_roles:
  math:thm-division-algorithm-in-z: mathematical-premise
  def-euler-two-square-counts: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-group-power: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
  math:def-p-adic-valuation: mathematical-premise
  math:lem-p-adic-valuation-basic: mathematical-premise
  lem-two-square-count-from-prime-exponents: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 5, §4, two-square formula application before Lemma 4.2
dependency_level: 2
---

## Statement

Let $u,n$ be positive integers with $1\le u\le n$. Write $r_2(u)$ for the number of ordered integer pairs $(x,y)$ with $x^2+y^2=u$, allowing negative, zero and positive coordinates.

For a positive integer $t$, let $P(t)$ be the product of $e+1$ over primes $q$ congruent to $1$ modulo $4$ whose exact positive exponent in $t$ is $e$. This means $q^e$ divides $t$ and $q^{e+1}$ fails to divide $t$, where $e$ is a nonzero natural number and $e+1$ in the exponent is its successor. The product over no primes is $1$. In the factors $e+1$ and in the inequality below, read natural numbers as their nonnegative integer images. Let $M(n)$ be the greatest value of $P(t)$ among integers $1\le t\le n$. Then
$$r_2(u)\le 4M(n).$$

## Facts & Assumptions

[F1] A positive integer is an element of $\mathbb Z$ greater than $0$ ([[math:def-integers]], [[math:def-int-order]]). Integer divisibility $d\mid t$ means $t=dk$ for an integer $k$. A prime is an integer greater than $1$ with only $1$ and itself as positive divisors. The congruence $q\equiv b\pmod4$ means $4\mid(q-b)$ ([[math:def-divides-in-z]], [[math:def-prime]], [[math:def-congruence-modulo-an-integer]]). The exponents lie in $\mathbb N$, which contains $0$ and is closed under successor ([[math:def-natural-numbers]]). Powers and finite products start at the integer identity $1$ and use integer multiplication by the base or next factor at each step, respectively ([[math:def-int-operations]], [[math:thm-int-ordered-ring]], [[math:def-group-power]], [[math:def-monoid-finite-product]]). Identify each natural number $j$ with $\iota(j)=[(j,0)]$ in integer products, counts and comparisons. This embedding has image the nonnegative integers and preserves addition, multiplication and order ([[math:lem-nat-embeds-int]]).

[F2] The count $r_2(t)$ includes all ordered integer pairs with square sum $t$, including zero coordinates. In the definition and justification of $P(t)$, a prime $q$ has exact positive exponent $e$ precisely when $e=v_q(t)$ and $v_q(t)>0$. The factors of $P(t)$ are multiplied in increasing prime order. The integer $M(n)$ is the attained greatest value in the list $P(1),\ldots,P(n)$ ([[def-euler-two-square-counts]]).

[F3] For each prime $q$ and positive integer $t$, $v_q(t)$ is the greatest natural exponent $j$ with $q^j\mid t$. Every prime $q$ satisfies $v_q(1)=0$ ([[math:def-p-adic-valuation]], [[math:lem-p-adic-valuation-basic]]).

[F4] For every positive integer $t$, the prime-exponent formula counts the same ordered integer pairs as $r_2(t)$ in [F2]. For any prime $q$, the value $\iota(v_q(t))$ is an integer, so its division by $2>0$ has a unique remainder ([[math:thm-division-algorithm-in-z]]). The count is zero if some prime $q\equiv3\pmod4$ has odd $v_q(t)$, meaning that its integer image has remainder $1$ on division by $2$. Otherwise the count is four times the product of $v_q(t)+1$ over primes $q\equiv1\pmod4$ with $v_q(t)>0$, in increasing prime order ([[lem-two-square-count-from-prime-exponents]]).

[F5] Integer order is compatible with addition, and multiplying two positive integers gives a positive integer. Together with the ring laws, this gives $ca\le cb$ for integers $a\le b$ and $c>0$, since $cb-ca=c(b-a)$ is zero if $a=b$ and positive if $a<b$ ([[math:def-int-operations]], [[math:thm-int-ordered-ring]]).

## Proof

**Given:** Positive integers $u,n$ with $1\le u\le n$.

**Goal:** Prove $r_2(u)\le4M(n)$.

1.1 The formula applies because $u>0$. The primes congruent to $1$ modulo $4$ with $v_q(u)>0$ are exactly those contributing to $P(u)$. The factors agree in increasing prime order because $e=v_q(u)$ gives $\iota(e)+1=\iota(v_q(u))+1$. Thus the two cases of the formula give $r_2(u)=0$ or $r_2(u)=4P(u)$. [given, F1, F2, F3, F4]

1.2 Every prime has exponent zero in $1$, so the product $P(1)$ is empty and equals $1$. Both $1$ and $u$ lie in the range defining $M(n)$. Consequently $M(n)\ge P(1)=1$ and $M(n)\ge P(u)$. [given, F1, F2, F3]

2.1 If $r_2(u)=0$, then $4M(n)\ge4>0=r_2(u)$. If $r_2(u)=4P(u)$, then multiplying $P(u)\le M(n)$ by $4$ gives $r_2(u)\le4M(n)$. This proves the bound in both cases. [F1, F5, step 1.1, step 1.2] ∎
