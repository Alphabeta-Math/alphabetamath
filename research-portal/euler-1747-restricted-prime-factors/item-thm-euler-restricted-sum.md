---
title: Euler’s restricted prime factor decomposition
status: draft
research_item: thm-euler-restricted-sum
dependency_level: 16
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: PDF p. 1, Abstract and Theorem 1.1, and p. 8, Proof of Theorem 1.1
      reading_limits: Read the cited PDF pages for the statement and the closing argument.
---

PDF p. 1: ` Abstract and Theorem 1.1 `; PDF p. 8: ` Proof of Theorem 1.1 `

## Prerequisites

- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [ex-euler-one-admissible](item-ex-euler-one-admissible)
- [lem-euler-remove-admissible-factors](item-lem-euler-remove-admissible-factors)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [prop-euler-analytic-range](item-prop-euler-analytic-range)
- [prop-euler-finite-range](item-prop-euler-finite-range)


## Statement

Assume the Axiom of Choice, which says that for every set of nonempty sets there is a function assigning to each member an element of that member.

Write $\mathbb Z$ for the integers and call an integer positive if it is greater than $0$. An integer $d$ divides an integer $x$ if $x=dq$ for some $q\in\mathbb Z$. An integer $p>1$ is prime if its only positive divisors are $1$ and $p$. A prime divisor is a divisor that is prime. For integers $x,r$, write $x\equiv r\pmod 4$ if $4$ divides $x-r$.

Let $\mathcal A$ be the set of positive integers all of whose prime divisors are congruent to $1$ modulo $4$. The integer $1$ is allowed because it has no prime divisor. Every positive integer $n\equiv2\pmod 4$ can be written as $n=a+b$ with $a,b\in\mathcal A$.

## Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[def-euler-prime-classes](item-def-euler-prime-classes)

[ex-euler-one-admissible](item-ex-euler-one-admissible)

## Facts & Assumptions

[F1] Write $\mathcal P_3$ for the set of primes congruent to $3$ modulo $4$. [def-euler-prime-classes](item-def-euler-prime-classes)

[F2] For every positive integer $n\equiv2\pmod 4$, the factor-removal lemma supplies $g\in\mathcal A$ and a positive integer $m_0$ whose prime divisors all lie in $\mathcal P_3$, such that $n=g(2m_0)$, $2m_0\ge2$, and $2m_0\equiv2\pmod 4$. The integer $m_0$ is odd, meaning that $2$ does not divide it. Step 2.2 of the lemma gives $m_0=2k+1$ for some integer $k$. If $2m_0=x+y$ with $x,y\in\mathcal A$, the lemma gives $n=gx+gy$ with $gx,gy\in\mathcal A$. [lem-euler-remove-admissible-factors](item-lem-euler-remove-admissible-factors)

[F3] Set $B=64^4$, the product of four copies of $64$. Iterating the natural-number multiplication and addition recurrences on successor numerals gives $64\cdot64=4096$ and $4096\cdot4096=16{,}777{,}216$. The embedding $\iota$ sends natural numerals to their integer values and satisfies $\iota(r)\iota(s)=\iota(rs)$ for natural numbers $r,s$, so both product equalities also hold in the integers. By associativity of integer multiplication, $B=4096\cdot4096=16{,}777{,}216$. The integer order is total, so for each integer $t$ either $t<B$ or $t\ge B$. [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[F4] Under the Axiom of Choice, if $u$ is positive, $u=2k+1$ for some integer $k$, every prime divisor of $u$ lies in $\mathcal P_3$, and $2u\ge B$, then $2u=x+y$ for some $x,y\in\mathcal A$. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [prop-euler-analytic-range](item-prop-euler-analytic-range)

[F5] If $t$ is an integer with $2\le t<B$ and $t\equiv2\pmod 4$, then $t=x+y$ for some $x,y\in\mathcal A$ with at least one of $x,y$ at most $313$. [prop-euler-finite-range](item-prop-euler-finite-range)

## Proof

**Given:** The Axiom of Choice and a positive integer $n\equiv2\pmod 4$.

**Goal:** Find $a,b\in\mathcal A$ with $n=a+b$.

1.1 Apply the factor-removal lemma to $n$ and set $t=2m_0$ for the resulting $m_0$. Then $n=gt$ with $g\in\mathcal A$. We have $t\ge2$, $t\equiv2\pmod 4$, and $m_0$ is positive with $m_0=2k+1$ for some integer $k$ and every prime divisor in $\mathcal P_3$. [given, F1, F2]

2.1 If $t\ge B$, the positive odd integer $u=m_0$ meets the prime-divisor hypothesis of the analytic range result and $2u=t\ge B$. Using the assumed Axiom of Choice, that result gives $t=x+y$ with $x,y\in\mathcal A$. If $t<B$, then $2\le t<B$ and $t\equiv2\pmod 4$, so the finite range result gives $t=x+y$ with $x,y\in\mathcal A$. By totality, one of the two cases holds for every integer $t$. [given, F3, F4, F5, step 1.1]

3.1 Apply the scaling conclusion of the factor-removal lemma to $2m_0=x+y$. This gives $n=gx+gy$ with $gx,gy\in\mathcal A$. Taking $a=gx$ and $b=gy$ proves the decomposition for the arbitrary positive integer $n\equiv2\pmod 4$. [F2, step 1.1, step 2.1] ∎
