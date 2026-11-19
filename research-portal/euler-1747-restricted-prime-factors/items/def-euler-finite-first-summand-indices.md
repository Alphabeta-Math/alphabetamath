---
id: def-euler-finite-first-summand-indices
kind: definition
title: Eligible first-summand indices
status: draft
domain: mathematics
deps:
  - def-author-c74aeff6099d-bounded-integer-indices
  - def-euler-finite-certificate-indices
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:thm-int-ordered-ring
  - math:thm-subset-of-a-finite-set
formulation_deps:
  - def-author-c74aeff6099d-bounded-integer-indices
  - def-euler-finite-certificate-indices
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
argument_deps:
  - def-author-c74aeff6099d-bounded-integer-indices
  - def-euler-finite-certificate-indices
  - math:def-int-operations
  - math:def-subset-and-proper-subset
  - math:thm-int-ordered-ring
  - math:thm-subset-of-a-finite-set
dependency_roles:
  def-author-c74aeff6099d-bounded-integer-indices: mathematical-premise
  def-euler-finite-certificate-indices: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, definition of J after Lemma 7.1
dependency_level: 3
---

## Definition

For a nonnegative integer $B$, let $I_B$ be the set of integers from $0$ through $B$, including both endpoints. Use the finite-range cutoff $H=4{,}194{,}303$ and its indicators $\varepsilon_i\in\{0,1\}$ defined for $i\in I_H$.

The set of eligible first-summand indices is
$$J=\{i\in I_{78}:\varepsilon_i=1\}.$$
The associated possible first summands are the integers in $\{4i+1:i\in J\}$, with one possible value $4i+1$ at each eligible index. Both sets are finite, meaning that their elements can each be listed once in a list of natural-number length.

## Definition references

[[def-author-c74aeff6099d-bounded-integer-indices]]

[[def-euler-finite-certificate-indices]]

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-subset-and-proper-subset]]

[[math:def-finite-cardinality]]

## Justification

Since $78$ is nonnegative and $78\le H$, the bounded integer index set $I_{78}$ is finite and every index in it belongs to $I_H$. Hence the indicator assigns exactly one value, either $0$ or $1$, to each $i\in I_{78}$ ([[def-author-c74aeff6099d-bounded-integer-indices|Bounded integer index sets]], [[def-euler-finite-certificate-indices|Finite-range indicators]], [[math:thm-int-ordered-ring|Integer order]]). Taking exactly the members with value $1$ defines a unique subset $J$ of $I_{78}$. That subset is finite because $I_{78}$ is finite ([[math:def-subset-and-proper-subset|Subset by a membership condition]], [[math:thm-subset-of-a-finite-set|Finiteness of a subset]]).

Integer multiplication and addition give exactly one value $4i+1$ at each $i\in J$. In fact, $0\le i\le78$ gives $1\le4i+1\le4\cdot78+1=313$ by multiplication by the positive integer $4$ and addition of $1$ ([[math:def-int-operations|Integer arithmetic]], [[math:thm-int-ordered-ring|Ordered integer arithmetic]]). Thus the associated values form the unique subset of the finite set $I_{313}$ consisting of those $s$ for which $s=4i+1$ for some $i\in J$. This subset is also finite ([[def-author-c74aeff6099d-bounded-integer-indices|Bounded integer index sets]], [[math:def-subset-and-proper-subset|Subset by a membership condition]], [[math:thm-subset-of-a-finite-set|Finiteness of a subset]]).
