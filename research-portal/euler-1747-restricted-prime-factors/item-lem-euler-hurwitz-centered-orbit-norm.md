---
title: Orthogonality and norm of the centered orbit indicator
status: published
research_item: lem-euler-hurwitz-centered-orbit-norm
dependency_level: 8
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §3.3, paragraph between (3.7) and (3.8)
---

PDF p. 4: ` §3.3, centered indicator and its norm before (3.8) `

## Prerequisites

- [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit)
- [def-euler-hurwitz-determinant-character](item-def-euler-hurwitz-determinant-character)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)
- [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus)
- [math:def-inner-product-space](https://alphabetamath.cc/item/def-inner-product-space)
- [math:def-inner-product-norm](https://alphabetamath.cc/item/def-inner-product-norm)
- [math:def-orthogonal-vectors-sets-and-orthonormal-bases](https://alphabetamath.cc/item/def-orthogonal-vectors-sets-and-orthonormal-bases)
- [lem-centered-indicator-rayleigh-bound](item-lem-centered-indicator-rayleigh-bound)
- [lem-euler-hurwitz-orbit-determinant-balance](item-lem-euler-hurwitz-orbit-determinant-balance)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition)
- [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete)
- [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)
- [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication)


## Statement

Let $p\in\mathcal P_3$, the set of primes of the form $4r+3$ with $r$ an integer. Use $Y_p=\Gamma_p\backslash G_p$, the finite nonempty set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$ in the fixed projective reduction. In that reduction $G_p$ consists of invertible two-by-two matrices modulo $p$ identified up to nonzero scalar multiples, and $\Gamma_p$ is the subgroup supplied by that reduction. Let $\mathcal O_p=\{\Gamma_p k:k\in K_p\}$ be the normalizer orbit, the nonempty subset obtained by translating the identity coset on the right by elements of the subgroup $K_p$ fixed in the orbit definition.

Write $|S|$ for the number of elements of a finite set $S$. Let $f_p$ be the indicator of $\mathcal O_p$, with value $1$ on $\mathcal O_p$ and $0$ elsewhere, and set $\mu_p=|\mathcal O_p|/|Y_p|$. Form the rational fraction from the integer images of the two counts and view it in $\mathbb R$ via the constant-sequence embedding. In scalar expressions a count is the sum of that many copies of the real unit $1$. Real scalars act on complex-valued functions through the field embedding $\mathbb R\to\mathbb C$. Write $\mathbf1$ for the function with value $1$ at every coset. The determinant character $\chi_p$ is the function on $Y_p$ which takes value $1$ if the determinant of a matrix representing the coset is a nonzero square modulo $p$, meaning $t^2$ for some nonzero residue $t$, and $-1$ otherwise. For a matrix with rows $(a,b)$ and $(c,d)$ the determinant is $ad-bc$.

On the complex-valued functions on $Y_p$ with addition and scalar multiplication on the values at each coset, use the counting inner product $\langle u,v\rangle_p=\sum_{y\in Y_p}u(y)\overline{v(y)}$, which sums one term per coset. The bar denotes complex conjugation, sending $a+bi$ to $a-bi$ for real $a,b$ and the complex imaginary unit $i$ with $i^2=-1$. Orthogonality means the pairing is zero, and the induced norm is $\|u\|_2=\sqrt{\langle u,u\rangle_p}$ with the nonnegative square root.

The centered indicator $h_p=f_p-\mu_p\mathbf1$ is orthogonal to both $\mathbf1$ and $\chi_p$, and
$$\|h_p\|_2^2=|\mathcal O_p|(1-\mu_p).$$

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit)

[def-euler-hurwitz-determinant-character](item-def-euler-hurwitz-determinant-character)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid)

[math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus)

