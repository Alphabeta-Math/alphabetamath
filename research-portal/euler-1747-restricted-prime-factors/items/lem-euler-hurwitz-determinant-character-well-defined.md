---
id: lem-euler-hurwitz-determinant-character-well-defined
kind: lemma
title: The determinant character descends to the quotient
status: draft
domain: mathematics
deps:
  - def-euler-prime-classes
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - def-degree-two-projective-linear-group
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - math:def-invertible-element
  - def-euler-hurwitz-projective-reduction
  - math:def-subgroup
  - math:def-coset
  - math:def-determinant-of-a-square-matrix
  - math:def-legendre-symbol
  - def-euler-hurwitz-determinant-character
  - lem-projective-determinant-square-class
  - lem-euler-hurwitz-unit-list
  - lem-euler-hurwitz-odd-split-reduction
formulation_deps:
  - def-euler-prime-classes
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - def-degree-two-projective-linear-group
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - math:def-invertible-element
  - def-euler-hurwitz-projective-reduction
  - math:def-subgroup
  - math:def-coset
  - math:def-determinant-of-a-square-matrix
  - math:def-legendre-symbol
  - def-euler-hurwitz-determinant-character
argument_deps:
  - def-euler-prime-classes
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - def-degree-two-projective-linear-group
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - math:def-invertible-element
  - def-euler-hurwitz-projective-reduction
  - math:def-subgroup
  - math:def-coset
  - math:def-determinant-of-a-square-matrix
  - math:def-legendre-symbol
  - def-euler-hurwitz-determinant-character
  - lem-projective-determinant-square-class
  - lem-euler-hurwitz-unit-list
  - lem-euler-hurwitz-odd-split-reduction
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  math:def-integers-modulo-n: mathematical-premise
  math:thm-z-mod-p-is-a-field: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  math:def-invertible-element: mathematical-premise
  def-euler-hurwitz-projective-reduction: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-determinant-of-a-square-matrix: mathematical-premise
  math:def-legendre-symbol: mathematical-premise
  def-euler-hurwitz-determinant-character: mathematical-premise
  lem-projective-determinant-square-class: mathematical-premise
  lem-euler-hurwitz-unit-list: mathematical-premise
  lem-euler-hurwitz-odd-split-reduction: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, §3.2, displayed determinant character and the justification
        immediately following it
      reading_limits: Checked the displayed formula and the following justification on
        the frozen PDF page. This citation records attribution.
dependency_level: 6
---

## Statement

Let $p\in\mathcal P_3$, the set of primes of the form $4r+3$ with $r$ an integer. Write $\mathbb F_p=\mathbb Z/p\mathbb Z$ for the field of integer residues modulo $p$. Two integers have the same residue when their difference is divisible by $p$.

The projective linear group $G_p=\mathrm{PGL}_2(\mathbb F_p)$ consists of classes $[A]=\{tA:t\in\mathbb F_p,\ t\ne0\}$ of invertible two-by-two matrices $A$ over $\mathbb F_p$. Invertible means having a two-sided matrix inverse. The product is $[A][B]=[AB]$, with ordinary matrix multiplication.

The Hurwitz order $\mathcal H$ consists of the rational quaternions $a+bi+cj+dk$ whose four coordinates are all integers or all integers plus $\tfrac12$. It uses quaternion multiplication, with $i^2=j^2=-1$ and $ij=k=-ji$. Its units $\mathcal H^\times$ are the elements with two-sided inverses in $\mathcal H$. Let $\rho_p(u)$ be the projective class of the matrix of a unit $u$ under the fixed reduction modulo $p$. Put $\Gamma_p=\rho_p(\mathcal H^\times)$, a subgroup of $G_p$, and let $Y_p$ be the set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$ for $g\in G_p$.

Write $\det A=ad-bc$ for the determinant of a matrix with rows $(a,b)$ and $(c,d)$. For a nonzero $x\in\mathbb F_p$, the Legendre symbol $\left(\frac{x}{p}\right)$ is $1$ if $x$ is the square of a nonzero residue and $-1$ otherwise. Then the determinant character formula
$$\chi_p(\Gamma_p[A])=\left(\frac{\det A}{p}\right)$$
gives a unique function $Y_p\to\{1,-1\}$. Replacing $A$ by $tA$ for $t\ne0$ multiplies its determinant by $t^2$, and every matrix representing an element of $\Gamma_p$ has nonzero square determinant.

## Statement references

[[def-euler-prime-classes]]

[[math:def-integers-modulo-n]]

[[math:thm-z-mod-p-is-a-field]]

[[def-degree-two-projective-linear-group]]

[[def-euler-hamilton-quaternions]]

[[def-euler-hurwitz-order]]

[[math:def-invertible-element]]

[[def-euler-hurwitz-projective-reduction]]

[[math:def-subgroup]]

[[math:def-coset]]

[[math:def-determinant-of-a-square-matrix]]

[[math:def-legendre-symbol]]

