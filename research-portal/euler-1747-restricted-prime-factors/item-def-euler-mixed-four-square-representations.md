---
title: Mixed-parity four-square representations
status: draft
research_item: def-euler-mixed-four-square-representations
dependency_level: 1
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §2, definition of the mixed set preceding (2.2)
---

PDF p. 2: ` §2, definition of the mixed set preceding (2.2) `

## Prerequisites

- [def-euler-four-square-representations](item-def-euler-four-square-representations)
- [lem-square-residue-parity](item-lem-square-residue-parity)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)


## Definition

Let $n$ be a positive integer, meaning $n\in\mathbb Z$ and $0<n$, where $\mathbb Z$ is the set of integers. A four-square representation of $n$ is an ordered quadruple $(x_1,x_2,x_3,x_4)$ of integers with $x_1^2+x_2^2+x_3^2+x_4^2=n$, where $x_i^2=x_i\cdot x_i$. The set of these representations is $\mathcal R(n)$. Each coordinate may be positive, zero, or negative, and equality of representations means equality in each of the four positions.

An integer $t$ is even if $t=2k$ for some integer $k$, and odd if $t=2k+1$ for some integer $k$. Two integers have opposite parity when one is even and the other is odd.

Define $\mathcal R_{\mathrm{mix}}(n)$ to be the subset of $\mathcal R(n)$ consisting of the quadruples for which $x_1$ and $x_2$ have opposite parity and $x_3$ and $x_4$ have opposite parity. Such a quadruple is a mixed-parity four-square representation. The notation $|\mathcal R_{\mathrm{mix}}(n)|$ denotes the number of elements of this set.

## Definition references

[def-euler-four-square-representations](item-def-euler-four-square-representations)

[lem-square-residue-parity](item-lem-square-residue-parity)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

## Facts & Assumptions

[F1] For each positive integer $n$, the set $\mathcal R(n)$ of signed, ordered four-square representations exists and is finite. [def-euler-four-square-representations](item-def-euler-four-square-representations)

[F2] Every integer is either even or odd, with these two conditions mutually exclusive. [lem-square-residue-parity](item-lem-square-residue-parity)

[F3] A fixed membership condition on the elements of a given set selects a unique subset consisting exactly of the elements that satisfy it. [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[F4] Every subset of a finite set is finite. [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)

[F5] A finite set has a unique cardinality, which is its number of elements. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

## Justification

**Given:** A positive integer $n$.

**Goal:** Show that the mixed-parity condition selects a unique set and that its count is defined.

1.1 For each quadruple in $\mathcal R(n)$, the parity of each coordinate is uniquely determined. For each of the two specified pairs, the test is whether its two parities differ. Requiring both tests to hold therefore selects a unique subset $\mathcal R_{\mathrm{mix}}(n)$ of $\mathcal R(n)$. [given, F1, F2, F3]

2.1 The set $\mathcal R(n)$ is finite, and the subset obtained in Step 1.1 is therefore finite as well. Its cardinality is unique, so $|\mathcal R_{\mathrm{mix}}(n)|$ is defined. [F1, F4, F5, step 1.1] ∎
