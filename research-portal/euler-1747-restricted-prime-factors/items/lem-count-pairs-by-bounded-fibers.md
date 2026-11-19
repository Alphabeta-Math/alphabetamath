---
id: lem-count-pairs-by-bounded-fibers
kind: lemma
title: Counting pairs by bounded fibers
status: published
domain: mathematics
deps:
  - math:def-natural-numbers
  - math:def-axiom-of-extensionality
  - math:def-ordered-pair
  - math:def-cartesian-product
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:def-real-numbers
  - math:thm-reals-ordered-field
  - math:def-canonical-natural
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:lem-nat-order-is-membership
  - math:thm-well-ordering-principle
  - math:def-nat-order
  - math:thm-nat-linear-order
  - math:thm-subset-of-a-finite-set
  - math:thm-sum-rule
  - math:def-sum-over-a-finite-index-set
  - math:def-finite-sum
  - math:def-nat-finite-sum-and-product
  - math:lem-nat-finite-sum-laws-and-the-canonical-embedding
  - math:lem-finite-sum-laws
  - math:prop-of-multiply-inequalities
  - math:def-indexed-family
  - math:def-power-set
  - math:def-real-order
  - math:def-indexed-union-and-intersection
  - math:def-field
  - math:def-ordered-field
formulation_deps:
  - math:def-natural-numbers
  - math:def-ordered-pair
  - math:def-cartesian-product
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:def-real-numbers
  - math:thm-reals-ordered-field
  - math:def-canonical-natural
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-real-order
  - math:def-field
argument_deps:
  - math:def-natural-numbers
  - math:def-axiom-of-extensionality
  - math:def-ordered-pair
  - math:def-cartesian-product
  - math:def-subset-and-proper-subset
  - math:def-finite-cardinality
  - math:def-real-numbers
  - math:thm-reals-ordered-field
  - math:def-canonical-natural
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-function
  - math:def-injection-surjection-bijection
  - math:lem-nat-order-is-membership
  - math:thm-well-ordering-principle
  - math:def-nat-order
  - math:thm-nat-linear-order
  - math:thm-subset-of-a-finite-set
  - math:thm-sum-rule
  - math:def-sum-over-a-finite-index-set
  - math:def-finite-sum
  - math:def-nat-finite-sum-and-product
  - math:lem-nat-finite-sum-laws-and-the-canonical-embedding
  - math:lem-finite-sum-laws
  - math:prop-of-multiply-inequalities
  - math:def-indexed-family
  - math:def-power-set
  - math:def-real-order
  - math:def-indexed-union-and-intersection
  - math:def-field
  - math:def-ordered-field
dependency_roles:
  math:def-natural-numbers: mathematical-premise
  math:def-axiom-of-extensionality: mathematical-premise
  math:def-ordered-pair: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:def-canonical-natural: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
  math:def-function: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:thm-well-ordering-principle: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:thm-nat-linear-order: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:thm-sum-rule: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:def-finite-sum: mathematical-premise
  math:def-nat-finite-sum-and-product: mathematical-premise
  math:lem-nat-finite-sum-laws-and-the-canonical-embedding: mathematical-premise
  math:lem-finite-sum-laws: mathematical-premise
  math:prop-of-multiply-inequalities: mathematical-premise
  math:def-indexed-family: mathematical-premise
  math:def-power-set: mathematical-premise
  math:def-real-order: mathematical-premise
  math:def-indexed-union-and-intersection: mathematical-premise
  math:def-field: mathematical-premise
  math:def-ordered-field: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 0
---

## Statement

Let $A$ and $B$ be sets and let $S$ be a finite subset of the Cartesian product $A\times B$, the set of ordered pairs $(x,y)$ with $x\in A$ and $y\in B$. Define the first-coordinate image $D$ and, for each $x\in D$, its fiber $S_x$ by
$$D=\{x\in A:\exists y\in B,\ (x,y)\in S\},\qquad S_x=\{(u,v)\in S:u=x\}.$$
Thus $D$ consists of the first coordinates that occur in $S$, and $S_x$ consists of all pairs in $S$ with first coordinate $x$. Both $D$ and each $S_x$ are finite. For a finite set $T$, write $|T|$ for its cardinality, the number of its elements, and interpret it as a real number when comparing it with a real bound.

Let $a,b\in\mathbb R$ be nonnegative, meaning $0\le a$ and $0\le b$. If $|D|\le a$ and $|S_x|\le b$ for every $x\in D$, then $|S|\le ab$.

## Statement references

[[math:def-ordered-pair|Ordered pair]]

[[math:thm-the-characterising-property-of-ordered-pairs|Equality of ordered pairs]]

[[math:def-cartesian-product|Cartesian product]]

[[math:def-subset-and-proper-subset|Subset and separation notation]]

[[math:def-finite-cardinality|Finite cardinality]]

[[math:def-natural-numbers|Von Neumann natural numbers]]

[[math:def-real-numbers|Real numbers]]

[[math:def-real-order|Definition of the real order]]

[[math:def-field|Field multiplication]]

