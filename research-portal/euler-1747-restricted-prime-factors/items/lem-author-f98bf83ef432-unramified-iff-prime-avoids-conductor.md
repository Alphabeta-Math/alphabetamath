---
id: lem-author-f98bf83ef432-unramified-iff-prime-avoids-conductor
kind: lemma
title: Unramified primes of a finite conductor
status: published
domain: mathematics
deps:
  - math:def-prime
  - math:def-divides-in-z
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - def-author-f98bf83ef432-finite-conductor
  - def-author-f98bf83ef432-local-conductor-exponent
  - lem-author-f98bf83ef432-unramified-iff-conductor-exponent-zero
  - math:cor-euclids-lemma-for-finite-products
  - math:def-monoid-finite-product
  - math:def-group-power
  - def-degree-two-projective-linear-group
  - math:thm-int-ordered-ring
  - math:def-rational-local-fields
  - def-author-f98bf83ef432-local-k-one-subgroup
  - math:thm-generalised-associativity
formulation_deps:
  - math:def-prime
  - math:def-divides-in-z
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - def-author-f98bf83ef432-finite-conductor
  - def-author-f98bf83ef432-local-conductor-exponent
  - lem-author-f98bf83ef432-unramified-iff-conductor-exponent-zero
  - def-degree-two-projective-linear-group
  - math:def-rational-local-fields
  - def-author-f98bf83ef432-local-k-one-subgroup
argument_deps:
  - math:def-prime
  - math:def-divides-in-z
  - def-author-f98bf83ef432-finite-conductor
  - def-author-f98bf83ef432-local-conductor-exponent
  - lem-author-f98bf83ef432-unramified-iff-conductor-exponent-zero
  - math:cor-euclids-lemma-for-finite-products
  - math:def-monoid-finite-product
  - math:def-group-power
  - math:thm-int-ordered-ring
  - math:def-rational-local-fields
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - def-author-f98bf83ef432-local-k-one-subgroup
  - def-degree-two-projective-linear-group
  - math:thm-generalised-associativity
dependency_roles:
  def-degree-two-projective-linear-group: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp: mathematical-premise
  def-author-f98bf83ef432-finite-conductor: mathematical-premise
  def-author-f98bf83ef432-local-conductor-exponent: mathematical-premise
  lem-author-f98bf83ef432-unramified-iff-conductor-exponent-zero: mathematical-premise
  math:cor-euclids-lemma-for-finite-products: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
  math:def-group-power: mathematical-premise
  math:def-rational-local-fields: mathematical-premise
  def-author-f98bf83ef432-local-k-one-subgroup: mathematical-premise
  math:thm-generalised-associativity: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

Let $(\rho_q)_q$ be a family of complex representations of $\mathrm{GL}_2(\mathbb Q_q)$ indexed by the primes. Suppose each conductor exponent $a(\rho_q)$ exists and only finitely many are positive, so the finite conductor is $C=\prod_q q^{a(\rho_q)}$. For a prime $\ell$, the representation $\rho_\ell$ is unramified, meaning $\mathrm{GL}_2(\mathbb Z_\ell)$ fixes a nonzero vector, if and only if $\ell\nmid C$. Here $\ell\nmid C$ means that $C$ is not an integer multiple of $\ell$.

## Statement references

[[math:def-prime|Prime integers]]

[[math:def-divides-in-z|Integer divisibility]]

[[math:def-rational-local-fields|Rational local fields]]

[[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp|Integral subring of the local field]]

[[def-author-f98bf83ef432-local-k-one-subgroup|Locality of the integral subring]]

[[def-degree-two-projective-linear-group|General linear group]]

[[def-author-f98bf83ef432-finite-conductor|Finite conductor]]

[[def-author-f98bf83ef432-local-conductor-exponent|Complex representations, fixed spaces and the local conductor exponent]]

[[lem-author-f98bf83ef432-unramified-iff-conductor-exponent-zero|Unramifiedness and exponent zero]]

