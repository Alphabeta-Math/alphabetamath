---
title: Zero conductor exponent and unramifiedness
status: published
research_item: lem-author-f98bf83ef432-unramified-iff-conductor-exponent-zero
dependency_level: 2
---

## Prerequisites

- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)
- [def-author-f98bf83ef432-local-k-one-subgroup](item-def-author-f98bf83ef432-local-k-one-subgroup)
- [def-author-f98bf83ef432-local-conductor-exponent](item-def-author-f98bf83ef432-local-conductor-exponent)


## Statement

Let $q$ be prime and let $\rho$ be a complex representation of the invertible two-by-two matrices over the $q$-adic field $\mathbb Q_q$. Suppose its conductor exponent $a(\rho)$ is defined, so some $K_{1,q}(n)$ fixes a nonzero vector and $a(\rho)$ is the smallest such $n\ge0$. Then $\rho$ is unramified, meaning $\mathrm{GL}_2(\mathbb Z_q)$ fixes a nonzero vector, if and only if $a(\rho)=0$.

## Statement references

[Prime integers](https://alphabetamath.cc/item/def-prime)

[General linear group](item-def-degree-two-projective-linear-group)

[The local field and its integral subring](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)

[Local congruence subgroups](item-def-author-f98bf83ef432-local-k-one-subgroup)

[Complex representations, fixed spaces and the local conductor exponent](item-def-author-f98bf83ef432-local-conductor-exponent)

## Facts & Assumptions

[F1] For a subgroup of the representation group, the fixed space consists of the vectors fixed by every element of that subgroup. The conductor exponent is the least nonnegative integer $n$ for which $K_{1,q}(n)$ has a nonzero fixed vector. [Fixed spaces and the local conductor exponent](item-def-author-f98bf83ef432-local-conductor-exponent)

[F2] At exponent zero the congruence subgroup equals the full integral group. [Local congruence subgroups](item-def-author-f98bf83ef432-local-k-one-subgroup)

## Proof

**Given:** The representation $\rho$ with conductor exponent $a(\rho)$.

**Goal:** Show that unramifiedness is equivalent to $a(\rho)=0$.

1.1 If the integral group fixes a nonzero vector then exponent zero already satisfies the fixed-vector condition by [F2]. It is the least possible nonnegative exponent, so $a(\rho)=0$. [F1, F2]

2.1 If $a(\rho)=0$, the minimum belongs to the set of exponents with nonzero fixed space by [F1]. Thus the full integral group fixes a nonzero vector by [F2]. This proves the equivalence. [F1, F2, step 1.1] ∎
