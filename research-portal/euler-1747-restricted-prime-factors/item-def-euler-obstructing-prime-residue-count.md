---
title: The eight residue classes and their counting function
status: published
research_item: def-euler-obstructing-prime-residue-count
dependency_level: 0
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 6, Lemma 5.2, definition of the residue set and counting function
---

PDF p. 6: ` Lemma 5.2, definition of the residue set and counting function `

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)
- [math:def-real-order](https://alphabetamath.cc/item/def-real-order)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-function](https://alphabetamath.cc/item/def-function)
- [math:def-inverse-relation-composition-and-restriction](https://alphabetamath.cc/item/def-inverse-relation-composition-and-restriction)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-power-set](https://alphabetamath.cc/item/def-power-set)
- [math:def-ring](https://alphabetamath.cc/item/def-ring)
- [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)


## Definition

Identify the integers $\mathbb Z$ with their ordered copy in the real numbers $\mathbb R$ by composing the canonical embedding of the integers into the rationals with the constant-sequence embedding of the rationals into the reals. A positive integer $n$ satisfies $0<n$.

For integers $n$ and $r$, congruence $n\equiv r\pmod{60}$ means that $n-r=60q$ for some integer $q$. For $0\le r<60$, let $[r]_{60}=\{n\in\mathbb Z:n\equiv r\pmod{60}\}$ be the residue class represented by $r$. Put
$$\mathcal S=\{[7]_{60},[11]_{60},[19]_{60},[23]_{60},[31]_{60},[43]_{60},[47]_{60},[59]_{60}\}.$$

For real $t\ge0$, let $C(t)$ be the subset of $\mathbb Z$ consisting of positive integers $n$ that satisfy $n\le t$ in the real order and belong to a class in $\mathcal S$. Define $A(t)=|C(t)|$, where $|C(t)|$ denotes the number of elements of the finite set $C(t)$.

## Definition references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-real-numbers](https://alphabetamath.cc/item/def-real-numbers)

[math:def-real-order](https://alphabetamath.cc/item/def-real-order)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)

[math:def-power-set](https://alphabetamath.cc/item/def-power-set)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:def-rat-order](https://alphabetamath.cc/item/def-rat-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-function](https://alphabetamath.cc/item/def-function)

[math:def-inverse-relation-composition-and-restriction](https://alphabetamath.cc/item/def-inverse-relation-composition-and-restriction)

[math:def-ring](https://alphabetamath.cc/item/def-ring)

[math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)

## Facts & Assumptions

[F1] For integers $n,r$, the congruence $n\equiv r\pmod{60}$ holds exactly when $n-r=60q$ for some integer $q$ ([math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)). Here $n-r$ abbreviates $n+(-r)$, with integer addition and negation ([math:def-ring](https://alphabetamath.cc/item/def-ring), [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)).

[F2] Division with remainder by the positive integer $60$ gives, for each integer $n$, a unique pair of integers $q,s$ such that $n=60q+s$ and $0\le s<60$ ([math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

[F3] For each real $t$, its integer part is the unique integer $h$ with $h\le t<h+1$, using the canonical order-preserving inclusion of the integers in the reals ([math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)).

[F4] The canonical map $\iota$ from the natural numbers $\mathbb N$ to the integers is injective, satisfies $\iota(j)\le\iota(m)$ exactly when $j\le m$, and has image the nonnegative integers ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int), [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order), [math:def-int-order](https://alphabetamath.cc/item/def-int-order)). By that order equivalence and injectivity, $\iota(j)<\iota(m)$ holds exactly when $j<m$.

[F5] Use the von Neumann natural numbers, with $0=\varnothing$ and successor $m\cup\{m\}$. In this convention a natural number $m$ is the set $\{j\in\mathbb N:j<m\}$ of its predecessors, where $<$ is the strict additive order ([math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers), [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order), [math:lem-nat-order-is-membership](https://alphabetamath.cc/item/lem-nat-order-is-membership)).

[F6] The identity map shows that the predecessor set $m$ has cardinality $m$. A set in bijection with a finite set is finite with the same cardinality. Every finite set has a unique natural number as its cardinality ([math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)).

[F7] Every subset of a finite set is finite ([math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)).

[F8] The integers, with their usual addition, multiplication and negation, form a totally ordered commutative ring, and the reals form a totally ordered field ([math:def-int-operations](https://alphabetamath.cc/item/def-int-operations), [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring), [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)).

[F9] The codomain of the canonical integer-to-rational embedding is the domain of the constant-sequence rational-to-real embedding. Both use the same rationals and rational order ([math:def-rationals](https://alphabetamath.cc/item/def-rationals), [math:def-rat-order](https://alphabetamath.cc/item/def-rat-order)). Their composite sends zero to zero and preserves and reflects order ([math:def-function](https://alphabetamath.cc/item/def-function), [math:def-inverse-relation-composition-and-restriction](https://alphabetamath.cc/item/def-inverse-relation-composition-and-restriction), [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat), [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)).

[F10] For a set and a specified predicate on its elements, separation gives the unique subset whose elements are exactly those satisfying the predicate ([math:def-subset-and-proper-subset](https://alphabetamath.cc/item/def-subset-and-proper-subset)).

[F11] A map is bijective when it is injective and surjective onto its codomain ([math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)).

[F12] Restricting a function to a subset of its domain keeps exactly the original pairs whose first coordinate belongs to that subset ([math:def-inverse-relation-composition-and-restriction](https://alphabetamath.cc/item/def-inverse-relation-composition-and-restriction)). A function with domain $A$ is a function from $A$ to $B$ if all its values lie in $B$ ([math:def-function](https://alphabetamath.cc/item/def-function)).

[F13] For any set $X$, its power set $\mathcal P(X)$ is the set whose elements are exactly the subsets of $X$ ([math:def-power-set](https://alphabetamath.cc/item/def-power-set)).

[F14] For real $a,b$, $a<b$ means $a\le b$ and $a\ne b$. The reversed comparisons $a>b$ and $a\ge b$ mean $b<a$ and $b\le a$, respectively ([math:def-real-order](https://alphabetamath.cc/item/def-real-order), [math:def-ordered-field](https://alphabetamath.cc/item/def-ordered-field)).

## Justification

**Given:** A real cutoff $t\ge0$ and the eight listed representatives.

**Goal:** Show that the representatives specify eight distinct residue classes and that $A(t)$ is well defined.

1.1 For every integer $r$ with $0\le r<60$, the congruence condition in [F1] defines $[r]_{60}$ by separation in $\mathbb Z$. Fix an integer $n$. By [F2] it has a unique remainder $s$ in the range $0\le s<60$. For any integer $r$ in this range, membership in $[r]_{60}$ is equivalent by [F1] to $n+(-r)=60q$ for some integer $q$. Adding $r$ to both sides gives $n=60q+r$, and adding $-r$ recovers the first equation by the additive group laws in [F8]. By [F2] such a $q$ exists exactly when $r=s$. [F1, F2, F8, F10]

2.1 For each listed representative $r$, the set $[r]_{60}$ from step 1.1 is a subset of $\mathbb Z$ and hence an element of $\mathcal P(\mathbb Z)$ by [F13]. Apply [F10] in $\mathcal P(\mathbb Z)$ with the predicate that a member equals one of the eight listed classes. The resulting set has precisely the elements prescribed for $\mathcal S$. [given, F10, F13, step 1.1]

2.2 Each listed representative $r$ has remainder $r$ because $r=60\cdot0+r$ and $0\le r<60$. By step 1.1 it belongs to its own class, so every listed class is nonempty. If an integer belonged to two listed classes, step 1.1 would force their representatives to equal its unique remainder. The eight representatives are distinct, so no two of their classes have a common element. Since each class is nonempty, the classes are distinct and pairwise disjoint. [F2, F8, step 1.1]

3.1 Let $h$ be the integer part of $t$ and put $M=h+1$. By [F3] and [F14], $0\le t<M$ in $\mathbb R$. If $M\le0$, transitivity in [F8] would give $M\le t$, contradicting $t<M$. Thus $0<M$ in $\mathbb R$, so $0<M$ in $\mathbb Z$ by order reflection in [F9]. Using the set $\mathcal S$ from step 2.1, the conditions defining $C(t)$ give a subset of $\mathbb Z$ by [F10]. Each $n\in C(t)$ is positive in $\mathbb Z$ and satisfies $n\le t<M$ in $\mathbb R$. By transitivity $n\le M$, and $n=M$ would contradict $t<M$. Hence $n<M$ in $\mathbb R$ by [F14], so $0<n<M$ in $\mathbb Z$ by [F9]. [given, F3, F8, F9, F10, F14, step 2.1]

4.1 By [F4] there is a unique $m\in\mathbb N$ with $\iota(m)=M$. By [F10], form $B=\{n\in\mathbb Z:0\le n<M\}$. Restrict $\iota$ to the predecessor set $m\subseteq\mathbb N$. Each $j\in m$ satisfies $j<m$ by [F5], so $0\le\iota(j)<\iota(m)=M$ by [F4]. The restriction therefore has one value in $B$ for each $j\in m$ and is a function $m\to B$ by [F12]. [F4, F5, F10, F12, step 3.1]

5.1 The restriction is injective by [F4]. For any $n\in B$, [F4] gives a unique natural $j$ with $\iota(j)=n$. Since $n<M=\iota(m)$, [F4] gives $j<m$, so $j\in m$ by [F5]. The function $m\to B$ is thus surjective and is a bijection by [F11]. Since $|m|=m$ by [F6], the bijection gives $|B|=m$ and $B$ is finite. [F4, F5, F6, F11, step 4.1]

6.1 Every element of $C(t)$ satisfies the defining conditions of $B$ by step 3.1, so $C(t)\subseteq B$ by [F10]. By [F7], $C(t)$ is finite, and [F6] gives a unique value $|C(t)|$. Thus the eight classes and their counting function $A(t)$ are well defined for every real $t\ge0$. [F6, F7, F10, step 2.1, step 3.1, step 2.2, step 5.1] ∎
