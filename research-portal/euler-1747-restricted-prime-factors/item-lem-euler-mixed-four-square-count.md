---
title: The mixed-parity count
status: draft
research_item: lem-euler-mixed-four-square-count
dependency_level: 2
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §2, equation (2.2)
---

PDF p. 2: ` §2, equation (2.2) `

## Prerequisites

- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [def-euler-four-square-representations](item-def-euler-four-square-representations)
- [def-euler-mixed-four-square-representations](item-def-euler-mixed-four-square-representations)
- [def-euler-divisor-functions](item-def-euler-divisor-functions)
- [lem-euler-four-square-parities](item-lem-euler-four-square-parities)
- [lem-euler-four-square-count](item-lem-euler-four-square-count)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)
- [math:lem-unions-and-intersections-of-small-families](https://alphabetamath.cc/item/lem-unions-and-intersections-of-small-families)
- [math:def-axiom-of-extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)
- [math:lem-int-cancellation](https://alphabetamath.cc/item/lem-int-cancellation)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)


## Statement

Let $m$ be a positive odd integer, so $m>0$ and $m=2k+1$ for some integer $k$. Set $n=2m$. Let $\mathcal R(n)$ consist of the ordered quadruples $(x_1,x_2,x_3,x_4)$ of integers whose squares sum to $n$, where $x_i^2=x_i\cdot x_i$. Zero and both signs are allowed in each position. Write $R(n)=|\mathcal R(n)|$, where $|S|$ is the number of elements of a finite set $S$.

Let $\mathcal R_{\mathrm{mix}}(n)$ consist of the quadruples in $\mathcal R(n)$ with one even and one odd entry in each of the pairs $(x_1,x_2)$ and $(x_3,x_4)$. An even integer has the form $2a$ for an integer $a$, and an odd integer has the form $2a+1$. Let $\sigma(m)$ be the sum of the positive integers $d$ such that $m=dq$ for some integer $q$. Then

$$|\mathcal R_{\mathrm{mix}}(n)|=16\sigma(m)=\frac{2}{3}R(n).$$

The counts and the divisor sum are identified with nonnegative integers. The last product is in the rationals, with each integer $a$ represented by $a/1$.

## Statement references

[def-euler-four-square-representations](item-def-euler-four-square-representations)

[def-euler-mixed-four-square-representations](item-def-euler-mixed-four-square-representations)

[def-euler-divisor-functions](item-def-euler-divisor-functions)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

## Facts & Assumptions

[F1] For each positive integer $u$, the set $\mathcal R(u)$ of ordered integer quadruples with square sum $u$ is finite and has cardinality $R(u)$. The cardinality of a finite set is the unique number of entries in a list that contains each element exactly once. [def-euler-four-square-representations](item-def-euler-four-square-representations) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F2] For each positive integer $u$, the finite set $\mathcal R_{\mathrm{mix}}(u)$ consists of the quadruples in $\mathcal R(u)$ with opposite parity in each of the two specified pairs, meaning one even and one odd entry in each pair. [def-euler-mixed-four-square-representations](item-def-euler-mixed-four-square-representations)

[F3] For each positive integer $u$, the sum $\sigma(u)$ adds each positive divisor of $u$ once. A positive divisor of $u$ is a positive integer $d$ with $u=dq$ for some integer $q$. [def-euler-divisor-functions](item-def-euler-divisor-functions)

[F4] Integers are represented by differences of natural numbers. An integer is positive if it is greater than zero. Integer addition and multiplication are associative and commutative, multiplication distributes over addition, adding the same integer preserves order, and products of positive integers are positive. Natural numbers are identified with nonnegative integers by a map that is one-to-one and preserves addition, multiplication and order. [math:def-integers](https://alphabetamath.cc/item/def-integers) [math:def-int-order](https://alphabetamath.cc/item/def-int-order) [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[F5] For positive $u$ of the form $4k+2$ with $k$ an integer, each quadruple in $\mathcal R(u)$ has exactly two odd entries. Let $X_D$ be the finite set of those quadruples whose odd entries occur exactly at the positions in the two-element set $D$. The six possible choices of $D$ give equal cardinalities. Exactly four choices put one odd entry in each of the specified pairs. [lem-euler-four-square-parities](item-lem-euler-four-square-parities)

[F6] For two finite sets that are disjoint, meaning they have no common element, their union is finite and its cardinality is the sum of their cardinalities. [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)

[F7] If $m>0$ is an integer, no integer $q$ satisfies $m=2q$, and $n=2m$, then $R(n)=24\sigma(m)$. [lem-euler-four-square-count](item-lem-euler-four-square-count)

[F8] A common nonzero factor can be cancelled from an equality of integer products. [math:lem-int-cancellation](https://alphabetamath.cc/item/lem-int-cancellation)

[F9] For integers $a,b,c,d$ with $b,d\ne0$, the rational numbers $a/b$ and $c/d$ are equal exactly when $ad=bc$. Their product is $(ac)/(bd)$, and the inclusion of an integer $a$ into the rationals sends it to $a/1$. [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[F10] For integers $a$ and $b$ with $b>0$, there is a unique pair of integers $(q,r)$ with $a=qb+r$ and $0\le r<b$. [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

[F11] By clause (iii) of [math:lem-unions-and-intersections-of-small-families](https://alphabetamath.cc/item/lem-unions-and-intersections-of-small-families), for any two sets $A$ and $B$, an element belongs to $A \cup B$ exactly when it belongs to $A$ or to $B$.

[F12] Two sets are equal if every element belongs to the first exactly when it belongs to the second. [math:def-axiom-of-extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)

## Proof

**Given:** A positive odd integer $m$ and $n=2m$.

**Goal:** Show that $|\mathcal R_{\mathrm{mix}}(n)|=16\sigma(m)=\frac{2}{3}R(n)$.

1.1 Write $m=2k+1$ with $k$ an integer. Then $n=2m>0$ and $n=4k+2$, so F5 applies to $\mathcal R(n)$. Every quadruple belongs to one of the six sets $X_D$ because it has exactly two odd entries. It cannot belong to two different sets, since its positions with odd entries determine $D$ uniquely. [given, F4, F5]

2.1 A quadruple in $\mathcal R(n)$ lies in $\mathcal R_{\mathrm{mix}}(n)$ exactly when it belongs to one of the four sets with $D$ equal to $\{1,3\}$, $\{1,4\}$, $\{2,3\}$, or $\{2,4\}$. These are the choices that put one odd entry in each pair. Let $c=|X_{\{1,2\}}|$. All six sets are finite and each has cardinality $c$. [F1, F2, F5, step 1.1]

2.2 By Step 1.1 and commutativity, $m=k\cdot2+1$ with $0\le1<2$, so the remainder on dividing $m$ by $2$ is $1$ by F10. If $m=2q$ for an integer $q$, then $m=q\cdot2+0$ with $0\le0<2$, which gives remainder $0$. Uniqueness of the remainder rules out such an integer $q$. [F4, F10, step 1.1]

3.1 For each collection of classes, start with one class and adjoin the other classes one at a time by binary union. Repeated use of F11 shows that an element belongs to the accumulated union exactly when it belongs to at least one class already adjoined. A member of the next class belongs to none of those classes by Step 1.1, so the next class and the accumulated union are disjoint. The first class is finite with count $c$, and F6 shows that adjoining each next class keeps the union finite and adds $c$ to its count. Steps 1.1 and 2.1 give the same membership conditions for the final unions and for $\mathcal R(n)$ and $\mathcal R_{\mathrm{mix}}(n)$, respectively. By F12 each final union equals the corresponding representation set. Thus $R(n)=6c$ and $|\mathcal R_{\mathrm{mix}}(n)|=4c$. [F1, F2, F4, F6, F11, F12, step 1.1, step 2.1]

4.1 Since $m>0$, $n=2m$ and no integer $q$ satisfies $m=2q$, F7 gives $6c=R(n)=24\sigma(m)=6(4\sigma(m))$ using Step 3.1. Cancelling the common factor $6$ gives $c=4\sigma(m)$, and hence $|\mathcal R_{\mathrm{mix}}(n)|=4c=16\sigma(m)$. [given, F3, F4, F7, F8, step 3.1, step 2.2]

5.1 In the rationals, $\frac{2}{3}R(n)=\frac{2R(n)}{3}$. Because $2R(n)=2(24\sigma(m))=3(16\sigma(m))$, the fraction equals $(16\sigma(m))/1$ by the equality rule in F9. Therefore $|\mathcal R_{\mathrm{mix}}(n)|=16\sigma(m)=\frac{2}{3}R(n)$. [F4, F9, step 4.1] ∎
