---
title: Counting a union of obstructions
status: published
research_item: lem-finite-obstruction-cover-bound
dependency_level: 0
---

## Prerequisites

- [math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-union-of-a-set-and-binary-union](https://alphabetamath.cc/item/def-union-of-a-set-and-binary-union)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product)
- [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair)
- [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)
- [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)
- [math:thm-nat-linear-order](https://alphabetamath.cc/item/thm-nat-linear-order)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-indexed-union-and-intersection](https://alphabetamath.cc/item/def-indexed-union-and-intersection)
- [math:def-axiom-of-extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)
- [math:def-power-set](https://alphabetamath.cc/item/def-power-set)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)
- [math:thm-the-empty-set-exists-and-is-unique](https://alphabetamath.cc/item/thm-the-empty-set-exists-and-is-unique)


## Statement

Let $S$ be a finite set. Let $(B_j)_{j\in I}$ be an indexed family, meaning that each index $j$ in the set $I$ is assigned a subset $B_j$ of $S$. Assume only finitely many $B_j$ are nonempty, so $J=\{j\in I:B_j\ne\varnothing\}$ is finite. Write $|A|$ for the number of elements of a finite set $A$. Write $\sum_{j\in I}|B_j|$ for the finite sum $\sum_{j\in J}|B_j|$, with value $0$ when $J$ is empty. Let $U=\bigcup_{j\in I} B_j$ be the set of elements that belong to at least one $B_j$. Then $|U|\le\sum_{j\in I}|B_j|$. If $\sum_{j\in I}|B_j|<|S|$, there is an $x\in S$ that belongs to none of the $B_j$.

## Statement references

[math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)

[math:def-function](https://alphabetamath.cc/item/def-function)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)

[math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

[math:def-indexed-union-and-intersection](https://alphabetamath.cc/item/def-indexed-union-and-intersection)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)

[math:thm-the-empty-set-exists-and-is-unique](https://alphabetamath.cc/item/thm-the-empty-set-exists-and-is-unique)

## Facts & Assumptions

[F1] For a finite set $A$, its cardinality $|A|$ is the unique natural number $n$ for which there is a bijection from $\{0,\ldots,n-1\}$ onto $A$, using the empty set of indices when $n=0$. A bijection from a finite set to another set makes the latter finite and preserves cardinality. Also $|\varnothing|=0$. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F2] A sum of natural numbers over a finite index set is obtained by listing the indices once each and adding the corresponding terms. Its value is independent of the listing, and the empty sum is zero. [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

[F3] Every subset of a finite set is finite and has cardinality at most that of the containing set. [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)

[F4] The Cartesian product $J\times S$ is the set of ordered pairs with first coordinate in $J$ and second coordinate in $S$. The ordered pair $(j,x)$ is $\{\{j\},\{j,x\}\}$, and two ordered pairs are equal exactly when their corresponding coordinates agree. [math:def-cartesian-product](https://alphabetamath.cc/item/def-cartesian-product) [math:def-ordered-pair](https://alphabetamath.cc/item/def-ordered-pair) [math:thm-the-characterising-property-of-ordered-pairs](https://alphabetamath.cc/item/thm-the-characterising-property-of-ordered-pairs)

[F5] A map is injective if equal outputs force equal inputs, surjective if every element of its target is an output, and bijective if it has both properties. [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)

[F6] Clause 2 of the sum rule gives the cardinality of the union of a finitely indexed family of pairwise disjoint finite sets as the sum of their cardinalities. Pairwise disjoint means that no element lies in two sets with different indices. [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)

[F7] Every nonempty subset of the natural numbers has a least element, meaning an element no greater than any member of the subset. Such an element is unique because the order is antisymmetric, meaning $a\le b$ and $b\le a$ imply $a=b$. Also $a<b$ means $a\le b$ and $a\ne b$. [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle) [math:thm-nat-linear-order](https://alphabetamath.cc/item/thm-nat-linear-order) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[F8] A subset of a set contains only elements of that set. Separation inside a given set forms its subset of elements satisfying a specified set-theoretic condition. The condition may use parameters and has no free occurrence of the variable for the resulting set. Two sets with the same elements are equal. [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset) [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation) [math:def-axiom-of-extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)

[F9] A graph contained in a Cartesian product defines a function from the first factor to the second when it has exactly one output in the second factor for each input in the first. Evaluation gives that unique output. [math:def-function](https://alphabetamath.cc/item/def-function)

[F10] An indexed family is a function with the index set as its domain. Its indexed union is the union of its range, so an element belongs to it exactly when it belongs to a set at some index. The indexed union over an empty index set is empty. [math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family) [math:def-indexed-union-and-intersection](https://alphabetamath.cc/item/def-indexed-union-and-intersection) [math:def-union-of-a-set-and-binary-union](https://alphabetamath.cc/item/def-union-of-a-set-and-binary-union)

[F11] The power set of a set is the set of all its subsets. Write $\mathbb{N}$ for the set of natural numbers. [math:def-power-set](https://alphabetamath.cc/item/def-power-set) [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[F12] The symbol $\varnothing$ denotes the unique set with no elements. [math:thm-the-empty-set-exists-and-is-unique](https://alphabetamath.cc/item/thm-the-empty-set-exists-and-is-unique)

## Proof

**Given:** A finite set $S$ and subsets $B_j\subseteq S$ indexed by $I$, with a finite set $J$ of indices at which $B_j$ is nonempty.

**Goal:** Bound the cardinality of $U$ by the sum of the cardinalities of the $B_j$ and find an element outside $U$ when that sum is strictly less than $|S|$.

1.1 The set $J$ is obtained by separating the indices of nonempty sets inside $I$. Keep from the graph of the given family just the pairs whose first coordinate lies in $J$. There is still exactly one output $B_j$ for each $j\in J$, so this defines the restricted family on $J$. Every element of $U$ lies in a nonempty $B_j$, hence lies in a $B_j$ with $j\in J$. Conversely every $B_j$ with $j\in J$ contributes to $U$ because $J\subseteq I$. Thus $U=\bigcup_{j\in J}B_j$. Each $B_j$ and $U$ are subsets of $S$, so they are finite. The unique count $|B_j|$ at each $j\in J$ defines the graph of the summands by separation inside $J\times\mathbb{N}$, so the sum over $J$ is defined. If $J=\varnothing$, then $U=\varnothing$ and both $|U|$ and the sum are zero. [given, F1, F2, F3, F4, F8, F9, F10, F11, F12]

1.2 For $j\in J$, let $D_j=\{(j,x)\in J\times S:x\in B_j\}$, formed by separation inside $J\times S$. Since $B_j\subseteq S$, each $x\in B_j$ has exactly one prescribed value $(j,x)\in D_j$. Keeping those input–output pairs from $B_j\times D_j$ gives the graph of a function from $B_j$ to $D_j$. This map is injective by equality of second coordinates and surjective by the definition of $D_j$. Thus $D_j$ is finite and $|D_j|=|B_j|$. [given, F1, F4, F5, F8, F9]

2.1 To form the indexed family $(D_j)_{j\in J}$, keep from $J\times\mathcal{P}(J\times S)$ the pairs $(j,T)$ for which $T$ consists exactly of the pairs $(j,x)$ with $x\in B_j$. Step 1.2 supplies one such set for each $j$, and equality of sets with the same elements gives uniqueness. Thus the graph defines a family on $J$. Let $D=\bigcup_{j\in J}D_j$. A pair in $D_j$ has first coordinate $j$, so no pair belongs to two sets with different indices. The sum rule gives $D$ finite and $|D|=\sum_{j\in J}|D_j|=\sum_{j\in J}|B_j|$. [given, step 1.2, F2, F4, F6, F8, F9, F10, F11]

3.1 Each pair in $D$ has a unique second coordinate, and that coordinate lies in $U$ by the indexed union rule applied to $D$ and to $U$. Therefore the subset of $D\times U$ that pairs each member of $D$ with its second coordinate is the graph of a function $\pi:D\to U$. It is surjective because every $x\in U$ lies in some $B_j$ with $j\in J$, giving $(j,x)\in D$ with $\pi((j,x))=x$. [step 1.1, step 1.2, step 2.1, F4, F5, F8, F9, F10]

4.1 Fix a bijection $e:\{0,\ldots,|J|-1\}\to J$, with an empty domain when $J$ is empty. For each $x\in U$, separate inside the domain of $e$ the positions $k$ with $x\in B_{e(k)}$. This subset of the natural numbers is nonempty because $x$ is covered by a set with index in $J$ and $e$ is onto $J$. Let $k_x$ be its unique least position. Then $(e(k_x),x)\in D$ is uniquely prescribed for each $x\in U$. Separating these input–output pairs inside $U\times D$ gives a function $h:U\to D$ satisfying $\pi(h(x))=x$ for every $x\in U$. When $U$ is empty the graph has no pairs, so it is $\varnothing$. [given, step 1.1, step 1.2, step 2.1, step 3.1, F1, F4, F5, F7, F8, F9, F10, F12, construct]

5.1 If $h(x)=h(y)$, applying $\pi$ gives $x=y$. Define the image $H$ by separating in $D$ the elements equal to $h(x)$ for some $x\in U$. With codomain $H$ the same function is a bijection from $U$ to $H$. Transporting cardinality along this bijection and applying the finite subset bound to $H\subseteq D$ gives $|U|=|H|\le |D|=\sum_{j\in I}|B_j|$. [step 1.1, step 2.1, step 4.1, F1, F3, F5, F8, F9]

6.1 Suppose $\sum_{j\in I}|B_j|<|S|$. If $U=S$, the bound just proved gives $|S|\le\sum_{j\in I}|B_j|$. Together with the strict inequality this contradicts antisymmetry. Hence $U\ne S$. Since $U\subseteq S$, some $x\in S$ lies outside $U$, for otherwise $U$ and $S$ would have the same elements. By indexed union membership, $x\notin B_j$ for every $j\in I$. [step 1.1, step 5.1, F7, F8, F10] ∎
