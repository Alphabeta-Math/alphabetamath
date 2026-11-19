---
title: The torus normalizer detects a vanishing coordinate pair
status: published
research_item: lem-euler-hurwitz-normalizer-coordinate-test
dependency_level: 6
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §3.3, opening paragraph; right multiplication as in p. 2, §3.1,
        (3.2)
      reading_limits: Attribution for the coordinate criterion and the multiplication
        convention in the cited passages.
---

PDF p. 4: ` §3.3, description of pair vanishing and multiplication by 1 + i `

## Prerequisites

- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)
- [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring)
- [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-normalizer-of-a-subgroup](https://alphabetamath.cc/item/def-normalizer-of-a-subgroup)


## Statement

Let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$. Write $\mathbb F_p=\mathbb Z/p\mathbb Z$ for the field of integer residue classes modulo $p$, with addition and multiplication on representatives. Let $\mathcal H$ be the Hurwitz order, the subring of the rational Hamilton quaternions whose coordinates in $1,i,j,k$ are all integers or all integers plus $\tfrac12$, with $i^2=j^2=-1$ and $k=ij=-ji$. Put $R_p=\mathcal H/p\mathcal H$, the ring of additive cosets $x+p\mathcal H$ with addition and multiplication on representatives, and write $\bar i,\bar j,\bar k$ for the images of $i,j,k$.

Write $G_p=\mathrm{PGL}_2(\mathbb F_p)$ for the group of invertible two-by-two matrices over $\mathbb F_p$ up to multiplication by nonzero scalars, with product induced by matrix multiplication. For $q\in R_p$ invertible, meaning that it has a two-sided multiplicative inverse, let $[q]$ be the class of its matrix under the fixed reduction isomorphism $\bar\Phi_p:R_p\to M_2(\mathbb F_p)$, a bijection preserving addition, multiplication, identity and scalar multiplication. For $x\in\mathcal H$ with invertible reduction, write $\rho_p(x)=[x+p\mathcal H]$.

Let $E_p=\{a+b\bar i:a,b\in\mathbb F_p\}$ and let $C_p$ be the projective image of its nonzero elements, called the nonsplit torus. Here $E_p$ is a field with the inherited operations and identity, and each of its elements has unique coefficients $a,b\in\mathbb F_p$. Write $K_p=C_p\cup C_p\rho_p(j)$ for its normalizer, the subgroup of $g\in G_p$ with $gC_pg^{-1}=C_p$, where $gC_pg^{-1}=\{gcg^{-1}:c\in C_p\}$. The right coset $C_p\rho_p(j)$ is $\{c\rho_p(j):c\in C_p\}$.

For an invertible $q=a+b\bar i+c\bar j+d\bar k$ in $R_p$, its first pair $(a,b)$ or its second pair $(c,d)$ equals $(0,0)$ if and only if $[q]\in K_p$. The reduction of $1+i$ is invertible, its class $\rho_p(1+i)$ belongs to $C_p$, and right multiplication by the reduction of $1+i$ preserves the vanishing-pair condition in both directions.

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)

