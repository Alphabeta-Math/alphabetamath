---
title: Unramified primes of a finite conductor
status: draft
research_item: lem-author-f98bf83ef432-unramified-iff-prime-avoids-conductor
dependency_level: 3
---

## Prerequisites

- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)
- [def-author-f98bf83ef432-finite-conductor](item-def-author-f98bf83ef432-finite-conductor)
- [def-author-f98bf83ef432-local-conductor-exponent](item-def-author-f98bf83ef432-local-conductor-exponent)
- [lem-author-f98bf83ef432-unramified-iff-conductor-exponent-zero](item-lem-author-f98bf83ef432-unramified-iff-conductor-exponent-zero)
- [math:cor-euclids-lemma-for-finite-products](https://alphabetamath.cc/item/cor-euclids-lemma-for-finite-products)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-rational-local-fields](https://alphabetamath.cc/item/def-rational-local-fields)
- [def-author-f98bf83ef432-local-k-one-subgroup](item-def-author-f98bf83ef432-local-k-one-subgroup)
- [math:thm-generalised-associativity](https://alphabetamath.cc/item/thm-generalised-associativity)


## Statement

Let $(\rho_q)_q$ be a family of complex representations of $\mathrm{GL}_2(\mathbb Q_q)$ indexed by the primes. Suppose each conductor exponent $a(\rho_q)$ exists and only finitely many are positive, so the finite conductor is $C=\prod_q q^{a(\rho_q)}$. For a prime $\ell$, the representation $\rho_\ell$ is unramified, meaning $\mathrm{GL}_2(\mathbb Z_\ell)$ fixes a nonzero vector, if and only if $\ell\nmid C$. Here $\ell\nmid C$ means that $C$ is not an integer multiple of $\ell$.

## Statement references

[Prime integers](https://alphabetamath.cc/item/def-prime)

[Integer divisibility](https://alphabetamath.cc/item/def-divides-in-z)

[Rational local fields](https://alphabetamath.cc/item/def-rational-local-fields)

[Integral subring of the local field](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)

[Locality of the integral subring](item-def-author-f98bf83ef432-local-k-one-subgroup)

[General linear group](item-def-degree-two-projective-linear-group)

[Finite conductor](item-def-author-f98bf83ef432-finite-conductor)

[Complex representations, fixed spaces and the local conductor exponent](item-def-author-f98bf83ef432-local-conductor-exponent)

[Unramifiedness and exponent zero](item-lem-author-f98bf83ef432-unramified-iff-conductor-exponent-zero)

## Facts & Assumptions

[F1] Each conductor exponent is a nonnegative integer and its power uses the corresponding natural exponent. The finite conductor uses the primes of positive exponent in increasing order. Integer multiplication is a commutative monoid with identity $1$. The finite product starts at $1$ and appends factors by multiplication, and the natural powers of $q$ follow this recursion with each appended factor equal to $q$. [Finite conductor](item-def-author-f98bf83ef432-finite-conductor) [Local conductor exponent](item-def-author-f98bf83ef432-local-conductor-exponent) [Ordered integer ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [Finite products](https://alphabetamath.cc/item/def-monoid-finite-product) [Natural powers](https://alphabetamath.cc/item/def-group-power)

[F2] A prime dividing a finite product divides some factor, with the implication also valid for the empty product. A prime dividing another prime equals it, since the dividing prime is positive and greater than $1$. [Euclid’s lemma for finite products](https://alphabetamath.cc/item/cor-euclids-lemma-for-finite-products) [Prime integers](https://alphabetamath.cc/item/def-prime) [Integer divisibility](https://alphabetamath.cc/item/def-divides-in-z)

[F3] For the given local representations, unramifiedness is equivalent to conductor exponent zero. [Unramifiedness and exponent zero](item-lem-author-f98bf83ef432-unramified-iff-conductor-exponent-zero)

[F4] For each prime $q$, the field $\mathbb Q_q$ is the completion of $\mathbb Q$ at the prime place $q$. Its closed unit ball is the canonically embedded ring $\mathbb Z_q$, which is local by the locality argument for the congruence subgroups. For a field or local ring, the general linear group uses two-sided matrix inverses and matrix multiplication given by the entry formulas. [Rational local fields](https://alphabetamath.cc/item/def-rational-local-fields) [Canonical embedding and closed unit ball](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp) [Locality of the integral subring](item-def-author-f98bf83ef432-local-k-one-subgroup) [General linear group and entry formulas](item-def-degree-two-projective-linear-group)

[F5] A finite product in a monoid may be computed by grouping consecutive blocks or by splitting off a first block. In a commutative monoid, permuting the list preserves its product. [Splitting, regrouping and permutation of finite products](https://alphabetamath.cc/item/thm-generalised-associativity)

## Proof

**Given:** The family, its finite conductor $C$, and the prime $\ell$.

**Goal:** Identify $\ell\nmid C$ with unramifiedness of $\rho_\ell$.

1.1 By [F4], the field $\mathbb Q_q$ and the local ring $\mathbb Z_q$ both meet the coefficient-ring hypothesis for the matrix groups in the statement. The canonical embedding preserves sums, products and the identity, so it sends an invertible integral matrix and its inverse to inverse matrices over the field. Since it is injective on entries, this realizes the integral group as a subgroup of the group over the field. [F4]

1.2 Replace each prime power in the increasing list from [F1] by a block of that many copies of its prime, using the conductor exponent as the block length. For a fixed prime $q$, the products of lists of copies of $q$ have the same initial value and recursion as the natural powers of $q$, so each block product is the corresponding prime power. Apply the regrouping law in [F5] with cuts at the cumulative block lengths. Thus $C$ is the product of the concatenated list of primes, including the empty list with product $1$. [F1, F5]

2.1 If $a(\rho_\ell)>0$, the concatenated list contains $\ell$. By [F5], permute one occurrence of $\ell$ to the front, then split off the first factor. This gives $C=\ell B$, where $B$ is the integer product of the remaining list, so $\ell\mid C$. Conversely, if $\ell\mid C$, [F2] gives a factor of the concatenated list divisible by $\ell$. That factor is prime and therefore equals $\ell$, so $a(\rho_\ell)>0$. For the empty list, [F2] precludes $\ell\mid C$. [F1, F2, F5, step 1.2]

3.1 Since the conductor exponent is nonnegative, step 2.1 gives $\ell\nmid C$ exactly when $a(\rho_\ell)=0$. By [F3] this is exactly the unramified condition. [F1, F3, step 1.1, step 2.1] ∎
