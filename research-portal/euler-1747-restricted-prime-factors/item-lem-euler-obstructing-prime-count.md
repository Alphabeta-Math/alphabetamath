---
title: Counting obstructing primes above 3 (Lemma 5.2)
status: draft
research_item: lem-euler-obstructing-prime-count
dependency_level: 3
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 6, Lemma 5.2, equation (5.2) and its proof through the periodicity
        argument
---

PDF p. 6: ` Lemma 5.2, equation (5.2) `

## Prerequisites

- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [def-euler-obstructing-prime-residue-count](item-def-euler-obstructing-prime-residue-count)
- [lem-euler-obstructing-prime-residue-inclusion](item-lem-euler-obstructing-prime-residue-inclusion)
- [lem-euler-obstructing-prime-residue-discrepancy](item-lem-euler-obstructing-prime-residue-discrepancy)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)


## Statement

Let $t\ge0$ be real. The set $\mathcal P_3$ consists of the primes congruent to $3$ modulo $4$. A prime is an integer $p>1$ whose only positive divisors are $1$ and $p$. A positive divisor is an integer $d>0$ with $p=dk$ for some integer $k$. Congruence to $3$ modulo $4$ means $p-3=4q$ for some integer $q$. Call the members of $\mathcal P_3$ obstructing primes.

Use the usual order-preserving inclusions of the integers and the nonnegative whole numbers in the reals to compare primes and counts with real numbers. Then the set $\{p\in\mathcal P_3:3<p\le t\}$ is finite and
$$\#\{p\in\mathcal P_3:3<p\le t\}\le \frac{2t}{15}+1.$$
A set is finite if, for some nonnegative integer $k$, its elements can be listed exactly once each in $k$ positions. For a finite set $S$, $\#S$ is the number of its elements.

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)

## Facts & Assumptions

[F1] The inclusions of nonnegative whole numbers into integers, integers into rationals, and rationals into reals preserve addition and multiplication. They preserve and reflect order. Their compositions justify the comparisons in the statement. [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[F2] For $t\ge0$, $C(t)$ is the finite set of integers $k$ with $0<k\le t$ and $k-r=60q$ for an integer $q$ and some $r\in\{7,11,19,23,31,43,47,59\}$. Its count is $A(t)=\#C(t)$. [def-euler-obstructing-prime-residue-count](item-def-euler-obstructing-prime-residue-count) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[F3] Every $p\in\mathcal P_3$ with $p>3$ has $p-r=60q$ for an integer $q$ and a representative $r$ from the list in [F2]. [lem-euler-obstructing-prime-residue-inclusion](item-lem-euler-obstructing-prime-residue-inclusion) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[F4] A condition on the elements of a set selects a unique subset. The notation $B\subseteq C$ means that every element of $B$ belongs to $C$. If $C$ is finite and $B\subseteq C$, then $B$ is finite and $\#B\le\#C$, using the number of elements of each set. [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F5] For the count $A(t)$ of [F2] and every real $t\ge0$, the upper bound for the difference from $2t/15$ is $A(t)-2t/15\le14/15$. [lem-euler-obstructing-prime-residue-discrepancy](item-lem-euler-obstructing-prime-residue-discrepancy)

[F6] The real order is transitive. Adding the same number to both sides preserves an inequality, and the reciprocal of a positive number is positive. [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field) [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)

## Proof

**Given:** A real number $t\ge0$ and the set $\mathcal P_3$ from the statement.

**Goal:** Prove that $\{p\in\mathcal P_3:3<p\le t\}$ is finite and has at most $2t/15+1$ elements.

1.1 Let $B(t)=\{p\in\mathcal P_3:3<p\le t\}$, the subset selected by the indicated inequalities. If $p\in B(t)$ then $p$ is an integer with $3<p\le t$ in the real order. The integer comparison $0<3$ also holds in the reals by [F1], so transitivity gives $0<p$ there. By order reflection in [F1], the comparisons $0<p$ and $3<p$ hold in the integers. By [F3], there is an integer $q$ with $p-r=60q$ for a representative $r$ from [F2]. Thus $p\in C(t)$, and $B(t)\subseteq C(t)$. [given, F1, F2, F3, F4, F6]

2.1 Since $C(t)$ is finite, the inclusion gives finiteness of $B(t)$ and $\#B(t)\le\#C(t)=A(t)$. This inequality of counts also holds in the reals. [F1, F2, F4, step 1.1]

3.1 Add $2t/15$ to both sides of the inequality in [F5] to get $A(t)\le2t/15+14/15$. Since $1-14/15=1/15>0$, it follows that $\#B(t)\le2t/15+14/15\le2t/15+1$. This is the claimed bound. [F1, F5, F6, step 2.1] ∎
