---
title: Divisor sum and divisor count
status: published
research_item: def-euler-divisor-functions
dependency_level: 0
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, §2, first sentence
---

PDF p. 1: ` §2, first sentence `

## Prerequisites

- [math:def-set-difference-and-symmetric-difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference)
- [math:def-unordered-pair-and-singleton](https://alphabetamath.cc/item/def-unordered-pair-and-singleton)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-countable](https://alphabetamath.cc/item/def-countable)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-int-abs](https://alphabetamath.cc/item/def-int-abs)
- [math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication)
- [math:lem-nat-mult-identity](https://alphabetamath.cc/item/lem-nat-mult-identity)


## Definition

Let $\mathbb N=\{0,1,2,\ldots\}$ and $\mathbb N_{>0}=\mathbb N\setminus\{0\}$. A **positive divisor** of $u\in\mathbb N_{>0}$ is a number $d\in\mathbb N_{>0}$ such that $u=dq$ for some integer $q$, using the usual inclusion of the natural numbers into the integers and integer multiplication. Write $d\mid u$ for divisibility and set $D(u)=\{d\in\mathbb N_{>0}:d\mid u\}$.

Given a finite set $S$ and a function $a:S\to\mathbb N$, write $a_d=a(d)$. The sum $\sum_{d\in S}a_d$ adds the natural number $a_d$ once for each $d\in S$. The **divisor sum** $\sigma$ and the **divisor count** $\tau$ are functions from $\mathbb N_{>0}$ to $\mathbb N$ given by

$$\sigma(u)=\sum_{d\mid u}d=\sum_{d\in D(u)}d,\qquad \tau(u)=\sum_{d\mid u}1=\sum_{d\in D(u)}1.$$

Thus both sums range over the positive divisors of $u$. Equivalently, $\tau(u)=|D(u)|$, where $|S|$ is the cardinality, or number of elements, of the finite set $S$.

## Definition references

[math:def-set-difference-and-symmetric-difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference)

[math:def-unordered-pair-and-singleton](https://alphabetamath.cc/item/def-unordered-pair-and-singleton)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-countable](https://alphabetamath.cc/item/def-countable)

[math:def-function](https://alphabetamath.cc/item/def-function)

[math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

## Facts & Assumptions

[F1] The natural numbers include $0$. The inclusion $\iota:\mathbb N\to\mathbb Z$ is injective and preserves and reflects order. Its image is the nonnegative integers, and $\iota(0)=[(0,0)]$ is integer zero. [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-integers](https://alphabetamath.cc/item/def-integers) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:def-int-order](https://alphabetamath.cc/item/def-int-order) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[F2] If $u$ and $d$ are positive integers and $d\mid u$, then $u\ne 0$ and the divisor bound gives $d\le |u|$. Since $u\ge 0$, the integer absolute value satisfies $|u|=u$, so $d\le u$. [math:def-integers](https://alphabetamath.cc/item/def-integers) [math:def-int-order](https://alphabetamath.cc/item/def-int-order) [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z) [math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound) [math:def-int-abs](https://alphabetamath.cc/item/def-int-abs)

[F3] For natural numbers $k,n$, write $s(n)$ for the successor of $n$, the next natural number after $n$. Then $k\le n$ if and only if $k<s(n)$. [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)

[F4] For any natural number $n$, the initial segment $I_n=\{k\in\mathbb N:k<n\}$ is finite. Every subset of a finite set is finite. [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) [math:def-countable](https://alphabetamath.cc/item/def-countable) [math:lem-cardinality-of-finite-natural-initial-segment](https://alphabetamath.cc/item/lem-cardinality-of-finite-natural-initial-segment) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)

[F5] For a finite set $S$, $|S|$ is the unique natural number $n$ for which $S$ can be listed with exactly $n$ entries, each element appearing once. For a function $a:S\to\mathbb N$, its finite sum is a natural number independent of the order of the list. For a constant natural summand $c$, the sum is $|S|\cdot c$. [math:def-countable](https://alphabetamath.cc/item/def-countable) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:def-function](https://alphabetamath.cc/item/def-function) [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set) [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication)

[F6] For every natural number $n$, $n\cdot 1=n$. [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication) [math:lem-nat-mult-identity](https://alphabetamath.cc/item/lem-nat-mult-identity)

## Justification

**Given:** A positive natural number $u$ and its positive divisor set $D(u)$ as defined above.

**Goal:** Show that the two sums give unique natural numbers and that $\tau(u)$ counts the elements of $D(u)$.

1.1 Let $d\in D(u)$. The definition gives $d\mid u$ with $d$ and $u$ nonzero naturals. Their images are nonnegative integers and are nonzero because the inclusion is injective and sends $0$ to $0$. The divisor bound thus applies to their positive integer images. Reflecting order back to the naturals gives $d\le u$. Hence $d<s(u)$. This holds for every $d\in D(u)$, so $D(u)\subseteq I_{s(u)}$. The segment $I_{s(u)}$ is finite, making $D(u)$ finite as well. [given, F1, F2, F3, F4]

2.1 The assignments $d\mapsto d$ and $d\mapsto 1$ define functions $D(u)\to\mathbb N$ since each $d\in D(u)$ is a natural number and $1\in\mathbb N$. Since $D(u)$ is finite, each sum gives a unique natural number independent of the order of the divisors. [step 1.1, F5]

3.1 The constant-summand rule gives $\tau(u)=|D(u)|\cdot 1=|D(u)|$, the number of positive divisors of $u$. Thus both functions are well defined for every positive $u$. [step 2.1, F5, F6] ∎
