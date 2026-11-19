---
id: def-euler-hurwitz-hecke-operator
kind: definition
title: Quaternionic Hecke operator on the finite quotient
status: draft
domain: mathematics
deps:
  - def-euler-prime-classes
  - math:def-divides-in-z
  - def-euler-hurwitz-order
  - def-euler-hurwitz-norm-shell
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-projective-reduction
  - math:def-coset
  - lem-euler-hurwitz-unit-list
  - math:lem-rat-embeds-dense
  - math:thm-complex-numbers-form-a-field
  - math:def-function-space
  - math:def-linear-map
  - math:def-finite-sum-in-a-commutative-monoid
  - lem-rational-hamilton-norm-and-inverse
  - math:thm-rat-ordered-field
  - math:lem-int-embeds-rat
  - math:lem-nat-embeds-int
  - math:def-finite-cardinality
  - math:thm-product-rule
  - math:thm-subset-of-a-finite-set
  - math:lem-finite-sum-reindexing-and-fubini
  - math:def-monoid-finite-product
  - math:thm-induction-principle
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  def-euler-hurwitz-norm-shell: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  def-euler-hurwitz-projective-reduction: mathematical-premise
  math:def-coset: mathematical-premise
  lem-euler-hurwitz-unit-list: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:thm-complex-numbers-form-a-field: mathematical-premise
  math:def-function-space: mathematical-premise
  math:def-linear-map: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  lem-rational-hamilton-norm-and-inverse: mathematical-premise
  math:thm-rat-ordered-field: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-product-rule: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:lem-finite-sum-reindexing-and-fubini: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
  math:thm-induction-principle: mathematical-premise
formulation_deps:
  - def-euler-prime-classes
  - math:def-divides-in-z
  - def-euler-hurwitz-order
  - def-euler-hurwitz-norm-shell
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-projective-reduction
  - math:def-coset
  - lem-euler-hurwitz-unit-list
  - math:lem-nat-embeds-int
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:thm-complex-numbers-form-a-field
  - math:def-function-space
  - math:def-linear-map
  - math:def-finite-sum-in-a-commutative-monoid
argument_deps:
  - def-euler-prime-classes
  - math:def-divides-in-z
  - def-euler-hurwitz-order
  - def-euler-hurwitz-norm-shell
  - def-degree-two-projective-linear-group
  - def-euler-hurwitz-projective-reduction
  - math:def-coset
  - lem-euler-hurwitz-unit-list
  - math:lem-rat-embeds-dense
  - math:thm-complex-numbers-form-a-field
  - math:def-function-space
  - math:def-linear-map
  - math:def-finite-sum-in-a-commutative-monoid
  - lem-rational-hamilton-norm-and-inverse
  - math:thm-rat-ordered-field
  - math:lem-int-embeds-rat
  - math:lem-nat-embeds-int
  - math:def-finite-cardinality
  - math:thm-product-rule
  - math:thm-subset-of-a-finite-set
  - math:lem-finite-sum-reindexing-and-fubini
  - math:def-monoid-finite-product
  - math:thm-induction-principle
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, §3.2, equation (3.4)
      reading_limits: Checked the formula and surrounding passage on PDF page 3 for
        attribution. The proof here is local.
dependency_level: 5
---

## Definition

Let $m$ be a positive odd integer, so $m>0$ and $m=2k+1$ for some integer $k$. Let $p\in\mathcal P_3$ be a prime congruent to $3$ modulo $4$, with $p\nmid m$, meaning $m$ is not an integer multiple of $p$.

Let $\mathcal H$ be the Hurwitz order, the rational Hamilton quaternions whose four coordinates in the basis $1,i,j,k$ are all integers or all integers plus $\tfrac12$. Let $Q_m$ be its norm shell, the set of $\alpha\in\mathcal H$ for which the reduced norm $\operatorname{nrd}(\alpha)$, the sum of the four coordinate squares, equals $m$.

Use the fixed projective reduction $\rho_p$ for $p$. It sends a quaternion in $\mathcal H$ whose reduced norm is not divisible by $p$ to its class in $G_p=\mathrm{PGL}_2(\mathbb F_p)$. This is the group of invertible two-by-two matrices over the field $\mathbb F_p$ of integer residues modulo $p$, with matrices identified when one is a nonzero scalar multiple of the other. Write $\mathcal H^\times$ for the units of $\mathcal H$, meaning the elements with a two-sided inverse in $\mathcal H$. Put $\Gamma_p=\rho_p(\mathcal H^\times)$ and let $Y_p=\Gamma_p\backslash G_p$ be the set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$.

