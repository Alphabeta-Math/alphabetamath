---
title: The determinant character on the finite quotient
status: published
research_item: def-euler-hurwitz-determinant-character
dependency_level: 5
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, §3.2, displayed definition of the character before Lemma 3.2
      reading_limits: Read the displayed definition and its accompanying justification
        on PDF p. 3. This reference supplies attribution.
---

PDF p. 3: ` §3.2, definition of the character before Lemma 3.2 `

## Prerequisites

- [lem-square-residue-parity](item-lem-square-residue-parity)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [math:def-invertible-element](https://alphabetamath.cc/item/def-invertible-element)
- [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)
- [math:def-legendre-symbol](https://alphabetamath.cc/item/def-legendre-symbol)
- [math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)
- [lem-projective-determinant-square-class](item-lem-projective-determinant-square-class)
- [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)
- [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction)


## Definition

Let $p\in\mathcal P_3$, the set of primes of the form $4r+3$ with $r$ an integer. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Use the field $\mathbb F_p=\mathbb Z/p\mathbb Z$ of integer residues modulo $p$. Two integers give the same residue when their difference is a multiple of $p$. Addition and multiplication use integer representatives, and every nonzero residue has a multiplicative inverse.

In the projective linear group $G_p=\mathrm{PGL}_2(\mathbb F_p)$, an element $g=[A]$ is represented by an invertible two-by-two matrix $A$ over $\mathbb F_p$. Invertibility means having a two-sided matrix inverse. Its projective class is $[A]=\{tA:t\in\mathbb F_p,\ t\ne0\}$, where $tA$ multiplies each entry of $A$ by $t$. The group product is $[A][B]=[AB]$, where the matrix product has entries $(AB)_{ij}=a_{i1}b_{1j}+a_{i2}b_{2j}$.

The Hurwitz order $\mathcal H$ consists of the rational quaternions $a+bi+cj+dk$ whose four coordinates are all integers or all integers plus $\tfrac12$. Quaternion multiplication is associative and distributive, with identity $1$, rational scalars commuting with all elements, and $i^2=j^2=-1$, $ij=k=-ji$. Write $\mathcal H^\times$ for the units, the elements with a two-sided multiplicative inverse in $\mathcal H$. For such a unit $u$, the fixed projective reduction $\rho_p(u)$ is the projective class of the matrix corresponding to the residue of $u$ under the chosen identification of $\mathcal H/p\mathcal H$ with the two-by-two matrices over $\mathbb F_p$. Two elements of $\mathcal H$ have the same residue when their difference is $p$ times an element of $\mathcal H$. The image $\Gamma_p=\rho_p(\mathcal H^\times)$ is a subgroup of $G_p$, meaning it contains the identity and is closed under products and inverses. The set $Y_p=\Gamma_p\backslash G_p$ consists of the right cosets $\Gamma_pg=\{\gamma g:\gamma\in\Gamma_p\}$.

For a matrix $A$ with rows $(a,b)$ and $(c,d)$, its determinant is $\det A=ad-bc$. For a nonzero residue $x$, write $\left(\frac{x}{p}\right)$ for its Legendre symbol, which is $1$ if $x=t^2$ for some nonzero $t\in\mathbb F_p$ and $-1$ otherwise. Define the determinant character as the function
$$\chi_p:Y_p\longrightarrow\{1,-1\},\qquad \chi_p(\Gamma_p[A])=\left(\frac{\det A}{p}\right).$$

## Definition references

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)

[def-euler-hurwitz-order](item-def-euler-hurwitz-order)

[math:def-invertible-element](https://alphabetamath.cc/item/def-invertible-element)

[math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)

[math:def-coset](https://alphabetamath.cc/item/def-coset)

[math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)

[math:def-legendre-symbol](https://alphabetamath.cc/item/def-legendre-symbol)

## Facts & Assumptions

[F1] Each member of $\mathcal P_3$ is a prime and has the form $4r+3$ for an integer $r$. An integer of the form $2k+1$ is odd, and an integer of the form $2k$ is even. These cases are mutually exclusive. [lem-square-residue-parity](item-lem-square-residue-parity) The relation $2\mid p$ means $p=2q$ for some integer $q$. [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z) The ring of integer residue classes modulo a prime is a field with the operations in the definition. [def-euler-prime-classes](item-def-euler-prime-classes) [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n) [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[F2] In $G_p$, the projective representatives are exactly the nonzero scalar multiples of any one representative. The fixed reduction maps every unit of $\mathcal H$ into $G_p$ and its image on the units is the subgroup $\Gamma_p$. A right coset represented by $g$ is the set of all products $\gamma g$ with $\gamma\in\Gamma_p$. [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup) [math:def-coset](https://alphabetamath.cc/item/def-coset)

[F3] The two-by-two determinant formula is $ad-bc$ by the two terms of the determinant definition. The Legendre symbol of a nonzero residue is $1$ on squares and $-1$ on the other nonzero residues. [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix) [math:def-legendre-symbol](https://alphabetamath.cc/item/def-legendre-symbol)

[F4] For a prime $p$ with $2\nmid p$, an invertible matrix over $\mathbb F_p$ has nonzero determinant, and the function $s_p([A])=\left(\frac{\det A}{p}\right)$ is a sign character on $G_p$. A sign character is a group homomorphism to the group $\{1,-1\}$ under multiplication, so $s_p(gh)=s_p(g)s_p(h)$ for $g,h\in G_p$. [lem-projective-determinant-square-class](item-lem-projective-determinant-square-class) [math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)

[F5] A unit $u$ of the Hurwitz order has a two-sided inverse $v$ in that order, so $uv=vu=1$. Every such unit has reduced norm $\operatorname{nrd}(u)=1$, where the reduced norm of the quaternion $a+bi+cj+dk$ is $a^2+b^2+c^2+d^2$. [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions) [def-euler-hurwitz-order](item-def-euler-hurwitz-order) [math:def-invertible-element](https://alphabetamath.cc/item/def-invertible-element) [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)

[F6] For the reduction fixed in [F2], each $u\in\mathcal H^\times$ has a matrix $A_p(u)$ obtained by the reduction before taking its projective class. It satisfies $[A_p(u)]=\rho_p(u)$ and $\det A_p(u)=\operatorname{nrd}(u)\bmod p$, where the latter denotes the residue in $\mathbb F_p$. [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [lem-euler-hurwitz-odd-split-reduction](item-lem-euler-hurwitz-odd-split-reduction)

## Justification

The projective determinant sign is constant on the right cosets because it preserves products and is $1$ on every reduced Hurwitz unit. The proof verifies this and the invariance under nonzero scalar multiplication of a matrix representative. This gives a unique function on $Y_p$ with the displayed values.

## Proof

**Given:** A prime $p\in\mathcal P_3$, with $G_p$, $\rho_p$, $\Gamma_p$ and $Y_p$ as above.

**Goal:** Verify that $\chi_p$ takes a unique value in $\{1,-1\}$ at each coset, independent of both choices of representative.

1.1 Since $p=4r+3=2(2r+1)+1$, it is odd by [F1]. If $2\mid p$, the integer $p$ would be even by [F1], contradicting the exclusivity of the two parity cases. Thus $2\nmid p$, as required by [F4]. For $g=[A]\in G_p$, the determinant of $A$ is nonzero. Any other matrix representative of $g$ is $tA$ with $t\ne0$. The two-by-two formula gives $\det(tA)=t^2\det A$. If $\det A=x^2$ for some nonzero $x$, then $\det(tA)=(tx)^2$. Conversely, if $\det(tA)=y^2$ for some nonzero $y$, then $\det A=(t^{-1}y)^2$. Thus all matrix representatives give the same value $s_p(g)\in\{1,-1\}$. [F1, F2, F3, F4]

2.1 For any $\gamma\in\Gamma_p$, there is a Hurwitz unit $u$ with $\gamma=\rho_p(u)$. The matrix $A_p(u)$ represents $\gamma$ and its determinant is the residue of $\operatorname{nrd}(u)=1$, so it has determinant $1=1^2$ in $\mathbb F_p$. Therefore $s_p(\gamma)=1$. [F1, F2, F3, F5, F6, step 1.1]

3.1 Suppose $\Gamma_ph=\Gamma_pg$. Since the identity belongs to $\Gamma_p$, the element $h$ belongs to $\Gamma_ph=\Gamma_pg$, so $h=\gamma g$ for some $\gamma\in\Gamma_p$. By multiplicativity and step 2.1, $s_p(h)=s_p(\gamma)s_p(g)=s_p(g)$. Thus a coset representative gives a sign independent of both that representative and its representing matrix. Every coset has a representative by the definition of $Y_p$, so these signs give the unique function $\chi_p$ with the stated formula. [F2, F4, step 1.1, step 2.1] ∎
