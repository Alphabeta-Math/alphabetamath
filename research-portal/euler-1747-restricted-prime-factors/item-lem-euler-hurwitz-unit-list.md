---
title: The 24 Hurwitz units
status: published
research_item: lem-euler-hurwitz-unit-list
dependency_level: 3
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §3.1, sentence immediately after the displayed Hurwitz order
      reading_limits: Read the unit enumeration and the preceding coordinate and norm
        formulas on PDF p. 2. This reference credits the enumeration.
---

PDF p. 2: ` §3.1, enumeration of units `

## Prerequisites

- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [math:def-ring](https://alphabetamath.cc/item/def-ring)
- [thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure)
- [lem-rational-hamilton-norm-and-inverse](item-lem-rational-hamilton-norm-and-inverse)
- [math:def-invertible-element](https://alphabetamath.cc/item/def-invertible-element)
- [math:def-group](https://alphabetamath.cc/item/def-group)
- [math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group)
- [math:thm-rat-ordered-field](https://alphabetamath.cc/item/thm-rat-ordered-field)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)
- [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)


## Statement

Let $B$ be the rational Hamilton quaternion algebra, with unique expressions $x=a+bi+cj+dk$ for $a,b,c,d\in\mathbb Q$, identity $1$, and multiplication determined by $i^2=j^2=-1$ and $ij=k=-ji$ by distributing over sums and moving rational scalars through products. Let $\mathcal H$ be its Hurwitz order, the quaternions whose four coordinates are all integers or all of the form $n+\tfrac12$ with $n\in\mathbb Z$. Write $N(x)=a^2+b^2+c^2+d^2$ for the reduced norm. The unit group $\mathcal H^\times$ is the set of $u\in\mathcal H$ with a two-sided inverse in $\mathcal H$, meaning some $v\in\mathcal H$ satisfies $uv=vu=1$, equipped with the inherited multiplication.

The units are exactly the elements of $\mathcal H$ of reduced norm $1$. The $24$ units comprise the eight elements $\pm1,\pm i,\pm j,\pm k$ and the sixteen elements $(\pm1\pm i\pm j\pm k)/2$, with the four signs chosen independently.

## Statement references

[Rational Hamilton quaternions and reduced norm](item-def-euler-hamilton-quaternions)

[The Hurwitz order](item-def-euler-hurwitz-order)

[Integral structure of the Hurwitz order](item-thm-hurwitz-order-integral-structure)

[Ring axiom (R2)](https://alphabetamath.cc/item/def-ring)

[Units and two-sided inverses](https://alphabetamath.cc/item/def-invertible-element)

[Groups](https://alphabetamath.cc/item/def-group)

[The group of units of a ring](https://alphabetamath.cc/item/lem-ring-units-form-a-group)

[Counting elements of a finite set](https://alphabetamath.cc/item/def-finite-cardinality)

## Facts & Assumptions

[F1] Coordinates in $1,i,j,k$ are unique in $B$, and the norm is the sum of their squares. [Rational Hamilton quaternions](item-def-euler-hamilton-quaternions) The coordinate description of $\mathcal H$ identifies it with a subring of $B$ with the inherited multiplication and the same identity $1$. [The Hurwitz order](item-def-euler-hurwitz-order) [Integral structure of the Hurwitz order](item-thm-hurwitz-order-integral-structure) By axiom (R2), its multiplication is associative and $1$ is a two-sided identity, so $(\mathcal H,\cdot,1)$ is a monoid. [Ring axiom (R2)](https://alphabetamath.cc/item/def-ring)

[F2] For each $x=a+bi+cj+dk\in\mathcal H$, its reduced norm $N(x)$ is an integer and its quaternion conjugate $\bar x=a-bi-cj-dk$ belongs to $\mathcal H$. [Integer norms and closure under conjugation](item-thm-hurwitz-order-integral-structure)

[F3] For rational Hamilton quaternions $x,y$, one has $N(xy)=N(x)N(y)$ and $x\bar x=\bar x x=N(x)1$. [Multiplicativity and the conjugate product](item-lem-rational-hamilton-norm-and-inverse)

[F4] A unit of a ring is an element with a two-sided inverse in its multiplicative monoid. A group has an associative operation defined for all pairs, a two-sided identity, and a two-sided inverse for every element. The units of a unital ring form a group under the ring multiplication with the same identity. [Two-sided inverses](https://alphabetamath.cc/item/def-invertible-element) [Group axioms](https://alphabetamath.cc/item/def-group) [The group of units of a ring](https://alphabetamath.cc/item/lem-ring-units-form-a-group)

[F5] The rationals have a total order compatible with addition, and the product of two rationals greater than zero is greater than zero. [The ordered rational field](https://alphabetamath.cc/item/thm-rat-ordered-field)

[F6] Both embeddings $\mathbb N\hookrightarrow\mathbb Z\hookrightarrow\mathbb Q$ preserve order and arithmetic and identify $0$ and $1$ in these systems. The image of $\mathbb N$ is exactly the nonnegative integers in $\mathbb Z$. In $\mathbb N$, $1$ is the immediate successor of $0$, so every natural number greater than $0$ is at least $1$. [Naturals as nonnegative integers](https://alphabetamath.cc/item/lem-nat-embeds-int) [Integers as rationals](https://alphabetamath.cc/item/lem-int-embeds-rat) [Discreteness of natural-number order](https://alphabetamath.cc/item/lem-nat-discrete)

[F7] The cardinality $\lvert A\rvert$ of a finite set $A$ is the unique natural number $m$ for which the $m$ indices from $0$ up to but excluding $m$ can be matched one-to-one with all the elements of $A$. A bijection, meaning a one-to-one and onto map, preserves cardinality. [Finite cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F8] The number of ordered tuples with one entry from each of finitely many finite sets is the product of their cardinalities. The cardinalities of two finite sets with no common elements add when the sets are united. [Product rule for finite sets](https://alphabetamath.cc/item/thm-product-rule) [Sum rule for disjoint finite sets](https://alphabetamath.cc/item/thm-sum-rule)

## Proof

**Given:** The Hurwitz order $\mathcal H$ in $B$, with its two types of coordinates and reduced norm $N$ as above.

**Goal:** Show that its units are precisely the norm-$1$ elements and that these give the stated list of $24$ distinct units.

1.1 A rational square is nonnegative because the square of a negative rational equals the square of its positive opposite. By the embeddings and discreteness in [F6], a positive integer is at least $1$ in $\mathbb Q$. If $z$ is a nonzero integer, take $t=z$ when $z>0$ and $t=-z$ when $z<0$. Then $t\ge 1$ and $z^2=t^2$. If $t>1$, the identity $t^2-1=(t-1)(t+1)$ gives $t^2>1$. Thus a nonzero integer square is at least $1$, with equality exactly for $z=1$ or $z=-1$. [F5, F6]

2.1 If $u$ is a unit with inverse $v\in\mathcal H$, then $N(u)N(v)=N(uv)=N(1)=1$. Both norms are nonnegative integers by their coordinate formula and [F2], so both are positive. The lower bound from step 1.1 forces each to equal $1$, since a factor greater than $1$ times a factor at least $1$ gives a product greater than $1$. Conversely, if $u\in\mathcal H$ and $N(u)=1$, then $\bar u\in\mathcal H$ and $u\bar u=\bar u u=1$, so $u$ is a unit. [F1, F2, F3, F4, F5, step 1.1]

2.2 If a norm-$1$ element of $\mathcal H$ has integer coordinates, it has at least one nonzero coordinate, since four zero coordinates would give norm $0$. Two nonzero coordinates would contribute at least $2$ to the norm, so there is exactly one. Its square is $1$, making that coordinate $1$ or $-1$ by step 1.1. Conversely, each such quadruple belongs to $\mathcal H$ and has norm $1$, giving exactly the elements $\pm1,\pm i,\pm j,\pm k$. [F1, F5, step 1.1]

2.3 If the four coordinates $a,b,c,d$ of $x\in\mathcal H$ are all of the form $n+\tfrac12$ with $n\in\mathbb Z$, then each doubled coordinate is an integer of the form $2n+1$. It is at least $1$ when $n\ge0$ and at most $-1$ when $n<0$, since then $-n\ge1$. If $N(x)=1$, the four doubled coordinates have squares summing to $4$. Each square is at least $1$, so all four equal $1$ and every coordinate is $\tfrac12$ or $-\tfrac12$. Conversely, each quadruple of these signs belongs to $\mathcal H$, since $\tfrac12=0+\tfrac12$ and $-\tfrac12=-1+\tfrac12$, and its norm is $4\cdot\tfrac14=1$. [F1, F5, F6, step 1.1]

3.1 By [F1] and [F4], $\mathcal H^\times$ is a group under the inherited multiplication with identity $1$. In the first list the coordinate position and sign determine distinct elements, so there are $4\cdot2=8$. In the second list distinct sign quadruples give distinct elements, so there are $2^4=16$. The lists have no common element because the first list has three zero coordinates and the second has none. The coordinate description exhausts $\mathcal H$, so the two lists exhaust its norm-$1$ elements. Step 2.1 identifies their union with the unit group, which therefore has $8+16=24$ elements, all of reduced norm $1$. [F1, F4, F7, F8, step 2.1, step 2.2, step 2.3] ∎