Write $\mathbb C[Y_p]$ for the functions $Y_p\to\mathbb C$, where $\mathbb C$ is the complex field. Addition and scalar multiplication take place at each coset. Define the **quaternionic Hecke operator of index $m$ at $p$** as the linear map $T_m:\mathbb C[Y_p]\to\mathbb C[Y_p]$ given, for $f\in\mathbb C[Y_p]$ and $g\in G_p$, by
$$(T_m f)(\Gamma_p g)=\frac{1}{24}\sum_{\alpha\in Q_m}f(\Gamma_p\rho_p(\alpha)g).$$
The sum adds one term per element of $Q_m$ in any order, with the empty sum equal to $0$. The denominator $24$ is the number of units of $\mathcal H$ and is interpreted as a complex scalar. Linearity means $T_m(af+bh)=aT_m f+bT_m h$ for complex $a,b$ and $f,h\in\mathbb C[Y_p]$.

## Definition references

[[def-euler-prime-classes]]

[[math:def-divides-in-z]]

[[def-euler-hurwitz-order]]

[[def-euler-hurwitz-norm-shell]]

[[def-degree-two-projective-linear-group]]

[[def-euler-hurwitz-projective-reduction]]

[[math:def-coset]]

[[lem-euler-hurwitz-unit-list]]

[[math:lem-nat-embeds-int]]

[[math:lem-int-embeds-rat]]

[[math:lem-rat-embeds-dense]]

[[math:thm-complex-numbers-form-a-field]]

[[math:def-function-space]]

[[math:def-linear-map]]

[[math:def-finite-sum-in-a-commutative-monoid]]

## Justification

The proof uses the coordinate description of the norm shell to obtain a finite sum. Reindexing by right multiplication by a unit then gives the same sum for every representative of the coset.

## Facts & Assumptions

[F1] The set $\mathcal P_3$ consists of primes congruent to $3$ modulo $4$, and $p\nmid m$ excludes $m=pq$ for any integer $q$. [[def-euler-prime-classes]] [[math:def-divides-in-z]] The Hurwitz order is closed under quaternion multiplication and has the coordinate description above. Its norm shell consists precisely of the elements with the stated norm. [[def-euler-hurwitz-order]] [[def-euler-hurwitz-norm-shell]]

[F2] For the stated prime $p$, projective reduction is defined on $D_p=\{\beta\in\mathcal H:p\nmid\operatorname{nrd}(\beta)\}$, preserves products there, and carries the units onto the subgroup $\Gamma_p$ of $G_p$. The product in $G_p$ is induced by matrix multiplication. Two right cosets $\Gamma_p g$ and $\Gamma_p g'$ are equal exactly when $g'=\gamma g$ for some $\gamma\in\Gamma_p$. [[def-euler-hurwitz-projective-reduction]] [[def-degree-two-projective-linear-group]] [[math:def-coset]]

[F3] Every Hurwitz unit has reduced norm $1$, and there are exactly $24$ such units. The reduced norm satisfies $\operatorname{nrd}(xy)=\operatorname{nrd}(x)\operatorname{nrd}(y)$ for rational Hamilton quaternions $x,y$. [[lem-euler-hurwitz-unit-list]] [[lem-rational-hamilton-norm-and-inverse]]

[F4] The rationals form an ordered field. The embeddings from the natural numbers to the integers and from the integers to the rationals preserve arithmetic and order and are injective. Thus they preserve and reflect strict order. Every nonnegative integer is the image of a natural number. [[math:thm-rat-ordered-field]] [[math:lem-nat-embeds-int]] [[math:lem-int-embeds-rat]]

[F5] A set is finite when it can be listed without repetition with indices $0,\ldots,n-1$ for a natural number $n$, including the empty list when $n=0$. Each initial segment of this form is finite. Products of finitely many finite sets are finite, and subsets of finite sets are finite. Finiteness transfers along a bijection, a function that is one-to-one and onto. [[math:def-finite-cardinality]] [[math:thm-product-rule]] [[math:thm-subset-of-a-finite-set]]

[F6] The rationals embed in the reals as an ordered subfield, and the reals embed as a subfield of the complex field. Every nonzero complex number has a reciprocal. [[math:lem-rat-embeds-dense]] [[math:thm-complex-numbers-form-a-field]] Pointwise operations make the functions on $Y_p$ a vector space over $\mathbb C$, with equality tested at each coset. For a map between such spaces, preserving the combinations $af+bh$ is exactly linearity. [[math:def-function-space]] [[math:def-linear-map]]

