---
title: A Hecke point value equals the normalized orbit pairing
status: published
research_item: lem-euler-hurwitz-orbit-average
dependency_level: 7
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §3.3, the two invariance assertions and (3.7)
      reading_limits: Read the relevant passage on PDF p. 4 for attribution.
---

PDF p. 4: ` §3.3, invariance and equation (3.7) `

## Prerequisites

- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer)
- [def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit)
- [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)
- [def-author-87b4d85727bc-counting-inner-product-on-finite-functions](item-def-author-87b4d85727bc-counting-inner-product-on-finite-functions)
- [lem-euler-hurwitz-hecke-basic-properties](item-lem-euler-hurwitz-hecke-basic-properties)
- [math:def-group](https://alphabetamath.cc/item/def-group)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [math:lem-finite-sum-reindexing-and-fubini](https://alphabetamath.cc/item/lem-finite-sum-reindexing-and-fubini)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)


## Statement

Let $m$ be a positive odd integer, so $m>0$ and $m=2a+1$ for some integer $a$. Let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$, with $p\nmid m$, meaning $m$ is not an integer multiple of $p$.

Use the fixed projective reduction $\rho_p$ at $p$. Its target $G_p$ is the group of invertible two-by-two matrices over the field $\mathbb F_p$ of integer residues modulo $p$, identified up to nonzero scalar multiples. The projective reduction sends a quaternion in the order whose reduced norm is not divisible by $p$ to the matrix class assigned to its residue by the fixed identification of the reduced Hurwitz order with the two-by-two matrix ring. Two elements of the order have the same residue when their difference is $p$ times an element of the order. A rational Hamilton quaternion has rational coordinates in the basis $1,i,j,k$, with multiplication determined by $i^2=j^2=-1$ and $ij=k=-ji$. Its reduced norm is the sum of the four coordinate squares. The Hurwitz order consists of the quaternions whose coordinates are all integers or all integers plus $\tfrac12$. The subgroup $\Gamma_p$ is the image of the Hurwitz units, the elements of the order with a two-sided inverse in that order. Write $Y_p=\Gamma_p\backslash G_p$ for the finite set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$, with $\Gamma_p$ the coset of the group identity $e$.

Let $C_p$ be the projective image of the nonzero elements of $\mathbb F_p[i]$, the field of residues of the form $a+b\bar i$ with $a,b\in\mathbb F_p$ and $\bar i$ the reduction of the basis quaternion $i$ modulo $p$. Let $K_p$ be the normalizer of $C_p$ in $G_p$, the subgroup consisting of $k$ for which $\{kck^{-1}:c\in C_p\}=C_p$. The orbit of $\Gamma_p$ under right translation by $K_p$ is the set of its translates $\mathcal O_p=\{\Gamma_p k:k\in K_p\}$. Its indicator $f_p$ is the complex-valued function on $Y_p$ equal to $1$ on $\mathcal O_p$ and $0$ elsewhere.

For a complex-valued function $f$ on $Y_p$, use the Hecke operator of index $m$ at $p$, given by
$$(T_m f)(\Gamma_p g)=\frac{1}{24}\sum_{\alpha\in Q_m} f(\Gamma_p\rho_p(\alpha)g),$$
where $Q_m$ is the set of Hurwitz quaternions whose reduced norm equals $m$. The sum has one term for each $\alpha\in Q_m$ and is $0$ when $Q_m$ is empty.

Both $f_p$ and $T_m f_p$ are invariant under right translation by $K_p$. This means that each of these functions $h$ satisfies $h(\Gamma_p gk)=h(\Gamma_p g)$ for all $g\in G_p$ and $k\in K_p$. Moreover,
$$(T_m f_p)(\Gamma_p)=\frac{\langle f_p,T_m f_p\rangle_p}{|\mathcal O_p|},$$
where $|\mathcal O_p|$ is the number of elements of $\mathcal O_p$ and $\langle f,h\rangle_p=\sum_{y\in Y_p}f(y)\overline{h(y)}$ is the counting inner product on complex functions on $Y_p$. In the denominator, a count $j$ denotes the image in $\mathbb C$ of the sum of $j$ copies of the real unit $1$. The bar on a complex number denotes conjugation, which sends $a+bi$ to $a-bi$ for real $a,b$ and the complex imaginary unit $i$.

## Statement references

[def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)

[def-euler-hurwitz-order](item-def-euler-hurwitz-order)

[def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer)

[def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit)

[def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)

[def-author-87b4d85727bc-counting-inner-product-on-finite-functions](item-def-author-87b4d85727bc-counting-inner-product-on-finite-functions)

[math:def-group](https://alphabetamath.cc/item/def-group)

[math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)

[math:def-coset](https://alphabetamath.cc/item/def-coset)

[math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

[math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)

## Facts & Assumptions

[F1] The fixed reduction gives a nonempty finite coset set $Y_p$ and a subgroup $K_p$ of $G_p$. Right translation on $Y_p$ sends $\Gamma_p g$ to $\Gamma_p(gk)$ independently of the representative $g$. Successive translations by $k$ and $t$ are translation by $kt$, and translation by $e$ fixes every coset. In particular, $\Gamma_p$ translates to $\Gamma_p k$, and the set of these translates is exactly the set where $f_p=1$. A group has associative multiplication, and a subgroup contains the identity and is closed under products and inverses. [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer) [def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit) [math:def-group](https://alphabetamath.cc/item/def-group) [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)

[F2] For a positive odd integer $m$ and a prime $p\in\mathcal P_3$ with $p\nmid m$, the Hecke operator is well-defined on the complex functions on $Y_p$. It satisfies $R_k(T_m f)=T_m(R_k f)$ with $(R_k f)(\Gamma_p g)=f(\Gamma_p(gk))$ for $k\in K_p\subseteq G_p$. It is self-adjoint for the counting inner product, meaning $\langle T_m f,h\rangle_p=\langle f,T_m h\rangle_p$ for all complex functions $f,h$ on $Y_p$. [lem-euler-hurwitz-hecke-basic-properties](item-lem-euler-hurwitz-hecke-basic-properties)

[F3] In the counting inner product the second input is conjugated. Complex conjugation fixes $0$ and $1$. The complex field contains $\mathbb R$ via an embedding that preserves $0$, $1$ and addition, and every nonzero complex number has a multiplicative inverse. The reals form an ordered field, so $1>0$ and the sum of two positive reals is positive. [def-author-87b4d85727bc-counting-inner-product-on-finite-functions](item-def-author-87b4d85727bc-counting-inner-product-on-finite-functions) [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus) [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field) [math:thm-reals-ordered-field](https://alphabetamath.cc/item/thm-reals-ordered-field)

[F4] Subsets of a finite set are finite. A finite set can be listed without repetition with length equal to its cardinality, and it has cardinality zero exactly when empty. Finite sums can be split over two disjoint sets. For a finite listing with terms $a_0,\ldots,a_{r-1}$, its partial sums satisfy $S_0=0$ and $S_{j+1}=S_j+a_j$ for $0\le j<r$. Induction on the length of a sum uses the case of zero terms and the implication from each length to its successor. [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:lem-finite-sum-reindexing-and-fubini](https://alphabetamath.cc/item/lem-finite-sum-reindexing-and-fubini) [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid) [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

## Proof

**Given:** $m>0$ odd and $p\in\mathcal P_3$ with $p\nmid m$, with all groups, functions and operators taken in the same fixed reduction at $p$.

**Goal:** Prove that $f_p$ and $T_m f_p$ are invariant under $K_p$ and identify the value of $T_m f_p$ at $\Gamma_p$.

1.1 Let $k\in K_p$ and $y\in Y_p$. If $y=\Gamma_p t$ for some $t\in K_p$, then right translation by $k$ sends $y$ to $\Gamma_p(tk)\in\mathcal O_p$ because $tk\in K_p$. Conversely, if translating $y$ by $k$ gives $\Gamma_p s$ with $s\in K_p$, translating that coset by $k^{-1}$ gives $y=\Gamma_p(sk^{-1})\in\mathcal O_p$. These two implications show that $f_p$ has the same value before and after translation, so $R_k f_p=f_p$ for each $k\in K_p$. [F1, F2]

2.1 Because the hypotheses of [F2] hold for the chosen $m$ and $p$, $R_k(T_m f_p)=T_m(R_k f_p)=T_m f_p$. Thus $T_m f_p$ is invariant under $K_p$. Every $y\in\mathcal O_p$ is obtained by translating $\Gamma_p$ by some $k\in K_p$. Hence $(T_m f_p)(y)=c$ on $\mathcal O_p$, where $c=(T_m f_p)(\Gamma_p)$. [given, F1, F2, step 1.1]

3.1 The identity $e$ belongs to $K_p$, so $\Gamma_p=\Gamma_p e$ lies in $\mathcal O_p$. As a nonempty subset of the finite set $Y_p$, the orbit has a positive number $n=|\mathcal O_p|$ of elements. Using the constant value established in step 2.1, together with self-adjointness and the counting formula,
$$\langle f_p,T_m f_p\rangle_p=\langle T_m f_p,f_p\rangle_p=\sum_{y\in Y_p}(T_m f_p)(y)\overline{f_p(y)}.$$
The summands on $\mathcal O_p$ equal $c$ and those on its complement equal $0$, since $\overline{1}=1$ and $\overline{0}=0$. Split the sum over these two sets, both finite subsets of $Y_p$. The partial sum on the complement remains zero by induction, since it starts at zero and every added term is zero. Let $r_j$ be the real sum of $j$ copies of $1$ and $z_j$ its complex image. The partial-sum rules give $r_0=0$ and $r_{j+1}=r_j+1$, so the embedding gives $z_0=0$ and $z_{j+1}=z_j+1$. The sum of $j$ copies of $c$ is $z_jc$ by induction. It is zero for $j=0$, and adding one more $c$ yields $z_jc+c=(z_j+1)c=z_{j+1}c$. Thus the orbit sum and the pairing both equal $z_nc$. [F1, F2, F3, F4, step 2.1]

4.1 The real sums satisfy $r_1=1>0$. If $r_j>0$, then $r_{j+1}=r_j+1>0$ by the ordered-field laws. Induction gives $r_j>0$ for every positive count $j$. Since $n>0$, we have $r_n>0$, so injectivity of the real embedding gives $z_n\ne0$. Dividing the pairing by $z_n$ gives $c=(T_m f_p)(\Gamma_p)$, which is the stated identity by the convention for the denominator. [F3, F4, step 1.1, step 2.1, step 3.1] ∎
