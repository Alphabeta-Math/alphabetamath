---
id: lem-author-f93d28423212-divisible-coordinate-count
kind: lemma
title: Counting pairs with one coordinate a multiple of the other
status: published
domain: mathematics
proof_strategy: direct
deps:
  - math:def-integers
  - math:def-int-order
  - math:def-divides-in-z
  - math:def-cartesian-product
  - math:def-finite-cardinality
  - math:def-rational-power
  - math:def-int-abs
  - math:lem-integer-part
  - math:lem-cardinality-of-finite-natural-initial-segment
  - math:thm-product-rule
  - math:thm-subset-of-a-finite-set
  - math:thm-sum-rule
  - math:lem-rational-power-laws
  - math:lem-rational-power-monotone
  - math:thm-reals-ordered-field
  - math:def-int-operations
  - math:def-real-numbers
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:lem-nat-embeds-int
  - math:thm-int-ordered-ring
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-injection-surjection-bijection
  - math:def-ordered-pair
  - math:def-subset-and-proper-subset
  - math:def-function
  - math:def-intersection-of-a-set-and-binary-intersection
  - math:def-natural-numbers
  - math:def-nat-order
  - math:def-rationals
  - math:def-rat-operations
  - math:def-axiom-of-extensionality
  - math:def-integer-power
  - math:def-rat-order
  - math:def-real-order
  - math:def-union-of-a-set-and-binary-union
  - math:lem-unions-and-intersections-of-small-families
  - math:thm-the-empty-set-exists-and-is-unique
dependency_roles:
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-rational-power: mathematical-premise
  math:def-int-abs: mathematical-premise
  math:lem-integer-part: mathematical-premise
  math:lem-cardinality-of-finite-natural-initial-segment: mathematical-premise
  math:thm-product-rule: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:thm-sum-rule: mathematical-premise
  math:lem-rational-power-laws: mathematical-premise
  math:lem-rational-power-monotone: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:def-ordered-pair: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-function: mathematical-premise
  math:def-intersection-of-a-set-and-binary-intersection: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:def-rationals: mathematical-premise
  math:def-rat-operations: mathematical-premise
  math:def-axiom-of-extensionality: mathematical-premise
  math:def-integer-power: mathematical-premise
  math:def-rat-order: mathematical-premise
  math:def-real-order: mathematical-premise
  math:def-union-of-a-set-and-binary-union: mathematical-premise
  math:lem-unions-and-intersections-of-small-families: mathematical-premise
  math:thm-the-empty-set-exists-and-is-unique: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 0
formulation_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-divides-in-z
  - math:def-cartesian-product
  - math:def-finite-cardinality
  - math:def-rational-power
  - math:thm-reals-ordered-field
  - math:def-int-operations
  - math:def-real-numbers
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:lem-nat-embeds-int
  - math:def-ordered-pair
  - math:def-natural-numbers
  - math:def-rationals
  - math:def-integer-power
  - math:def-real-order
argument_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-divides-in-z
  - math:def-cartesian-product
  - math:def-finite-cardinality
  - math:def-rational-power
  - math:def-int-abs
  - math:lem-integer-part
  - math:lem-cardinality-of-finite-natural-initial-segment
  - math:thm-product-rule
  - math:thm-subset-of-a-finite-set
  - math:thm-sum-rule
  - math:lem-rational-power-laws
  - math:lem-rational-power-monotone
  - math:thm-reals-ordered-field
  - math:def-int-operations
  - math:def-real-numbers
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:lem-nat-embeds-int
  - math:thm-int-ordered-ring
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-injection-surjection-bijection
  - math:def-ordered-pair
  - math:def-subset-and-proper-subset
  - math:def-function
  - math:def-intersection-of-a-set-and-binary-intersection
  - math:def-natural-numbers
  - math:def-nat-order
  - math:def-rationals
  - math:def-rat-operations
  - math:def-axiom-of-extensionality
  - math:def-integer-power
  - math:def-rat-order
  - math:def-real-order
  - math:def-union-of-a-set-and-binary-union
  - math:lem-unions-and-intersections-of-small-families
  - math:thm-the-empty-set-exists-and-is-unique
---

## Statement

For an integer $n\ge1$, there are at most $6n^{3/4}$ ordered pairs of integers $(d,x)$ satisfying $d>0$, $d\mid x$ and $d^2+x^2\le n$. Here $d\mid x$ means $x=dk$ for some integer $k$, and $n^{3/4}$ is the cube of the positive fourth root of $n$.

## Facts & Assumptions

