---
id: def-euler-hurwitz-order
kind: definition
title: The Hurwitz order
status: draft
domain: mathematics
deps:
  - def-euler-hamilton-quaternions
  - math:def-natural-numbers
  - math:def-nat-addition
  - math:lem-nat-embeds-int
  - math:def-integers
  - math:lem-int-embeds-rat
  - math:thm-rat-field
  - math:def-subring
  - def-author-53081a7cb32d-order-in-a-rational-algebra
  - thm-hurwitz-order-integral-structure
formulation_deps:
  - def-euler-hamilton-quaternions
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:def-integers
  - math:lem-int-embeds-rat
  - math:thm-rat-field
  - math:def-subring
  - def-author-53081a7cb32d-order-in-a-rational-algebra
argument_deps:
  - def-euler-hamilton-quaternions
  - math:def-natural-numbers
  - math:def-nat-addition
  - math:lem-nat-embeds-int
  - math:def-integers
  - math:lem-int-embeds-rat
  - math:thm-rat-field
  - math:def-subring
  - def-author-53081a7cb32d-order-in-a-rational-algebra
  - thm-hurwitz-order-integral-structure
dependency_roles:
  math:def-natural-numbers: mathematical-premise
  math:def-nat-addition: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  math:def-integers: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:thm-rat-field: mathematical-premise
  math:def-subring: mathematical-premise
  def-author-53081a7cb32d-order-in-a-rational-algebra: mathematical-premise
  thm-hurwitz-order-integral-structure: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §3.1, displayed definition of the order
dependency_level: 2
---

## Definition

Let $B$ be the rational Hamilton quaternion algebra, whose elements have unique expressions $a+bi+cj+dk$ with $a,b,c,d\in\mathbb Q$. Write $\mathbb Z$ for the integers, identified with their images $n/1$ in $\mathbb Q$. Put $\mathbb Z+\tfrac12=\{n+\tfrac12:n\in\mathbb Z\}$, where $\tfrac12$ is the inverse of $2$ in $\mathbb Q$. For a set $S$ of rational numbers, $S^4$ denotes the set of ordered quadruples with all four entries in $S$.

The **Hurwitz order** $\mathcal H$ is the subset of $B$ with coordinate set
$$\mathbb Z^4\cup(\mathbb Z+\tfrac12)^4$$
in the basis $1,i,j,k$. Its addition and multiplication are inherited from $B$.

A **$\mathbb Z$-order in $B$** is a subring of $B$ that equals the set of integer linear combinations of some finite list of its elements and whose elements give all of $B$ by rational linear combinations. Here a subring contains $1$ and is closed under addition, additive inverses and multiplication.

## Facts & Assumptions

[F1] The rational Hamilton quaternion algebra consists of the real Hamilton quaternions with rational coordinates. Its operations are inherited from the real quaternions, its rational scalars act by multiplication by $t1$ for $t\in\mathbb Q$, and its coordinates in the basis $1,i,j,k$ are unique. [[def-euler-hamilton-quaternions|The rational Hamilton quaternion algebra]]

[F2] The integers $\mathbb Z$ are classes of pairs of natural numbers, with $(a,b)$ and $(c,d)$ in the same class exactly when $a+d=b+c$. [[math:def-integers|The integers]] The equation $a+d=b+c$ uses natural-number addition. [[math:def-nat-addition|Addition of natural numbers]] The map $n\mapsto n/1$ from $\mathbb Z$ into $\mathbb Q$ is injective and preserves addition and multiplication. [[math:lem-int-embeds-rat|The embedding of integers into rationals]]

[F3] The rationals $\mathbb Q$ form a field, so rational addition is defined everywhere and a nonzero rational has a multiplicative inverse in $\mathbb Q$. [[math:thm-rat-field|The rational field]]

[F4] A subring contains the ambient identity and is closed under addition, additive inverses and multiplication. [[math:def-subring|Subrings]] A $\mathbb Z$-order in a rational algebra is such a subring with a finite list of additive generators over $\mathbb Z$ and with rational span equal to the ambient algebra. [[def-author-53081a7cb32d-order-in-a-rational-algebra|Orders in rational algebras]]

[F5] In the rational-coordinate subalgebra of the real Hamilton quaternions, the set $O$ of integer linear combinations of $1,i,j,(-1+i+j+k)/2$ is a $\mathbb Z$-order. Its coordinate set in the basis $1,i,j,k$ is $\mathbb Z^4\cup(\mathbb Z+\tfrac12)^4$. [[thm-hurwitz-order-integral-structure|Integral structure of the Hurwitz order]]

[F6] The natural numerals $0=\varnothing$ and $2=\{0,1\}$ are distinct. [[math:def-natural-numbers|The natural numbers]] Natural-number addition gives $0+0=0$. [[math:def-nat-addition|Addition of natural numbers]] A natural numeral is viewed in $\mathbb Q$ by the map $e$ obtained by composing the additive injections $n\mapsto[(n,0)]$ into $\mathbb Z$ and $m\mapsto m/1$ into $\mathbb Q$. [[math:lem-nat-embeds-int|The embedding of naturals into integers]] [[math:lem-int-embeds-rat|The embedding of integers into rationals]]

## Justification

The proof below establishes that the rational denominator is nonzero. The integer embedding and rational addition then make both coordinate classes subsets of the rationals. Uniqueness of the four coordinates makes membership a predicate on elements of $B$. The proof below verifies the subring, generation and spanning conditions for the inherited operations.

## Proof

**Given:** The rational Hamilton quaternion algebra $B$ and the embeddings in [F2] and [F6].

**Goal:** Verify that the coordinate prescription is well-defined and gives a $\mathbb Z$-order in $B$.

1.1 Since $0+0=0$, additivity gives $e(0)+e(0)=e(0)$. Cancelling in the additive group of $\mathbb Q$ gives $e(0)=0_{\mathbb Q}$. Injectivity and $2\ne0$ in $\mathbb N$ give $e(2)\ne e(0)$. The rational numeral $e(2)$ is therefore nonzero and has the multiplicative inverse $\tfrac12$. [F3, F6]

2.1 Both an integer and its sum with $\tfrac12$ are rational. Each ordered quadruple from either part of the displayed union therefore gives an element of $B$, and each element of $B$ has just one coordinate quadruple. [F1, F2, F3, step 1.1]

3.1 The carrier, inherited operations, scalar action and ordered basis in [F1] are those of the rational Hamilton algebra in [F5]. Thus the coordinate set of $O$ from [F5] is precisely the defining coordinate set of $\mathcal H$ in this same algebra. Coordinate uniqueness gives $\mathcal H=O$. [F1, F5, step 2.1]

4.1 Under the inherited operations, $O$ contains $1$, is closed under addition, additive inverses and multiplication, and has the finite integer generation and rational spanning properties in [F4], since [F5] makes it a $\mathbb Z$-order. All those properties hold for $\mathcal H$ by step 3.1. Hence the displayed prescription defines a $\mathbb Z$-order in $B$. [F4, F5, step 3.1] ∎
