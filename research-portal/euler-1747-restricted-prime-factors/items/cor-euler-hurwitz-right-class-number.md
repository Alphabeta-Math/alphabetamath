---
id: cor-euler-hurwitz-right-class-number
kind: corollary
title: Principal right ideals and class number one
status: draft
domain: mathematics
deps:
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-quaternion-right-ideal-and-reduced-norm
  - def-author-291c0ff6bd53-quaternion-right-ideal-classes
  - thm-hurwitz-order-integral-structure
  - lem-rational-hamilton-norm-and-inverse
  - lem-euler-hurwitz-euclidean
  - math:lem-nat-embeds-int
  - math:thm-well-ordering-principle
  - math:lem-ring-elementary-consequences
  - math:def-subgroup
  - def-author-24fda87362bc-local-adic-valuation
  - def-author-24fda87362bc-hamilton-algebra-and-reduced-norm
  - def-author-24fda87362bc-quaternion-orders-and-lattice-completions
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
formulation_deps:
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-quaternion-right-ideal-and-reduced-norm
  - def-author-291c0ff6bd53-quaternion-right-ideal-classes
  - math:def-subgroup
  - def-author-24fda87362bc-local-adic-valuation
  - def-author-24fda87362bc-hamilton-algebra-and-reduced-norm
  - def-author-24fda87362bc-quaternion-orders-and-lattice-completions
argument_deps:
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-quaternion-right-ideal-and-reduced-norm
  - def-author-291c0ff6bd53-quaternion-right-ideal-classes
  - thm-hurwitz-order-integral-structure
  - lem-rational-hamilton-norm-and-inverse
  - lem-euler-hurwitz-euclidean
  - math:lem-nat-embeds-int
  - math:thm-well-ordering-principle
  - math:lem-ring-elementary-consequences
  - math:def-subgroup
  - def-author-24fda87362bc-local-adic-valuation
  - def-author-24fda87362bc-hamilton-algebra-and-reduced-norm
  - def-author-24fda87362bc-quaternion-orders-and-lattice-completions
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
dependency_roles:
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  def-quaternion-right-ideal-and-reduced-norm: mathematical-premise
  def-author-291c0ff6bd53-quaternion-right-ideal-classes: mathematical-premise
  thm-hurwitz-order-integral-structure: mathematical-premise
  lem-rational-hamilton-norm-and-inverse: mathematical-premise
  lem-euler-hurwitz-euclidean: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:thm-well-ordering-principle: mathematical-premise
  math:lem-ring-elementary-consequences: mathematical-premise
  math:def-subgroup: mathematical-premise
  def-author-24fda87362bc-local-adic-valuation: mathematical-premise
  def-author-24fda87362bc-hamilton-algebra-and-reduced-norm: mathematical-premise
  def-author-24fda87362bc-quaternion-orders-and-lattice-completions: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 2, §3.1, consequence of norm-Euclidean division
      reading_limits: PDF p. 2, §3.1, through the class-number assertion. The
        reference attributes the claim.
dependency_level: 5
---

## Statement

Let $B$ be the rational Hamilton quaternion algebra, with rational coordinates in the basis $1,i,j,k$ and the Hamilton product. Let $\mathcal H$ be its Hurwitz order, the subring of quaternions whose coordinates are all integers or all of the form $n+\tfrac12$ for integers $n$.

Every right ideal of $\mathcal H$ is principal. A right ideal is an additive subgroup of $\mathcal H$ closed under right multiplication by $\mathcal H$, and it is principal if it equals $b\mathcal H=\{bh:h\in\mathcal H\}$ for some $b\in\mathcal H$. Every right fractional ideal of $\mathcal H$, an integer span of a rational basis of $B$ stable under right multiplication by $\mathcal H$, has the form $b\mathcal H$ for some invertible $b\in B$.