[F1] A Cartesian product consists of the ordered pairs with first and second entries from the respective sets. For finite sets its cardinality, the number of elements, is the product of their cardinalities. A subset of a finite set is finite and has at most the cardinality of that set. Cardinalities of disjoint finite sets add. A bijection from a finite set makes its target finite of the same cardinality. [[math:def-cartesian-product]] [[math:def-ordered-pair]] [[math:def-finite-cardinality]] [[math:thm-product-rule]] [[math:thm-subset-of-a-finite-set]] [[math:thm-sum-rule]]

[F2] For a real $T$, the integer part $\lfloor T\rfloor$ is the unique integer $h$ with $h\le T<h+1$. For a natural $j$, the initial segment $\{t\in\mathbb{N}:t<j\}$ is finite with cardinality $j$. Absolute value is $|k|=k$ for $k\ge0$ and $|k|=-k$ otherwise. [[math:lem-integer-part]] [[math:lem-cardinality-of-finite-natural-initial-segment]] [[math:def-natural-numbers]] [[math:def-nat-order]] [[math:def-int-abs]]

[F3] In the real order, multiplication or division by positive numbers preserves inequalities. For positive real bases, rational powers are defined by roots and integer powers, obey the exponent addition law and increase with the base when the exponent is positive. The exponents use rational addition. A rational with positive denominator is positive exactly when its numerator is positive. [[math:def-real-order]] [[math:thm-reals-ordered-field]] [[math:def-rational-power]] [[math:lem-rational-power-laws]] [[math:def-rationals]] [[math:def-rat-operations]] [[math:def-rat-order]] [[math:lem-rational-power-monotone]]

[F4] An integer square $u^2$ is the integer product $u\cdot u$. For any real $u$, the natural powers $u^2$ and $u^3$ are the repeated products $u\cdot u$ and $(u\cdot u)\cdot u$. Identify the naturals and integers with their canonical images along $\mathbb{N}\to\mathbb{Z}\to\mathbb{Q}\to\mathbb{R}$. These embeddings preserve addition, multiplication and order. The image of the naturals in the integers consists exactly of the nonnegative integers. The integers form a totally ordered commutative ring, so translation by an integer preserves inequalities in both directions. [[math:def-int-operations]] [[math:def-integer-power]] [[math:def-real-numbers]] [[math:lem-nat-embeds-int]] [[math:lem-int-embeds-rat]] [[math:lem-rat-embeds-dense]] [[math:thm-int-ordered-ring]]

[F5] Ordered pairs are equal exactly when their corresponding coordinates agree. If $f:A\to D$ and $g:D\to A$ satisfy $g(f(a))=a$ for all $a\in A$ and $f(g(b))=b$ for all $b\in D$, then $f$ is a bijection. If $f(a)=f(a\prime)$, applying $g$ to both values gives $a=a\prime$, so $f$ is injective. For each $b\in D$, the element $g(b)$ maps to $b$, so $f$ is surjective. The same criterion with the maps exchanged makes $g$ a bijection. [[math:thm-the-characterising-property-of-ordered-pairs]] [[math:def-function]] [[math:def-injection-surjection-bijection]]

[F6] A condition on elements of a set defines a subset by separation. A function from one set to another is specified by a graph in their Cartesian product with exactly one value for each element of the domain. [[math:def-subset-and-proper-subset]] [[math:def-cartesian-product]] [[math:def-function]]

[F7] Membership in the binary union $A\cup D$ means membership in at least one of $A,D$. Membership in the binary intersection $A\cap D$ means membership in both. Sets with the same elements are equal. The unique set with no elements is $\varnothing$, and $A,D$ are disjoint when $A\cap D=\varnothing$. [[math:def-union-of-a-set-and-binary-union]] [[math:def-intersection-of-a-set-and-binary-intersection]] [[math:lem-unions-and-intersections-of-small-families]] [[math:def-axiom-of-extensionality]] [[math:thm-the-empty-set-exists-and-is-unique]]

## Proof

**Given:** An integer $n\ge1$.

**Goal:** Prove the bound $6n^{3/4}$.

1.1 Inside $\mathbb{Z}\times\mathbb{Z}$, let $S$ be the subset defined by the conditions in the statement and $B$ the subset of pairs $(d,k)$ with $d>0$ and $d^2+d^2k^2\le n$. For $(d,x)\in S$, divisibility gives an integer $k$ with $x=dk$. It is unique since in the reals $k=x/d$ and the integer embedding is injective. The integer ring identity $(dk)^2=d^2k^2$ puts $(d,k)$ in $B$. Conversely $(d,k)\in B$ gives $(d,dk)\in S$ by the same identity and divisibility. By separation in $S\times B$ and $B\times S$, these rules with unique outputs define functions $f:S\to B$ and $g:B\to S$. For $(d,x)\in S$ the resulting $k$ satisfies $g(f((d,x)))=(d,dk)=(d,x)$. For $(d,k)\in B$ one has $f(g((d,k)))=f((d,dk))=(d,k)$ by uniqueness of the integer multiplier. The pointwise inverse criterion gives bijections in both directions. [given, F1, F3, F4, F5, F6]