## Facts & Assumptions

[F1] Each conductor exponent is a nonnegative integer and its power uses the corresponding natural exponent. The finite conductor uses the primes of positive exponent in increasing order. Integer multiplication is a commutative monoid with identity $1$. The finite product starts at $1$ and appends factors by multiplication, and the natural powers of $q$ follow this recursion with each appended factor equal to $q$. [[def-author-f98bf83ef432-finite-conductor|Finite conductor]] [[def-author-f98bf83ef432-local-conductor-exponent|Local conductor exponent]] [[math:thm-int-ordered-ring|Ordered integer ring]] [[math:def-monoid-finite-product|Finite products]] [[math:def-group-power|Natural powers]]

[F2] A prime dividing a finite product divides some factor, with the implication also valid for the empty product. A prime dividing another prime equals it, since the dividing prime is positive and greater than $1$. [[math:cor-euclids-lemma-for-finite-products|Euclid’s lemma for finite products]] [[math:def-prime|Prime integers]] [[math:def-divides-in-z|Integer divisibility]]

[F3] For the given local representations, unramifiedness is equivalent to conductor exponent zero. [[lem-author-f98bf83ef432-unramified-iff-conductor-exponent-zero|Unramifiedness and exponent zero]]

[F4] For each prime $q$, the field $\mathbb Q_q$ is the completion of $\mathbb Q$ at the prime place $q$. Its closed unit ball is the canonically embedded ring $\mathbb Z_q$, which is local by the locality argument for the congruence subgroups. For a field or local ring, the general linear group uses two-sided matrix inverses and matrix multiplication given by the entry formulas. [[math:def-rational-local-fields|Rational local fields]] [[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp|Canonical embedding and closed unit ball]] [[def-author-f98bf83ef432-local-k-one-subgroup|Locality of the integral subring]] [[def-degree-two-projective-linear-group|General linear group and entry formulas]]

[F5] A finite product in a monoid may be computed by grouping consecutive blocks or by splitting off a first block. In a commutative monoid, permuting the list preserves its product. [[math:thm-generalised-associativity|Splitting, regrouping and permutation of finite products]]

## Proof

**Given:** The family, its finite conductor $C$, and the prime $\ell$.

**Goal:** Identify $\ell\nmid C$ with unramifiedness of $\rho_\ell$.

1.1 By [F4], the field $\mathbb Q_q$ and the local ring $\mathbb Z_q$ both meet the coefficient-ring hypothesis for the matrix groups in the statement. The canonical embedding preserves sums, products and the identity, so it sends an invertible integral matrix and its inverse to inverse matrices over the field. Since it is injective on entries, this realizes the integral group as a subgroup of the group over the field. [F4]

1.2 Replace each prime power in the increasing list from [F1] by a block of that many copies of its prime, using the conductor exponent as the block length. For a fixed prime $q$, the products of lists of copies of $q$ have the same initial value and recursion as the natural powers of $q$, so each block product is the corresponding prime power. Apply the regrouping law in [F5] with cuts at the cumulative block lengths. Thus $C$ is the product of the concatenated list of primes, including the empty list with product $1$. [F1, F5]

2.1 If $a(\rho_\ell)>0$, the concatenated list contains $\ell$. By [F5], permute one occurrence of $\ell$ to the front, then split off the first factor. This gives $C=\ell B$, where $B$ is the integer product of the remaining list, so $\ell\mid C$. Conversely, if $\ell\mid C$, [F2] gives a factor of the concatenated list divisible by $\ell$. That factor is prime and therefore equals $\ell$, so $a(\rho_\ell)>0$. For the empty list, [F2] precludes $\ell\mid C$. [F1, F2, F5, step 1.2]

3.1 Since the conductor exponent is nonnegative, step 2.1 gives $\ell\nmid C$ exactly when $a(\rho_\ell)=0$. By [F3] this is exactly the unramified condition. [F1, F3, step 1.1, step 2.1] ∎
