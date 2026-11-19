---
id: def-euler-four-square-representations
kind: definition
title: Signed ordered four-square representations
status: published
domain: mathematics
deps:
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-cartesian-product
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:thm-int-ordered-ring
  - math:lem-nat-embeds-int
  - math:lem-nat-order-is-membership
  - math:def-injection-surjection-bijection
  - math:thm-product-rule
  - math:thm-subset-of-a-finite-set
  - math:def-natural-numbers
  - math:def-nat-order
  - math:def-function
formulation_deps:
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-cartesian-product
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
argument_deps:
  - math:def-integers
  - math:def-int-operations
  - math:def-int-order
  - math:def-cartesian-product
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:thm-int-ordered-ring
  - math:lem-nat-embeds-int
  - math:lem-nat-order-is-membership
  - math:def-injection-surjection-bijection
  - math:thm-product-rule
  - math:thm-subset-of-a-finite-set
  - math:def-natural-numbers
  - math:def-nat-order
  - math:def-function
dependency_roles:
  math:def-integers: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:thm-product-rule: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:def-function: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §2, definition preceding (2.1) and notation in (2.1)
dependency_level: 0
---

## Definition

Let $n$ be a positive integer, meaning $n\in\mathbb Z$ and $0<n$ in the integer order. Write $\mathbb Z^4=(\mathbb Z\times\mathbb Z)\times(\mathbb Z\times\mathbb Z)$, where $A\times B$ is the set of pairs with first entry in $A$ and second entry in $B$. Write $((x_1,x_2),(x_3,x_4))$ as $(x_1,x_2,x_3,x_4)$ and call its entries coordinates. With $x^2=x\cdot x$, define

$$\mathcal R(n)=\{(x_1,x_2,x_3,x_4)\in\mathbb Z^4:x_1^2+x_2^2+x_3^2+x_4^2=n\}.$$

A signed, ordered representation of $n$ by four squares is an element of $\mathcal R(n)$. Each coordinate may be positive, zero, or negative. Two representations are equal exactly when the entries agree in all four positions. Define $R(n)=|\mathcal R(n)|$, the number of elements of this set.

## Definition references

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-cartesian-product]]

[[math:thm-the-characterising-property-of-ordered-pairs]]

[[math:def-subset-and-proper-subset]]

[[math:def-finite-cardinality]]

## Facts & Assumptions

**Given:** A positive integer $n$.

[F1] The integers are classes representing differences of natural numbers. Integer addition, multiplication and negation are well defined. Any two integers can be compared, adding the same integer on both sides preserves their order, and the product of positive integers is positive. Integer addition and multiplication are associative and commutative, multiplication distributes over addition, and each integer has an additive inverse. [[math:def-integers]] [[math:def-int-operations]] [[math:def-int-order]] [[math:thm-int-ordered-ring]]

[F2] The Cartesian product of two sets exists and consists of the ordered pairs with one entry from each factor in the specified order. Two ordered pairs are equal exactly when their first entries agree and their second entries agree. [[math:def-cartesian-product]] [[math:thm-the-characterising-property-of-ordered-pairs]]

[F3] Selecting the elements of a given set that satisfy a fixed condition defines a unique subset. [[math:def-subset-and-proper-subset]]

[F4] Let $\mathbb N=\omega$ be the von Neumann natural numbers, with $0=\varnothing$ and $1=\{0\}$. Comparisons in $\mathbb N$ use the additive order. The map $\iota(j)=[(j,0)]$ identifies the natural numbers with the nonnegative integers, preserving and reflecting order. For $k\in\mathbb N$, the elements of $k$ are exactly the natural numbers $j<k$. Since $0\in1$, we have $0<1$ in $\mathbb N$, and $\iota(0)=0$ and $\iota(1)=1$ give $0<1$ in $\mathbb Z$. [[math:def-natural-numbers]] [[math:def-nat-order]] [[math:lem-nat-embeds-int]] [[math:lem-nat-order-is-membership]] [[math:def-int-operations]]

[F5] A subset $f$ of $A\times C$ is the graph of a function $A\to C$ when each $a\in A$ occurs with exactly one $c\in C$. A function $A\to C$ is bijective when each $c\in C$ has exactly one preimage in $A$. A set is finite if it admits a bijection to a von Neumann natural number $k\in\mathbb N$, viewed as the set of its predecessors. The unique such $k$ is its cardinality. [[math:def-function]] [[math:def-injection-surjection-bijection]] [[math:def-natural-numbers]] [[math:lem-nat-order-is-membership]] [[math:def-finite-cardinality]]

[F6] The Cartesian product of two finite sets is finite. [[math:thm-product-rule]]

[F7] Every subset of a finite set is finite. [[math:thm-subset-of-a-finite-set]]

## Justification

**Goal:** Show that the defining equation selects a unique set of tuples and that its count is a uniquely defined natural number.

1.1 The iterated Cartesian product exists, and equality of its pairs of pairs is equality in all four positions. Integer multiplication and addition give one integer sum of squares for each tuple, so selecting the tuples whose sum equals $n$ defines a unique set $\mathcal R(n)$. [F1, F2, F3, given]

1.2 Every integer square is nonnegative. It is zero for $x=0$, positive for $x>0$, and equal to $(-x)^2>0$ for $x<0$. In a tuple in $\mathcal R(n)$, each $x_i^2$ is at most $n$ because the other three squares are nonnegative. Put $u=n+1$. Then $u>n$ and $u>1$. If $x_i\ge u$ or $x_i\le -u$, let $t=x_i$ in the first case and $t=-x_i$ in the second. Then $t\ge u>1$, so $t^2-t=t(t-1)>0$ and $x_i^2=t^2>t\ge u>n$, a contradiction. Thus every coordinate satisfies $-u<x_i<u$. [F1, F4, given]

2.1 Let $B=\{a\in\mathbb Z:-u\le a<u\}$. Choose the natural number $k$ with $\iota(k)=u+u$, which exists since $u>1>0$. Translation by $u$ carries the bounds on $a$ to $0\le a+u<u+u$. By the embedding and the additive order on $\mathbb N$, each $a\in B$ has exactly one $j\in\mathbb N$ with $\iota(j)=a+u$, and that $j$ satisfies $j<k$. The initial-segment identity then gives $j\in k$. Form the set $G=\{(a,j)\in B\times k:\iota(j)=a+u\}$ by separation. Each $a\in B$ occurs with exactly one $j\in k$, so $G$ is the graph of a function $B\to k$. For each $j\in k$, the integer $a=\iota(j)-u$ lies in $B$ by the same translated bounds and is the only solution of $\iota(j)=a+u$. Thus each $j\in k$ has exactly one preimage in $B$, so the function is a bijection and $B$ is finite. [F1, F2, F3, F4, F5, step 1.2]

3.1 Two applications of the product rule, first to $B\times B$ and then to its product with itself, show that $(B\times B)\times(B\times B)$ is finite. Every tuple in $\mathcal R(n)$ lies in this finite set by the coordinate bounds, so $\mathcal R(n)$ is finite. Its cardinality $R(n)$ is consequently a uniquely defined element of $\mathbb N$. [F2, F5, F6, F7, step 1.1, step 1.2, step 2.1] ∎