1.2 Fix a real $T\ge1$ and put $h=\lfloor T\rfloor$. There is no integer $j$ strictly between any integer $m$ and $m+1$, since otherwise both $m$ and $j$ would satisfy the defining floor inequalities at $T=j$. Thus $h\ge1$ (if $h<1$, then $h+1\le1\le T$), and an integer is at most $T$ exactly when it is at most $h$, since $T<h+1$. In particular, $h$ and $2h+1$ are nonnegative integers and correspond to naturals. [F2, F3, F4]

2.1 Write $R=n^{1/4}$ and $U=n^{1/2}$. The rational exponents $1/4$ and $1/2$ are positive because the numerator and both denominators are positive integers. Since $n\ge1$ and the positive fourth and square roots of $1$ equal $1$, base monotonicity gives $R,U\ge1$. The root convention gives $U^2=n$. The exponent addition law gives $R^2=R\cdot R=U$ and $RU=n^{3/4}$, using $1/4+1/4=8/16=1/2$ and $1/4+1/2=6/8=3/4$. For $(d,k)\in B$, preservation of operations and order gives $d^2\le n$ and $(d|k|)^2=d^2k^2\le n$ in the reals, since squares are nonnegative and $|k|^2=k^2$. Squaring is strictly increasing on nonnegative reals because for $u>v\ge0$ one has $u^2-v^2=(u-v)(u+v)>0$. Thus $d\le U$ and $d|k|\le U$, so $|k|\le U/d$ as $d>0$. [given, step 1.1, F2, F3, F4]

2.2 The positive integers at most $T$ are precisely the integers $1\le d\le h$. The translation $f_1(d)=d-1$ gives $0\le d-1<h$, and $g_1(t)=t+1$ sends $0\le t<h$ back to $1\le t+1\le h$ by discreteness. The integers with $|k|\le T$ are precisely those with $-h\le k\le h$. The translation $f_2(k)=k+h$ gives $0\le k+h<2h+1$, and $g_2(t)=t-h$ sends $0\le t<2h+1$ back to $-h\le t-h\le h$ by discreteness. The targets of $f_1,f_2$ are the natural initial segments of lengths $h$ and $2h+1$ under the canonical identification. Each formula gives exactly one output for each input in its domain, so separation in the appropriate product supplies its function graph. For inputs in the indicated domains, $g_1(f_1(d))=(d-1)+1=d$ and $f_1(g_1(t))=(t+1)-1=t$. Likewise $g_2(f_2(k))=(k+h)-h=k$ and $f_2(g_2(t))=(t-h)+h=t$. The pointwise criterion gives bijections, so transporting cardinality from the initial segments along $g_1,g_2$ gives the two intervals cardinalities $h\le T$ and $2h+1\le 2T+1\le3T$, respectively. [step 1.2, F1, F2, F3, F4, F5, F6]

3.1 Let $B_1$ and $B_2$ be the subsets of $B$ with $d\le R$ and $d>R$, respectively. By the binary union membership rule, belonging to $B_1\cup B_2$ means belonging to $B$ with $d\le R$ or $d>R$. Totality makes this equivalent to belonging to $B$, giving $B=B_1\cup B_2$ by extensionality. The binary intersection membership rule would require both inequalities, which is impossible, so $B_1\cap B_2=\varnothing$. [step 1.1, step 2.1, F3, F6, F7]

4.1 Since every positive integer $d$ is at least $1$, the first part lies in the product of the positive integers at most $R$ and the integers with $|k|\le U$, by $|k|\le U/d\le U$. The second lies in the product of the positive integers at most $U$ and the integers with $|k|\le R$, by $|k|\le U/d<U/R=R$. The two products are finite by the interval counts and the product rule. Their respective subsets have cardinalities at most $3RU$ and $3UR$. The two-set sum rule makes $B$ finite with cardinality at most $6RU=6n^{3/4}$. Transport along the bijection from $B$ to $S$ gives the same bound for $S$. [step 1.1, step 1.2, step 2.1, step 2.2, step 3.1, F1, F3, F4] ∎
