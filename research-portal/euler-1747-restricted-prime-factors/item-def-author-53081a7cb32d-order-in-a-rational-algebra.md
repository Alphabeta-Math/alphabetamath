---
title: Orders in rational algebras
status: published
research_item: def-author-53081a7cb32d-order-in-a-rational-algebra
dependency_level: 0
---

## Prerequisites

- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)
- [math:def-subring](https://alphabetamath.cc/item/def-subring)
- [math:def-rat-operations](https://alphabetamath.cc/item/def-rat-operations)
- [math:thm-rat-field](https://alphabetamath.cc/item/thm-rat-field)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:def-ring](https://alphabetamath.cc/item/def-ring)
- [math:lem-subgroups-of-z-are-cyclic](https://alphabetamath.cc/item/lem-subgroups-of-z-are-cyclic)
- [math:lem-group-homomorphism-basic-properties](https://alphabetamath.cc/item/lem-group-homomorphism-basic-properties)
- [math:lem-integer-multiples-in-a-ring](https://alphabetamath.cc/item/lem-integer-multiples-in-a-ring)
- [math:thm-int-comm-ring](https://alphabetamath.cc/item/thm-int-comm-ring)


## Definition

Write $\mathbb Q$ for the rationals, whose elements are fractions of integers with nonzero denominator. Use the usual rational addition and multiplication, which make $\mathbb Q$ a commutative ring with identity $1_{\mathbb Q}=1/1$. An integer $n\in\mathbb Z$ is read as a rational scalar by the embedding $n\mapsto n/1$.

Let $A$ be a rational algebra, meaning a ring with identity and a specified map $\eta:\mathbb Q\to A$ that preserves addition, multiplication and identity and whose values commute with every element of $A$. For $q\in\mathbb Q$ and $a\in A$, let $q\cdot a=\eta(q)a$. Finite sums in $A$ use its commutative additive monoid, with empty sum $0_A$.

A **$\mathbb Z$-order in $A$** is a subring $S\subseteq A$, meaning it contains $1_A$ and is closed under addition, additive inverses and multiplication, with the following two properties.

- There is a fixed finite list $s_1,\ldots,s_r$ of elements of $S$ such that $S=\{\sum_{j=1}^r (n_j/1)\cdot s_j : n_1,\ldots,n_r\in\mathbb Z\}$.
- For every $a\in A$ there are a finite list $t_1,\ldots,t_m$ of elements of $S$ and rational coefficients $q_1,\ldots,q_m\in\mathbb Q$ such that $a=\sum_{j=1}^m q_j\cdot t_j$.

An order $S$ is **maximal** if every order $T$ in $A$ with $S\subseteq T$ satisfies $T=S$.

## Definition references

[The integers](https://alphabetamath.cc/item/def-integers)

[Rational numbers](https://alphabetamath.cc/item/def-rationals)

[Rational arithmetic](https://alphabetamath.cc/item/def-rat-operations)

[The rational field](https://alphabetamath.cc/item/thm-rat-field)

[The embedding of integers into rationals](https://alphabetamath.cc/item/lem-int-embeds-rat)

[Rings with identity](https://alphabetamath.cc/item/def-ring)

[Algebras over a commutative ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)

[Finite sums in a commutative monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)

[Subrings](https://alphabetamath.cc/item/def-subring)

## Justification

The subring conditions give $S$ the ring operations and identity inherited from $A$. Write $f(n)=\eta(n/1)$. The integer embedding and the scalar map are additive, and the rational identity $1_{\mathbb Q}=1/1$ gives $f(1)=1_A$. In the additive group of $\mathbb Z$, step 1.2 of [the cyclic-subgroup lemma](https://alphabetamath.cc/item/lem-subgroups-of-z-are-cyclic) with $g=1$ identifies the additive $n$-th power of $1$ with the integer product $1\cdot n$. The multiplicative identity law [for the integers](https://alphabetamath.cc/item/thm-int-comm-ring) gives $1\cdot n=n$. The additive group homomorphism $f$ preserves these powers [by the power law for group homomorphisms](https://alphabetamath.cc/item/lem-group-homomorphism-basic-properties), so $f(n)$ is the additive $n$-th power of $1_A$. For positive $n$ this power is the sum of $n$ copies of $1_A$, for $n=0$ it is $0_A$, and for negative $n$ it is the additive inverse of the corresponding positive sum.

The distributivity consequence $(n\,1_A)s=ns$ for signed additive multiples [in a ring](https://alphabetamath.cc/item/lem-integer-multiples-in-a-ring) gives $(n/1)\cdot s=f(n)s=ns$. Closure under addition and additive inverses, together with $0_A\in S$, keeps all the sums in the first condition in $S$. The second condition uses sums in $A$, where all the rational scalar products are defined. Maximality compares the resulting orders by inclusion.