[F7] Addition in a field is associative and commutative with identity $0$, so its finite sums are defined by enumeration. Under a bijection of finite index sets, the sum with reindexed terms equals the original sum. [[math:def-finite-sum-in-a-commutative-monoid]] [[math:lem-finite-sum-reindexing-and-fubini]]

[F8] The partial sum of the first zero terms is $0$, and the next partial sum adds the next term to the preceding partial sum. Induction proves a property for all natural numbers by proving it at $0$ and proving that it passes from each natural number to its successor. [[math:def-monoid-finite-product]] [[math:thm-induction-principle]]

## Proof

**Given:** $m$, $p$, and the fixed projective reduction from the definition.

**Goal:** Show that the formula gives a unique complex-linear map on $\mathbb C[Y_p]$.

1.1 For $\alpha\in Q_m$, double each of its four coordinates to obtain integers $z_1,z_2,z_3,z_4$ with $\sum_{j=1}^4 z_j^2=4m$. Each square is nonnegative, so $z_j^2\le4m$. Set $B=4m+1$. If $z_j\ge B$ or $-z_j\ge B$, the corresponding signed integer $s\in\{z_j,-z_j\}$ satisfies $s\ge B>1$, so $z_j^2=s^2\ge s\ge B>4m$, a contradiction. Hence $0<z_j+B<2B$. Identify $2B$ with the natural number having that integer image. The tuple $(z_1+B,z_2+B,z_3+B,z_4+B)$ is an ordered quadruple from the finite initial segment $0,\ldots,2B-1$. This assignment is one-to-one by recovering each original coordinate from its doubled and shifted value. Its image is a subset of a finite product, so that image and hence $Q_m$ are finite. [F1, F4, F5]

2.1 For every $\alpha\in Q_m$ we have $p\nmid\operatorname{nrd}(\alpha)$ because $\operatorname{nrd}(\alpha)=m$. Thus $\rho_p(\alpha)$ is defined and $\Gamma_p\rho_p(\alpha)g$ is in $Y_p$ for each $g\in G_p$. Evaluation of $f$ there gives a complex number. The sum is finite by step 1.1. The unit count $24$ is a positive natural number, so its rational image is positive by the order-preserving embeddings through the integers. The field embeddings into the reals and then into the complex numbers preserve $0$ and are injective. Thus the complex image of $24$ is nonzero and has a reciprocal. [F1, F2, F3, F4, F6, F7, step 1.1]

3.1 Suppose $\Gamma_p g'=\Gamma_p g$. Write $g'=\gamma g$ with $\gamma\in\Gamma_p$ and take $u\in\mathcal H^\times$ with $\rho_p(u)=\gamma$. The map $\alpha\mapsto\alpha u$ from $Q_m$ to itself has inverse $\alpha\mapsto\alpha u^{-1}$. Indeed, both multiplications stay in $\mathcal H$ and preserve the norm because $u$ and $u^{-1}$ have norm $1$. For each $\alpha\in Q_m$, multiplicativity of projective reduction gives $\rho_p(\alpha)g'=\rho_p(\alpha)\rho_p(u)g=\rho_p(\alpha u)g$. [F1, F2, F3, step 2.1]

4.1 Apply finite-sum reindexing to the bijection $\alpha\mapsto\alpha u$ on $Q_m$. The terms for $g'$ are exactly the reindexed terms for $g$, so the two sums agree. Each coset has a representative by definition, and the value is the same for every representative. This gives a unique function $T_m f:Y_p\to\mathbb C$ for each $f\in\mathbb C[Y_p]$. [F2, F6, F7, step 2.1, step 3.1]

5.1 For $f,h\in\mathbb C[Y_p]$ and $a,b\in\mathbb C$, evaluate at a coset $\Gamma_p g$. In any enumeration of $Q_m$, each summand for $af+bh$ is $a$ times the corresponding summand for $f$ plus $b$ times that for $h$. Write $A_n,B_n,C_n$ for the sums of the first $n$ terms for $f,h,af+bh$, respectively, extending each list by zeros. At $n=0$ all three sums are $0$. If $C_n=aA_n+bB_n$ and the next terms for $f,h$ are $x,y$, then $C_{n+1}=C_n+ax+by=a(A_n+x)+b(B_n+y)=aA_{n+1}+bB_{n+1}$. By induction, the identity holds for the full sums. Multiplying by $1/24$ preserves the identity by the field laws. Since the equality holds at every coset, $T_m(af+bh)=aT_m f+bT_m h$. Thus the formula defines the stated linear map. [F6, F7, F8, step 2.1, step 4.1] ∎