In particular, the right ideal class number of $\mathcal H$ is one. Its set of locally principal right fractional ideals modulo left multiplication by invertible elements of $B$ has the sole class $[\mathcal H]$. A fractional ideal $I$ is locally principal if at every prime $\ell$ the completed ideal is $I_\ell=x_\ell\mathcal H_\ell$ with $x_\ell$ invertible in the Hamilton algebra over the $\ell$-adic numbers. The completions are spans over the $\ell$-adic integers.

## Statement references

[[def-euler-hamilton-quaternions|Rational Hamilton quaternions]]

[[def-euler-hurwitz-order|The Hurwitz order]]

[[def-quaternion-right-ideal-and-reduced-norm|Right ideals and local principality]]

[[def-author-291c0ff6bd53-quaternion-right-ideal-classes|The right ideal class set and its cardinality]]

[[math:def-subgroup|Additive subgroup conditions]]

[[def-author-24fda87362bc-local-adic-valuation|The local field and its ring of integers]]

[[def-author-24fda87362bc-hamilton-algebra-and-reduced-norm|The local Hamilton algebra and its units]]

[[def-author-24fda87362bc-quaternion-orders-and-lattice-completions|The coefficient inclusion and lattice completions]]

## Facts & Assumptions

[F1] The rational Hamilton algebra $B$ has rational coefficients in $1,i,j,k$, with $i^2=j^2=k^2=-1$, $ij=k=-ji$, $jk=i=-kj$ and $ki=j=-ik$. The multiplication is associative and linear over the rationals in each factor. Rational scalars act centrally, meaning they commute with each quaternion. Its reduced norm is $N(a+bi+cj+dk)=a^2+b^2+c^2+d^2$. [[def-euler-hamilton-quaternions]]

[F2] The coordinate description of $\mathcal H$ is as in the statement. It is a unital subring of $B$, is the integer span of a rational basis of $B$, and $N(x)\in\mathbb Z$ for $x\in\mathcal H$. [[def-euler-hurwitz-order]] [[thm-hurwitz-order-integral-structure]]

[F3] The reduced norm of a nonzero rational Hamilton quaternion is positive, as its real value is the sum of four squares with at least one positive term. Every nonzero element of $B$ has a two-sided inverse in $B$. [[lem-rational-hamilton-norm-and-inverse]]

[F4] A right ideal of the ring is an additive subgroup stable under right multiplication. A right fractional ideal is a full integral lattice, the integer span of a rational basis, stable under the same multiplication. A positive integer can clear the denominators of the basis of a fractional ideal expressed in a basis of the order, so the scaled ideal lies in the order. An additive subgroup contains zero and is closed under addition and additive inverses. [[def-quaternion-right-ideal-and-reduced-norm]] [[math:def-subgroup]]

[F5] For $a,b\in\mathcal H$ with $b\ne0$, norm-Euclidean division with the quotient on the right gives $q,r\in\mathcal H$ with $a=bq+r$ and $N(r)<N(b)$ in the real order. [[lem-euler-hurwitz-euclidean]]

[F6] The natural numbers embed order-preservingly in the integers with image the nonnegative integers. Every nonempty subset of the natural numbers has a least element, an element less than or equal to all its members. [[math:lem-nat-embeds-int]] [[math:thm-well-ordering-principle]]

[F7] In a ring the zero element multiplied by any element is zero. [[math:lem-ring-elementary-consequences]]

[F8] The class set consists of locally principal right fractional ideals modulo $I\sim J$ if $J=xI$ for $x\in B^\times$. This is an equivalence relation on the set of locally principal right fractional ideals. [[def-author-291c0ff6bd53-quaternion-right-ideal-classes]]

[F9] For each prime $\ell$, $\mathbb Q_\ell$ is the $\ell$-adic completion of $\mathbb Q$, and $\mathbb Z_\ell$ is its subring of $\ell$-adic integers. [[def-author-24fda87362bc-local-adic-valuation]] The algebra $B_\ell=B(\mathbb Q_\ell)$ uses the Hamilton product over $\mathbb Q_\ell$. Its units are the elements with two-sided inverses. [[def-author-24fda87362bc-hamilton-algebra-and-reduced-norm]] The rational algebra embeds in $B_\ell$ by coefficient inclusion. The completions $I_\ell$ and $\mathcal H_\ell$ are the $\mathbb Z_\ell$-spans of $I$ and $\mathcal H$ inside $B_\ell$. [[def-author-24fda87362bc-quaternion-orders-and-lattice-completions]]