[[math:thm-reals-ordered-field|The real numbers as an ordered field]]

[[math:def-canonical-natural|Natural numbers interpreted in a field]]

## Justification

The ordered pair $(x,y)$ is $\{\{x\},\{x,y\}\}$, and equality of ordered pairs forces equality of their respective coordinates. Hence the phrase “first coordinate” singles out a unique value for each pair. The defining predicates for $D$ and $S_x$ separate subsets of $A$ and $S$, respectively, so they specify unique sets.

A set $T$ is finite when it admits a bijection with a von Neumann natural number $n\in\mathbb N$, viewed as the set of indices $k<n$. A bijection matches each element on either side with exactly one on the other side. This $n$ is unique and gives $|T|$. Its real interpretation is $\iota(n)=n\cdot1_{\mathbb R}$, given by $\iota(0)=0$ and $\iota(n+1)=\iota(n)+1$.

## Facts & Assumptions

[F1] The first coordinate of a pair is unique by [[math:thm-the-characterising-property-of-ordered-pairs|the ordered-pair equality theorem]]. [[math:def-function|A function]] assigns a unique output to each element of its domain. A function is [[math:def-injection-surjection-bijection|bijective]] when distinct inputs have distinct outputs and every element of its target is an output.

[F2] Write $\mathbb N$ for the [[math:def-natural-numbers|set of von Neumann natural numbers]]. The natural number $m$ satisfies $0\le m$ and is the set of indices $k<m$ by [[math:lem-nat-order-is-membership|the identification of natural order with membership]]. Every nonempty set of natural numbers has a least member by [[math:thm-well-ordering-principle|well-ordering]]. For natural indices, $k<\ell$ means $k\le\ell$ and $k\ne\ell$ by [[math:def-nat-order|the definition of natural order]]. The natural-number order is antisymmetric by [[math:thm-nat-linear-order|the natural-number linear-order theorem]].

[F3] Every finite set has a unique natural number as its [[math:def-finite-cardinality|cardinality]]. Each natural number is finite by [[math:def-finite-cardinality|finite cardinality, clause (a)]]. Every subset of a finite set is finite by [[math:thm-subset-of-a-finite-set|the finite-subset theorem]]. A bijection from a finite set transports finiteness and preserves cardinality by [[math:def-finite-cardinality|finite cardinality, clause (c)]].

[F4] For a finite index set and a family of finite sets indexed by it, the sets are pairwise disjoint when no element belongs to two sets with distinct indices. An element belongs to the [[math:def-indexed-union-and-intersection|indexed union]] if and only if it belongs to at least one member of the family. If the sets are pairwise disjoint, [[math:thm-sum-rule|the sum rule, clause 2]] gives the size of their union as the natural-number sum of their cardinalities.

[F5] For a finite index set $I$ of size $d$, the [[math:def-sum-over-a-finite-index-set|sum over $I$]] of a function $q:I\to\mathbb N$ or $q:I\to\mathbb R$ is computed by any bijection $g:d\to I$, adding $q(g(k))$ in order for $k<d$. The [[math:def-nat-finite-sum-and-product|natural-number sum]] and the [[math:def-finite-sum|real sum]] start at zero and add one term at each successive index. For a finite list of length $d$, both definitions extend the list by zero at every index $k\ge d$. The [[math:def-canonical-natural|canonical map]] into the reals sends the natural zero to the real zero, so $\iota(0)=0$. By [[math:lem-nat-finite-sum-laws-and-the-canonical-embedding|the canonical-embedding laws, clauses 6 and 7]], $\iota$ carries the finite sum of a natural-number sequence to the real sum of its embedded terms and is strictly increasing.

[F6] For real sequences on $\mathbb N$, inequalities between corresponding terms at every index $k<d$ imply the same inequality between the sums of the first $d$ terms, and the sum of the first $d$ terms of the constant sequence with value $b$ is $\iota(d)b$, by [[math:lem-finite-sum-laws|the real finite-sum laws, clauses 4 and 2]].

[F7] By [[math:thm-reals-ordered-field|the real ordered-field theorem]], the reals form an [[math:def-ordered-field|ordered field]] and their order is reflexive and transitive. For the [[math:def-real-order|real order]], $u<v$ implies $u\le v$. For the [[math:def-field|field multiplication]], [[math:prop-of-multiply-inequalities|multiplication of nonnegative inequalities]] gives $uv\le u'v'$ when $0\le u\le u'$ and $0\le v\le v'$.

[F8] The [[math:def-power-set|power set]] $\mathcal P(S)$ is the set of all subsets of $S$. An [[math:def-indexed-family|indexed family]] with index set $D$ is a function with domain $D$. [[math:def-subset-and-proper-subset|Separation]] inside a [[math:def-cartesian-product|Cartesian product]] gives the subset of pairs satisfying the defining predicate.

[F9] By [[math:def-axiom-of-extensionality|extensionality]], two sets with the same elements are equal.

## Proof

**Given:** $A,B,S,D,S_x$ as in the statement, and nonnegative reals $a,b$ with the stated bounds on $|D|$ and $|S_x|$ once their finiteness is established.

