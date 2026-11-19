---
title: Sizes of the projective unit image and quotient
status: published
research_item: lem-euler-hurwitz-quotient-size
dependency_level: 5
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: pp. 2–3, §3.1, reduction setup and equation (3.3)
      reading_limits: Read the order, unit list and reduction setup on PDF p. 2 and
        the scalar-unit assertion and counts on p. 3. This reference attributes
        the claims.
---

PDF p. 3: ` §3.1, scalar reductions and equation (3.3) `

## Prerequisites

- [def-euler-prime-classes](item-def-euler-prime-classes)
- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)
- [math:thm-standard-representatives-modulo-n](https://alphabetamath.cc/item/thm-standard-representatives-modulo-n)
- [math:def-group](https://alphabetamath.cc/item/def-group)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [lem-degree-two-projective-group-cardinality](item-lem-degree-two-projective-group-cardinality)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule)
- [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)


## Statement

Let $p\in\mathcal P_3$, the set of primes congruent to $3$ modulo $4$, and let $\mathbb F_p=\mathbb Z/p\mathbb Z$ be the field of integer residues modulo $p$. In the rational Hamilton quaternion algebra $B$, write elements in their unique coordinates as $a+bi+cj+dk$, with $a,b,c,d\in\mathbb Q$, identity $1$, and $i^2=j^2=-1$, $k=ij=-ji$. Its Hurwitz order $\mathcal H$ consists of the quaternions whose four coordinates are all integers or all in $\mathbb Z+\tfrac12=\{n+\tfrac12:n\in\mathbb Z\}$. It contains $1$ and is closed under addition, subtraction and multiplication. Write $\mathcal H^\times$ for its group of units, the elements $u$ admitting $v\in\mathcal H$ with $uv=vu=1$.

Use the reduction isomorphism $\bar\Phi_p:\mathcal H/p\mathcal H\to M_2(\mathbb F_p)$ of the chosen projective reduction. Here $\mathcal H/p\mathcal H$ has elements $u+p\mathcal H$, where $p\mathcal H=\{px:x\in\mathcal H\}$, and $M_2(\mathbb F_p)$ consists of the two-by-two matrices over $\mathbb F_p$. For $u\in\mathcal H^\times$, put $A_p(u)=\bar\Phi_p(u+p\mathcal H)$. In the projective linear group $G_p=\mathrm{PGL}_2(\mathbb F_p)$ an element is a class $[A]=\{tA:0\ne t\in\mathbb F_p\}$ of an invertible matrix $A$, and multiplication is $[A][B]=[AB]$. An invertible matrix has a two-sided matrix inverse. A unit has scalar reduction if $A_p(u)=tI_2$ for some $t\in\mathbb F_p$, where $I_2$ has ones on the diagonal and zeros elsewhere.

Write $\rho_p(u)=[A_p(u)]$, $\Gamma_p=\{\rho_p(u):u\in\mathcal H^\times\}$, and $Y_p=\Gamma_p\backslash G_p$ for the set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$ as $g$ ranges over $G_p$. The units with scalar reduction are exactly $1$ and $-1$. With $|S|$ denoting the number of elements of a finite set $S$, the counts are
$$|\Gamma_p|=12,\qquad |Y_p|=\frac{p(p^2-1)}{12}.$$

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[math:def-field](https://alphabetamath.cc/item/def-field)

[def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)

[def-euler-hurwitz-order](item-def-euler-hurwitz-order)

[math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group)

[lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction)

[def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[math:def-coset](https://alphabetamath.cc/item/def-coset)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

## Facts & Assumptions

[F1] A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Membership in $\mathcal P_3$ means $p$ is prime and $p=4r+3$ for some integer $r$. [def-euler-prime-classes](item-def-euler-prime-classes)

[F2] Quaternion coordinates are unique, addition is coordinatewise, and multiplying by a rational scalar multiplies each coordinate by it. The Hurwitz order has the coordinate description and the inherited operations in the Statement. [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions) [def-euler-hurwitz-order](item-def-euler-hurwitz-order)

[F3] The units of a ring form a group under multiplication. In $\mathcal H$ its $24$ units are $\pm1,\pm i,\pm j,\pm k$ and the sixteen elements $(\pm1\pm i\pm j\pm k)/2$ with four independent signs. [math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group) [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)

[F4] Every element of $\mathbb F_p$ is represented by an integer. Two integer representatives give the same residue exactly when their difference is an integer multiple of $p$. Addition of residues is computed by adding representatives, so the residue represented by $0$ is the additive identity. For prime $p$ the arithmetic of residues makes $\mathbb F_p$ a field, so its identities $0$ and $1$ are distinct and every nonzero element has a multiplicative inverse. The integers $0,\ldots,p-1$ represent distinct residues and exhaust the field. [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n) [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field) [math:def-field](https://alphabetamath.cc/item/def-field) [math:thm-standard-representatives-modulo-n](https://alphabetamath.cc/item/thm-standard-representatives-modulo-n)

[F5] At each odd prime the reduction map $\bar\Phi_p$ is a bijection preserving addition, multiplication, identity and the field scalar action. In the quotient the scalar represented by an integer $n$ acts by multiplication by $n1+p\mathcal H$. In particular, $\bar\Phi_p(n1+p\mathcal H)=(n\bmod p)I_2$. Two representatives of a coset of $p\mathcal H$ differ by an element of $p\mathcal H$. [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[F6] A group has an associative product with a two-sided identity and a two-sided inverse for every element. A subgroup contains the identity and is closed under products and inverses. In $G_p$ the identity $[I_2]$ consists of the nonzero scalar matrices. On $\mathcal H^\times$ the projective reduction preserves products and identity, and its image $\Gamma_p$ is a subgroup of $G_p$. The right coset represented by $g$ is $\Gamma_p g$ as in the Statement. [math:def-group](https://alphabetamath.cc/item/def-group) [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup) [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [math:def-coset](https://alphabetamath.cc/item/def-coset)

[F7] For a field $F$ with $q$ elements, $\mathrm{PGL}_2(F)$ is finite with $q(q^2-1)$ elements. For any subgroup $H$ of that group, the number of right cosets of $H$ is $q(q^2-1)/|H|$. [lem-degree-two-projective-group-cardinality](item-lem-degree-two-projective-group-cardinality)

[F8] The cardinality of a finite set is its number of elements. Every subset of a finite set is finite. The size of the union of a finite family of finite sets with no elements shared by distinct members equals the sum of the members' sizes. This finite sum adds one term per index, so a constant value $c$ across an index set $S$ gives the sum $c|S|$. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:thm-sum-rule](https://alphabetamath.cc/item/thm-sum-rule) [math:def-sum-over-a-finite-index-set](https://alphabetamath.cc/item/def-sum-over-a-finite-index-set)

## Proof

**Given:** $p\in\mathcal P_3$ and the Hurwitz units with the projective reduction at $p$ in the Statement.

**Goal:** Identify the units whose reductions are scalar matrices and compute $|\Gamma_p|$ and $|Y_p|$.

1.1 Since $p=4r+3>1$ for an integer $r$, one has $r\ge0$, so $p$ is odd and $p\ge3$. The residues of $0,1,2$ are therefore distinct by [F4]. Write $\overline{n}$ for the residue of an integer $n$. By addition on representatives, $\overline{n}+\overline{-n}=\overline{n+(-n)}=\overline{0}$, so the residue of $-n$ is the additive inverse of the residue of $n$. If $\overline{-n}$ were zero, this sum would give $\overline{n}=\overline{0}$. Applying this to $n=1,2$ shows that the residues of $1,2,-1,-2$ are all nonzero. [F1, F4]

2.1 Suppose $A_p(u)=tI_2$ for a unit $u$. Take an integer $n$ representing $t$ by [F4]. By [F5], $A_p(u)=\bar\Phi_p(n1+p\mathcal H)$, and injectivity gives $u+p\mathcal H=n1+p\mathcal H$. Thus $u-n1=pv$ for some $v\in\mathcal H$. Write $u=a+bi+cj+dk$ and $v=a'+b'i+c'j+d'k$. Comparing coordinates and doubling gives $2b=p(2b')$, $2c=p(2c')$ and $2d=p(2d')$. The doubled coordinates of every element of $\mathcal H$ are integers, so $2b,2c,2d$ differ from $0$ by integer multiples of $p$. By [F4], all three have residue zero modulo $p$. [F2, F4, F5, step 1.1]

3.1 Each of the coordinate units $\pm i,\pm j,\pm k$ has a doubled coordinate among $2b,2c,2d$ equal to $2$ or $-2$. For each of the sixteen units in the second list in [F3], all three of these doubled coordinates are $1$ or $-1$. Step 1.1 excludes zero residues in both cases, contradicting step 2.1. The remaining units $1$ and $-1$ both have nonzero scalar reduction by [F5] and step 1.1. Thus $\rho_p(w)=[I_2]$ holds for a unit $w$ exactly when $w=1$ or $w=-1$. [F3, F5, F6, step 1.1, step 2.1]

4.1 For units $u,v$, multiplicativity and identity preservation give $\rho_p(u^{-1})=\rho_p(u)^{-1}$, by applying $\rho_p$ to both inverse equations for $u$. If $\rho_p(v)=\rho_p(u)$, then $\rho_p(u^{-1}v)=[I_2]$, so step 3.1 gives $u^{-1}v=\pm1$ and $v=\pm u$. Conversely, $\rho_p(u\cdot 1)=\rho_p(u\cdot(-1))=\rho_p(u)$ by step 3.1. These two units are distinct because equality would give $1=-1$ upon multiplying by $u^{-1}$, even though $1$ and $-1$ have different first coordinates. For each $\gamma\in\Gamma_p$ there exists a unit with projective value $\gamma$, by the definition of $\Gamma_p$. Thus the set $S_\gamma=\{u\in\mathcal H^\times:\rho_p(u)=\gamma\}$ has exactly two elements. [F2, F3, F6, F8, step 3.1]

5.1 By [F4], the field $\mathbb F_p$ has $p$ elements, so [F7] gives $|G_p|=p(p^2-1)$. The subset $\Gamma_p$ of the finite group $G_p$ is finite. The sets $S_\gamma$ cover $\mathcal H^\times$ by the definition of $\Gamma_p$, and distinct indices give disjoint sets because a unit has a single value under $\rho_p$. By the finite sum rule, $24=|\mathcal H^\times|=\sum_{\gamma\in\Gamma_p}|S_\gamma|=2|\Gamma_p|$, hence $|\Gamma_p|=12$. [F3, F4, F6, F7, F8, step 4.1]

6.1 The subgroup $\Gamma_p$ satisfies the hypotheses of the right coset formula in [F7] with $q=p$. Consequently $|Y_p|=p(p^2-1)/|\Gamma_p|=p(p^2-1)/12$. Together with step 3.1 and step 5.1, this gives the scalar reductions and both cardinalities. [F4, F6, F7, step 3.1, step 5.1] ∎
