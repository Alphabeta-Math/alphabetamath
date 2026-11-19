---
title: Maximum from nonincreasing successive ratios
status: draft
research_item: lem-positive-sequence-ratio-maximum
dependency_level: 0
---

## Prerequisites

- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:thm-nat-linear-order](https://alphabetamath.cc/item/thm-nat-linear-order)
- [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)
- [math:lem-nat-nonzero-is-successor](https://alphabetamath.cc/item/lem-nat-nonzero-is-successor)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)


## Statement

Let $I$ be the set of natural numbers $j$ with $1\le j$. Write $j+1$ for the successor of $j$. A positive real sequence $(a_j)_{j\in I}$ assigns one real number $a_j>0$ to each $j\in I$.

Write $r_j=a_{j+1}/a_j$ for the successive ratios. Assume the ratios are nonincreasing, meaning $r_i\ge r_j$ whenever $i\le j$ in $I$.

Let $k\in I$. Assume $r_k\le1$ and, if $k>1$, also assume $r_{k-1}\ge1$. Here $k-1$ denotes the positive index whose successor is $k$. Then $a_k$ is a maximum, meaning $a_j\le a_k$ for every $j\in I$. If $r_k=1$, the term at $k+1$ also equals $a_k$. If $k>1$ and $r_{k-1}=1$, the term at $k-1$ also equals $a_k$.

## Statement references

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)

[math:def-function](https://alphabetamath.cc/item/def-function)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)

[math:thm-nat-linear-order](https://alphabetamath.cc/item/thm-nat-linear-order)

[math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)

[math:lem-nat-nonzero-is-successor](https://alphabetamath.cc/item/lem-nat-nonzero-is-successor)

## Facts & Assumptions

[F1] In the real order ([math:def-real-order](https://alphabetamath.cc/item/def-real-order)), $x\le y$ means $x=y$ or $y-x>0$. With this order the reals form a totally ordered field ([math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)), so real comparison is reflexive and transitive and the product of two positive elements is positive ([math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)).

[F2] For $y\ne0$, division in a field is $x/y=xy^{-1}$, with $y^{-1}y=1$. Field multiplication is commutative and associative, has identity $1$, and distributes over addition and hence subtraction ([math:def-field](https://alphabetamath.cc/item/def-field)).

[F3] For natural numbers, the successor sends $j$ to $j\cup\{j\}$, denoted here by $j+1$, with $1$ the successor of $0$ ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)). The order $i\le j$ means $i+d=j$ for some natural $d$, using natural addition ([math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)), and $i<j$ also requires $i\ne j$ ([math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)). This comparison is a total order, so any two indices are comparable, and it is reflexive and transitive ([math:thm-nat-linear-order](https://alphabetamath.cc/item/thm-nat-linear-order)). On the naturals, $i<j$ is equivalent to $i+1\le j$. In particular $j<j+1$ by applying the equivalence with $i=j$ and right endpoint $j+1$ ([math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)). Every nonzero natural is the successor of some natural ([math:lem-nat-nonzero-is-successor](https://alphabetamath.cc/item/lem-nat-nonzero-is-successor)).

[F4] If $P(0)$ holds and for every natural $t$ the truth of $P(t)$ implies that of $P(t+1)$, then $P(t)$ holds for every natural $t$ ([math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)).

## Proof

**Given:** The positive sequence and its nonincreasing ratios, with $r_k\le1$ and $r_{k-1}\ge1$ when $k>1$.

**Goal:** Show that $a_j\le a_k$ for every $j\in I$.

1.1 For $j\in I$, we have $1\le j<j+1$ by the successor rule, so $j+1\in I$ and both terms in the ratio exist. Each ratio $r_j$ is defined because $a_j>0$ implies $a_j\ne0$. For $k>1$, the preceding index is well defined. Because $0<1$ by the successor rule, $k\ne0$, so $k=h+1$ for some natural $h$. If $h<1$, then $k=h+1\le1$, a contradiction. If two predecessors were distinct, the smaller $u$ and larger $v$ would satisfy $u+1\le v<v+1$, so their successors could not coincide. Hence $h=k-1$ is unique and lies in $I$. [given, F1, F2, F3]

1.2 Fix $m,n\in I$ with $m\le n$. Let $\preceq$ mean either $\le$ throughout or $\ge$ throughout on the reals, and suppose $a_i\preceq a_{i+1}$ for all $m\le i<n$. Define $P(t)$ to assert $a_m\preceq a_t$ when $m\le t\le n$, with $P(t)$ true outside that range. Since $0<1\le m$, $P(0)$ holds. Assume $P(t)$. If $t+1$ lies outside the range, $P(t+1)$ holds by definition, and if $t+1=m$, it holds by reflexivity. Otherwise $m<t+1\le n$. If $t<m$, then $t+1\le m$, contrary to $m<t+1$. Hence $m\le t$. As $t<t+1\le n$, this gives $m\le t<n$. By $P(t)$ and the adjacent comparison, $a_m\preceq a_t\preceq a_{t+1}$, which gives $P(t+1)$ by transitivity. By induction, $P(n)$ holds, giving $a_m\preceq a_n$. [F1, F3, F4]

2.1 For real $x\le y$ and $c>0$, we have $cx\le cy$. If $x=y$ the products agree, and if $x<y$ then $cy-cx=c(y-x)>0$ by distributivity and closure of the positive elements under multiplication. Since $a_jr_j=a_{j+1}$ by the inverse law, we can multiply the ratio bounds by $a_j>0$. If $1\le j<k$, then $k>1$ and $j\le k-1$, since $k-1<j$ would imply $k\le j$. Thus $r_j\ge r_{k-1}\ge1$, so $a_j\le a_{j+1}$. If $j\ge k$, then $r_j\le r_k\le1$, so $a_{j+1}\le a_j$. [given, F1, F2, F3, step 1.1]

3.1 If $j<k$, apply the preceding induction argument on $j\le i\le k$ with $\preceq$ meaning $\le$. If $j>k$, apply it on $k\le i\le j$ with $\preceq$ meaning $\ge$. The respective adjacent comparisons come from step 2.1. At $j=k$, equality holds. Thus $a_j\le a_k$ for every $j\in I$. Equality of an adjacent ratio with $1$ gives equal neighboring terms by $a_{i+1}=a_ir_i$, so $r_k=1$ gives a tie at $k+1$, and $r_{k-1}=1$ for $k>1$ gives a tie at $k-1$. [F1, F2, F3, step 1.1, step 2.1, step 1.2] ∎
