---
title: Well-definedness, equivariance and self-adjointness of the Hecke operator
status: draft
research_item: lem-euler-hurwitz-hecke-basic-properties
dependency_level: 6
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, §3.2, first three claims following (3.4)
      reading_limits: Read the displayed formula and the first three claims that
        follow it on PDF p. 3 for attribution.
---

PDF p. 3: ` §3.2, first three claims following (3.4) `

## Prerequisites

- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)
- [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [math:def-group](https://alphabetamath.cc/item/def-group)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:def-function-space](https://alphabetamath.cc/item/def-function-space)
- [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map)
- [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [def-author-87b4d85727bc-counting-inner-product-on-finite-functions](item-def-author-87b4d85727bc-counting-inner-product-on-finite-functions)
- [math:def-adjoint-of-a-linear-map-between-inner-product-spaces](https://alphabetamath.cc/item/def-adjoint-of-a-linear-map-between-inner-product-spaces)
- [lem-rational-hamilton-norm-and-inverse](item-lem-rational-hamilton-norm-and-inverse)
- [thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure)
- [lem-degree-two-projective-group-cardinality](item-lem-degree-two-projective-group-cardinality)
- [math:thm-standard-representatives-modulo-n](https://alphabetamath.cc/item/thm-standard-representatives-modulo-n)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:lem-finite-sum-reindexing-and-fubini](https://alphabetamath.cc/item/lem-finite-sum-reindexing-and-fubini)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [lem-finite-coset-inversion-and-adjoints](item-lem-finite-coset-inversion-and-adjoints)


## Statement

Let $m$ be a positive odd integer, so $m>0$ and $m=2k+1$ for some integer $k$. Let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$, with $p\nmid m$. Thus $m$ is not an integer multiple of $p$. Here a prime is an integer greater than $1$ with only positive divisors $1$ and itself, and the congruence means $4$ divides $p-3$.

Let $\mathcal H$ be the Hurwitz order in the rational Hamilton quaternions. A quaternion has unique rational coordinates in $1,i,j,k$, with associative multiplication given by $i^2=j^2=-1$ and $ij=k=-ji$ and extended by distributivity with rational scalars commuting with all quaternions. In $\mathcal H$ the four coordinates are all integers or all integers plus $\tfrac12$. For $\alpha=a+bi+cj+dk$, its reduced norm is $\operatorname{nrd}(\alpha)=a^2+b^2+c^2+d^2$, and its quaternion conjugate is $\bar\alpha=a-bi-cj-dk$. Put $Q_m=\{\alpha\in\mathcal H:\operatorname{nrd}(\alpha)=m\}$. Write $\mathcal H^\times$ for the group of units, the elements with a two-sided multiplicative inverse in $\mathcal H$. The left-unit class of $\alpha\in Q_m$ is $\mathcal H^\times\alpha=\{v\alpha:v\in\mathcal H^\times\}$.

Use the fixed projective reduction $\rho_p(\alpha)=[A_p(\alpha)]$ for elements whose reduced norm has nonzero residue modulo $p$. Here $A_p$ is the fixed map to two-by-two matrices over the field $\mathbb F_p$ of integer residues modulo $p$, obtained from the chosen identification of $\mathcal H/p\mathcal H$ with that matrix ring. In this residue ring two quaternions represent the same element when their difference lies in $p\mathcal H=\{p\beta:\beta\in\mathcal H\}$. The group $G_p=\mathrm{PGL}_2(\mathbb F_p)$ consists of classes of invertible two-by-two matrices, with matrices equivalent when one is a nonzero scalar multiple of the other, and product $[A][B]=[AB]$. Let $\Gamma_p=\rho_p(\mathcal H^\times)$ be the image subgroup and $Y_p=\Gamma_p\backslash G_p$ the set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$.

Write $\mathbb C[Y_p]$ for complex-valued functions on $Y_p$, with addition and scalar multiplication at each coset. The Hecke operator is specified by the following finite sum, with one term for each $\alpha\in Q_m$ and the empty sum equal to $0$.
$$(T_m f)(\Gamma_p g)=\frac1{24}\sum_{\alpha\in Q_m}f(\Gamma_p\rho_p(\alpha)g).$$

Right multiplication by each $u\in\mathcal H^\times$ permutes the left-unit classes in $Q_m$. The formula for $T_m$ is well-defined, meaning it gives the same value for every representative $g$ of the same coset, and defines a complex-linear map on $\mathbb C[Y_p]$, meaning it preserves complex linear combinations. For each $r\in G_p$ it commutes with right translation, meaning $T_mR_r=R_rT_m$ for $(R_rf)(\Gamma_p g)=f(\Gamma_p gr)$. It is self-adjoint, meaning $\langle T_m f,h\rangle_p=\langle f,T_m h\rangle_p$ for all $f,h\in\mathbb C[Y_p]$, with the counting inner product
$$\langle f,h\rangle_p=\sum_{y\in Y_p}f(y)\overline{h(y)}.$$
Here $\overline{h(y)}$ denotes complex conjugation, which sends $a+bi$ to $a-bi$ for real $a,b$ and the complex imaginary unit $i$. Quaternion conjugation permutes $Q_m$ and satisfies $\rho_p(\bar\alpha)=\rho_p(\alpha)^{-1}$ for every $\alpha\in Q_m$.

## Statement references

[Primes congruent to 3 modulo 4](item-def-euler-prime-classes)

[Integer divisibility](https://alphabetamath.cc/item/def-divides-in-z)

[Hamilton quaternions, reduced norm and conjugation](item-def-euler-hamilton-quaternions)

[The Hurwitz order](item-def-euler-hurwitz-order)

[The norm shell](item-def-euler-hurwitz-norm-shell)

[Hurwitz units](item-lem-euler-hurwitz-unit-list)

[Integer residues](https://alphabetamath.cc/item/def-integers-modulo-n)

[The field of prime residues](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[The degree-two projective group](item-def-degree-two-projective-linear-group)

[The fixed projective reduction and its quotient](item-def-euler-hurwitz-projective-reduction)

[Group laws](https://alphabetamath.cc/item/def-group)

[Subgroups](https://alphabetamath.cc/item/def-subgroup)

[Right cosets](https://alphabetamath.cc/item/def-coset)

[The complex field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

[Functions with pointwise operations](https://alphabetamath.cc/item/def-function-space)

[Linear maps](https://alphabetamath.cc/item/def-linear-map)

[Quaternionic Hecke operator](item-def-euler-hurwitz-hecke-operator)

[Finite sums](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)

[Counting inner product](item-def-author-87b4d85727bc-counting-inner-product-on-finite-functions)

[Adjoint pairing](https://alphabetamath.cc/item/def-adjoint-of-a-linear-map-between-inner-product-spaces)

## Facts & Assumptions

[F1] The set $\mathcal P_3$ consists of the primes congruent to $3$ modulo $4$, and $p\nmid m$ means there is no integer $q$ with $m=pq$. The residue field $\mathbb F_p$ consists of classes of integers with two integers in the same class when their difference is divisible by $p$. Since $p$ is prime, every nonzero class has a multiplicative inverse. The representatives $0,\ldots,p-1$ are distinct and exhaustive. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z) [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n) [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field) [math:thm-standard-representatives-modulo-n](https://alphabetamath.cc/item/thm-standard-representatives-modulo-n)

[F2] Quaternion multiplication is associative. The Hurwitz order contains $1$ and is closed under products. Its elements of reduced norm $m$ are exactly $Q_m$. Quaternion conjugation and the reduced norm are given by the coordinate formulas in the Statement. [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions) [def-euler-hurwitz-order](item-def-euler-hurwitz-order) [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)

[F3] The $24$ Hurwitz units form a group, and all have reduced norm $1$. A group has associative multiplication, an identity, and a two-sided inverse for each element. A subgroup contains the identity and is closed under products and inverses in the ambient group. The right coset of a subgroup $H$ represented by $g$ is $Hg=\{hg:h\in H\}$. [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list) [math:def-group](https://alphabetamath.cc/item/def-group) [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup) [math:def-coset](https://alphabetamath.cc/item/def-coset)

[F4] In the rational Hamilton algebra $\operatorname{nrd}(xy)=\operatorname{nrd}(x)\operatorname{nrd}(y)$ and $x\bar x=\bar x x=\operatorname{nrd}(x)1$. The coordinate set of the Hurwitz order is closed under quaternion conjugation, and the reduced norms of its elements are integers. [lem-rational-hamilton-norm-and-inverse](item-lem-rational-hamilton-norm-and-inverse) [thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure)

[F5] For the fixed reduction, $A_p$ preserves addition, multiplication and $1$. On the elements whose reduced norm is not divisible by $p$, $\rho_p(\alpha)=[A_p(\alpha)]$ is defined and preserves products. Projective matrix classes multiply by taking the class of the product, and the class of every nonzero scalar matrix equals $[I_2]$, the identity class. The image of the Hurwitz units is the subgroup $\Gamma_p$. Over a finite field of size $q$, the degree-two projective group has $q(q^2-1)$ elements. Thus $G_p$ is finite. The quotient $Y_p$ is finite and nonempty, with $\Gamma_p$ its identity coset. [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group) [lem-degree-two-projective-group-cardinality](item-lem-degree-two-projective-group-cardinality)

[F6] The defining sum for $T_m$ has coefficient $1/24$. The finiteness argument in step 1.1 of its definition embeds $Q_m$ into a finite set of bounded integer quadruples by doubling and shifting its coordinates. [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)

[F7] The cardinality $|E|$ counts the elements of a finite set $E$, and a one-to-one and onto map between finite sets preserves cardinality. Each subset of a finite set is finite. Finite sums in the additive system of the complex field are independent of enumeration, can be reindexed by a one-to-one and onto map, and split over two disjoint sets. Induction on a nonnegative integer is justified by proving the case $0$ and the implication from each case to its successor. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid) [math:lem-finite-sum-reindexing-and-fubini](https://alphabetamath.cc/item/lem-finite-sum-reindexing-and-fubini) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F8] The complex field contains the reals, so $1/24$ is a defined real scalar. The complex functions on $Y_p$ have pointwise vector operations, and a map between such function spaces is linear when it preserves every combination $af+bh$ with complex $a,b$. On the nonempty finite set $Y_p$, the counting formula is an inner product linear in the first input and conjugate symmetric, meaning $\langle f,h\rangle_p=\overline{\langle h,f\rangle_p}$. A linear map on this space is its own adjoint when it satisfies the pairing identity in the Statement. [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field) [math:def-function-space](https://alphabetamath.cc/item/def-function-space) [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map) [def-author-87b4d85727bc-counting-inner-product-on-finite-functions](item-def-author-87b4d85727bc-counting-inner-product-on-finite-functions) [math:def-adjoint-of-a-linear-map-between-inner-product-spaces](https://alphabetamath.cc/item/def-adjoint-of-a-linear-map-between-inner-product-spaces)

[F9] For a finite group $G$, a subgroup $H$ and nonnegative integer multiplicities $\nu(s)$ on $G$, the finite-coset averaging lemma applies if $\nu(sh)=\nu(s)$ for every $s\in G,h\in H$ and $\nu(s^{-1})=\nu(s)$ for every $s\in G$. Under these hypotheses the sum $F\mapsto[g\mapsto\sum_{s\in G}\nu(s)F(sg)]$ on functions on $G$ induces the linear map $S$ on functions on the right cosets with $(Sf)(Hg)=\sum_{s\in G}\nu(s)f(Hsg)$. This induced map is self-adjoint for the counting inner product on $H\backslash G$ and commutes with each right translation $(R_r f)(Hg)=f(Hgr)$. [lem-finite-coset-inversion-and-adjoints](item-lem-finite-coset-inversion-and-adjoints)

## Justification

Left multiplication by a unit of norm $1$ stays in $\mathcal H$ and preserves the reduced norm. The relation of differing by left multiplication by a unit is reflexive by $1$, symmetric by the inverse of the unit, and transitive by multiplication of units. Its classes are therefore the stated subsets of $Q_m$. For any $r\in G_p$, $\Gamma_p(gr)$ equals the set of products of elements of $\Gamma_p g$ with $r$ on the right by associativity. This makes $R_r$ a map on the indicated functions independent of the chosen representative.

## Proof

**Given:** $m>0$ odd, $p\in\mathcal P_3$, $p\nmid m$, and the fixed projective reduction at $p$.

**Goal:** Prove the permutation of left-unit classes, well-definedness and translation commutation of the Hecke formula, and self-adjointness by quaternion conjugation.

1.1 For $u\in\mathcal H^\times$ and $\alpha\in Q_m$, the product $\alpha u$ is in $\mathcal H$ and has norm $m\operatorname{nrd}(u)=m$. Right multiplication by $u^{-1}$ has the same property and is inverse to right multiplication by $u$ on $Q_m$. For any $v\in\mathcal H^\times$, $(v\alpha)u=v(\alpha u)$, so the first map sends the entire class $\mathcal H^\times\alpha$ onto $\mathcal H^\times(\alpha u)$. The inverse has the same compatibility with the classes. Thus right multiplication by $u$ permutes the classes. [F2, F3, F4]

1.2 The coordinate formula gives $\operatorname{nrd}(\bar\alpha)=\operatorname{nrd}(\alpha)$ and $\overline{\bar\alpha}=\alpha$. Since conjugation stays in $\mathcal H$, it is a permutation of $Q_m$. Both $\alpha$ and $\bar\alpha$ are in the domain of $\rho_p$ by $p\nmid m$. The norm identities give $\alpha\bar\alpha=\bar\alpha\alpha=m1$. The image under $A_p$ of $m1$, the sum of $m$ copies of $1$, is $(m\bmod p)I_2$ by preservation of addition and identity. Since this scalar matrix has nonzero scalar, its projective class is the identity. Taking classes in the two product identities gives $\rho_p(\bar\alpha)=\rho_p(\alpha)^{-1}$. [F1, F2, F4, F5]

2.1 For each $s\in G_p$ put $Q_s'=\{\alpha\in Q_m:\rho_p(\alpha)=s\}$ and $\nu(s)=|Q_s'|$. These counts exist because each $Q_s'$ is a subset of the finite set $Q_m$. If $\gamma\in\Gamma_p$, choose a unit $u$ with $\rho_p(u)=\gamma$. Multiplicativity of $\rho_p$ shows that right multiplication by $u$ takes $Q_s'$ to $Q_{s\gamma}'$, and right multiplication by $u^{-1}$ takes $Q_{s\gamma}'$ back to $Q_s'$, since $\rho_p(u)\rho_p(u^{-1})=\rho_p(1)=[I_2]$ gives $\rho_p(u^{-1})=\gamma^{-1}$. They are inverse maps by step 1.1, giving $\nu(s\gamma)=\nu(s)$. Conjugation takes $Q_s'$ to $Q_{s^{-1}}'$ and is its own inverse by step 1.2, giving $\nu(s^{-1})=\nu(s)$. [F3, F5, F6, F7, step 1.1, step 1.2]

3.1 Every $\alpha\in Q_m$ has exactly one image in $G_p$, so the sets $Q_s'$ are disjoint and have union $Q_m$. Splitting the sum over the first $n$ of these sets gives the sum of their individual contributions by induction on $n$. The union of zero sets contributes $0$, and adjoining the next disjoint set adds its finite sum. On $Q_s'$ the summand $f(\Gamma_p\rho_p(\alpha)g)$ has constant value $z=f(\Gamma_p sg)$. The sum of $n$ identical terms $z$ is $nz$, by the empty sum and the identity $nz+z=(n+1)z$ in the complex field. Hence the unnormalized sum is $\sum_{s\in G_p}\nu(s)f(\Gamma_p sg)$. By step 2.1 both multiplicity hypotheses of [F9] hold on the finite group $G_p$ with subgroup $\Gamma_p$. The sum therefore gives $(Sf)(\Gamma_p g)$ for the induced linear map $S$ in [F9]. With the coefficient in [F6], the Hecke formula is $T_m=S/24$, so it defines a unique linear map on the coset functions. [F5, F6, F7, F8, F9, step 2.1]

4.1 The induced map $S$ from step 3.1 commutes with each $R_r$ by [F9]. Right translation preserves multiplication of functions by a scalar by evaluation at $\Gamma_p gr$, so $S/24$ also commutes with $R_r$. For all coset functions $f,h$, linearity in the first input and conjugate symmetry of the counting inner product give
$$\langle T_m f,h\rangle_p=\tfrac{1}{24}\langle Sf,h\rangle_p=\tfrac{1}{24}\langle f,Sh\rangle_p=\langle f,T_m h\rangle_p.$$
The middle equality uses self-adjointness of $S$ and the last uses that $1/24$ is real. This proves self-adjointness and completes the claims. [F8, F9, step 1.1, step 1.2, step 3.1] ∎