**Goal:** Show that $D$ and the fibers are finite and that $\iota(|S|)\le ab$.

1.1 Let $m=|S|$ and take a bijection $e:m\to S$. By separation, form the set $J$ of indices $k\in m$ for which no earlier index has the same first coordinate as $e(k)$. For any $x\in D$, separate from $m$ the indices whose pairs have first coordinate $x$. This set is nonempty by surjectivity of $e$. Well-ordering gives a least matching index $\ell$, so $\ell\le k$ for every matching index $k$. If a matching index $k$ satisfied $k<\ell$, then $k\le\ell$ and $k\ne\ell$ by the definition of strict order, while $\ell\le k$ and antisymmetry would give $k=\ell$. Thus $\ell$ belongs to $J$. Every other matching index $k$ has $\ell\le k$ and $\ell\ne k$, hence $\ell<k$, so $k$ is excluded from $J$. Separate from $J\times D$ the graph $H=\{(k,x)\in J\times D:e(k)\text{ has first coordinate }x\}$. For each $k\in J$, the pair $e(k)\in S$ has exactly one first coordinate and that coordinate belongs to $D$, so $H$ is a function with domain $J$ and codomain $D$. For each $x\in D$, the least-index argument gives exactly one $k\in J$ with $(k,x)\in H$, making $H$ a bijection. Since $J$ is a subset of the finite set $m$, the set $D$ is finite. [given, F1, F2, F3, F8]

2.1 By separation inside $D\times\mathcal P(S)$, form $G=\{(x,T)\in D\times\mathcal P(S):T=S_x\}$. Each $x\in D$ has exactly one such $T$ because the defining predicate of $S_x$ specifies a unique subset of $S$. Hence $G$ is a function with domain $D$ whose value at $x$ is $S_x$, so $G$ is the indexed family $(S_x)_{x\in D}$. Each fiber $S_x$ is a subset of $S$ and hence finite. Each pair in $S$ belongs to the fiber of its first coordinate, and coordinate uniqueness prevents a pair from belonging to fibers with distinct indices. Every element of any fiber lies in $S$ because $S_x\subseteq S$. By the indexed-union membership criterion, the union of $(S_x)_{x\in D}$ has exactly the same elements as $S$. By extensionality the union equals $S$. [F1, F3, F4, F8, F9, step 1.1]

3.1 By separation in $D\times\mathbb N$, form the graph $K=\{(x,n)\in D\times\mathbb N:n=|S_x|\}$. Each fiber is finite by Step 2.1, so each $x\in D$ has exactly one such $n$ by the definition of finite cardinality. Thus $K$ defines a function $K:D\to\mathbb N$ with $K(x)=|S_x|$. Applying the sum rule to the disjoint family in Step 2.1 gives $|S|=\sum_{x\in D}K(x)$ as an equality of natural numbers. [F1, F2, F3, F4, F5, F8, step 1.1, step 2.1]

4.1 Put $d=|D|$ and take a bijection $g:d\to D$ by the definition of cardinality. Using the zero extension for natural-number sums, set $c_k=K(g(k))$ for $k<d$ and $c_k=0$ for the other natural indices. For $k<d$, the index $k$ belongs to the domain $d$ of $g$, and $g(k)\in D$ belongs to the domain of $K$. For each $k\in\mathbb N$, set $r_k=\iota(c_k)$ and $s_k=b$. Each rule gives a unique value at every natural index, so separation in $\mathbb N\times\mathbb N$ and $\mathbb N\times\mathbb R$ gives the graphs of the three sequences. Enumerating the sum of $K$ in Step 3.1 by $g$ gives $|S|=\sum_{k<d}c_k$ as an equality of natural numbers. [given, F1, F2, F3, F5, F8, step 1.1, step 3.1]

5.1 By the canonical-embedding law, the real image of the natural sum in Step 4.1 is the sum of the first $d$ terms of $r$. For $k<d$, we have $r_k=\iota(K(g(k)))=\iota(|S_{g(k)}|)\le b=s_k$ by the fiber bound. The real sum comparison and constant-sum laws give
$$\iota(|S|)=\sum_{k<d}r_k\le\sum_{k<d}s_k=\iota(d)b.$$
When $d=0$, the sums are empty and have value zero. [given, F5, F6, step 3.1, step 4.1]

6.1 Since $0\le d$ in the natural order, either $d=0$ or $0<d$. In the first case $\iota(d)=\iota(0)=0$. In the second case strict increase gives $0=\iota(0)<\iota(d)$. Thus $0\le\iota(d)$ in the real order. The bound on $|D|$ gives $\iota(d)\le a$, and nonnegativity and reflexivity give $0\le b\le b$. Apply the product inequality to $0\le\iota(d)\le a$ and $0\le b\le b$. It gives $\iota(d)b\le ab$. Real-order transitivity with Step 5.1 gives $\iota(|S|)\le ab$. [given, F2, F5, F7, step 4.1, step 5.1] ∎
