---
id: lem-euler-hurwitz-unit-list
kind: lemma
title: The 24 Hurwitz units
status: published
domain: mathematics
deps:
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - math:def-ring
  - thm-hurwitz-order-integral-structure
  - lem-rational-hamilton-norm-and-inverse
  - math:def-invertible-element
  - math:def-group
  - math:lem-ring-units-form-a-group
  - math:thm-rat-ordered-field
  - math:lem-int-embeds-rat
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
  - math:def-finite-cardinality
  - math:thm-product-rule
  - math:thm-sum-rule
formulation_deps:
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - thm-hurwitz-order-integral-structure
  - math:def-ring
  - math:lem-ring-units-form-a-group
  - math:def-invertible-element
  - math:def-group
  - math:def-finite-cardinality
argument_deps:
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - math:def-ring
  - thm-hurwitz-order-integral-structure
  - lem-rational-hamilton-norm-and-inverse
  - math:def-invertible-element
  - math:def-group
  - math:lem-ring-units-form-a-group
  - math:thm-rat-ordered-field
  - math:lem-int-embeds-rat
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
  - math:def-finite-cardinality
  - math:thm-product-rule
  - math:thm-sum-rule
dependency_roles:
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  thm-hurwitz-order-integral-structure: mathematical-premise
  lem-rational-hamilton-norm-and-inverse: mathematical-premise
  math:def-ring: mathematical-premise
  math:def-invertible-element: mathematical-premise
  math:def-group: mathematical-premise
  math:lem-ring-units-form-a-group: mathematical-premise
  math:thm-rat-ordered-field: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-product-rule: mathematical-premise
  math:thm-sum-rule: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §3.1, sentence immediately after the displayed Hurwitz order
      reading_limits: Read the unit enumeration and the preceding coordinate and norm
        formulas on PDF p. 2. This reference credits the enumeration.
dependency_level: 3
---

## Statement

Let $B$ be the rational Hamilton quaternion algebra, with unique expressions $x=a+bi+cj+dk$ for $a,b,c,d\in\mathbb Q$, identity $1$, and multiplication determined by $i^2=j^2=-1$ and $ij=k=-ji$ by distributing over sums and moving rational scalars through products. Let $\mathcal H$ be its Hurwitz order, the quaternions whose four coordinates are all integers or all of the form $n+\tfrac12$ with $n\in\mathbb Z$. Write $N(x)=a^2+b^2+c^2+d^2$ for the reduced norm. The unit group $\mathcal H^\times$ is the set of $u\in\mathcal H$ with a two-sided inverse in $\mathcal H$, meaning some $v\in\mathcal H$ satisfies $uv=vu=1$, equipped with the inherited multiplication.

The units are exactly the elements of $\mathcal H$ of reduced norm $1$. The $24$ units comprise the eight elements $\pm1,\pm i,\pm j,\pm k$ and the sixteen elements $(\pm1\pm i\pm j\pm k)/2$, with the four signs chosen independently.

## Statement references

[[def-euler-hamilton-quaternions|Rational Hamilton quaternions and reduced norm]]

[[def-euler-hurwitz-order|The Hurwitz order]]

[[thm-hurwitz-order-integral-structure|Integral structure of the Hurwitz order]]

[[math:def-ring|Ring axiom (R2)]]

[[math:def-invertible-element|Units and two-sided inverses]]

[[math:def-group|Groups]]

[[math:lem-ring-units-form-a-group|The group of units of a ring]]

[[math:def-finite-cardinality|Counting elements of a finite set]]

## Facts & Assumptions

[F1] Coordinates in $1,i,j,k$ are unique in $B$, and the norm is the sum of their squares. [[def-euler-hamilton-quaternions|Rational Hamilton quaternions]] The coordinate description of $\mathcal H$ identifies it with a subring of $B$ with the inherited multiplication and the same identity $1$. [[def-euler-hurwitz-order|The Hurwitz order]] [[thm-hurwitz-order-integral-structure|Integral structure of the Hurwitz order]] By axiom (R2), its multiplication is associative and $1$ is a two-sided identity, so $(\mathcal H,\cdot,1)$ is a monoid. [[math:def-ring|Ring axiom (R2)]]

[F2] For each $x=a+bi+cj+dk\in\mathcal H$, its reduced norm $N(x)$ is an integer and its quaternion conjugate $\bar x=a-bi-cj-dk$ belongs to $\mathcal H$. [[thm-hurwitz-order-integral-structure|Integer norms and closure under conjugation]]

[F3] For rational Hamilton quaternions $x,y$, one has $N(xy)=N(x)N(y)$ and $x\bar x=\bar x x=N(x)1$. [[lem-rational-hamilton-norm-and-inverse|Multiplicativity and the conjugate product]]

