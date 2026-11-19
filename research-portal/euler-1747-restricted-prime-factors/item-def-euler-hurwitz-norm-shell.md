---
title: The Hurwitz norm shell
status: draft
research_item: def-euler-hurwitz-norm-shell
dependency_level: 3
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §3.1, definition of the norm shell preceding (3.2)
---

PDF p. 2: ` §3.1, definition of the norm shell preceding (3.2) `

## Prerequisites

- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)
- [math:def-axiom-of-extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)


## Definition

Let $m$ be a positive integer, meaning $m\in\mathbb Z$ and $0<m$. Identify $m$ with the rational number $m/1$ when comparing it with a reduced norm.

Write each rational Hamilton quaternion as $\alpha=a+bi+cj+dk$, with unique rational coordinates $(a,b,c,d)$ in the basis $1,i,j,k$. The **Hurwitz order** $\mathcal H$ consists of these quaternions whose coordinates are either all integers or all of the form $n+\tfrac12$ with $n\in\mathbb Z$. The **reduced norm** is $\operatorname{nrd}(\alpha)=a^2+b^2+c^2+d^2$.

The **Hurwitz norm shell of norm $m$** is the set of elements of $\mathcal H$ whose reduced norm equals $m$.
$$Q_m=\{\alpha\in\mathcal H:\operatorname{nrd}(\alpha)=m\}.$$

## Definition references

[The integers](https://alphabetamath.cc/item/def-integers)

[Order and positivity in the integers](https://alphabetamath.cc/item/def-int-order)

[The embedding of the integers into the rationals](https://alphabetamath.cc/item/lem-int-embeds-rat)

[Rational quaternion coordinates and reduced norm](item-def-euler-hamilton-quaternions)

[The Hurwitz order](item-def-euler-hurwitz-order)

[Subsets and separation notation](https://alphabetamath.cc/item/def-subset-and-proper-subset)

## Facts & Assumptions

[F1] The Hurwitz order is an existing subset of the rational Hamilton quaternion algebra with the coordinate membership rule given above. [The Hurwitz order](item-def-euler-hurwitz-order)

[F2] In that algebra every element has a unique rational coordinate tuple, and its reduced norm is the rational number given by the sum of the four coordinate squares. [Rational quaternion coordinates and reduced norm](item-def-euler-hamilton-quaternions)

[F3] The integer embedding $n\mapsto n/1$ represents distinct integers by distinct rational numbers. [The embedding of the integers into the rationals](https://alphabetamath.cc/item/lem-int-embeds-rat)

[F4] Separation gives a subset of an existing set containing exactly the elements that satisfy a given condition with fixed parameters. [The Axiom Schema of Separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)

[F5] Extensionality says that two sets having the same elements are equal. [The Axiom of Extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)

[F6] A set is a subset of an ambient set if every element of the set belongs to the ambient set. [The definition of a subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

## Justification

The norm equality is a condition on each element of the Hurwitz order, so it specifies a unique subset by Separation and Extensionality.

## Proof

**Given:** A positive integer $m$ and the Hurwitz order $\mathcal H$.

**Goal:** Show that there is exactly one subset of $\mathcal H$ with the defining membership rule for $Q_m$.

1.1 Each $\alpha\in\mathcal H$ belongs to the rational Hamilton quaternion algebra and has a unique rational reduced norm. The image $m/1$ is a fixed rational number, so the comparison $\operatorname{nrd}(\alpha)=m/1$ is determined for every $\alpha\in\mathcal H$. [F1, F2, F3]

2.1 Apply Separation to $\mathcal H$ with the condition in step 1.1. This gives a set whose elements are exactly the $\alpha\in\mathcal H$ with $\operatorname{nrd}(\alpha)=m/1$. Every element of this set belongs to $\mathcal H$, so the set is a subset of $\mathcal H$. [F1, F4, F6, step 1.1]

3.1 Any two sets satisfying this membership rule have the same elements, so Extensionality makes them equal. Thus $Q_m$ exists and is uniquely defined for every positive integer $m$. [F5, step 2.1] ∎
