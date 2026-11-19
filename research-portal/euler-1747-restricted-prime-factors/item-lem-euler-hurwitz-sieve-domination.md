---
title: The obstruction count is bounded by the Hecke orbit count
status: draft
research_item: lem-euler-hurwitz-sieve-domination
dependency_level: 9
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §3.3, equation (3.6)
      reading_limits: Read the surrounding §3.3 passage on PDF page 4 for attribution.
---

PDF p. 4: ` §3.3, equation (3.6) `

## Prerequisites

- [def-euler-prime-classes](item-def-euler-prime-classes)
- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)
- [def-euler-four-square-representations](item-def-euler-four-square-representations)
- [def-euler-mixed-four-square-representations](item-def-euler-mixed-four-square-representations)
- [def-euler-prime-obstruction-count](item-def-euler-prime-obstruction-count)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer)
- [def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit)
- [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [lem-euler-hurwitz-four-square-bijection](item-lem-euler-hurwitz-four-square-bijection)
- [lem-euler-hurwitz-normalizer-coordinate-test](item-lem-euler-hurwitz-normalizer-coordinate-test)
- [lem-euler-hurwitz-normalizer-unit-count](item-lem-euler-hurwitz-normalizer-unit-count)
- [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [math:lem-nat-finite-sum-laws-and-the-canonical-embedding](https://alphabetamath.cc/item/lem-nat-finite-sum-laws-and-the-canonical-embedding)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)


## Statement

Let $n=2m$ for a positive odd integer $m$, so $m=2r+1$ for an integer $r$. Let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$, and suppose $p\nmid m$. Here a prime is an integer greater than $1$ with no positive divisors other than $1$ and itself, congruence means $4\mid(p-3)$, and $s\mid t$ means $t=sv$ for some integer $v$.

Write $\mathcal R(n)$ for the ordered integer quadruples $x=(x_1,x_2,x_3,x_4)$ with $\sum_{j=1}^4x_j^2=n$. A quadruple has mixed parity if each of $(x_1,x_2)$ and $(x_3,x_4)$ contains one even and one odd entry. The even integers are those of the form $2v$, and the odd integers are those of the form $2v+1$, for integers $v$. Let $E_p(n)$ be the set of mixed-parity quadruples in $\mathcal R(n)$ with both entries of at least one pair divisible by $p$. Set $b_p(n)=|E_p(n)|$, where $|S|$ is the length of a listing of all elements of $S$ without repetition. Finiteness means such a listing has a nonnegative integer length.

In the rational Hamilton quaternions, multiplication is associative and determined by $i^2=j^2=-1$, $ij=k=-ji$, distributivity and commutation with rational scalars. Each quaternion has unique coordinates in the basis $1,i,j,k$. The Hurwitz order $\mathcal H$ is the subring consisting of the elements $a+bi+cj+dk$ whose coordinates are all integers or all integers plus $\tfrac12$. This subset contains $1$ and is closed under addition, negatives and multiplication. Let $Q_m$ be its norm shell, the set of elements whose reduced norm $N(a+bi+cj+dk)=a^2+b^2+c^2+d^2$ equals $m$.

Use one fixed projective reduction $\rho_p$ at $p$. The field $\mathbb F_p$ consists of integer residues modulo $p$, with classes equal when representatives differ by a multiple of $p$. Addition and multiplication are induced from the integers. The group $G_p$ consists of classes of invertible two-by-two matrices over $\mathbb F_p$, where matrices are identified up to nonzero scalar multiplication and classes multiply on representatives. An invertible element has a two-sided multiplicative inverse. For $\alpha\in\mathcal H$ of norm not divisible by $p$, $\rho_p(\alpha)$ is the class of the matrix of the residue $\alpha+p\mathcal H$ under the fixed isomorphism from $\mathcal H/p\mathcal H$ to the two-by-two matrix algebra over $\mathbb F_p$ that preserves addition, multiplication, identity and scalars. Here $\mathcal H/p\mathcal H$ consists of the additive cosets $\alpha+p\mathcal H=\{\alpha+p\beta:\beta\in\mathcal H\}$ with operations on representatives.

Write $\Gamma_p=\rho_p(\mathcal H^\times)$ for the subgroup of $G_p$ formed by the images of the Hurwitz units, where $\mathcal H^\times$ consists of the elements invertible in $\mathcal H$. A subgroup contains the group identity and is closed under products and inverses. Let $Y_p$ consist of the right cosets $\Gamma_pg=\{\gamma g:\gamma\in\Gamma_p\}$ for $g\in G_p$. The base coset is $\Gamma_p=\Gamma_pe$ for the identity $e$ of $G_p$. Let $C_p$ be the subgroup consisting of the projective classes of the nonzero residues $a+b\bar i$ with $a,b\in\mathbb F_p$, where $\bar i$ is the image of $i$ in $\mathcal H/p\mathcal H$. Its normalizer $K_p$ is the subgroup of elements $g\in G_p$ such that $\{gcg^{-1}:c\in C_p\}=C_p$.

Let $\mathcal O_p=\{\Gamma_pk:k\in K_p\}$ be the normalizer orbit of the base coset, the set of its right translates by elements of $K_p$. Its indicator $f_p$ on $Y_p$ has value $1$ on $\mathcal O_p$ and $0$ elsewhere. The Hecke operator $T_m$ on complex-valued functions $f$ on $Y_p$ is given by
$$(T_mf)(\Gamma_pg)=\frac1{24}\sum_{\alpha\in Q_m} f(\Gamma_p\rho_p(\alpha)g).$$
Then $(T_m f_p)(\Gamma_p)$ is a nonnegative integer and
$$b_p(n)\le 8(T_m f_p)(\Gamma_p).$$

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)

[def-euler-hurwitz-order](item-def-euler-hurwitz-order)

[def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)

[def-euler-four-square-representations](item-def-euler-four-square-representations)

[def-euler-mixed-four-square-representations](item-def-euler-mixed-four-square-representations)

[def-euler-prime-obstruction-count](item-def-euler-prime-obstruction-count)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer)

[def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit)

[def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)

[math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

## Facts & Assumptions

[F1] A prime in $\mathcal P_3$ is odd. In $\mathbb F_p$ the residue of an integer is zero exactly when $p$ divides that integer. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[F2] The sets $\mathcal R(n)$, $\mathcal H$, $Q_m$ and $E_p(n)$ have the coordinate descriptions above, and $b_p(n)$ counts the elements of $E_p(n)$ once each. Quaternion coordinates in $1,i,j,k$ are unique. [def-euler-four-square-representations](item-def-euler-four-square-representations) [def-euler-mixed-four-square-representations](item-def-euler-mixed-four-square-representations) [def-euler-prime-obstruction-count](item-def-euler-prime-obstruction-count) [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions) [def-euler-hurwitz-order](item-def-euler-hurwitz-order) [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)

[F3] For positive odd $m$, right multiplication by $1+i$ and taking coordinates gives a bijection $F:Q_m\to\mathcal R(2m)$, meaning that each tuple is the image of exactly one element. [lem-euler-hurwitz-four-square-bijection](item-lem-euler-hurwitz-four-square-bijection)

[F4] The reduction to $\mathcal H/p\mathcal H$ preserves products. In the projective reduction, the residue of any $\alpha\in Q_m$ is invertible when $p\nmid m$. Under the same reduction, the four coefficients of an integral quaternion in $1,i,j,k$ reduce to the four residue coefficients in $1,\bar i,\bar j,\bar k$, where the bars denote the respective images in $\mathcal H/p\mathcal H$. The latter four basis elements give unique coefficients by steps 1.1 and 2.1 of the torus construction. [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell) [def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer)

[F5] An invertible residue has a zero first or second coordinate pair exactly when its projective class lies in $K_p$. Right multiplication by the invertible residue of $1+i$ gives another invertible residue and preserves that condition in both directions. [lem-euler-hurwitz-normalizer-coordinate-test](item-lem-euler-hurwitz-normalizer-coordinate-test)

[F6] The left-unit classes $\mathcal H^\times\alpha=\{u\alpha:u\in\mathcal H^\times\}$ partition $Q_m$: each element lies in exactly one such class. The map $u\mapsto u\alpha$ takes the units one-to-one onto that class by step 1.1 of the unit-count lemma. There are $24$ Hurwitz units. For all members $\beta$ of a class the coset $\Gamma_p\rho_p(\beta)$ is the same. If this coset is in $\mathcal O_p$, exactly eight members satisfy $\rho_p(\beta)\in K_p$. Otherwise there are no such members. [lem-euler-hurwitz-normalizer-unit-count](item-lem-euler-hurwitz-normalizer-unit-count) [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)

[F7] The cosets in $\mathcal O_p$ have indicator value $1$ and the other cosets have value $0$. The displayed formula defines $T_m$ under the hypotheses of the Statement, and step 1.1 of its proof gives finiteness of $Q_m$. [def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit) [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)

[F8] Cardinality is the length of a listing without repetitions, so a bijection preserves it. A subset of a finite set is finite and its cardinality is at most that of the larger set. For a finite family of pairwise disjoint finite sets the cardinality of the union is the sum of the cardinalities. Here disjoint means having no element in common. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)

[F9] A finite sum in the natural numbers or the complex numbers is computed by adding its terms in any enumeration, with empty sum $0$. A constant natural number $c$ added over a list of length $h$ gives $hc$. The natural numbers are identified with their images in the reals by the map that preserves $0,1$, addition, multiplication and order, and the real numbers embed as a subfield of the complex numbers, with the same arithmetic on their images. [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid) [math:lem-nat-finite-sum-laws-and-the-canonical-embedding](https://alphabetamath.cc/item/lem-nat-finite-sum-laws-and-the-canonical-embedding) [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

## Proof

**Given:** The integers $n=2m$ and $p$ with the hypotheses of the Statement and the fixed projective reduction at $p$.

**Goal:** Show that $(T_m f_p)(\Gamma_p)$ is a nonnegative integer and that eight times this integer bounds $b_p(n)$.

1.1 Put $A=\{\alpha\in Q_m:\rho_p(\alpha)\in K_p\}$. For $x\in E_p(n)$ take its unique preimage $\alpha\in Q_m$ under $F$. The quaternion $\alpha(1+i)$ has integral coordinates $x_1,x_2,x_3,x_4$. At least one pair becomes zero upon reduction modulo $p$ by the divisibility condition on $x$ and the coefficient rule of [F4]. The residue of $\alpha$ is invertible since $p\nmid m$. The residue of $\alpha(1+i)$ is its product on the right by the residue of $1+i$ because reduction preserves products. By [F5] the residue of $\alpha$ also has a zero pair and $\rho_p(\alpha)\in K_p$. Therefore $F^{-1}(E_p(n))\subseteq A$. The restriction of $F$ maps this preimage one-to-one onto $E_p(n)$, so $b_p(n)\le |A|$ by finiteness of $Q_m$ and the cardinality rule. [given, F1, F2, F3, F4, F5, F7, F8]

1.2 Put $S=\{\alpha\in Q_m:\Gamma_p\rho_p(\alpha)\in\mathcal O_p\}$. By [F6], $S$ is a union of entire left-unit classes and no member of $A$ lies in a class outside $S$. The classes contained in $S$ form a finite set because listing $S$ and keeping each class upon its first occurrence lists all of them once, since every class contains its defining element. Write $h$ for the number of these classes, allowing $h=0$. Each contains $24$ elements, and its intersection with $A$ contains eight. Taking the sums over the pairwise disjoint classes, and over their pairwise disjoint intersections with $A$, respectively, gives $|S|=24h$ and $|A|=8h$. [F6, F7, F8, F9]

2.1 Evaluate the Hecke formula at $\Gamma_pe$ on $f_p$. The summands are $1$ for $\alpha\in S$ and $0$ for the other shell elements. Enumerate the finite shell with $S$ first. Adding $|S|$ copies of $1$ and then the zeros gives $|S|$, using the same arithmetic under the natural number inclusion into the complex numbers. As $24$ has nonzero image, the formula yields $(T_mf_p)(\Gamma_p)=|S|/24=h$. Thus the value is a nonnegative integer, and step 1.1 gives $b_p(n)\le |A|=8h=8(T_mf_p)(\Gamma_p)$. [F7, F8, F9, step 1.1, step 1.2] ∎
