---
title: Intersection of the unit image and the normalizer
status: published
research_item: lem-euler-hurwitz-units-in-normalizer
dependency_level: 7
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §3.3, unit-image intersection preceding the orbit definition
      reading_limits: Read the opening of §3.3 through the intersection claim on PDF
        p. 4 for attribution.
---

PDF p. 4: ` §3.3, unit-image intersection preceding the orbit definition `

## Prerequisites

- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [math:def-invertible-element](https://alphabetamath.cc/item/def-invertible-element)
- [math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring)
- [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer)
- [math:def-normalizer-of-a-subgroup](https://alphabetamath.cc/item/def-normalizer-of-a-subgroup)
- [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)
- [lem-euler-hurwitz-normalizer-coordinate-test](item-lem-euler-hurwitz-normalizer-coordinate-test)


## Statement

Let $p\in\mathcal P_3$, the set of primes congruent to $3$ modulo $4$, and let $\mathbb F_p=\mathbb Z/p\mathbb Z$ be the field of integer residue classes modulo $p$. In the rational Hamilton quaternion algebra each element has unique coordinates in $1,i,j,k$ with rational coefficients. Multiplication distributes over sums, commutes with rational scalars, and obeys $i^2=j^2=-1$ and $k=ij=-ji$. Its Hurwitz order $\mathcal H$ is the subring of quaternions whose four coordinates are either all integers or all integers plus $\tfrac12$. Write $\mathcal H^\times$ for its units, the elements $u$ with $uv=vu=1$ for some $v\in\mathcal H$.

Write $\bar x=x+p\mathcal H$ for the residue of $x\in\mathcal H$ in $R_p=\mathcal H/p\mathcal H$, the ring of additive cosets of $p\mathcal H=\{ph:h\in\mathcal H\}$ with operations on representatives. Use the fixed reduction isomorphism $\bar\Phi_p:R_p\to M_2(\mathbb F_p)$, a bijection preserving addition, multiplication, identity and scalars into the algebra of two-by-two matrices with row-by-column multiplication. In $G_p=\mathrm{PGL}_2(\mathbb F_p)$ an invertible matrix $A$ represents the class $[A]=\{tA:t\in\mathbb F_p,\ t\ne0\}$, and classes multiply on representatives. Invertibility means having a two-sided multiplicative inverse. For $x$ with invertible residue define its projective reduction $\rho_p(x)=[\bar\Phi_p(\bar x)]$. Put $\Gamma_p=\{\rho_p(u):u\in\mathcal H^\times\}$.

Let $E_p=\{a+b\bar i:a,b\in\mathbb F_p\}$ be the field in $R_p$ with the inherited operations, and let $C_p$ be the group of classes $[\bar\Phi_p(e)]$ with $e\in E_p$ nonzero. Its normalizer is $K_p=\{g\in G_p:gC_pg^{-1}=C_p\}$, where $gC_pg^{-1}=\{gcg^{-1}:c\in C_p\}$. Then the elements common to $\Gamma_p$ and $K_p$ are exactly the four distinct classes
$$\Gamma_p\cap K_p=\{\rho_p(1),\rho_p(i),\rho_p(j),\rho_p(k)\}.$$

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[math:def-field](https://alphabetamath.cc/item/def-field)

[def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)

[def-euler-hurwitz-order](item-def-euler-hurwitz-order)

[math:def-invertible-element](https://alphabetamath.cc/item/def-invertible-element)

[math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring)

[lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction)

[def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer)

[math:def-normalizer-of-a-subgroup](https://alphabetamath.cc/item/def-normalizer-of-a-subgroup)

## Facts & Assumptions

[F1] Since $p\in\mathcal P_3$, it is a prime greater than $2$. Integer residues are equal exactly when their representatives differ by a multiple of $p$, so the residue of $2$ is nonzero. Nonzero elements of the prime residue field have multiplicative inverses. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n) [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer) [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field) [math:def-field](https://alphabetamath.cc/item/def-field)

[F2] The rational Hamilton coordinates are taken in the order $1,i,j,k$, and $\mathcal H$ has the same identity and operations as the ambient algebra on its elements. In a ring a two-sided inverse of $u$ is an element $v$ with $uv=vu=1$. [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions) [def-euler-hurwitz-order](item-def-euler-hurwitz-order) [math:def-invertible-element](https://alphabetamath.cc/item/def-invertible-element)

[F3] The quotient map $x\mapsto\bar x$ preserves addition, multiplication and $1$. In $R_p$ each element has a unique expansion in $1,\bar i,\bar j,\bar k$ over $\mathbb F_p$, as established in step 2.1 of the torus construction. The reduction isomorphism $\bar\Phi_p$ preserves the scalar action and is injective. Projective classes of invertible matrices are equal exactly when the matrices are nonzero scalar multiples of one another. The map $\rho_p$ takes the class of the reduced matrix. [math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring) [def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer) [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction) [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[F4] The units of $\mathcal H$ are $\pm1,\pm i,\pm j,\pm k$ and $(\varepsilon_0+\varepsilon_1 i+\varepsilon_2 j+\varepsilon_3 k)/2$ with each $\varepsilon_r\in\{1,-1\}$. [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)

[F5] For an invertible $q=a+b\bar i+c\bar j+d\bar k$ in $R_p$, its matrix class belongs to $K_p$ exactly when $(a,b)=(0,0)$ or $(c,d)=(0,0)$. [lem-euler-hurwitz-normalizer-coordinate-test](item-lem-euler-hurwitz-normalizer-coordinate-test)

## Proof

**Given:** $p\in\mathcal P_3$ and the projective reduction and normalizer defined above using the same $\bar\Phi_p$.

**Goal:** Identify the elements common to $\Gamma_p$ and $K_p$ and show that the four listed classes are distinct.

1.1 If $u\in\mathcal H^\times$ has inverse $v\in\mathcal H$, reduction of $uv=vu=1$ gives $\bar u\bar v=\bar v\bar u=1$. Thus $\bar u$ is invertible in $R_p$ and the projective reduction and coordinate test apply to every unit. [F2, F3, F5]

2.1 For $x\in\{1,i,j,k\}$, the residues of $x$ and $-x$ have just one nonzero coordinate, equal to $1$ and $-1$ respectively in the same position. Each residue has a zero coordinate pair, so their classes lie in $K_p$. The residues differ by the nonzero scalar $-1$, so $\rho_p(-x)=\rho_p(x)$. The eight units of this form therefore contribute the four listed classes to $\Gamma_p\cap K_p$. [F1, F3, F4, F5, step 1.1]

2.2 For a unit $u=(\varepsilon_0+\varepsilon_1 i+\varepsilon_2 j+\varepsilon_3 k)/2$, reduce the equality $2u=\varepsilon_0+\varepsilon_1 i+\varepsilon_2 j+\varepsilon_3 k$. Using the inverse of $2$ in $\mathbb F_p$ gives the four residue coordinates $\varepsilon_0 2^{-1},\varepsilon_1 2^{-1},\varepsilon_2 2^{-1},\varepsilon_3 2^{-1}$. All four are nonzero because $1$ and $-1$ are nonzero in the field and each is multiplied by an invertible scalar. Both coordinate pairs are consequently nonzero, so the class of $u$ lies outside $K_p$. [F1, F3, F4, F5, step 1.1]

3.1 If two of the four listed classes were equal, their matrices would be nonzero scalar multiples of each other. By injectivity and scalar preservation of $\bar\Phi_p$, their residues would then be nonzero scalar multiples of each other in $R_p$. The single nonzero coordinates of two different members of the list occur in different positions, and a nonzero scalar preserves that position by the unique expansion in [F3]. The four classes are thus distinct. The unit list is exhausted by steps 2.1 and 2.2, proving the asserted intersection. [F3, F4, step 2.1, step 2.2] ∎
