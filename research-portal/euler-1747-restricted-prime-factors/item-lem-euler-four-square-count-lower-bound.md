---
title: A lower bound on the four-square representation count
status: draft
research_item: lem-euler-four-square-count-lower-bound
dependency_level: 2
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 5, Lemma 4.2, last line of proof
---

PDF p. 5: ` Lemma 4.2, last line of proof `

## Prerequisites

- [def-euler-four-square-representations](item-def-euler-four-square-representations)
- [def-euler-divisor-functions](item-def-euler-divisor-functions)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [math:lem-nat-finite-sum-laws-and-the-canonical-embedding](https://alphabetamath.cc/item/lem-nat-finite-sum-laws-and-the-canonical-embedding)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [lem-euler-four-square-count](item-lem-euler-four-square-count)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product)


## Statement

Let $m$ be a positive odd integer, so $0<m$ and no integer $q$ satisfies $m=2q$. Put $n=2m$. Let $R(n)$ be the number of ordered integer quadruples $(x_1,x_2,x_3,x_4)$ satisfying $x_1^2+x_2^2+x_3^2+x_4^2=n$, with zero and either sign allowed in every position. Let $\sigma(m)$ be the sum of all positive divisors of $m$, meaning all integers $d>0$ for which $m=dq$ for some integer $q$, counted once each. View the count and the sum as integers by identifying the natural numbers with the nonnegative integers. Then

$$R(n)=24\sigma(m)\ge12n.$$

## Statement references

[def-euler-four-square-representations](item-def-euler-four-square-representations)

[def-euler-divisor-functions](item-def-euler-divisor-functions)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[Integer divisibility](https://alphabetamath.cc/item/def-divides-in-z)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

## Facts & Assumptions

[F1] For a positive integer $u$, the ordered quadruples of integers with square sum $u$ form a finite set, and $R(u)$ is its number of elements. [def-euler-four-square-representations](item-def-euler-four-square-representations)

[F2] For a positive input $u$, $\sigma(u)$ is the natural-number sum over the finite set $D(u)$ of its positive divisors. An integer $d$ divides $u$ exactly when $u=dq$ for some integer $q$. [def-euler-divisor-functions](item-def-euler-divisor-functions) [Integer divisibility](https://alphabetamath.cc/item/def-divides-in-z)

[F3] The usual inclusion of the natural numbers into the integers preserves and reflects order, preserves addition and multiplication, and has image the nonnegative integers. [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[F4] A sum over a finite set can be evaluated by listing its elements in any order, each exactly once, and adding their terms along the list. For a list of $k$ natural numbers, use the sequence on $\mathbb N$ that agrees with the list at indices $i<k$ and has value $0$ at indices $i\ge k$. For any sequence of natural numbers, each term among the first $k$ terms is at most their sum, for every natural number $k$. [Summation over a finite set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order) [Zero extension for natural-number sums](https://alphabetamath.cc/item/def-nat-finite-sum-and-product) [Finite natural-number sum laws, clause 4](https://alphabetamath.cc/item/lem-nat-finite-sum-laws-and-the-canonical-embedding)

[F5] Integer addition has identity $0$ and additive inverses. Integer multiplication is associative, has identity $1$, and distributes over addition. Adding the same integer on both sides preserves order, and a product of positive integers is positive. [math:def-integers](https://alphabetamath.cc/item/def-integers) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:def-int-order](https://alphabetamath.cc/item/def-int-order) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)

[F6] For a positive odd integer $m$ and $n=2m$, the signed, ordered count with zeros allowed is $R(n)=24\sigma(m)$. [lem-euler-four-square-count](item-lem-euler-four-square-count)

## Proof

**Given:** A positive odd integer $m$ and $n=2m$.

**Goal:** Prove $R(n)=24\sigma(m)\ge12n$.

1.1 Since $2>0$ and $m>0$, we have $n=2m>0$. The count in the statement therefore has the finite interpretation in [F1], and [F6] applies with the given $m$ and $n$, yielding $R(n)=24\sigma(m)$. [given, F1, F5, F6]

1.2 The identity $m=m\cdot1$ and the assumption $m>0$ give $m\in D(m)$. Choose a list of the elements of $D(m)$, each exactly once, of length $k$. Its entry at some index $j<k$ is the natural number corresponding to $m$ under [F3]. Extend the list to $a:\mathbb N\to\mathbb N$ by taking $a_i$ to be the list entry at index $i$ for $i<k$ and $0$ for $i\ge k$. By [F2] and [F4], $\sigma(m)=\sum_{i<k}a_i$ in the natural numbers. The single-term bound in [F4] gives $m=a_j\le\sum_{i<k}a_i=\sigma(m)$ in the natural numbers. The inclusion in [F3] preserves this inequality in the integers. [given, F2, F3, F4, F5]

2.1 Adding $-m$ to $m\le\sigma(m)$ gives $0\le\sigma(m)-m$. Its product with $24>0$ is zero if $\sigma(m)-m=0$ and positive otherwise. By distributivity this product equals $24\sigma(m)-24m$, so adding $24m$ gives $24m\le24\sigma(m)$. Finally $24m=12(2m)=12n$, and step 1.1 gives $R(n)=24\sigma(m)\ge12n$. [given, F5, step 1.1, step 1.2] ∎
