---
title: Reciprocal-square tail for the eight residue classes
status: draft
research_item: lem-euler-residue-reciprocal-square-tail
dependency_level: 2
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: PDF p. 6, proof of Lemma 5.2, displayed identity and upper bound after
        “Partial summation yields”
---

PDF p. 6: ` Lemma 5.2, displayed partial-summation identity and upper bound `

## Prerequisites

- [math:lem-unions-and-intersections-of-small-families](https://alphabetamath.cc/item/lem-unions-and-intersections-of-small-families)
- [math:def-axiom-of-extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)
- [def-euler-obstructing-prime-residue-count](item-def-euler-obstructing-prime-residue-count)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)
- [math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum)
- [math:def-series](https://alphabetamath.cc/item/def-series)
- [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-interval](https://alphabetamath.cc/item/def-interval)
- [math:def-darboux-integral](https://alphabetamath.cc/item/def-darboux-integral)
- [math:def-darboux-sums](https://alphabetamath.cc/item/def-darboux-sums)
- [math:def-infimum](https://alphabetamath.cc/item/def-infimum)
- [math:def-improper-integral-at-infinity](https://alphabetamath.cc/item/def-improper-integral-at-infinity)
- [math:def-limits-at-infinity](https://alphabetamath.cc/item/def-limits-at-infinity)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)
- [lem-euler-obstructing-prime-residue-discrepancy](item-lem-euler-obstructing-prime-residue-discrepancy)
- [lem-reciprocal-square-tail-from-counting](item-lem-reciprocal-square-tail-from-counting)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-bounded-set](https://alphabetamath.cc/item/def-bounded-set)
- [math:def-partition-and-refinement](https://alphabetamath.cc/item/def-partition-and-refinement)


## Statement

Use the complete ordered field of real numbers, with integers included in a way that preserves order and arithmetic. Completeness means that each nonempty set of reals bounded above has a least upper bound. The absolute value of a real number is the number itself when it is nonnegative and its negative otherwise.

Let $\mathcal S$ consist of the eight residue classes modulo $60$ represented by $7,11,19,23,31,43,47,59$. The class represented by $r$ consists of the integers $k$ for which $k-r$ is an integer multiple of $60$. Write $D$ for the set of positive integers in these classes, where positive means $k>0$. For real $t\ge0$, let $A(t)$ be the number of elements of the finite set $\{k\in D:k\le t\}$.

For every real $P\ge3$, the following series and improper integral both converge and satisfy
$$\sum_{\substack{k>P\\k\in D}}\frac{1}{k^2}=2\int_P^\infty\frac{A(t)-A(P)}{t^3}\,dt\le\frac{2}{15P}+\frac{2}{P^2}.$$

Identify the natural numbers $0,1,2,\ldots$ with the nonnegative integers by the canonical order- and addition-preserving embedding. The series is the limit of the finite sums through positive integer $n$. The $n$th partial sum starts at zero and adds the terms for natural indices $j<n$ in order. At index $j$, let $k$ be the integer corresponding to the successor of $j$. The term is $1/k^2$ if $k>P$ and $k\in D$, and is zero otherwise. A sequence has limit $L$ if for every positive rational tolerance all sufficiently late terms differ from $L$ by less than that tolerance in absolute value. The rationals in this limit criterion are the real quotients $a/b$ of integers $a,b$ with $b\ne0$.

The improper integral is the finite limit of the integrals over $[P,R]=\{t:P\le t\le R\}$ as the real endpoint $R$ increases without bound. This means that for every positive real tolerance the finite integral differs from the limit by less than that tolerance in absolute value for every $R$ beyond some real cutoff. Each finite integral is a Darboux integral. For a bounded function on $[P,R]$, this integral is defined when the least upper bound of the lower sums equals the greatest lower bound of the upper sums, with both bounds taken over all subdivisions. A greatest lower bound is a number at most every element of the set and at least every other lower bound. A subdivision is a finite strictly increasing list of points starting at $P$ and ending at $R$. Its subintervals include both endpoints. For each subinterval the lower sum adds its length times the greatest lower bound of the function there, and the upper sum adds its length times the least upper bound of the function there. For positive real $x$, $x^2=x\cdot x$ and $x^3=x\cdot x\cdot x$, and $1/x^r$ denotes the reciprocal of $x^r$ for $r=2,3$.

## Statement references

[def-euler-obstructing-prime-residue-count](item-def-euler-obstructing-prime-residue-count)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)

[math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum)

[math:def-series](https://alphabetamath.cc/item/def-series)

[math:def-real-limit](https://alphabetamath.cc/item/def-real-limit)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:def-interval](https://alphabetamath.cc/item/def-interval)

[math:def-darboux-integral](https://alphabetamath.cc/item/def-darboux-integral)

[math:def-darboux-sums](https://alphabetamath.cc/item/def-darboux-sums)

[math:def-infimum](https://alphabetamath.cc/item/def-infimum)

[math:def-improper-integral-at-infinity](https://alphabetamath.cc/item/def-improper-integral-at-infinity)

[math:def-limits-at-infinity](https://alphabetamath.cc/item/def-limits-at-infinity)

[math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-bounded-set](https://alphabetamath.cc/item/def-bounded-set)

[math:def-partition-and-refinement](https://alphabetamath.cc/item/def-partition-and-refinement)

## Facts & Assumptions

[F1] For every real $x\ge0$, the finite set of positive integers in the eight classes that are at most $x$ has cardinality $A(x)$. The cardinality of a finite set is its number of elements ([def-euler-obstructing-prime-residue-count](item-def-euler-obstructing-prime-residue-count), [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)).

[F2] Every subset of a finite set is finite ([math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)). For two disjoint finite sets, meaning that they have no common element, the number of elements in their union is the sum of their cardinalities ([math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule), two-block case).

[F3] For the count $A$ in [F1] and real $t\ge P\ge3$, $A(t)-A(P)\le(2/15)(t-P)+2$ ([lem-euler-obstructing-prime-residue-discrepancy](item-lem-euler-obstructing-prime-residue-discrepancy)).

[F4] Let $D$ be a subset of the positive integers and let $P>0$ be real. Put $C_P(t)=|\{k\in D:P<k\le t\}|$ for real $t\ge P$, where the bars give the number of elements. If $C_P(t)\le a(t-P)+b$ for all real $t\ge P$ with $a,b\ge0$ real, then the series over $k\in D$ with $k>P$ and the improper integral of $C_P(t)/t^3$ converge, and
$$\sum_{\substack{k\in D\\k>P}}\frac{1}{k^2}=2\int_P^\infty\frac{C_P(t)}{t^3}\,dt\le\frac aP+\frac b{P^2}.$$
[lem-reciprocal-square-tail-from-counting](item-lem-reciprocal-square-tail-from-counting)

[F5] Real addition and multiplication obey the ordered field laws. In particular, inequalities are preserved by adding a fixed real number, and products of positive numbers are positive ([math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)). The canonical embedding from the natural numbers into the integers preserves addition and order and has image the nonnegative integers ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)). For real arithmetic, first send each natural-number count to the integers by the canonical map, then send each integer $k$ to $k/1$ in the rationals, and finally take the canonical real image of that rational. The natural-number order and addition here are the usual ones ([math:def-nat-order](https://alphabetamath.cc/item/def-nat-order), [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)). The integer-to-rational and rational-to-real maps preserve addition and order ([math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat), [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)). These maps agree with the inclusions used for the residue count ([def-euler-obstructing-prime-residue-count](item-def-euler-obstructing-prime-residue-count)) and in [F4].

[F6] Separation forms a subset of a given set by retaining exactly the elements that satisfy the specified condition. Inclusion in a set means that every member belongs to that set ([math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)). An element belongs to a binary union exactly when it belongs to at least one of the two sets. Sets with the same members are equal. [math:lem-unions-and-intersections-of-small-families](https://alphabetamath.cc/item/lem-unions-and-intersections-of-small-families) [math:def-axiom-of-extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)

## Proof

**Given:** The residue classes and the count $A$ in the Statement, and a real cutoff $P\ge3$.

**Goal:** Prove convergence, the integral identity and the stated upper bound.

1.1 Fix real $t\ge P$. By separation in [F6], form $B(x)=\{k\in D:k\le x\}$ for $x\ge0$. The sets $B(P)$ and $B(t)$ are finite and have cardinalities $A(P)$ and $A(t)$. Let $E=\{k\in D:P<k\le t\}$ be the set counted by $C_P(t)$ in [F4]. Every member of $B(t)$ belongs to $B(P)$ if it is at most $P$, and belongs to $E$ if it exceeds $P$. Conversely both $B(P)$ and $E$ are contained in $B(t)$, and the two cutoff conditions show they are disjoint. By binary union membership and extensionality in [F6], $B(t)=B(P)\cup E$. As a subset of $B(t)$, the set $E$ is finite. The two-block case in [F2] gives $A(t)=A(P)+C_P(t)$ as natural cardinalities. Each of the three maps in [F5] preserves addition, so the composite gives the same equality for the real images of the counts. Subtracting $A(P)$ in the real field gives $C_P(t)=A(t)-A(P)$. [given, F1, F2, F4, F5, F6]

2.1 By step 1.1 and [F3], $C_P(t)\le(2/15)(t-P)+2$ for every real $t\ge P$. Every member of $D$ is a positive integer, so $D$ is a subset of the positive integers by [F6]. We have $P\ge3>0$ and the real numbers $2/15$ and $2$ are nonnegative. Hence [F4] applies with $a=2/15$ and $b=2$. [given, F3, F4, F5, F6, step 1.1]

3.1 By [F4] the series and improper integral converge. The series in [F4] and the Statement have the same finite sums through each positive integer cutoff, since both include $1/k^2$ exactly for $k>P$ with $k\in D$ and use zero elsewhere. By step 1.1 the integrands $C_P(t)/t^3$ and $(A(t)-A(P))/t^3$ agree for every $t\ge P$, including the endpoint. Thus their finite integrals agree for each $R>P$ and have the same limit. The bound in [F4] becomes $(2/15)/P+2/P^2=2/(15P)+2/P^2$, which proves the displayed identity and inequality. [F4, F5, step 1.1, step 2.1] ∎
