---
title: The recurrence set has size U(a)
status: published
research_item: lem-euler-finite-unrepresented-recurrence-equivalence
dependency_level: 6
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, equivalence of equations (7.2) and (7.3), p. 8, Table 1 caption
---

PDF p. 7: ` §7, equivalence of equations (7.2) and (7.3) `; PDF p. 8: ` Table 1 caption `

## Prerequisites

- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [def-author-c74aeff6099d-bounded-integer-indices](item-def-author-c74aeff6099d-bounded-integer-indices)
- [def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)
- [def-euler-finite-first-summand-indices](item-def-euler-finite-first-summand-indices)
- [alg-euler-finite-unrepresented-recurrence](item-alg-euler-finite-unrepresented-recurrence)
- [math:def-set-difference-and-symmetric-difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [def-euler-finite-unrepresented-count](item-def-euler-finite-unrepresented-count)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [lem-finite-deletions-and-translated-support](item-lem-finite-deletions-and-translated-support)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [lem-euler-finite-unrepresented-count-meaning](item-lem-euler-finite-unrepresented-count-meaning)
- [math:def-axiom-of-extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality)
- [math:def-indexed-family](https://alphabetamath.cc/item/def-indexed-family)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)


## Statement

Let $a$ be an integer cutoff with $1\le a\le313$ and $a\equiv1\pmod4$. For integers $v,w$, $v\equiv w\pmod4$ means $v-w=4q$ for some integer $q$, where subtraction adds the additive inverse. Write $m=(a-1)/4$ for the integer satisfying $a=4m+1$. For a nonnegative integer $B$, let $I_B$ be the integers from $0$ through $B$, including both endpoints.

Use $H=4{,}194{,}303$ and the certificate indicators $\varepsilon_j$ of (7.1). Each $\varepsilon_j$ is $0$ or $1$ for $j\in I_H$, and $\varepsilon_j=0$ for integers $j<0$. Let $J=\{i\in I_{78}:\varepsilon_i=1\}$ be the eligible first indices. Let $C(a)$ be the finite set left by the following repeated update. Start with $I_H$ and scan $i\in I_m$ in increasing order. At an index $i\in J$ remove every current element $k$ with $i\le k$ and $\varepsilon_{k-i}=1$. Removing these elements means keeping precisely the current elements outside the deletion set. At all other indices the set stays the same. A set is finite if it has a list of natural-number length consisting exactly of its elements, each appearing once.

For $k\in I_H$ write $P_k$ for the term at index $k$ in the sum defining $U(a)$:
$$P_k=\prod_{i\in I_m}(1-\varepsilon_i\varepsilon_{k-i}),\qquad U(a)=\sum_{k\in I_H}P_k.$$
The finite sum adds one term per index and the finite product multiplies one factor per index. They use the natural numbers $0,1,2,\ldots$, identified with their nonnegative integer copies. A difference $1-b$ for $b\in\{0,1\}$ is $1$ when $b=0$ and $0$ when $b=1$.

Let $\mathcal A$ be the set of positive integers whose prime divisors are all congruent to $1$ modulo $4$. An integer is positive if it is greater than $0$. A divisor of $x$ is an integer $d$ with $x=dq$ for an integer $q$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. A prime divisor is a divisor that is prime.

For every $k\in I_H$, the following are equivalent:

- $k$ belongs to $C(a)$.
- $P_k=1$.
- There are no $x,y\in\mathcal A$ with $x\le a$ and $4k+2=x+y$.

In particular, $|C(a)|=U(a)$, where the cardinality $|C(a)|$ is the length of a list consisting exactly of the elements of $C(a)$, each appearing once.

## Statement references

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:def-int-order](https://alphabetamath.cc/item/def-int-order)

[math:def-int-operations](https://alphabetamath.cc/item/def-int-operations)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

[def-author-c74aeff6099d-bounded-integer-indices](item-def-author-c74aeff6099d-bounded-integer-indices)

[def-euler-finite-certificate-indices](item-def-euler-finite-certificate-indices)

[def-euler-finite-first-summand-indices](item-def-euler-finite-first-summand-indices)

[alg-euler-finite-unrepresented-recurrence](item-alg-euler-finite-unrepresented-recurrence)

[math:def-set-difference-and-symmetric-difference](https://alphabetamath.cc/item/def-set-difference-and-symmetric-difference)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[def-euler-finite-unrepresented-count](item-def-euler-finite-unrepresented-count)

[math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

[math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

## Justification

The well-definedness proof for the recurrence gives a unique integer $m$ in the range $0\le m\le78$ and a unique finite set $C(a)$ for each allowed cutoff. [alg-euler-finite-unrepresented-recurrence](item-alg-euler-finite-unrepresented-recurrence)

The definition of $U(a)$ establishes that the factor at every $i\in I_m$ is defined for each $k\in I_H$. The finite product over these factors has a unique value, so $P_k$ names a definite term of $U(a)$. [def-euler-finite-unrepresented-count](item-def-euler-finite-unrepresented-count) [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

## Facts & Assumptions

[F1] The [well-definedness proof for the cutoff scan](item-alg-euler-finite-unrepresented-recurrence) constructs an [indexed family](https://alphabetamath.cc/item/def-indexed-family) $(E_j)_{j\in L}$. It assigns exactly one set $E_j$ of integers to each $j\in L$. Here $L$ consists of the natural numbers $j$ with $1\le j\le r$ in the [natural order](https://alphabetamath.cc/item/def-nat-order), and $r$ is the natural number whose integer copy is $m+1$. Write $\iota(j)$ for the [integer copy](https://alphabetamath.cc/item/lem-nat-embeds-int) of $j$. By step 2.1 of the cutoff scan proof, for each $j\in L$ the scan index $i=\iota(j)-1$ lies in $I_m$, and each $i\in I_m$ arises from exactly one $j\in L$ this way. The scan index increases as $j$ increases. At that scan index, if $i\in J$, $E_j$ consists of the $k\in I_H$ with $i\le k$ and $\varepsilon_{k-i}=1$. If $i\notin J$, then $E_j$ is empty. The last set is $C(a)$ and all its elements lie in $I_H$.

[F2] The [finite deletion invariant](item-lem-finite-deletions-and-translated-support) says that, for a finite starting set of integers and an indexed family of sets of integers on the natural numbers from $1$ through $r$, a starting element remains after all deletions exactly when it belongs to none of the deletion sets.

[F3] Each [bounded index set](item-def-author-c74aeff6099d-bounded-integer-indices) $I_B$ for nonnegative $B$ is finite. The [total order on the integers](https://alphabetamath.cc/item/thm-int-ordered-ring) is transitive, so $0\le m\le78$ implies that every $i\in I_m$ belongs to $I_{78}$. On $I_{78}$, the [definition of the eligible indices](item-def-euler-finite-first-summand-indices) gives $i\in J$ exactly when $\varepsilon_i=1$.

[F4] The [product-count lemma and its zero-factor criterion](item-lem-euler-finite-unrepresented-count-meaning) applies to the stated cutoff and certificate indicators. For $k\in I_H$ and $i\in I_m$ the factor at $i$ is zero exactly when $\varepsilon_i=\varepsilon_{k-i}=1$, which implies $i\le k$. A zero factor exists exactly when $4k+2=x+y$ for some $x,y\in\mathcal A$ with $x\le a$. The product at $k$ is $1$ exactly when no such equality exists, and $U(a)$ is the cardinality of the set of those indices with no such equality.

[F5] By [extensionality](https://alphabetamath.cc/item/def-axiom-of-extensionality), two sets with exactly the same elements are equal. A finite set has a unique cardinality by [the finite cardinality definition](https://alphabetamath.cc/item/def-finite-cardinality).

## Proof

**Given:** A cutoff $a$ and the certificate indicators in the Statement.

**Goal:** Identify the indices in $C(a)$ and prove $|C(a)|=U(a)$.

1.1 The starting set $I_H$ is a finite set of integers by [F3]. By [F1], each natural index from $1$ through $r$ has exactly one deletion set, which is a set of integers. Apply [F2] to $I_H$ and this family, whose deletions end at $C(a)$ by [F1]. For a fixed $k\in I_H$, exclusion from $C(a)$ is equivalent to membership in some $E_j$. If $k\in E_j$, the scan index $i=\iota(j)-1$ lies in $I_m$ and satisfies $i\in J$, $i\le k$ and $\varepsilon_{k-i}=1$ by [F1]. Conversely, if an $i\in I_m$ satisfies these three conditions, [F1] supplies the unique $j\in L$ with $i=\iota(j)-1$ and gives $k\in E_j$. Thus $k\notin C(a)$ exactly when some $i\in I_m$ satisfies those conditions. [given, F1, F2, F3]

2.1 An index $i$ satisfying the criterion in step 1.1 gives $\varepsilon_i=1$ by [F3], so the factor at $i$ is zero by [F4]. Conversely, a zero factor gives $\varepsilon_i=\varepsilon_{k-i}=1$ and $i\le k$ by [F4]. Since $i\in I_m$ gives $i\in I_{78}$, [F3] gives $i\in J$, so $i$ satisfies the deletion criterion in step 1.1. Thus $k$ belongs to $C(a)$ exactly when every factor of $P_k$ is nonzero. [F3, F4, step 1.1]

3.1 By [F4], having every factor nonzero is equivalent to the absence of the specified equality $4k+2=x+y$. The absence of that equality is equivalent to $P_k=1$ by the same lemma. This proves the three equivalent conditions. [F4, step 2.1]

4.1 All members of $C(a)$ belong to $I_H$ by [F1]. For each $k\in I_H$, step 3.1 gives exactly the membership condition of the finite set counted by $U(a)$ in [F4]. The two sets therefore have the same elements and are equal by [F5]. Taking their cardinalities gives $|C(a)|=U(a)$. [F1, F4, F5, step 3.1] ∎
