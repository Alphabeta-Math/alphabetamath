---
title: The Hecke eigenvalue on the determinant character
status: published
research_item: lem-euler-hurwitz-hecke-character-eigenvalue
dependency_level: 7
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, §3.2, character eigenvalue before Lemma 3.2
      reading_limits: Checked equation (3.4) and the determinant-character paragraph
        on PDF page 3. Citation for attribution.
---

PDF p. 3: ` §3.2, character eigenvalue before Lemma 3.2 `

## Prerequisites

- [math:thm-int-comm-ring](https://alphabetamath.cc/item/thm-int-comm-ring)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:def-canonical-natural](https://alphabetamath.cc/item/def-canonical-natural)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction)
- [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)
- [math:def-legendre-symbol](https://alphabetamath.cc/item/def-legendre-symbol)
- [lem-projective-determinant-square-class](item-lem-projective-determinant-square-class)
- [def-euler-hurwitz-determinant-character](item-def-euler-hurwitz-determinant-character)
- [lem-euler-hurwitz-determinant-character-well-defined](item-lem-euler-hurwitz-determinant-character-well-defined)
- [math:def-function-space](https://alphabetamath.cc/item/def-function-space)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map)
- [def-euler-divisor-functions](item-def-euler-divisor-functions)
- [lem-euler-hurwitz-hecke-constant-eigenvalue](item-lem-euler-hurwitz-hecke-constant-eigenvalue)
- [math:def-eigenvalue-eigenvector-eigenspace-and-spectrum](https://alphabetamath.cc/item/def-eigenvalue-eigenvector-eigenspace-and-spectrum)


## Statement

Let $m>0$ be an odd integer, so $m=2k+1$ for some integer $k$. Let $p\in\mathcal P_3$, the set of primes of the form $4r+3$ with $r$ an integer. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Assume $p\nmid m$, meaning that $m$ is not an integer multiple of $p$.

Write $\mathbb F_p=\mathbb Z/p\mathbb Z$ for the field of integer residues, where two integers have the same residue when their difference is a multiple of $p$. Let $G_p=\mathrm{PGL}_2(\mathbb F_p)$ be the group of invertible two-by-two matrices over $\mathbb F_p$ up to nonzero scalar multiplication. Invertible means having a two-sided matrix inverse. Write $[A]$ for the class of $A$, with product $[A][B]=[AB]$.

The Hurwitz order $\mathcal H$ consists of rational quaternions $a+bi+cj+dk$ with all four coordinates integral or all four in $\mathbb Z+\tfrac12$, using $i^2=j^2=-1$ and $ij=k=-ji$. The reduced norm $\operatorname{nrd}(\alpha)$ is the sum of the squares of the four coordinates of $\alpha$. The norm shell $Q_m$ consists of the elements $\alpha\in\mathcal H$ with $\operatorname{nrd}(\alpha)=m$. For $\alpha$ whose norm has nonzero residue, the fixed projective reduction $\rho_p$ sends $\alpha$ to the projective class of its reduction matrix. This matrix is obtained by taking the residue of $\alpha$ modulo $p\mathcal H$ and applying the fixed identification with two-by-two matrices over $\mathbb F_p$. Let $\mathcal H^\times$ consist of the elements with two-sided inverses in $\mathcal H$. Put $\Gamma_p=\rho_p(\mathcal H^\times)$ and write $Y_p=\Gamma_p\backslash G_p$ for the set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$.

On the space $\mathbb C[Y_p]$ of complex-valued functions with pointwise vector operations, use the quaternionic Hecke operator
$$(T_m f)(\Gamma_p g)=\frac1{24}\sum_{\alpha\in Q_m} f(\Gamma_p\rho_p(\alpha)g).$$
The finite sum adds one value per element of the shell. The operator is linear, meaning that it preserves combinations $af+bh$ for complex scalars $a,b$. The determinant character is the function $\chi_p(\Gamma_p[A])=\left(\frac{\det A}{p}\right)$. Here $\det A=ad-bc$ for rows $(a,b)$ and $(c,d)$. For a nonzero residue $t$, the Legendre symbol $\left(\frac{t}{p}\right)$ is $1$ if $t$ is a square of a nonzero residue and $-1$ otherwise. For the numerator $m$ it is evaluated on the residue of $m$. Regard the two signs as the complex unit $1$ and its additive inverse $-1$. For a nonnegative integer $d$ used as a complex scalar, let $d_{\mathbb N}$ be its unique preimage under the canonical inclusion $\mathbb N\to\mathbb Z$. Use the sum of $d_{\mathbb N}$ copies of the complex unit $1$, with the empty sum equal to zero. Let $\sigma(m)$ be the sum of the positive divisors of $m$.

Then $\chi_p$ is an eigenvector of $T_m$ with eigenvalue $\left(\frac{m}{p}\right)\sigma(m)$. In other words, $\chi_p$ is a nonzero function and
$$T_m\chi_p=\left(\frac{m}{p}\right)\sigma(m)\chi_p.$$

## Facts & Assumptions

[F1] A prime in $\mathcal P_3$ has the form $4r+3$. The integer residue of $m$ modulo $p$ is nonzero when $p\nmid m$, and those residues form a field for prime $p$. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n) [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[F2] The coordinate rule defines the Hurwitz order $\mathcal H$. The finite shell $Q_m$ consists of its quaternions of reduced norm $m$. [def-euler-hurwitz-order](item-def-euler-hurwitz-order) [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell) [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator)

[F3] With the fixed reduction, write $A_p(\alpha)$ for the matrix of the residue of $\alpha$ before passing to a projective class. For norm not divisible by $p$, this matrix is invertible and $\rho_p(\alpha)=[A_p(\alpha)]$. The group $G_p$ has product induced by matrix multiplication and identity $[I_2]$, where $I_2$ has ones on the diagonal and zeros elsewhere. The subgroup of images of the Hurwitz units is $\Gamma_p$, and each point of $Y_p$ is a right coset $\Gamma_p g$ of this subgroup. [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group) [math:def-coset](https://alphabetamath.cc/item/def-coset)

[F4] The norm–determinant formula for the fixed reduction at an odd prime gives $\det A_p(\alpha)=\operatorname{nrd}(\alpha)\bmod p$ for $\alpha\in\mathcal H$. The determinant in size two is $ad-bc$. [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction) [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)

[F5] For an odd prime, the Legendre symbol on nonzero residues takes the indicated square and nonsquare values. The function $s_p([A])=\left(\frac{\det A}{p}\right)$ on $G_p$ preserves multiplication, so $s_p(hg)=s_p(h)s_p(g)$ for $h,g\in G_p$. The determinant-character definition and its well-definedness give $\chi_p(\Gamma_p g)=s_p(g)$ for every $g\in G_p$, independently of the representative of the coset. [math:def-legendre-symbol](https://alphabetamath.cc/item/def-legendre-symbol) [lem-projective-determinant-square-class](item-lem-projective-determinant-square-class) [def-euler-hurwitz-determinant-character](item-def-euler-hurwitz-determinant-character) [lem-euler-hurwitz-determinant-character-well-defined](item-lem-euler-hurwitz-determinant-character-well-defined)

[F6] The Hecke formula in the statement defines $T_m$ for positive odd $m$, $p\in\mathcal P_3$ and $p\nmid m$. Equal terms at each element of a finite index set give equal sums, since both sums add the same list of terms. Linearity gives $T_m(cf)=cT_mf$ for a complex scalar $c$ by setting the second coefficient to zero. [def-euler-hurwitz-hecke-operator](item-def-euler-hurwitz-hecke-operator) [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid) [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map)

[F7] Under these same hypotheses, $\mathbf1$, the function of value $1$ at each coset, is an eigenvector of $T_m$ with scalar the canonical complex image of the natural divisor sum $\sigma(m_{\mathbb N})$. This sum ranges over the positive naturals whose integer images divide $m$. [lem-euler-hurwitz-hecke-constant-eigenvalue](item-lem-euler-hurwitz-hecke-constant-eigenvalue) [def-euler-divisor-functions](item-def-euler-divisor-functions)

[F8] The complex scalars form a commutative field. The inclusion of real numbers preserves the scalar signs, so $1$ and $-1$ are both nonzero in $\mathbb C$. Scalar multiplication of functions is evaluated pointwise, and functions are equal when their values agree at every point. A nonzero function $v$ with $T_m v=\lambda v$ is an eigenvector with eigenvalue $\lambda$. [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field) [math:def-function-space](https://alphabetamath.cc/item/def-function-space) [math:def-eigenvalue-eigenvector-eigenspace-and-spectrum](https://alphabetamath.cc/item/def-eigenvalue-eigenvector-eigenspace-and-spectrum)

[F9] The canonical inclusion $\iota:\mathbb N\to\mathbb Z$ preserves zero, addition and order, and gives every nonnegative integer a unique natural preimage. In an additive monoid a finite partial sum starts at zero and its successor adds the next term. Induction gives equality of two such partial-sum lists at every position if the base and successor values agree. The canonical complex image of a natural number is the sum of that many copies of the complex unit. Integer addition is associative and commutative with identity $0$, so $(\mathbb Z,+,0)$ is a commutative monoid. Its finite sums can be computed in any enumeration of the index set. [math:thm-int-comm-ring](https://alphabetamath.cc/item/thm-int-comm-ring) [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle) [math:def-canonical-natural](https://alphabetamath.cc/item/def-canonical-natural)

## Proof

**Given:** An odd integer $m>0$ and $p\in\mathcal P_3$ with $p\nmid m$, using the same fixed projective reduction for $T_m$ and $\chi_p$.

**Goal:** Prove the eigenvalue equation and show that $\chi_p$ is nonzero.

1.1 Since $p=4r+3=2(2r+1)+1$, it is an odd prime. Put $\varepsilon=\left(\frac{m}{p}\right)\in\{1,-1\}$. For every $\alpha\in Q_m$, its reduced norm equals $m$, whose residue is nonzero. Thus $\rho_p(\alpha)$ is defined and is represented by $A_p(\alpha)$. Its representative has determinant the residue of $m$, so $s_p(\rho_p(\alpha))=\varepsilon$. [given, F1, F2, F3, F4, F5]

1.2 The positive natural divisors in [F7] correspond bijectively under $\iota$ to the positive integer divisors of $m$. Indeed, the natural divisor test is the same integer equality $m=\iota(d)q$, and every positive integer divisor has a unique positive natural preimage. List the finite divisor sets in corresponding order. By [F9], the integer divisor sum is the final partial sum in this order. The integer partial sum is the image of the natural partial sum at each position. This holds at zero, and appending any divisor preserves it since $\iota$ is additive. Thus the integer divisor sum is $\iota(\sigma(m_{\mathbb N}))$ by [F9]. Its complex image in the Statement uses exactly the natural preimage $\sigma(m_{\mathbb N})$, so it is the scalar in [F7]. [F6, F7, F9]

2.1 Fix $y=\Gamma_p g\in Y_p$ and let $c_y=\varepsilon\chi_p(y)$. For each $\alpha\in Q_m$, the coset formula for $\chi_p$ and the multiplication rule for $s_p$ give $\chi_p(\Gamma_p\rho_p(\alpha)g)=s_p(\rho_p(\alpha)g)=s_p(\rho_p(\alpha))s_p(g)=c_y$. [F3, F5, step 1.1]

3.1 At this fixed $y$, the terms in the Hecke sum for $\chi_p$ are exactly the terms for the constant function $c_y\mathbf1$, since $(c_y\mathbf1)(\Gamma_p\rho_p(\alpha)g)=c_y$ for every $\alpha\in Q_m$. Hence $(T_m\chi_p)(y)=(T_m(c_y\mathbf1))(y)$. [F6, F7, F8, step 2.1]

4.1 By linearity and the constant-function eigenvalue, $(T_m(c_y\mathbf1))(y)=c_y(T_m\mathbf1)(y)=c_y\sigma(m)=\varepsilon\sigma(m)\chi_p(y)$, using commutativity of complex multiplication. Since $y$ was arbitrary, pointwise equality gives $T_m\chi_p=\varepsilon\sigma(m)\chi_p$. [F6, F7, F8, step 1.2, step 2.1, step 3.1]

5.1 The coset $\Gamma_p[I_2]$ belongs to $Y_p$. Its $\chi_p$ value is a sign, which is nonzero as a complex number. Thus $\chi_p$ is nonzero, and the equation in step 4.1 proves that its eigenvalue is $\left(\frac{m}{p}\right)\sigma(m)$. [F3, F5, F8, step 4.1] ∎