[math:def-inner-product-space](https://alphabetamath.cc/item/def-inner-product-space)

[math:def-inner-product-norm](https://alphabetamath.cc/item/def-inner-product-norm)

[math:def-orthogonal-vectors-sets-and-orthonormal-bases](https://alphabetamath.cc/item/def-orthogonal-vectors-sets-and-orthonormal-bases)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

## Justification

The count $|Y_p|$ is positive by nonemptiness, and the embeddings preserve positivity up to $\mathbb R$ and preserve nonzero values in $\mathbb C$. Thus the density has a nonzero denominator in each scalar field. Orbit membership assigns exactly one indicator value to each coset, and the determinant character gives a sign independent of the chosen representative. The counting pairing on $Y_p$ uses pointwise function operations, so the difference defining $h_p$ is again a function on $Y_p$. The diagonal pairing is a nonnegative real, so the induced norm uses its unique nonnegative square root.

## Facts & Assumptions

[F1] For $p\in\mathcal P_3$, the fixed reduction gives the nonempty finite coset set $Y_p$ with the stated counting inner product. The orbit definition gives its nonempty subset $\mathcal O_p$, its indicator $f_p$ and the fraction $\mu_p$, whose denominator counts the nonempty set $Y_p$. [def-euler-prime-classes](item-def-euler-prime-classes) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F2] The counting inner product is linear in its first argument, and the squared induced norm is the diagonal pairing. A zero pairing gives orthogonality. [math:def-inner-product-space](https://alphabetamath.cc/item/def-inner-product-space) [math:def-inner-product-norm](https://alphabetamath.cc/item/def-inner-product-norm) [math:def-orthogonal-vectors-sets-and-orthonormal-bases](https://alphabetamath.cc/item/def-orthogonal-vectors-sets-and-orthonormal-bases)

[F3] For any nonempty subset $O$ of a nonempty finite set $Y$, the indicator $f$ and density $\mu=|O|/|Y|$ give a centered function $f-\mu\mathbf1$ orthogonal to $\mathbf1$ with squared counting norm $|O|(1-\mu)$. These two conclusions hold for the complex function space with the counting inner product. [lem-centered-indicator-rayleigh-bound](item-lem-centered-indicator-rayleigh-bound)

[F4] The determinant character is a well-defined function on the cosets with real values $1$ and $-1$, which complex conjugation fixes. For this fixed reduction at $p\in\mathcal P_3$, each of $\mathcal O_p$ and $Y_p$ has equally many cosets of each sign. [def-euler-hurwitz-determinant-character](item-def-euler-hurwitz-determinant-character) [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus) [lem-euler-hurwitz-orbit-determinant-balance](item-lem-euler-hurwitz-orbit-determinant-balance)

[F5] A finite sum may be evaluated by listing the summands in any order, and the empty sum is zero. The additive partial-sum recursion starts at zero and adds the next term at each successor. [math:def-finite-sum-in-a-commutative-monoid](https://alphabetamath.cc/item/def-finite-sum-in-a-commutative-monoid) [math:def-monoid-finite-product](https://alphabetamath.cc/item/def-monoid-finite-product)

[F6] The canonical maps from $\mathbb N$ to $\mathbb Z$ and from $\mathbb Z$ to $\mathbb Q$ preserve arithmetic and order, with each sending $0$ and $1$ to their counterparts. The constant-sequence map from $\mathbb Q$ to $\mathbb R$ is an ordered-field embedding. The field embedding from $\mathbb R$ to $\mathbb C$ preserves addition and the unit. Both field embeddings preserve division by a nonzero scalar. [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense) [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

[F7] If a property of natural numbers holds at zero and its truth at any natural number implies its truth at the successor, then it holds at every natural number. [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F8] Every subset of a finite set is finite. A finite set $U$ admits an enumeration without repetitions of length $|U|$. [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F9] For natural numbers $a,b$, addition gives $a+0=a$ and $a+1=\sigma(a)$, where $\sigma(a)$ is the successor of $a$. Discreteness gives $\sigma(a)\le b$ if and only if $a<b$, and the definition of strict order gives $a\le b$ from $a<b$. Also $a\le a$, witnessed by $a+0=a$. The addition recursion gives $a+\sigma(b)=\sigma(a+b)$. [math:def-nat-addition](https://alphabetamath.cc/item/def-nat-addition) [math:lem-nat-discrete](https://alphabetamath.cc/item/lem-nat-discrete) [math:def-nat-order](https://alphabetamath.cc/item/def-nat-order)

[F10] Natural-number multiplication in its second argument satisfies $a\cdot 0=0$ and $a\cdot\sigma(b)=a\cdot b+a$. [math:def-nat-multiplication](https://alphabetamath.cc/item/def-nat-multiplication)

## Proof

**Given:** A prime $p\in\mathcal P_3$, with $Y_p,\mathcal O_p,f_p,\mu_p,\chi_p$ as in the statement.

**Goal:** Show $\langle h_p,\mathbf1\rangle_p=\langle h_p,\chi_p\rangle_p=0$ and $\|h_p\|_2^2=|\mathcal O_p|(1-\mu_p)$.

1.1 By [F1], $Y_p$ is finite and nonempty and $\mathcal O_p$ is a nonempty subset of $Y_p$. By [F8], $\mathcal O_p$ is finite. Thus the finiteness and nonemptiness hypotheses of [F3] hold. The indicator and counting pairing in [F1] agree with those in [F3] for $Y=Y_p$ and $O=\mathcal O_p$. Since an integer image of a count is a sum of that many integer ones, the embeddings in [F6] send each count to the sum of that many real ones and then complex ones. The real embedding preserves the quotient defining the rational density because the denominator is positive. The resulting real density and its complex image are therefore precisely those used for the centered indicator in [F3]. Applying its centered-indicator conclusion gives $\langle h_p,\mathbf1\rangle_p=0$ and $\|h_p\|_2^2=|\mathcal O_p|(1-\mu_p)$. [given, F1, F3, F6, F8]

2.1 Take $S=\mathcal O_p$ or $S=Y_p$. Each sign class is a subset of $S$, which is finite by step 1.1, so each class is finite by [F8]. Write $n_+(S)$ and $n_-(S)$ for the counts of cosets in $S$ with sign $1$ and $-1$, respectively. By [F4] these counts are equal. Write $n$ for the common count and enumerate $S$ by alternating its $n$ positive-sign cosets with its $n$ negative-sign cosets, starting with a positive-sign coset if $n>0$. The enumeration is empty if $n=0$. Apply [F7] to the property that if $k\le n$, the partial sum after the first $2k$ terms is zero. At $k=0$, [F10] gives $2\cdot0=0$, so the sum is empty and equals zero by [F5]. If $k+1\le n$, then $\sigma(k)\le n$, so $k<n$ and therefore $k\le n$ by [F9]. By the induction hypothesis the preceding $2k$ terms sum to zero. By [F9] and [F10], $2(k+1)=2\cdot\sigma(k)=2k+2=\sigma(\sigma(2k))$, since $2=\sigma(\sigma(0))$. The next two terms are the positive and negative signs of pair $k+1$. The two successive additions of $1$ and $-1$ in [F5] give $(0+1)+(-1)=0$. Hence the property holds for every $k$ by induction. Taking $k=n$ and using $n\le n$ from [F9] gives $\sum_{y\in S}\chi_p(y)=0$. [F4, F5, F7, F8, F9, F10, step 1.1]

3.1 The sign is real, so in the counting pairings conjugation fixes $\chi_p(y)$. Thus $\langle\mathbf1,\chi_p\rangle_p=\sum_{y\in Y_p}\chi_p(y)=0$ by step 2.1. The complement $C=Y_p\setminus\mathcal O_p$ is a subset of the finite set $Y_p$, so it is finite by [F8]. For $\langle f_p,\chi_p\rangle_p$, put the enumeration of the $r=|\mathcal O_p|$ orbit cosets first and append the enumeration of the $c=|C|$ complement cosets from [F8]. The two sets are disjoint and cover $Y_p$, so this lists each coset exactly once. The summands in the first list are the orbit signs and those in the second list are zero by the indicator values. Apply [F7] to the property that if $j\le c$, the partial sum after the first $r+j$ terms equals the orbit sum. At $j=0$ the first $r$ terms give exactly the orbit sum by [F5]. If $j+1\le c$, then $\sigma(j)\le c$, so $j<c$ and therefore $j\le c$ by [F9]. The preceding partial sum equals the orbit sum by the induction hypothesis. The next term is zero, so [F5] leaves that sum unchanged. Induction gives the property at $j=c$, and $c\le c$ by [F9], so $\langle f_p,\chi_p\rangle_p=\sum_{y\in\mathcal O_p}\chi_p(y)=0$ by step 2.1. [F1, F4, F5, F7, F8, F9, step 2.1]

4.1 By first-variable linearity, $\langle h_p,\chi_p\rangle_p=\langle f_p,\chi_p\rangle_p-\mu_p\langle\mathbf1,\chi_p\rangle_p=0$. With step 1.1, this gives both asserted orthogonalities and the squared norm identity. [F2, step 1.1, step 3.1] ∎
