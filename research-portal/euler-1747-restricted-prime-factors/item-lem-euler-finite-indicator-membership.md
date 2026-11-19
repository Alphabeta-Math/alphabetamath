---
title: "Lemma 7.1: The finite indicator detects admissible integers"
status: published
research_item: lem-euler-finite-indicator-membership
dependency_level: 4
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, Lemma 7.1 (statement and proof)
---

PDF p. 7: ` Lemma 7.1, statement `

## Prerequisites

- [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [lem-euler-finite-indicator-factor-test](item-lem-euler-finite-indicator-factor-test)
- [lem-euler-finite-small-obstructing-divisor](item-lem-euler-finite-small-obstructing-divisor)
- [lem-binary-products-and-avoidance](item-lem-binary-products-and-avoidance)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)


## Statement

Let $j$ be an integer with $0\le j\le H$, where $H=4{,}194{,}303$, and put $a=4j+1$. An integer $d$ divides an integer $m$, written $d\mid m$, if $m=dt$ for some integer $t$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself, where positive means greater than $0$. A prime divisor is a prime that divides the integer under consideration. Write $p\equiv r\pmod 4$ if $4\mid(p-r)$.

Let $\mathcal P_3$ consist of the primes congruent to $3$ modulo $4$, and let $S$ consist of those primes in $\mathcal P_3$ at most $4096$. The indicator $\varepsilon_j$ is the product of the certificate factors from (7.1), with one factor for each $p\in S$ and value $1$ for an empty product. Let $\mathcal A$ be the set of positive integers whose prime divisors are all congruent to $1$ modulo $4$.

Then $\varepsilon_j=1$ if and only if $4j+1\in\mathcal A$.

## Statement references

[def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

## Facts & Assumptions

[F1] The finite certificate supplies $H$ and the product defining $\varepsilon_j$ for $0\le j\le H$. Its index set $S$ is finite, meaning its members can be listed once each in a list of natural length. The product multiplies the listed factors and is $1$ for the empty list. [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

[F2] For every integer $j$ in the certificate range and every $p\in S$, the factor indexed by $p$ is $0$ if $p\mid a$ and $1$ otherwise. The certificate product can be taken in the natural numbers when its factors are $0$ or $1$. [lem-euler-finite-indicator-factor-test](item-lem-euler-finite-indicator-factor-test) [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)

[F3] For any finite index set and any natural values $b_p$ equal to $0$ or $1$, the complement $1-b_p$ is the natural value that satisfies $b_p+(1-b_p)=1$. It is $1$ for $b_p=0$ and $0$ for $b_p=1$. The product of these complements is $1$ if every $b_p=0$, and $0$ if some $b_p=1$. [lem-binary-products-and-avoidance](item-lem-binary-products-and-avoidance) [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)

[F4] For an integer $j$ with $0\le j\le H$, the integer $a=4j+1$ is positive and odd, meaning $2$ does not divide it. If a prime in $\mathcal P_3$ divides $a$, then some prime $p$ in $\mathcal P_3$ divides $a$ and satisfies $p<4096$. [lem-euler-finite-small-obstructing-divisor](item-lem-euler-finite-small-obstructing-divisor)

[F5] For an integer $x$ and a positive integer $m$, there exist unique integers $q,r$ satisfying $x=mq+r$ and $0\le r<m$. Here $r$ is called the remainder. Integer multiplication is associative and commutative and distributes over addition. [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[F6] The natural numbers are $0,1,2,\ldots$, with each numeral followed by its successor. The natural numbers map in order to exactly the nonnegative integers, preserving the numerals. No natural number lies strictly between a natural number and its successor. [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)

[F7] The defining conditions for $\mathcal P_3$ and $\mathcal A$ use integer divisibility, primality and congruence as stated above. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z) [math:def-prime](https://alphabetamath.cc/item/def-prime) [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

## Proof

**Given:** An integer $j$ with $0\le j\le H$ and its certificate product $\varepsilon_j$.

**Goal:** Prove that $\varepsilon_j=1$ exactly when $4j+1\in\mathcal A$.

1.1 For each $p\in S$, take $b_p=1$ if $p\mid a$ and $b_p=0$ otherwise. The two cases are exclusive and exhaustive, so they assign exactly one natural value to each $p$. The factor indexed by $p$ in $\varepsilon_j$ is $1-b_p$, since both are $0$ in the divisibility case and $1$ in the other case. The product rule on the finite set $S$ gives $\varepsilon_j=1$ exactly when no member of $S$ divides $a$. [given, F1, F2, F3, F7]

1.2 Any divisor in $S$ is a prime divisor in $\mathcal P_3$. Conversely, if any prime in $\mathcal P_3$ divides $a$, the bound in [F4] gives such a divisor strictly below $4096$, hence in $S$. Therefore no member of $S$ divides $a$ exactly when no prime in $\mathcal P_3$ divides $a$. [given, F1, F4, F7]

1.3 Let $d$ be any prime divisor of $a$, and write $a=dt$ for an integer $t$. Divide $d$ by $4$ to obtain $d=4q+r$ with $0\le r<4$. By the integer copy of the natural numbers and the absence of integers between successive nonnegative numerals, $r\in\{0,1,2,3\}$. If $r=0$ then $a=2(2qt)$, and if $r=2$ then $a=2((2q+1)t)$. Each case makes $a$ divisible by $2$, contrary to its oddness. Thus $r$ is $1$ or $3$. For either value $s\in\{1,3\}$, $d\equiv s\pmod4$ means $d=4v+s$ for an integer $v$, and uniqueness of the remainder makes this condition equivalent to $r=s$. [F4, F5, F6, F7]

2.1 If $a\in\mathcal A$, every prime divisor has remainder $1$ on division by $4$, so no prime in $\mathcal P_3$ divides $a$. Conversely, if no prime in $\mathcal P_3$ divides $a$, every prime divisor has remainder $1$ by step 1.3, and $a>0$, so $a\in\mathcal A$. Combining this equivalence with steps 1.1 and 1.2 yields $\varepsilon_j=1$ exactly when $4j+1\in\mathcal A$ for the whole stated range. [F4, F7, step 1.1, step 1.2, step 1.3] ∎
