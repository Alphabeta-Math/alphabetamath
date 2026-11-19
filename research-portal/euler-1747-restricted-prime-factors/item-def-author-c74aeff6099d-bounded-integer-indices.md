---
title: Bounded integer index sets
status: draft
research_item: def-author-c74aeff6099d-bounded-integer-indices
dependency_level: 0
---

## Prerequisites

- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)


## Definition

Write $\mathbb Z$ for the integers and $0$ for their zero element. For a nonnegative integer $B$, meaning $0\le B$, let $I_B=\{m\in\mathbb Z:0\le m\le B\}$. Thus $I_B$ contains exactly the integers from $0$ through $B$, including both endpoints.

The set $I_B$ is finite, meaning that for some natural number $n$ there is a bijection $n\to I_B$. A list of length $n$ with entries in $I_B$ is a function from the von Neumann natural number $n$ to $I_B$, so this bijection lists each member exactly once.

## Definition references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-function](https://alphabetamath.cc/item/def-function)

[math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)

## Justification

Integer zero is $[(0,0)]$ ([Arithmetic on the integers](https://alphabetamath.cc/item/def-int-operations)). The integer comparison is independent of representatives and reflexive ([Order on the integers](https://alphabetamath.cc/item/def-int-order), [Total order on the integers](https://alphabetamath.cc/item/thm-int-ordered-ring)). Separation gives a unique subset of $\mathbb Z$ with membership condition $0\le m\le B$ ([Subset by a membership condition](https://alphabetamath.cc/item/def-subset-and-proper-subset)). Since $0\le B$ by hypothesis and reflexivity gives $0\le 0$ and $B\le B$, both $0$ and $B$ satisfy that condition.

Let $\iota:\mathbb N\to\mathbb Z$ be the natural-number embedding, where $\iota(t)=[(t,0)]$. It is injective, its image is the set of nonnegative integers, and $s\le t$ holds in $\mathbb N$ exactly when $\iota(s)\le\iota(t)$ ([Natural numbers in the integers](https://alphabetamath.cc/item/lem-nat-embeds-int), Statement and step 1.4). There is therefore a unique $b\in\mathbb N$ with $B=\iota(b)$. The von Neumann successor $\sigma(b)=b\cup\{b\}$ is a natural number whose elements are precisely the natural numbers $t$ with $t\le b$ ([Natural numbers](https://alphabetamath.cc/item/def-natural-numbers), [Natural order and membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)).

For every $t\in\sigma(b)$, the value $\iota(t)$ is nonnegative and satisfies $\iota(t)\le\iota(b)=B$. Separating from the graph of $\iota$ the pairs whose first coordinate belongs to $\sigma(b)$ therefore gives a function $e:\sigma(b)\to I_B$ with $e(t)=\iota(t)$ ([Separation](https://alphabetamath.cc/item/def-subset-and-proper-subset), [Functions](https://alphabetamath.cc/item/def-function)). Its injectivity follows from that of $\iota$. For any $m\in I_B$, nonnegativity gives a unique $t\in\mathbb N$ with $m=\iota(t)$. Since $m\le B$, order reflection gives $t\le b$, so $t\in\sigma(b)$ and $e(t)=m$. Thus $e$ is also surjective and hence a bijection ([Bijections](https://alphabetamath.cc/item/def-injection-surjection-bijection)). For $s,t\in\sigma(b)$ with $s<t$ in $\mathbb N$, the natural strict order gives $s\le t$ and $s\ne t$. Order preservation and injectivity of $\iota$ give $e(s)\le e(t)$ and $e(s)\ne e(t)$, so $e(s)<e(t)$ by the definition of strict integer order ([Natural order](https://alphabetamath.cc/item/def-nat-order), [Natural numbers in the integers](https://alphabetamath.cc/item/lem-nat-embeds-int), [Integer order](https://alphabetamath.cc/item/def-int-order)). Since the natural number $\sigma(b)$ is finite, finiteness transfers to $I_B$ along this bijection ([Finite cardinality](https://alphabetamath.cc/item/def-finite-cardinality), parts (a) and (c)).

The increasing list has length $\sigma(b)=b+1$ in $\mathbb N$, because $1=\sigma(0)$ and the addition rule gives $b+1=\sigma(b+0)=\sigma(b)$ ([Natural numbers](https://alphabetamath.cc/item/def-natural-numbers), [Addition on the naturals](https://alphabetamath.cc/item/def-nat-addition)). The integer copy of this length is $B+1$, since $\iota$ preserves addition and sends the natural $1$ to the integer $1$ ([Natural numbers in the integers](https://alphabetamath.cc/item/lem-nat-embeds-int), [Integer arithmetic](https://alphabetamath.cc/item/def-int-operations)).