[[def-euler-hurwitz-determinant-character]]

## Facts & Assumptions

[F1] A prime in $\mathcal P_3$ has the form $4r+3$ and is therefore odd. The integer residues modulo $p$ form a field, so every nonzero residue has a multiplicative inverse. [[def-euler-prime-classes]] [[math:def-integers-modulo-n]] [[math:thm-z-mod-p-is-a-field]]

[F2] The matrices representing a projective class $[A]$ are exactly the entrywise scalar multiples $tA$ with $t\ne0$. The group product is $[A][B]=[AB]$. [[def-degree-two-projective-linear-group]]

[F3] The fixed reduction assigns to a Hurwitz unit $u$ an invertible matrix $A_p(u)$ by taking its residue in $\mathcal H/p\mathcal H$ and applying the chosen identification with two-by-two matrices over $\mathbb F_p$. Two elements of $\mathcal H$ have the same residue here when their difference is $p$ times an element of $\mathcal H$. The class is $\rho_p(u)=[A_p(u)]$, and the image of the units is the subgroup $\Gamma_p$. A subgroup contains the group identity and is closed under products and inverses. The right coset represented by $g$ is precisely the set $\{\gamma g:\gamma\in\Gamma_p\}$. [[def-euler-hurwitz-projective-reduction]] [[math:def-subgroup]] [[math:def-coset]]

[F4] The two terms of the determinant definition give $ad-bc$ in size two. For odd $p$ the Legendre symbol is $1$ on nonzero squares and $-1$ on all other nonzero residues. [[math:def-determinant-of-a-square-matrix]] [[math:def-legendre-symbol]]

[F5] For an odd prime $p$, an invertible matrix over $\mathbb F_p$ has nonzero determinant, and $s_p([A])=\left(\frac{\det A}{p}\right)$ defines a map on $G_p$ with $s_p(gh)=s_p(g)s_p(h)$ for $g,h\in G_p$. [[lem-projective-determinant-square-class]]

[F6] The reduced norm of $u=a+bi+cj+dk$ is $\operatorname{nrd}(u)=a^2+b^2+c^2+d^2$. Its value is $1$ for every Hurwitz unit, meaning an element $u$ of the specified order with $uv=vu=1$ for some $v$ in the order. [[def-euler-hamilton-quaternions]] [[def-euler-hurwitz-order]] [[math:def-invertible-element]] [[lem-euler-hurwitz-unit-list]]

[F7] For the reduction in [F3] at an odd prime $p$, the determinant of $A_p(u)$ equals the residue of the integer $\operatorname{nrd}(u)$ modulo $p$. [[lem-euler-hurwitz-odd-split-reduction]]

[F8] The prescribed formula for $\chi_p$ assigns to $\Gamma_p[A]$ the Legendre symbol of $\det A$. [[def-euler-hurwitz-determinant-character]]

## Proof

**Given:** A prime $p\in\mathcal P_3$ and the fixed reduction used to construct $\Gamma_p$ and $Y_p$.

**Goal:** Verify the scalar determinant formula, square determinant on $\Gamma_p$, and independence of the choices in the formula for $\chi_p$.

1.1 For $g=[A]$ and another matrix representative $tA$, the determinant formula gives $\det(tA)=(ta)(td)-(tb)(tc)=t^2(ad-bc)=t^2\det A$. The determinant of $A$ is nonzero. If $\det A=x^2$, then $\det(tA)=(tx)^2$. Conversely, if $\det(tA)=y^2$, then $\det A=(t^{-1}y)^2$. Thus the Legendre symbol is unchanged and equals $s_p(g)$ for every matrix representing $g$. [F1, F2, F4, F5]

2.1 Take any $\gamma\in\Gamma_p$ and choose $u\in\mathcal H^\times$ with $\gamma=\rho_p(u)$. Then $A_p(u)$ represents $\gamma$, and its determinant is the residue of $\operatorname{nrd}(u)=1$. Every matrix representing $\gamma$ is $tA_p(u)$ for some nonzero $t$, so its determinant is the nonzero square $t^2$. In particular $s_p(\gamma)=1$. [F1, F2, F3, F4, F5, F6, F7, step 1.1]

3.1 If $\Gamma_p h=\Gamma_p g$, then $h\in\Gamma_p h$ because the identity belongs to $\Gamma_p$. Consequently $h=\gamma g$ for some $\gamma\in\Gamma_p$. The product rule for $s_p$ gives $s_p(h)=s_p(\gamma)s_p(g)=s_p(g)$. [F3, F5, step 2.1]

4.1 Every point in $Y_p$ is represented by some $g=[A]$. Its value in the prescribed formula is $s_p(g)$ by step 1.1, and step 3.1 gives the same value for every representative of that coset. Hence the rule determines exactly one value in $\{1,-1\}$ at each point and defines the claimed function $\chi_p$. [F2, F3, F5, F8, step 1.1, step 3.1] ∎
