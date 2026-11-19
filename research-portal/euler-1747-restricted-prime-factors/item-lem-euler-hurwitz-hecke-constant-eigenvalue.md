---
title: The Hecke eigenvalue on constants
status: draft
research_item: lem-euler-hurwitz-hecke-constant-eigenvalue
dependency_level: 6
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, §3.2, constant eigenvalue following (3.4)
      reading_limits: Read the eigenvalue passage on PDF page 3 and the cited
        equations (2.1) and (3.2) on PDF page 2 for attribution.
---

PDF p. 3: ` §3.2, constant eigenvalue following (3.4) `

## Prerequisites

- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:def-function-space](https://alphabetamath.cc/item/def-function-space)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [def-euler-divisor-functions](item-def-euler-divisor-functions)
- [math:def-canonical-natural](https://alphabetamath.cc/item/def-canonical-natural)
- [math:def-eigenvalue-eigenvector-eigenspace-and-spectrum](https://alphabetamath.cc/item/def-eigenvalue-eigenvector-eigenspace-and-spectrum)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)
- [def-euler-four-square-representations](item-def-euler-four-square-representations)
- [lem-euler-hurwitz-four-square-bijection](item-lem-euler-hurwitz-four-square-bijection)
- [lem-euler-four-square-count](item-lem-euler-four-square-count)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:lem-nat-finite-sum-laws-and-the-canonical-embedding](https://alphabetamath.cc/item/lem-nat-finite-sum-laws-and-the-canonical-embedding)


## Statement

Let $m>0$ be an odd integer, so $m=2k+1$ for some integer $k$. Let $p\in\mathcal P_3$ be a prime congruent to $3$ modulo $4$, with $p\nmid m$, meaning that $m$ is not an integer multiple of $p$.

Use the quaternionic Hecke operator $T_m$ at $p$ on $\mathbb C[Y_p]$, the space of functions from $Y_p$ to the complex field $\mathbb C$ with scalar multiplication at each point. Here $G_p$ is the group of invertible two-by-two matrices over the field of residues modulo $p$, identified up to nonzero scalar multiples. The subgroup $\Gamma_p$ is the image of the Hurwitz units under the fixed projective reduction modulo $p$. Thus $Y_p=\Gamma_p\backslash G_p$ is the set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$ for $g\in G_p$.

Let $\mathbf1$ be the function with value $1$ at every coset. Write $m_{\mathbb N}$ for the unique positive natural number whose image under the canonical inclusion into the integers is $m$. Use $\sigma(m)$ as shorthand for $\sigma(m_{\mathbb N})$, the natural-number sum of the positive naturals whose integer images divide $m$. These images are exactly the positive integers $d$ such that $m=dq$ for some integer $q$. In scalar expressions, a natural number denotes its image in $\mathbb C$ under the canonical embedding of the natural numbers. Then
$$T_m\mathbf1=\sigma(m)\mathbf1.$$
Moreover, $\mathbf1$ is nonzero, so it is an eigenvector with eigenvalue $\sigma(m)$, meaning that applying $T_m$ to this nonzero vector equals scalar multiplication by $\sigma(m)$.

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)

[def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[math:def-coset](https://alphabetamath.cc/item/def-coset)

[math:def-function-space](https://alphabetamath.cc/item/def-function-space)

[math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

[def-euler-divisor-functions](item-def-euler-divisor-functions)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:def-canonical-natural](https://alphabetamath.cc/item/def-canonical-natural)

[math:def-eigenvalue-eigenvector-eigenspace-and-spectrum](https://alphabetamath.cc/item/def-eigenvalue-eigenvector-eigenspace-and-spectrum)

## Facts & Assumptions

[F1] The division algorithm by $2$ gives a unique quotient and remainder, with remainder $0$ or $1$. Divisibility by $2$ holds exactly for remainder $0$. [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

[F2] For positive odd $m$, $p\in\mathcal P_3$ and $p\nmid m$, the operator is a complex-linear map defined at every coset by the following formula. The index set $Q_m$ is finite. For each $\alpha\in Q_m$, the fixed reduction $\rho_p(\alpha)$ is in $G_p$, so $\Gamma_p\rho_p(\alpha)g$ belongs to $Y_p$. The projective reduction uses the fixed identification of Hurwitz residues modulo $p$ with two-by-two matrices over the residue field and takes the class of the resulting invertible matrix up to a nonzero scalar. Its image on the Hurwitz units, the elements with two-sided inverses in the Hurwitz order, is $\Gamma_p$. [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
$$(T_m f)(\Gamma_p g)=\frac1{24}\sum_{\alpha\in Q_m}f(\Gamma_p\rho_p(\alpha)g).$$

[F3] The shell $Q_m$ is the set of quaternions in the Hurwitz order with reduced norm $m$. In coordinates on the rational Hamilton quaternion basis $1,i,j,k$, the elements of the Hurwitz order have coordinates that are all integers or all integers plus $\tfrac12$, and the reduced norm is the sum of their four squares. Write $\mathcal R(2m)$ for the set of ordered integer quadruples whose squared entries sum to $2m$, with every sign and zero allowed, and $R(2m)=|\mathcal R(2m)|$ for its cardinality. [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell) [def-euler-four-square-representations](item-def-euler-four-square-representations)

[F4] If $m>0$ and $m=2k+1$ for an integer $k$, right multiplication by $1+i$ followed by taking the coordinate tuple is a bijection from $Q_m$ onto $\mathcal R(2m)$. A bijection pairs each element of one set with exactly one element of the other. [lem-euler-hurwitz-four-square-bijection](item-lem-euler-hurwitz-four-square-bijection)

[F5] The canonical inclusion of the naturals into the integers preserves order, sends $0$ to $0$, and gives every positive integer a unique positive natural preimage. If $m>0$ and $2\nmid m$, the four-square count gives $R(2m)=24\sigma(m_{\mathbb N})$ as an equality of natural numbers, where $m_{\mathbb N}$ is the positive natural corresponding to $m$. [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [def-euler-divisor-functions](item-def-euler-divisor-functions) [lem-euler-four-square-count](item-lem-euler-four-square-count)

[F6] The cardinality $|S|$ of a finite set $S$ is the length of a list of its elements without repetitions. A bijection from a finite set transports such a list to its target and preserves cardinality. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F7] A finite sum adds the terms in any enumeration of its index set. For complex numbers, the sum starts at $0$ and appending a term adds it to the preceding sum. Induction establishes an identity for every natural index by checking index $0$ and passage to its successor. [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid) [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F8] Write $\iota(n)$ for the canonical image of a natural number $n$ in $\mathbb C$. It starts at $\iota(0)=0$ and satisfies $\iota(n+1)=\iota(n)+1$. The canonical images in $\mathbb R$ preserve multiplication and are distinct for distinct natural numbers. The inclusion of $\mathbb R$ into the complex field preserves $0$, $1$, addition and multiplication and is injective, so these real images become the complex images by the same recursion. In particular, $\iota(24)\ne0$. [math:def-canonical-natural](https://alphabetamath.cc/item/def-canonical-natural) [math:lem-nat-finite-sum-laws-and-the-canonical-embedding](https://alphabetamath.cc/item/lem-nat-finite-sum-laws-and-the-canonical-embedding) [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

[F9] The group $G_p$ contains the class of the identity matrix $I_2$, which has ones on the diagonal and zeros elsewhere. Hence $Y_p$ contains the right coset $\Gamma_p[I_2]$. In $\mathbb C[Y_p]$ the zero function is zero at each coset, scalar multiplication takes place at each coset, and equality is tested at each coset. A nonzero vector $v$ is an eigenvector with eigenvalue $\lambda$ of a linear map $T$ from a vector space to itself exactly when $Tv=\lambda v$. [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group) [math:def-coset](https://alphabetamath.cc/item/def-coset) [math:def-function-space](https://alphabetamath.cc/item/def-function-space) [math:def-eigenvalue-eigenvector-eigenspace-and-spectrum](https://alphabetamath.cc/item/def-eigenvalue-eigenvector-eigenspace-and-spectrum)

## Proof

**Given:** A positive integer $m=2k+1$ with $k$ an integer and a prime $p\in\mathcal P_3$ with $p\nmid m$.

**Goal:** Show $T_m\mathbf1=\sigma(m)\mathbf1$ and $\mathbf1\ne0$.

1.1 The representation $m=2k+1$ has remainder $1$ upon division by $2$. The uniqueness in the division algorithm gives $2\nmid m$. Thus $m$ satisfies the hypotheses of both the bijection and the four-square count. [given, F1, F4, F5]

1.2 Fix a coset $\Gamma_p g\in Y_p$. Every argument $\Gamma_p\rho_p(\alpha)g$ with $\alpha\in Q_m$ belongs to $Y_p$, so every term in the formula for $(T_m\mathbf1)(\Gamma_p g)$ is $1$. Enumerate $Q_m$ without repetitions using $|Q_m|$ entries. The numerator in that formula is therefore a sum of $|Q_m|$ copies of $1$. [F2, F6, F7]

2.1 Apply the bijection from the finite shell $Q_m$ onto the ordered representations of $2m$ by four squares. Cardinality is preserved. Evaluating the divisor sum at the positive natural $m_{\mathbb N}$ corresponding to $m$, the four-square count gives the equality of natural numbers $|Q_m|=R(2m)=24\sigma(m_{\mathbb N})$. [F2, F3, F4, F5, F6, step 1.1]

3.1 The sum of the first zero copies is $0=\iota(0)$. If a sum of $j$ copies is $\iota(j)$, adding one more gives $\iota(j)+1=\iota(j+1)$. By induction the numerator in step 1.2 is $\iota(|Q_m|)$. Applying $\iota$ to the natural-number equality in step 2.1 gives $\iota(|Q_m|)=\iota(24)\iota(\sigma(m_{\mathbb N}))$ by preservation of multiplication. Cancelling the nonzero normalization factor $\iota(24)$ in the complex field yields $(T_m\mathbf1)(\Gamma_p g)=\iota(\sigma(m))$. [F7, F8, step 2.1, step 1.2]

4.1 The coset was arbitrary, and $(\sigma(m)\mathbf1)(\Gamma_p g)=\iota(\sigma(m))$ at every coset by pointwise scalar multiplication. Therefore $T_m\mathbf1=\sigma(m)\mathbf1$. At $\Gamma_p[I_2]$ the function $\mathbf1$ has value $1\ne0$, so the eigenvector condition holds with eigenvalue $\sigma(m)$. [F8, F9, step 3.1] ∎
