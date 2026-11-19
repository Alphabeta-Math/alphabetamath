---
title: Finite binary products as avoidance indicators
status: published
research_item: lem-binary-products-and-avoidance
dependency_level: 0
---

## Prerequisites

- [math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-unordered-pair-and-singleton](https://alphabetamath.cc/item/def-unordered-pair-and-singleton)
- [math:def-indexed-union-and-intersection](https://alphabetamath.cc/item/def-indexed-union-and-intersection)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:lem-nat-add-identity](https://alphabetamath.cc/item/lem-nat-add-identity)
- [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication)
- [math:lem-nat-mult-identity](https://alphabetamath.cc/item/lem-nat-mult-identity)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)


## Statement

Let $I$ be a finite set, meaning that its elements can be listed once each in a list of natural length $|I|$, called its cardinality. Let $(b_i)_{i\in I}$ be an indexed family of binary test values in $\{0,1\}$, with $1$ denoting success. The product $\prod_{i\in I}(1-b_i)$ is the avoidance indicator. It is $1$ if every $b_i=0$ and $0$ if some $b_i=1$.

Let $X$ be another finite set and let $\big((b_{x,i})_{i\in I}\big)_{x\in X}$ be an $X$-indexed family whose rows are $I$-indexed families of values in $\{0,1\}$. For each $x$ put $P_x=\prod_{i\in I}(1-b_{x,i})$. The set $A=\{x\in X : b_{x,i}=0\text{ for every }i\in I\}$ is finite, and
$$\sum_{x\in X}P_x=|A|.$$

The sums and products are taken in the natural numbers, with empty sum $0$ and empty product $1$. For a binary value $b$, the difference $1-b$ is the unique natural $d$ satisfying $b+d=1$.

## Statement references

[math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-unordered-pair-and-singleton](https://alphabetamath.cc/item/def-unordered-pair-and-singleton)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

[math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)

## Facts & Assumptions

[F1] A finite set of cardinality $n$ has a listing indexed by the first $n$ natural numbers in which each of its elements occurs exactly once. The natural number $0$ is $\varnothing$, and the successor of $n$ is $n\cup\{n\}$, so $1=\{0\}$. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[F2] A sum or product over a finite set is the sum or product of the corresponding list of values, independent of the listing. The empty sum is $0$ and the empty product is $1$. [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

[F3] A product of a list of naturals starts at $1$ and appending one entry multiplies the previous product by that entry. When $b\le 1$, the truncated difference $1-b$ is the unique natural $d$ with $b+d=1$. The condition $b\le 1$ means that such a natural $d$ exists. [math:def-nat-finite-sum-and-product](https://alphabetamath.cc/item/def-nat-finite-sum-and-product) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[F4] Natural addition is defined by $m+0=m$ and $m+(n+1)=(m+n)+1$, where $n+1$ denotes the successor. Also $0+m=m$ for every natural $m$. [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:lem-nat-add-identity](https://alphabetamath.cc/item/lem-nat-add-identity)

[F5] For every natural $m$ we have $m\cdot0=0$ by the definition of natural multiplication and $m\cdot1=m$ by the right identity law. [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication) [math:lem-nat-mult-identity](https://alphabetamath.cc/item/lem-nat-mult-identity)

[F6] Induction proves a property for all natural numbers from its case at $0$ and the implication from each $n$ to its successor. [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F7] For a finite set $X$ and finite sets $A_x$ for $x\in X$ that are pairwise disjoint, meaning no element belongs to both $A_x$ and $A_y$ for distinct $x,y\in X$, their union is finite and its cardinality is $\sum_{x\in X}|A_x|$. [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)

[F8] An indexed family with index set $I$ is a function with domain $I$. The subscript specifies its value at that index. [math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)

[F9] The singleton $\{x\}$ has $x$ as its only element. [math:def-unordered-pair-and-singleton](https://alphabetamath.cc/item/def-unordered-pair-and-singleton)

[F10] An element belongs to the indexed union $\bigcup_{x\in X}A_x$ exactly when it belongs to $A_x$ for some $x\in X$. [math:def-indexed-union-and-intersection](https://alphabetamath.cc/item/def-indexed-union-and-intersection)

[F11] Separation inside $X$ defines the subset consisting of exactly the elements of $X$ that satisfy the given condition. [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

## Proof

**Given:** Finite sets $I$ and $X$ and the binary test values in the statement.

**Goal:** Evaluate the single product and show that the sum of the products equals the number of indices with no successful test.

1.1 If $b=0$, then $b+1=1$, so the unique difference $1-b$ equals $1$. If $b=1$, then $b+0=1$, so the unique difference equals $0$. This gives existence and the required value of the difference in both cases. [F3, F4]

1.2 A list of length $0$ has no successful test, and the product equals $1$ by the empty product clause. [base, F3]

1.3 Fix a natural number $n$ and assume that for every list of $n$ binary values the product of their differences from $1$ is $1$ if all the values are $0$ and $0$ if at least one is $1$. [ih]

2.1 For a list of length $n+1$, the first $n$ entries form a list of length $n$. The product for the full list is the product for those first $n$ entries multiplied by the difference from $1$ of the last entry. If the last test value is $1$, this multiplies by $0$ and gives $0$. If the last test value is $0$, this multiplies by $1$ and leaves the first product unchanged, and the full list has a successful test exactly when the first $n$ entries do. This proves the rule for length $n+1$. [F1, F3, F5, step 1.1, step 1.3]

3.1 By induction the rule holds for all finite lists. A listing of $I$ contains each index exactly once, so the indexed family gives exactly one entry at each position, and a successful test in that list means a successful test at some $i\in I$. The definition of the finite-set product therefore gives the claimed rule on $I$. [F1, F2, F6, F8, step 1.2, step 2.1]

4.1 For each $x\in X$, apply the rule on $I$ to the row $(b_{x,i})_{i\in I}$. The products form an $X$-indexed family with $P_x=1$ for $x\in A$ and $P_x=0$ for $x\in X$ with $x\notin A$. Define a family $(A_x)_{x\in X}$ by setting $A_x=\{x\}$ if $P_x=1$ and $A_x=\varnothing$ if $P_x=0$. The two cases assign exactly one set to each $x$. The singleton has the one-entry listing with entry $x$, and the empty set has the empty listing, so $|A_x|=P_x$ in either case. [given, F1, F8, F9, F11, step 3.1]

5.1 Any element of $A_x$ must equal $x$, so sets with distinct indices have no common element. An element $z$ belongs to $\bigcup_{x\in X}A_x$ exactly when it equals some $x\in X$ with $P_x=1$. By step 4.1 and the membership condition for $A$, this is equivalent to $z\in A$. Thus the union is $A$. The finite disjoint union rule makes $A$ finite and gives $|A|=\sum_{x\in X}|A_x|=\sum_{x\in X}P_x$. [F2, F7, F9, F10, F11, step 4.1]

6.1 The product rule of step 3.1 and the count of step 5.1 give both conclusions, including the empty index sets covered by the same product and sum conventions. [F2, step 3.1, step 5.1, discharge-induction] ∎
