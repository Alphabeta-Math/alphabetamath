---
title: Equivalent restrictions on positive summands
status: published
research_item: lem-euler-historical-restriction
dependency_level: 3
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, §1, Euler’s divisor condition and the definition of admissible
        summands
---

PDF p. 1: ` §1, Euler’s divisor condition and the definition of admissible summands `

## Prerequisites

- [def-euler-prime-classes](item-def-euler-prime-classes)
- [lem-euler-admissible-products](item-lem-euler-admissible-products)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:lem-divisibility-basic](https://alphabetamath.cc/item/lem-divisibility-basic)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)


## Statement

Write $\mathbb Z$ for the integers. An integer is positive if it is greater than $0$. An integer $d$ is a divisor of $a$, written $d\mid a$, if $a=dq$ for some $q\in\mathbb Z$. A prime is an integer $p>1$ whose only positive divisors are $1$ and $p$. A prime divisor is a divisor that is prime. Write $x\equiv y\pmod4$ if $x-y=4q$ for some $q\in\mathbb Z$.

Let $\mathcal A$ be the set of positive integers whose prime divisors are all congruent to $1$ modulo $4$. A positive integer $a$ with $a\equiv1\pmod4$ belongs to $\mathcal A$ if and only if it has no positive divisor $d$ with $d\equiv3\pmod4$.

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

## Facts & Assumptions

[F1] Membership in $\mathcal A$ means positivity and congruence to $1$ modulo $4$ for every prime divisor ([def-euler-prime-classes](item-def-euler-prime-classes)). Every member of $\mathcal A$ is itself congruent to $1$ modulo $4$ ([lem-euler-admissible-products](item-lem-euler-admissible-products)).

[F2] Divisibility $d\mid a$ means $a=dq$ for an integer $q$ ([math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)). A prime $p$ is greater than $1$ ([math:def-prime](https://alphabetamath.cc/item/def-prime)). Congruence $x\equiv y\pmod4$ means $x=4q+y$ for an integer $q$ ([math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)).

[F3] For integers $b,c,e$, if $b\mid c$ and $c\mid e$, then $b\mid e$ ([math:lem-divisibility-basic](https://alphabetamath.cc/item/lem-divisibility-basic), transitivity).

[F4] For each integer $x$ and positive integer $b$ there is a unique pair of integers $q,r$ with $x=bq+r$ and $0\le r<b$. In this expression $r$ is called the remainder. It is $0$ exactly when $b\mid x$ ([math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

[F5] The integers form a totally ordered commutative ring. In particular, multiplication distributes over addition and is associative and commutative ([math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)).

[F6] Write $\mathbb N$ for the natural numbers, with $0$ and successor $\sigma$. The numerals $1,2,3,4$ are obtained by applying $\sigma$ successively from $0$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)). In the natural order, $m<n$ means $m\le n$ and $m\ne n$ ([math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)). Discreteness gives $m<n$ if and only if $\sigma(m)\le n$ ([math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)). The embedding $\iota(n)=[(n,0)]$ preserves addition, preserves and reflects order, and has image exactly the nonnegative integers ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)). We use the same numerals for their integer images, with $\iota(0)=0$ and $\iota(1)=1$ by the definitions of the integer constants ([math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)). The natural addition recursion $m+0=m$ and $m+\sigma(n)=\sigma(m+n)$ gives $\sigma(m)=m+1$ ([math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)).

## Proof

**Given:** A positive integer $a$ with $a\equiv1\pmod4$.

**Goal:** Prove that $a$ belongs to $\mathcal A$ if and only if it has no positive divisor congruent to $3$ modulo $4$.

1.1 By reflexivity and discreteness, $n<\sigma(n)$ for every natural $n$. The embedding therefore gives $0<1<2<3<4$ in the integers. Any integer strictly between consecutive entries would have a natural preimage strictly between a natural number and its successor, which discreteness excludes. By totality, the integers with $0\le r<4$ are exactly $0,1,2,3$. Since $\sigma(n)=n+1$ and the embedding preserves addition, the integer numerals satisfy $2=1+1$ and $4=2+2$. [F5, F6]

2.1 Suppose $a\in\mathcal A$ and let $d$ be any positive divisor of $a$. If $p$ is a prime divisor of $d$, then $p\mid d$ and $d\mid a$, so $p\mid a$. Hence $p\equiv1\pmod4$. Since $d>0$ and every prime divisor of $d$ meets the defining condition, $d\in\mathcal A$. Consequently $d\equiv1\pmod4$. If also $d\equiv3\pmod4$, then $d=4u+1=4v+3$ for integers $u,v$. Both $1$ and $3$ are in the interval $0\le r<4$, contrary to uniqueness of the remainder for division by $4$. Thus no positive divisor of $a$ is congruent to $3$ modulo $4$. [F1, F2, F3, F4, F5, step 1.1]

2.2 Conversely, assume that no positive divisor of $a$ is congruent to $3$ modulo $4$. The given congruence writes $a=4k+1=2(2k)+1$ for an integer $k$. Since $0\le1<2$, the remainder when $a$ is divided by $2$ is $1$, so $2$ does not divide $a$. [given, F2, F4, F5, step 1.1]

3.1 Let $p$ be any prime divisor of $a$. Division by $4$ gives $p=4q+r$ with $r\in\{0,1,2,3\}$. If $r=0$, then $p=2(2q)$, and if $r=2$, then $p=2(2q+1)$. In either case $2\mid p$, so $2\mid a$, contrary to step 2.2. If $r=3$, then $p\equiv3\pmod4$, which the assumption excludes since $p>1>0$ and $p\mid a$. It follows that $r=1$ and $p\equiv1\pmod4$. [F2, F3, F4, F5, step 1.1, step 2.2]

4.1 Thus every prime divisor of the positive integer $a$ is congruent to $1$ modulo $4$, so $a\in\mathcal A$. Together with step 2.1 this proves the equivalence. [given, F1, step 2.1, step 3.1] ∎