[F10] The maps $n\mapsto n/1$ from the integers to the rationals and $t\mapsto\widehat t$ from the rationals to the constant-sequence classes in the reals preserve arithmetic and preserve and reflect strict order. The composite map sends zero to zero and sends the integer norm of each $a\in\mathcal H$ to the real value of the same sum of coordinate squares. [[math:lem-int-embeds-rat]] [[math:lem-rat-embeds-dense]]

## Proof

**Given:** The Hurwitz order $\mathcal H$ in $B$.

**Goal:** Generate every right ideal and every right fractional ideal by one element, and show that the right ideal class set has exactly one element.

1.1 Let $I$ be a right ideal of the ring $\mathcal H$. If $I=\{0\}$, then $I=0\mathcal H$ by [F7]. Otherwise the set $\{N(a):a\in I,\ a\ne0\}$ is nonempty and consists of integers by [F2]. The real images of those integers are positive by [F3], so the integer norms are positive by [F10]. The norm set therefore has a nonempty preimage in the natural numbers. By [F6] its least element maps to a least integer norm. By the definition of the norm set there is a nonzero $b\in I$ whose norm is that element. [given, F2, F3, F4, F6, F7, F10]

2.1 Take $a\in I$ in the nonzero case. Apply [F5] to $a,b$ to write $a=bq+r$ with $q,r\in\mathcal H$ and $N(r)<N(b)$. Since $b\in I$ and $q\in\mathcal H$, we have $bq\in I$. Closure under additive inverses and addition gives $r=a+(-(bq))\in I$. If $r\ne0$, its integer norm belongs to the norm set in step 1.1 by [F2]. The strict inequality of real norms gives a strict inequality of integer norms by [F10], contradicting the choice of $b$. Hence $r=0$ and $a\in b\mathcal H$. Conversely $b\mathcal H\subseteq I$ by stability under right multiplication. Thus $I=b\mathcal H$. [F2, F4, F5, F10, step 1.1]

3.1 Let $J$ be a right fractional ideal of $\mathcal H$. Choose a positive integer $d$ clearing the denominators of its four basis vectors in the rational basis of $\mathcal H$ as in [F4], so $dJ\subseteq\mathcal H$. The rational scalar $d$ has an inverse in $B$ by [F1] and [F3], so $dJ$ is nonzero because $J$ contains its rational basis. The integer span $J$ contains zero and is closed under addition and additive inverses. Multiplication by $d$ preserves these operations, so $dJ$ is an additive subgroup. Also $(dy)h=d(yh)\in dJ$ for $y\in J$ and $h\in\mathcal H$. Thus $dJ$ is a nonzero right ideal of the ring, and the preceding steps give $dJ=b\mathcal H$ for a nonzero $b\in\mathcal H$. Multiplying on the left by $d^{-1}$ gives $J=(d^{-1}b)\mathcal H$ with $d^{-1}b\in B^\times$, since its inverse is $b^{-1}d$. [F1, F2, F3, F4, step 1.1, step 2.1]

4.1 By [F2], $\mathcal H$ is a full integral lattice stable under right multiplication by $\mathcal H$. At every prime $\ell$ its span from [F9] satisfies $\mathcal H_\ell=1\mathcal H_\ell$, with $1$ its own two-sided inverse in $B_\ell$. Thus $\mathcal H$ is locally principal and represents a class by [F8]. For each locally principal right fractional ideal $J$, step 3.1 supplies $x\in B^\times$ with $J=x\mathcal H$. Hence $\mathcal H\sim J$, so every such ideal represents $[\mathcal H]$. This is the sole class, and the class number is one. The principal generation claims follow from the preceding steps. [F2, F4, F8, F9, step 1.1, step 2.1, step 3.1] ∎