[math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[math:def-field](https://alphabetamath.cc/item/def-field)

[def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)

[def-euler-hurwitz-order](item-def-euler-hurwitz-order)

[math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring)

[lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction)

[def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer)

[math:def-coset](https://alphabetamath.cc/item/def-coset)

[math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)

[math:def-normalizer-of-a-subgroup](https://alphabetamath.cc/item/def-normalizer-of-a-subgroup)

## Facts & Assumptions

[F1] A prime $p\in\mathcal P_3$ satisfies $p=4h+3$ for some integer $h$, so $p>2$. Integer residue classes are equal exactly when their representatives differ by a multiple of $p$. Addition and multiplication on representatives make these classes a field for prime $p$. In a field every nonzero element has a multiplicative inverse. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n) [math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n) [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field) [math:def-field](https://alphabetamath.cc/item/def-field)

[F2] The Hurwitz order contains $1,i,j,k$. The quotient operations preserve the relations $\bar i^2=\bar j^2=-1$ and $\bar i\bar j=\bar k=-\bar j\bar i$. Step 2.1 of the torus construction gives unique coordinates in $1,\bar i,\bar j,\bar k$ over $\mathbb F_p$. Step 3.1 there establishes that $E_p$ is a field with the inherited operations and identity, so every nonzero element of $E_p$ is invertible in $R_p$. [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions) [def-euler-hurwitz-order](item-def-euler-hurwitz-order) [math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring) [def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer) [math:def-field](https://alphabetamath.cc/item/def-field)

[F3] For odd prime $p$ the fixed reduction isomorphism sends $t1$ to the scalar matrix $tI_2$, with $I_2$ the two-by-two identity matrix. Projective classes of invertible matrices agree exactly up to a nonzero scalar multiple and multiply on representatives. The projective reduction $\rho_p$ on elements with invertible reduction is the class of their reduced matrix. [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction) [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[F4] The subgroup $K_p$ consists of the classes of the nonzero elements of $E_p$ and their right products with $\rho_p(j)=[\bar j]$. A subgroup contains the ambient identity and is closed under multiplication and inverses. [def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer) [math:def-coset](https://alphabetamath.cc/item/def-coset) [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)

## Proof

**Given:** $p\in\mathcal P_3$ and an invertible $q=a+b\bar i+c\bar j+d\bar k$ in $R_p$.

**Goal:** Characterize membership of $[q]$ in $K_p$ by the two coordinate pairs, establish $\rho_p(1+i)\in C_p$, and prove preservation under right multiplication.

1.1 Put $u=a+b\bar i$ and $v=c+d\bar i$. Since $\bar i\bar j=\bar k$, one has $q=u+v\bar j$. Coordinate uniqueness gives $u=0$ exactly when $(a,b)=(0,0)$ and $v=0$ exactly when $(c,d)=(0,0)$. Also $q\ne0$, since $q$ is invertible and the embedded scalar field has $1\ne0$. [given, F1, F2, F3]

1.2 Set $w=1+\bar i$, the reduction of $1+i$. Both products $(1+\bar i)(1-\bar i)$ and $(1-\bar i)(1+\bar i)$ equal $2$ by $\bar i^2=-1$. Since $p>2$, the residue of $2$ is nonzero in $\mathbb F_p$, and the scalar $2^{-1}$ gives $w^{-1}=2^{-1}(1-\bar i)$. Thus $w$ is a nonzero element of $E_p$ and $\rho_p(1+i)=[w]\in C_p\subseteq K_p$. [F1, F2, F3, F4]

2.1 If $v=0$, then $q=u$ is a nonzero element of $E_p$, so $[q]\in C_p$. If $u=0$, then $q=v\bar j$ with $v\ne0$. Here $\bar j$ has inverse $-\bar j$, so $[q]=[v][\bar j]\in C_p\rho_p(j)$. In either case $[q]\in K_p$. [F2, F3, F4, step 1.1]

2.2 Conversely, if $[q]\in K_p$, take $e\in E_p$ nonzero such that $[q]=[e]$ or $[q]=[e][\bar j]=[e\bar j]$. Equality of classes and the scalar-preserving isomorphism give $q=te$ in the first case and $q=te\bar j$ in the second, for some nonzero $t\in\mathbb F_p$. Since $te\in E_p$, coordinate uniqueness gives $v=0$ in the first case and $u=0$ in the second. [F2, F3, F4, step 1.1]

3.1 The product $qw$ has inverse $w^{-1}q^{-1}$ by associativity, and $[qw]=[q][w]$. If $[q]\in K_p$, then $[qw]\in K_p$ by closure under products. If $[qw]\in K_p$, then $[q]=[qw][w]^{-1}\in K_p$ by closure under inverses and products. Applying the coordinate criterion from steps 2.1 and 2.2 to $q$ and $qw$ shows that the vanishing-pair condition holds for $qw$ exactly when it holds for $q$. This proves the coordinate criterion, the class membership for $1+i$, and preservation. [F3, F4, step 1.1, step 1.2, step 2.1, step 2.2] ∎
