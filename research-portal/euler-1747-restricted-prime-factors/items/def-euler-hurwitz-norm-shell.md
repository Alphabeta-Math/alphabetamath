---
id: def-euler-hurwitz-norm-shell
kind: definition
title: The Hurwitz norm shell
status: published
domain: mathematics
deps:
  - def-euler-hurwitz-order
  - def-euler-hamilton-quaternions
  - math:def-integers
  - math:def-int-order
  - math:lem-int-embeds-rat
  - math:def-axiom-schema-of-separation
  - math:def-axiom-of-extensionality
  - math:def-subset-and-proper-subset
formulation_deps:
  - def-euler-hurwitz-order
  - def-euler-hamilton-quaternions
  - math:def-integers
  - math:def-int-order
  - math:lem-int-embeds-rat
  - math:def-subset-and-proper-subset
argument_deps:
  - def-euler-hurwitz-order
  - def-euler-hamilton-quaternions
  - math:lem-int-embeds-rat
  - math:def-axiom-schema-of-separation
  - math:def-axiom-of-extensionality
  - math:def-subset-and-proper-subset
dependency_roles:
  def-euler-hurwitz-order: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:def-axiom-schema-of-separation: mathematical-premise
  math:def-axiom-of-extensionality: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §3.1, definition of the norm shell preceding (3.2)
dependency_level: 3
---

## Definition

Let $m$ be a positive integer, meaning $m\in\mathbb Z$ and $0<m$. Identify $m$ with the rational number $m/1$ when comparing it with a reduced norm.

Write each rational Hamilton quaternion as $\alpha=a+bi+cj+dk$, with unique rational coordinates $(a,b,c,d)$ in the basis $1,i,j,k$. The **Hurwitz order** $\mathcal H$ consists of these quaternions whose coordinates are either all integers or all of the form $n+\tfrac12$ with $n\in\mathbb Z$. The **reduced norm** is $\operatorname{nrd}(\alpha)=a^2+b^2+c^2+d^2$.

The **Hurwitz norm shell of norm $m$** is the set of elements of $\mathcal H$ whose reduced norm equals $m$.
$$Q_m=\{\alpha\in\mathcal H:\operatorname{nrd}(\alpha)=m\}.$$

## Definition references

[[math:def-integers|The integers]]

[[math:def-int-order|Order and positivity in the integers]]

[[math:lem-int-embeds-rat|The embedding of the integers into the rationals]]

[[def-euler-hamilton-quaternions|Rational quaternion coordinates and reduced norm]]

[[def-euler-hurwitz-order|The Hurwitz order]]

[[math:def-subset-and-proper-subset|Subsets and separation notation]]

## Facts & Assumptions

[F1] The Hurwitz order is an existing subset of the rational Hamilton quaternion algebra with the coordinate membership rule given above. [[def-euler-hurwitz-order|The Hurwitz order]]

[F2] In that algebra every element has a unique rational coordinate tuple, and its reduced norm is the rational number given by the sum of the four coordinate squares. [[def-euler-hamilton-quaternions|Rational quaternion coordinates and reduced norm]]

[F3] The integer embedding $n\mapsto n/1$ represents distinct integers by distinct rational numbers. [[math:lem-int-embeds-rat|The embedding of the integers into the rationals]]

[F4] Separation gives a subset of an existing set containing exactly the elements that satisfy a given condition with fixed parameters. [[math:def-axiom-schema-of-separation|The Axiom Schema of Separation]]

[F5] Extensionality says that two sets having the same elements are equal. [[math:def-axiom-of-extensionality|The Axiom of Extensionality]]

[F6] A set is a subset of an ambient set if every element of the set belongs to the ambient set. [[math:def-subset-and-proper-subset|The definition of a subset]]

## Justification

The norm equality is a condition on each element of the Hurwitz order, so it specifies a unique subset by Separation and Extensionality.

## Proof

**Given:** A positive integer $m$ and the Hurwitz order $\mathcal H$.

**Goal:** Show that there is exactly one subset of $\mathcal H$ with the defining membership rule for $Q_m$.

1.1 Each $\alpha\in\mathcal H$ belongs to the rational Hamilton quaternion algebra and has a unique rational reduced norm. The image $m/1$ is a fixed rational number, so the comparison $\operatorname{nrd}(\alpha)=m/1$ is determined for every $\alpha\in\mathcal H$. [F1, F2, F3]

2.1 Apply Separation to $\mathcal H$ with the condition in step 1.1. This gives a set whose elements are exactly the $\alpha\in\mathcal H$ with $\operatorname{nrd}(\alpha)=m/1$. Every element of this set belongs to $\mathcal H$, so the set is a subset of $\mathcal H$. [F1, F4, F6, step 1.1]

3.1 Any two sets satisfying this membership rule have the same elements, so Extensionality makes them equal. Thus $Q_m$ exists and is uniquely defined for every positive integer $m$. [F5, step 2.1] ∎
