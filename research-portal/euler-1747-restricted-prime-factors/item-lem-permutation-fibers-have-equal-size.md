---
title: Equal coordinate-label fibers under permutation
status: draft
research_item: lem-permutation-fibers-have-equal-size
dependency_level: 0
---

## Prerequisites

- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:def-symmetric-group](https://alphabetamath.cc/item/def-symmetric-group)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)
- [math:lem-nat-add-cancellative](https://alphabetamath.cc/item/lem-nat-add-cancellative)
- [math:lem-unions-and-intersections-of-small-families](https://alphabetamath.cc/item/lem-unions-and-intersections-of-small-families)
- [math:def-axiom-of-extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)
- [math:thm-a-function-is-a-bijection-exactly-when-it-has-a-two-sided-inverse](https://alphabetamath.cc/item/thm-a-function-is-a-bijection-exactly-when-it-has-a-two-sided-inverse)


## Statement

Let $I$ be a finite set of coordinate positions. An integer tuple on $I$ is a function $x:I\to\mathbb Z$, where $\mathbb Z$ is the set of integers and $x_i=x(i)$ is the entry at position $i$. A permutation $\pi$ of $I$ is a bijection $I\to I$, meaning every position $j$ has a unique preimage $\pi^{-1}(j)$ with $\pi(\pi^{-1}(j))=j$. Reindexing $x$ by $\pi$ puts the entry $x_{\pi^{-1}(j)}$ at position $j$.

Let $S$ be a finite set of integer tuples on $I$ that is closed under coordinate permutations, meaning that every such reindexing of an element of $S$ belongs to $S$. An integer $a$ is odd if $a=(k+k)+1$ for some $k\in\mathbb Z$. For a subset $D\subseteq I$, let the fiber $F_D$ be the set of tuples $x\in S$ for which $x_i$ is odd exactly at the positions $i\in D$. For all subsets $A,B\subseteq I$ with the same number of elements, the fibers $F_A$ and $F_B$ have equal cardinality.

## Facts & Assumptions

[F1] The [definition of a function](https://alphabetamath.cc/item/def-function) specifies exactly one output in the target set for each input in the domain. Such a function can be specified by its graph, the set of ordered pairs of inputs and their outputs in the [Cartesian product](https://alphabetamath.cc/item/def-cartesian-product) of the two sets.

[F2] A [bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) is a function for which each target element has exactly one preimage. For a bijection, the inverse value at a target element is its unique preimage. A [permutation of a set](https://alphabetamath.cc/item/def-symmetric-group) is a bijection from that set to itself.

[F3] The notation $\mathbb Z$ denotes the [set of integers](https://alphabetamath.cc/item/def-integers). The addition and the constant $1$ in the oddness condition are those of [integer arithmetic](https://alphabetamath.cc/item/def-int-operations).

[F4] A [subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) contains only elements of the given set. Selecting the elements of a set that satisfy a specified condition defines a unique subset.

[F5] A set $X$ is finite if it admits a bijection to some natural number considered as the set of its predecessors. The unique such number is the [finite cardinality](https://alphabetamath.cc/item/def-finite-cardinality) $\lvert X\rvert$. Parts (c) and (d) give transport of finite cardinality along a bijection and existence of a bijection between finite sets of equal cardinality.

[F6] A [subset of a finite set is finite](https://alphabetamath.cc/item/thm-subset-of-a-finite-set).

[F7] By the [sum rule for two finite sets](https://alphabetamath.cc/item/thm-sum-rule), if the finite sets $U,V$ have no common element, then $\lvert U\cup V\rvert=\lvert U\rvert+\lvert V\rvert$.

[F8] [Right cancellation for addition of natural numbers](https://alphabetamath.cc/item/lem-nat-add-cancellative) states that $r+c=s+c$ implies $r=s$ for natural numbers $r,s,c$.

[F9] Clause (iii) of the [binary-union membership lemma](https://alphabetamath.cc/item/lem-unions-and-intersections-of-small-families) gives $z\in U\cup V$ exactly when $z\in U$ or $z\in V$. By the [Axiom of Extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality), two sets with the same elements are equal.

[F10] By the [two-sided inverse theorem](https://alphabetamath.cc/item/thm-a-function-is-a-bijection-exactly-when-it-has-a-two-sided-inverse), the inverse of a bijection $f:U\to V$ is a bijection $f^{-1}:V\to U$ with $f^{-1}(f(u))=u$ for $u\in U$ and $f(f^{-1}(v))=v$ for $v\in V$.

## Proof

**Given:** A finite set $I$, a finite set $S$ of integer tuples on $I$ closed under coordinate permutations, and subsets $A,B\subseteq I$ with $\lvert A\rvert=\lvert B\rvert$.

**Goal:** Prove $\lvert F_A\rvert=\lvert F_B\rvert$.

1.1 For any $D\subseteq I$, each entry $x_i$ of a tuple $x\in S$ is a specified integer. The oddness condition is a predicate on that value, so the condition that it holds exactly at the positions in $D$ selects a unique subset $F_D$ of $S$. This subset is finite because $S$ is finite. [given, F1, F3, F4, F6]

1.2 Write $I\setminus D$ for the subset of positions in $I$ outside $D$. The sets $A,B,I\setminus A,I\setminus B$ are finite because they are subsets of $I$. For $D=A$ and for $D=B$, binary-union membership gives $z\in D\cup(I\setminus D)$ exactly when $z\in D$ or $z\in I\setminus D$. Either alternative implies $z\in I$, and every $z\in I$ lies in one of the two sets by the definition of the complement. Therefore $D\cup(I\setminus D)=I$ by extensionality. The two sets have no common element by the same definition. Thus $\lvert I\setminus A\rvert+\lvert A\rvert=\lvert I\rvert=\lvert I\setminus B\rvert+\lvert B\rvert$. Since $\lvert A\rvert=\lvert B\rvert$, right cancellation gives $\lvert I\setminus A\rvert=\lvert I\setminus B\rvert$. [given, F4, F6, F7, F8, F9]

2.1 Choose bijections $u:A\to B$ and $v:I\setminus A\to I\setminus B$. Define $\pi(i)=u(i)$ for $i\in A$ and $\pi(i)=v(i)$ for $i\in I\setminus A$. These rules give one value for each $i\in I$, so selecting their ordered pairs in $I\times I$ defines a function $\pi:I\to I$. Each $j\in B$ has exactly one preimage under $u$ and none under $v$. Each $j\in I\setminus B$ has exactly one preimage under $v$ and none under $u$. Thus $\pi$ is a permutation, and $\pi^{-1}(j)\in A$ exactly when $j\in B$. [given, F1, F2, F4, F5, step 1.2]

3.1 For $x\in F_A$, let $P_\pi x$ be the tuple with entry $x_{\pi^{-1}(j)}$ at position $j$. Its graph is obtained by selecting in $I\times\mathbb Z$ the pairs with exactly these entries, one for each $j\in I$. By closure, $P_\pi x$ belongs to $S$. Its entry at $j$ is odd exactly when $\pi^{-1}(j)\in A$, equivalently when $j\in B$. Thus $P_\pi x\in F_B$, and the pairs $(x,P_\pi x)$ selected in $F_A\times F_B$ define a function $P_\pi:F_A\to F_B$. [given, F1, F2, F4, step 1.1, step 2.1]

4.1 By the two-sided inverse theorem, $\pi^{-1}$ is a bijection $I\to I$ and hence a permutation of $I$. Its inverse is $\pi$, so reindexing $y\in F_B$ by $\pi^{-1}$ gives the tuple with entry $y_{\pi(i)}$ at position $i$. This tuple belongs to $S$ by closure, and its odd entries occur exactly where $\pi(i)\in B$, which by the construction of $\pi$ is exactly where $i\in A$. Select the graph of this reindexing in $F_B\times F_A$ to define $P_{\pi^{-1}}:F_B\to F_A$. The two reindexings undo each other at every position because $\pi^{-1}(\pi(i))=i$ and $\pi(\pi^{-1}(i))=i$. Since tuples are determined by their entries, every $y\in F_B$ has exactly one preimage under $P_\pi$, namely $P_{\pi^{-1}}y$. Thus $P_\pi:F_A\to F_B$ is a bijection. [given, F1, F2, F4, F10, step 1.1, step 2.1, step 3.1]

5.1 Since $F_A$ is finite and $P_\pi$ is a bijection onto $F_B$, transport of finite cardinality gives $\lvert F_A\rvert=\lvert F_B\rvert$. [F5, step 1.1, step 4.1] ∎
