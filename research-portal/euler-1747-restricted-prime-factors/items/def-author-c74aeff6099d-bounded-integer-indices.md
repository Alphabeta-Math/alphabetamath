---
id: def-author-c74aeff6099d-bounded-integer-indices
kind: definition
title: Bounded integer index sets
status: published
domain: mathematics
deps:
  - math:def-nat-order
  - math:def-integers
  - math:def-int-order
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:lem-nat-order-is-membership
  - math:def-int-operations
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:thm-int-ordered-ring
  - math:def-nat-addition
formulation_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:def-int-operations
  - math:def-natural-numbers
  - math:def-function
  - math:def-injection-surjection-bijection
argument_deps:
  - math:def-nat-order
  - math:def-subset-and-proper-subset
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:lem-nat-order-is-membership
  - math:def-finite-cardinality
  - math:def-int-operations
  - math:def-int-order
  - math:thm-int-ordered-ring
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:def-nat-addition
dependency_roles:
  math:def-nat-order: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-function: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-nat-addition: mathematical-premise
provenance:
  statement: ai-generated
  proof: not-applicable
dependency_level: 0
---

## Definition

Write $\mathbb Z$ for the integers and $0$ for their zero element. For a nonnegative integer $B$, meaning $0\le B$, let $I_B=\{m\in\mathbb Z:0\le m\le B\}$. Thus $I_B$ contains exactly the integers from $0$ through $B$, including both endpoints.

The set $I_B$ is finite, meaning that for some natural number $n$ there is a bijection $n\to I_B$. A list of length $n$ with entries in $I_B$ is a function from the von Neumann natural number $n$ to $I_B$, so this bijection lists each member exactly once.

## Definition references

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-subset-and-proper-subset]]

[[math:def-finite-cardinality]]

[[math:def-int-operations]]

[[math:def-natural-numbers]]

[[math:def-function]]

[[math:def-injection-surjection-bijection]]

## Justification

Integer zero is $[(0,0)]$ ([[math:def-int-operations|Arithmetic on the integers]]). The integer comparison is independent of representatives and reflexive ([[math:def-int-order|Order on the integers]], [[math:thm-int-ordered-ring|Total order on the integers]]). Separation gives a unique subset of $\mathbb Z$ with membership condition $0\le m\le B$ ([[math:def-subset-and-proper-subset|Subset by a membership condition]]). Since $0\le B$ by hypothesis and reflexivity gives $0\le 0$ and $B\le B$, both $0$ and $B$ satisfy that condition.

Let $\iota:\mathbb N\to\mathbb Z$ be the natural-number embedding, where $\iota(t)=[(t,0)]$. It is injective, its image is the set of nonnegative integers, and $s\le t$ holds in $\mathbb N$ exactly when $\iota(s)\le\iota(t)$ ([[math:lem-nat-embeds-int|Natural numbers in the integers]], Statement and step 1.4). There is therefore a unique $b\in\mathbb N$ with $B=\iota(b)$. The von Neumann successor $\sigma(b)=b\cup\{b\}$ is a natural number whose elements are precisely the natural numbers $t$ with $t\le b$ ([[math:def-natural-numbers|Natural numbers]], [[math:lem-nat-order-is-membership|Natural order and membership]]).

For every $t\in\sigma(b)$, the value $\iota(t)$ is nonnegative and satisfies $\iota(t)\le\iota(b)=B$. Separating from the graph of $\iota$ the pairs whose first coordinate belongs to $\sigma(b)$ therefore gives a function $e:\sigma(b)\to I_B$ with $e(t)=\iota(t)$ ([[math:def-subset-and-proper-subset|Separation]], [[math:def-function|Functions]]). Its injectivity follows from that of $\iota$. For any $m\in I_B$, nonnegativity gives a unique $t\in\mathbb N$ with $m=\iota(t)$. Since $m\le B$, order reflection gives $t\le b$, so $t\in\sigma(b)$ and $e(t)=m$. Thus $e$ is also surjective and hence a bijection ([[math:def-injection-surjection-bijection|Bijections]]). For $s,t\in\sigma(b)$ with $s<t$ in $\mathbb N$, the natural strict order gives $s\le t$ and $s\ne t$. Order preservation and injectivity of $\iota$ give $e(s)\le e(t)$ and $e(s)\ne e(t)$, so $e(s)<e(t)$ by the definition of strict integer order ([[math:def-nat-order|Natural order]], [[math:lem-nat-embeds-int|Natural numbers in the integers]], [[math:def-int-order|Integer order]]). Since the natural number $\sigma(b)$ is finite, finiteness transfers to $I_B$ along this bijection ([[math:def-finite-cardinality|Finite cardinality]], parts (a) and (c)).

The increasing list has length $\sigma(b)=b+1$ in $\mathbb N$, because $1=\sigma(0)$ and the addition rule gives $b+1=\sigma(b+0)=\sigma(b)$ ([[math:def-natural-numbers|Natural numbers]], [[math:def-nat-addition|Addition on the naturals]]). The integer copy of this length is $B+1$, since $\iota$ preserves addition and sends the natural $1$ to the integer $1$ ([[math:lem-nat-embeds-int|Natural numbers in the integers]], [[math:def-int-operations|Integer arithmetic]]).