[F4] A unit of a ring is an element with a two-sided inverse in its multiplicative monoid. A group has an associative operation defined for all pairs, a two-sided identity, and a two-sided inverse for every element. The units of a unital ring form a group under the ring multiplication with the same identity. [[math:def-invertible-element|Two-sided inverses]] [[math:def-group|Group axioms]] [[math:lem-ring-units-form-a-group|The group of units of a ring]]

[F5] The rationals have a total order compatible with addition, and the product of two rationals greater than zero is greater than zero. [[math:thm-rat-ordered-field|The ordered rational field]]

[F6] Both embeddings $\mathbb N\hookrightarrow\mathbb Z\hookrightarrow\mathbb Q$ preserve order and arithmetic and identify $0$ and $1$ in these systems. The image of $\mathbb N$ is exactly the nonnegative integers in $\mathbb Z$. In $\mathbb N$, $1$ is the immediate successor of $0$, so every natural number greater than $0$ is at least $1$. [[math:lem-nat-embeds-int|Naturals as nonnegative integers]] [[math:lem-int-embeds-rat|Integers as rationals]] [[math:lem-nat-discrete|Discreteness of natural-number order]]

[F7] The cardinality $\lvert A\rvert$ of a finite set $A$ is the unique natural number $m$ for which the $m$ indices from $0$ up to but excluding $m$ can be matched one-to-one with all the elements of $A$. A bijection, meaning a one-to-one and onto map, preserves cardinality. [[math:def-finite-cardinality|Finite cardinality]]

[F8] The number of ordered tuples with one entry from each of finitely many finite sets is the product of their cardinalities. The cardinalities of two finite sets with no common elements add when the sets are united. [[math:thm-product-rule|Product rule for finite sets]] [[math:thm-sum-rule|Sum rule for disjoint finite sets]]

## Proof

**Given:** The Hurwitz order $\mathcal H$ in $B$, with its two types of coordinates and reduced norm $N$ as above.

**Goal:** Show that its units are precisely the norm-$1$ elements and that these give the stated list of $24$ distinct units.

1.1 A rational square is nonnegative because the square of a negative rational equals the square of its positive opposite. By the embeddings and discreteness in [F6], a positive integer is at least $1$ in $\mathbb Q$. If $z$ is a nonzero integer, take $t=z$ when $z>0$ and $t=-z$ when $z<0$. Then $t\ge 1$ and $z^2=t^2$. If $t>1$, the identity $t^2-1=(t-1)(t+1)$ gives $t^2>1$. Thus a nonzero integer square is at least $1$, with equality exactly for $z=1$ or $z=-1$. [F5, F6]

2.1 If $u$ is a unit with inverse $v\in\mathcal H$, then $N(u)N(v)=N(uv)=N(1)=1$. Both norms are nonnegative integers by their coordinate formula and [F2], so both are positive. The lower bound from step 1.1 forces each to equal $1$, since a factor greater than $1$ times a factor at least $1$ gives a product greater than $1$. Conversely, if $u\in\mathcal H$ and $N(u)=1$, then $\bar u\in\mathcal H$ and $u\bar u=\bar u u=1$, so $u$ is a unit. [F1, F2, F3, F4, F5, step 1.1]

2.2 If a norm-$1$ element of $\mathcal H$ has integer coordinates, it has at least one nonzero coordinate, since four zero coordinates would give norm $0$. Two nonzero coordinates would contribute at least $2$ to the norm, so there is exactly one. Its square is $1$, making that coordinate $1$ or $-1$ by step 1.1. Conversely, each such quadruple belongs to $\mathcal H$ and has norm $1$, giving exactly the elements $\pm1,\pm i,\pm j,\pm k$. [F1, F5, step 1.1]

2.3 If the four coordinates $a,b,c,d$ of $x\in\mathcal H$ are all of the form $n+\tfrac12$ with $n\in\mathbb Z$, then each doubled coordinate is an integer of the form $2n+1$. It is at least $1$ when $n\ge0$ and at most $-1$ when $n<0$, since then $-n\ge1$. If $N(x)=1$, the four doubled coordinates have squares summing to $4$. Each square is at least $1$, so all four equal $1$ and every coordinate is $\tfrac12$ or $-\tfrac12$. Conversely, each quadruple of these signs belongs to $\mathcal H$, since $\tfrac12=0+\tfrac12$ and $-\tfrac12=-1+\tfrac12$, and its norm is $4\cdot\tfrac14=1$. [F1, F5, F6, step 1.1]

3.1 By [F1] and [F4], $\mathcal H^\times$ is a group under the inherited multiplication with identity $1$. In the first list the coordinate position and sign determine distinct elements, so there are $4\cdot2=8$. In the second list distinct sign quadruples give distinct elements, so there are $2^4=16$. The lists have no common element because the first list has three zero coordinates and the second has none. The coordinate description exhausts $\mathcal H$, so the two lists exhaust its norm-$1$ elements. Step 2.1 identifies their union with the unit group, which therefore has $8+16=24$ elements, all of reduced norm $1$. [F1, F4, F7, F8, step 2.1, step 2.2, step 2.3] ∎
