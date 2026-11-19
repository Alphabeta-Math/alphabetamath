---
title: The Hurwitz order
status: published
research_item: def-euler-hurwitz-order
dependency_level: 2
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §3.1, displayed definition of the order
---

PDF p. 2: ` §3.1, displayed definition of the order `

## Prerequisites

- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:thm-rat-field](https://alphabetamath.cc/item/thm-rat-field)
- [math:def-subring](https://alphabetamath.cc/item/def-subring)
- [def-author-53081a7cb32d-order-in-a-rational-algebra](item-def-author-53081a7cb32d-order-in-a-rational-algebra)
- [thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure)


## Definition

Let $B$ be the rational Hamilton quaternion algebra, whose elements have unique expressions $a+bi+cj+dk$ with $a,b,c,d\in\mathbb Q$. Write $\mathbb Z$ for the integers, identified with their images $n/1$ in $\mathbb Q$. Put $\mathbb Z+\tfrac12=\{n+\tfrac12:n\in\mathbb Z\}$, where $\tfrac12$ is the inverse of $2$ in $\mathbb Q$. For a set $S$ of rational numbers, $S^4$ denotes the set of ordered quadruples with all four entries in $S$.

The **Hurwitz order** $\mathcal H$ is the subset of $B$ with coordinate set
$$\mathbb Z^4\cup(\mathbb Z+\tfrac12)^4$$
in the basis $1,i,j,k$. Its addition and multiplication are inherited from $B$.

A **$\mathbb Z$-order in $B$** is a subring of $B$ that equals the set of integer linear combinations of some finite list of its elements and whose elements give all of $B$ by rational linear combinations. Here a subring contains $1$ and is closed under addition, additive inverses and multiplication.

## Facts & Assumptions

[F1] The rational Hamilton quaternion algebra consists of the real Hamilton quaternions with rational coordinates. Its operations are inherited from the real quaternions, its rational scalars act by multiplication by $t1$ for $t\in\mathbb Q$, and its coordinates in the basis $1,i,j,k$ are unique. [The rational Hamilton quaternion algebra](item-def-euler-hamilton-quaternions)

[F2] The integers $\mathbb Z$ are classes of pairs of natural numbers, with $(a,b)$ and $(c,d)$ in the same class exactly when $a+d=b+c$. [The integers](https://alphabetamath.cc/item/def-integers) The equation $a+d=b+c$ uses natural-number addition. [Addition of natural numbers](https://alphabetamath.cc/item/def-nat-addition) The map $n\mapsto n/1$ from $\mathbb Z$ into $\mathbb Q$ is injective and preserves addition and multiplication. [The embedding of integers into rationals](https://alphabetamath.cc/item/lem-int-embeds-rat)

[F3] The rationals $\mathbb Q$ form a field, so rational addition is defined everywhere and a nonzero rational has a multiplicative inverse in $\mathbb Q$. [The rational field](https://alphabetamath.cc/item/thm-rat-field)

[F4] A subring contains the ambient identity and is closed under addition, additive inverses and multiplication. [Subrings](https://alphabetamath.cc/item/def-subring) A $\mathbb Z$-order in a rational algebra is such a subring with a finite list of additive generators over $\mathbb Z$ and with rational span equal to the ambient algebra. [Orders in rational algebras](item-def-author-53081a7cb32d-order-in-a-rational-algebra)

[F5] In the rational-coordinate subalgebra of the real Hamilton quaternions, the set $O$ of integer linear combinations of $1,i,j,(-1+i+j+k)/2$ is a $\mathbb Z$-order. Its coordinate set in the basis $1,i,j,k$ is $\mathbb Z^4\cup(\mathbb Z+\tfrac12)^4$. [Integral structure of the Hurwitz order](item-thm-hurwitz-order-integral-structure)

[F6] The natural numerals $0=\varnothing$ and $2=\{0,1\}$ are distinct. [The natural numbers](https://alphabetamath.cc/item/def-natural-numbers) Natural-number addition gives $0+0=0$. [Addition of natural numbers](https://alphabetamath.cc/item/def-nat-addition) A natural numeral is viewed in $\mathbb Q$ by the map $e$ obtained by composing the additive injections $n\mapsto[(n,0)]$ into $\mathbb Z$ and $m\mapsto m/1$ into $\mathbb Q$. [The embedding of naturals into integers](https://alphabetamath.cc/item/lem-nat-embeds-int) [The embedding of integers into rationals](https://alphabetamath.cc/item/lem-int-embeds-rat)

## Justification

The proof below establishes that the rational denominator is nonzero. The integer embedding and rational addition then make both coordinate classes subsets of the rationals. Uniqueness of the four coordinates makes membership a predicate on elements of $B$. The proof below verifies the subring, generation and spanning conditions for the inherited operations.

## Proof

**Given:** The rational Hamilton quaternion algebra $B$ and the embeddings in [F2] and [F6].

**Goal:** Verify that the coordinate prescription is well-defined and gives a $\mathbb Z$-order in $B$.

1.1 Since $0+0=0$, additivity gives $e(0)+e(0)=e(0)$. Cancelling in the additive group of $\mathbb Q$ gives $e(0)=0_{\mathbb Q}$. Injectivity and $2\ne0$ in $\mathbb N$ give $e(2)\ne e(0)$. The rational numeral $e(2)$ is therefore nonzero and has the multiplicative inverse $\tfrac12$. [F3, F6]

2.1 Both an integer and its sum with $\tfrac12$ are rational. Each ordered quadruple from either part of the displayed union therefore gives an element of $B$, and each element of $B$ has just one coordinate quadruple. [F1, F2, F3, step 1.1]

3.1 The carrier, inherited operations, scalar action and ordered basis in [F1] are those of the rational Hamilton algebra in [F5]. Thus the coordinate set of $O$ from [F5] is precisely the defining coordinate set of $\mathcal H$ in this same algebra. Coordinate uniqueness gives $\mathcal H=O$. [F1, F5, step 2.1]

4.1 Under the inherited operations, $O$ contains $1$, is closed under addition, additive inverses and multiplication, and has the finite integer generation and rational spanning properties in [F4], since [F5] makes it a $\mathbb Z$-order. All those properties hold for $\mathcal H$ by step 3.1. Hence the displayed prescription defines a $\mathbb Z$-order in $B$. [F4, F5, step 3.1] ∎
