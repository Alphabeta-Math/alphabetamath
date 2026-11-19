---
title: One-dimensional spectrum in the finite quotient
status: published
research_item: lem-euler-hurwitz-automorphic-characters
dependency_level: 8
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, Lemma 3.2, paragraph beginning with the one-dimensional
        automorphic representations
      reading_limits: Read the paragraph and surrounding proof on the frozen PDF page.
        Attribution for the article claim.
---

PDF p. 3: ` Lemma 3.2, paragraph on one-dimensional automorphic representations `

## Prerequisites

- [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)
- [math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra)
- [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)
- [math:def-locally-compact-space](https://alphabetamath.cc/item/def-locally-compact-space)
- [math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)
- [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [def-euler-prime-classes](item-def-euler-prime-classes)
- [def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [def-finite-quaternion-adeles-and-projective-units](item-def-finite-quaternion-adeles-and-projective-units)
- [def-author-5b8600b4f4af-full-adelic-hamilton-group](item-def-author-5b8600b4f4af-full-adelic-hamilton-group)
- [def-author-6f52147f3ab3-finite-quaternion-ideles](item-def-author-6f52147f3ab3-finite-quaternion-ideles)
- [def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles)
- [math:def-radon-measure-on-an-lch-space](https://alphabetamath.cc/item/def-radon-measure-on-an-lch-space)
- [lem-author-5b8600b4f4af-hamilton-invariant-quotient](item-lem-author-5b8600b4f4af-hamilton-invariant-quotient)
- [def-definite-quaternion-automorphic-fixed-space](item-def-definite-quaternion-automorphic-fixed-space)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)
- [def-euler-hurwitz-adelic-level](item-def-euler-hurwitz-adelic-level)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [lem-euler-hurwitz-adelic-identification](item-lem-euler-hurwitz-adelic-identification)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)
- [math:def-legendre-symbol](https://alphabetamath.cc/item/def-legendre-symbol)
- [lem-euler-hurwitz-determinant-character-well-defined](item-lem-euler-hurwitz-determinant-character-well-defined)
- [lem-projective-determinant-square-class](item-lem-projective-determinant-square-class)
- [thm-projective-quaternion-norm-characters](item-thm-projective-quaternion-norm-characters)
- [math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes)
- [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)
- [math:cor-square-matrix-invertible-iff-determinant-is-a-unit](https://alphabetamath.cc/item/cor-square-matrix-invertible-iff-determinant-is-a-unit)
- [math:cor-p-adic-simple-root-lifting](https://alphabetamath.cc/item/cor-p-adic-simple-root-lifting)
- [math:def-polynomial-ring-over-a-commutative-ring](https://alphabetamath.cc/item/def-polynomial-ring-over-a-commutative-ring)
- [math:def-polynomial-evaluation-and-root](https://alphabetamath.cc/item/def-polynomial-evaluation-and-root)
- [math:def-formal-derivative-of-a-polynomial](https://alphabetamath.cc/item/def-formal-derivative-of-a-polynomial)
- [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)
- [math:prop-legendre-symbol-on-units-is-homomorphism](https://alphabetamath.cc/item/prop-legendre-symbol-on-units-is-homomorphism)
- [def-euler-hurwitz-determinant-character](item-def-euler-hurwitz-determinant-character)
- [math:def-double-cosets-of-two-subgroups](https://alphabetamath.cc/item/def-double-cosets-of-two-subgroups)
- [math:def-complex-lp-and-euclidean-test-function-conventions](https://alphabetamath.cc/item/def-complex-lp-and-euclidean-test-function-conventions)


## Statement

Assume the Axiom of Choice, that every family of nonempty sets admits a function choosing one member from each set. Let $B$ be the rational Hamilton quaternion algebra with basis $1,i,j,k$, where $i^2=j^2=-1$ and $ij=k=-ji$. Its reduced norm is $N(x)=x_0^2+x_1^2+x_2^2+x_3^2$ in these coordinates. Let $\mathcal H$ be the Hurwitz order, the subring whose four coordinates are all integers or all in $\mathbb Z+\tfrac12$. A unit is an element with a two-sided multiplicative inverse.

Write $G=PB^\times$ for the projective quaternion unit group. At a field of coefficients its elements are quaternion units identified up to multiplication by nonzero scalars. Let $H=G(\mathbb R)\times G(\mathbb A_f)$ be the full adelic group. An element of $G(\mathbb A_f)$ is a tuple of local projective classes lying in $K_\ell=\operatorname{im}(\mathcal H_\ell^\times\to G(\mathbb Q_\ell))$ at all but finitely many primes $\ell$. Here $\mathbb Q_\ell$ is the completion of $\mathbb Q$ for the distance $\ell^{-v_\ell(a-b)}$ for $a\ne b$ and zero for $a=b$, where $v_\ell$ counts the exponent of $\ell$ in the numerator minus that in the denominator. The ring $\mathbb Z_\ell$ consists of compatible residues modulo powers of $\ell$, with each residue after the first reducing to the preceding one. Via the canonical embedding, these residues form the subring of $\mathbb Q_\ell$ of elements with $\ell$-adic absolute value at most one. The local order $\mathcal H_\ell$ is the $\mathbb Z_\ell$-span of $\mathcal H$ in the algebra with coefficients extended to $\mathbb Q_\ell$. Use the finite restricted product topology, whose basic open boxes have factors $K_\ell$ at all but finitely many primes, and the product with the real projective topology induced from real quaternion coordinates. Put $\Gamma=G(\mathbb Q)$ embedded by taking the same rational class at every place, and let $X=\Gamma\backslash H$ be the space of right cosets with the quotient topology from the projection $h\mapsto\Gamma h$ on $H$. Under the stated Choice assumption, $X$ is locally compact Hausdorff.

Fix a nonzero right-invariant Radon measure $\mu$ on $X$. This is a measure on the Borel sets, the sigma-algebra generated by open sets. It is finite on compact sets, outer regular on Borel sets by approximation by open supersets, and inner regular on open sets by approximation by compact subsets. Right invariance is $\mu(Eh)=\mu(E)$ for every Borel set $E$ and $h\in H$. A one-dimensional automorphic representation here is a nonzero complex line $M$ in $L^2(X,\mu;\mathbb C)$ invariant under all right translations $R(h)[f]=[x\mapsto f(xh)]$. The space consists of square-integrable complex functions modulo equality outside a set of measure zero.

On each such line the action factors through the reduced norm. More precisely, the line is represented by the functions $\Gamma h\mapsto c\,\eta([N(\widetilde h)])$ for $c\in\mathbb C$, and $R(h)$ acts by the scalar $\eta([N(\widetilde h)])$. Here $\widetilde h$ is a lift consisting of a real quaternion unit and a finite tuple of local quaternion units belonging to $\mathcal H_\ell^\times$ at all but finitely many primes. The norm idele $N(\widetilde h)$ is the tuple of the coordinatewise reduced norms. A scalar idele consists of a nonzero real number and nonzero local scalars in $\mathbb Z_\ell^\times$ at all but finitely many primes, with componentwise multiplication. Give the real factor $\mathbb R^\times$ its usual topology and the finite factor $\mathbb A_f^\times$ the restricted product topology, whose basic boxes have factors $\mathbb Z_\ell^\times$ at all but finitely many primes. The full scalar idele group $\mathbb A^\times=\mathbb R^\times\times\mathbb A_f^\times$ has the product of these two topologies. The brackets on the norm denote its class modulo diagonal nonzero rational scalars. The idele class group $\mathbb Q^\times\backslash\mathbb A^\times$ has the quotient topology from the canonical projection of $\mathbb A^\times$. A subset is open exactly when its preimage under this projection is open. A quadratic idele class character $\eta$ is a continuous map from that quotient group to the signs $\{1,-1\}$ that preserves products. The signs have the discrete topology, in which every subset is open. The constant value $1$ is allowed.

Now let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$. Use the fixed integral splitting at $p$, an algebra isomorphism taking the local quaternion algebra and its order to the two-by-two matrices over $\mathbb Q_p$ and $\mathbb Z_p$, respectively. The group $G_p=\mathrm{PGL}_2(\mathbb F_p)$ consists of invertible two-by-two matrices over the field $\mathbb F_p=\mathbb Z/p\mathbb Z$ of integer residues modulo $p$, identified up to multiplication by nonzero scalars. The reduction $r_p:K_p\to G_p$ sends the class of an integral invertible matrix to the projective class of its entrywise reduction modulo $p$. Put $U(p)=\{(g_\ell):g_\ell\in K_\ell\ \text{for }\ell\ne p,\ g_p\in K_p,\ r_p(g_p)=1\}$. Let $\Gamma_p$ be the image of $\mathcal H^\times$ by taking each unit's local class at $p$ and applying $r_p$, and let $Y_p=\Gamma_p\backslash G_p$ be the set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$.

The fixed space at this level consists of vectors fixed by every element of $G(\mathbb R)\times U(p)$. Identify it with the complex functions on $Y_p$ via $X\to G(\mathbb Q)\backslash G(\mathbb A_f)/U(p)\simeq Y_p$, where a double coset $G(\mathbb Q)gU(p)$ consists of the products $agu$ with $a\in G(\mathbb Q)$ and $u\in U(p)$. For each one-dimensional automorphic representation with a nonzero fixed vector at this level, its functions on $Y_p$ depend only on the determinant square class in $\mathbb F_p^\times/(\mathbb F_p^\times)^2$. The square class of $t$ is the coset of $t$ modulo the subgroup of nonzero squares. Each such function is a scalar multiple of $\mathbf1$, the constant function of value $1$, or of $\chi_p$, which assigns $\Gamma_p[A]$ the Legendre symbol of $\det A$. For nonzero residues the Legendre symbol is $1$ on squares and $-1$ on nonsquares, and the determinant for rows $(a,b),(c,d)$ is $ad-bc$. In particular the span of the one-dimensional contributions at this level is contained in $\operatorname{span}_{\mathbb C}\{\mathbf1,\chi_p\}$, the space of complex linear combinations of these two functions.

## Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[def-euler-prime-classes](item-def-euler-prime-classes)

[def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)

[def-euler-hurwitz-order](item-def-euler-hurwitz-order)

[def-finite-quaternion-adeles-and-projective-units](item-def-finite-quaternion-adeles-and-projective-units)

[def-author-5b8600b4f4af-full-adelic-hamilton-group](item-def-author-5b8600b4f4af-full-adelic-hamilton-group)

[def-author-6f52147f3ab3-finite-quaternion-ideles](item-def-author-6f52147f3ab3-finite-quaternion-ideles)

[def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles)

[math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)

[lem-author-5b8600b4f4af-hamilton-invariant-quotient](item-lem-author-5b8600b4f4af-hamilton-invariant-quotient)

[math:def-radon-measure-on-an-lch-space](https://alphabetamath.cc/item/def-radon-measure-on-an-lch-space)

[math:def-locally-compact-space](https://alphabetamath.cc/item/def-locally-compact-space)

[math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space)

[math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)

[def-definite-quaternion-automorphic-fixed-space](item-def-definite-quaternion-automorphic-fixed-space)

[math:def-coset](https://alphabetamath.cc/item/def-coset)

[math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)

[def-euler-hurwitz-adelic-level](item-def-euler-hurwitz-adelic-level)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[lem-euler-hurwitz-adelic-identification](item-lem-euler-hurwitz-adelic-identification)

[def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)

[math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)

[math:def-legendre-symbol](https://alphabetamath.cc/item/def-legendre-symbol)

[lem-euler-hurwitz-determinant-character-well-defined](item-lem-euler-hurwitz-determinant-character-well-defined)

[lem-projective-determinant-square-class](item-lem-projective-determinant-square-class)

[thm-projective-quaternion-norm-characters](item-thm-projective-quaternion-norm-characters)

[math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes)

[math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[def-euler-hurwitz-determinant-character](item-def-euler-hurwitz-determinant-character)

[math:def-double-cosets-of-two-subgroups](https://alphabetamath.cc/item/def-double-cosets-of-two-subgroups)

[math:def-complex-lp-and-euclidean-test-function-conventions](https://alphabetamath.cc/item/def-complex-lp-and-euclidean-test-function-conventions)

[math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)

[math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra)

[math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)

[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)

## Facts & Assumptions

[A1] Assume the Axiom of Choice in the stated form. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] For the Hamilton algebra over the real or local field, conjugation is $\bar x=x_0-x_1i-x_2j-x_3k$ and $x\bar x=N(x)1$. This norm is multiplicative and $N(s1)=s^2$ for scalars $s$. [def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)

[F2] The full projective adelic group has the real and finite factors stated above. Representatives of the same full adelic element differ by multiplication by a scalar idele. Both types of ideles multiply componentwise and the quotient groups multiply classes by multiplying their representatives. [def-author-5b8600b4f4af-full-adelic-hamilton-group](item-def-author-5b8600b4f4af-full-adelic-hamilton-group) [def-finite-quaternion-adeles-and-projective-units](item-def-finite-quaternion-adeles-and-projective-units) [def-author-6f52147f3ab3-finite-quaternion-ideles](item-def-author-6f52147f3ab3-finite-quaternion-ideles) [def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles) [math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)

[F3] Under [A1], the Hamilton quotient $X$ with the quotient topology from $h\mapsto\Gamma h$ on $H$ is locally compact Hausdorff. Under [A1], the norm-character theorem for the full projective Hamilton quotient with a nonzero right-invariant Radon measure gives, on each nonzero invariant complex line, the continuous representatives $\Gamma h\mapsto c\,\eta([N(\widetilde h)])$ for some quadratic idele class character $\eta$. The stated Radon regularity and compact finiteness are taken on that locally compact Hausdorff space. The measure is defined on the Borel sigma-algebra generated by the open sets of $X$. As in the norm-character theorem, the idele class group takes its topology from the quotient projection $\mathbb A^\times\to\mathbb Q^\times\backslash\mathbb A^\times$. The domain has the product of the usual topology on $\mathbb R^\times$ and the restricted product topology on $\mathbb A_f^\times$. [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology) [math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra) [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology) [def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles) [lem-author-5b8600b4f4af-hamilton-invariant-quotient](item-lem-author-5b8600b4f4af-hamilton-invariant-quotient) [thm-projective-quaternion-norm-characters](item-thm-projective-quaternion-norm-characters) [math:def-radon-measure-on-an-lch-space](https://alphabetamath.cc/item/def-radon-measure-on-an-lch-space) [math:def-locally-compact-space](https://alphabetamath.cc/item/def-locally-compact-space) [math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space) [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)

[F4] At a compact open finite level $U$, the fixed-space identification sends a function on the double coset set to the class of its composition with the quotient map. This applies to $U(p)$. Every finite double coset has an integral representative $k\in\prod_\ell K_\ell$ and maps to $\Gamma_p r_p(k_p)$. Both reductions use the same splitting, and $r_p$ is onto. [def-definite-quaternion-automorphic-fixed-space](item-def-definite-quaternion-automorphic-fixed-space) [def-euler-hurwitz-adelic-level](item-def-euler-hurwitz-adelic-level) [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [lem-euler-hurwitz-adelic-identification](item-lem-euler-hurwitz-adelic-identification) [math:def-coset](https://alphabetamath.cc/item/def-coset) [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[F5] The fixed splitting identifies $K_p$ with the classes of invertible matrices over $\mathbb Z_p$ modulo unit scalars. Reduction takes such a class to the class of the entrywise reduction. The splitting preserves multiplication, the identity and scalar multiplication. For a square matrix of positive size over a commutative ring, invertibility is equivalent to its determinant being a unit. In size two the determinant is $ad-bc$. [def-euler-hurwitz-adelic-level](item-def-euler-hurwitz-adelic-level) [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group) [math:cor-square-matrix-invertible-iff-determinant-is-a-unit](https://alphabetamath.cc/item/cor-square-matrix-invertible-iff-determinant-is-a-unit) [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)

[F6] The ring of compatible residues modulo $p^n$ has componentwise operations and is identified with the elements of $p$-adic absolute value at most one in the completion field $\mathbb Q_p$. The residue ring modulo the integer $p$ in $\mathbb Z$ is the field $\mathbb F_p$. The prime $p$ here is odd since it is congruent to $3$ modulo $4$. [math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes) [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers) [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp) [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field) [def-euler-prime-classes](item-def-euler-prime-classes)

[F7] The polynomial ring $\mathbb Z_p[T]$ consists of finite formal sums $P(T)=\sum_{j\ge0}a_jT^j$ with coefficients $a_j\in\mathbb Z_p$. Evaluation at $t\in\mathbb Z_p$ is $P(t)=\sum_{j\ge0}a_jt^j$, and a root is a $t$ with $P(t)=0$. The formal derivative is $P'(T)=\sum_{j\ge1}ja_jT^{j-1}$, with $ja_j$ denoting the sum of $j$ copies of $a_j$. A polynomial $P(T)\in\mathbb Z_p[T]$ with $P(t_0)\equiv0\pmod{p\mathbb Z_p}$ and formal derivative $P'(t_0)\not\equiv0\pmod{p\mathbb Z_p}$ has a unique root in $\mathbb Z_p$ congruent to $t_0$ modulo $p\mathbb Z_p$. [math:def-polynomial-ring-over-a-commutative-ring](https://alphabetamath.cc/item/def-polynomial-ring-over-a-commutative-ring) [math:def-polynomial-evaluation-and-root](https://alphabetamath.cc/item/def-polynomial-evaluation-and-root) [math:def-formal-derivative-of-a-polynomial](https://alphabetamath.cc/item/def-formal-derivative-of-a-polynomial) [math:cor-p-adic-simple-root-lifting](https://alphabetamath.cc/item/cor-p-adic-simple-root-lifting)

[F8] On $\mathbb F_p^\times$ for odd $p$, the Legendre symbol is the unique nontrivial homomorphism to the signs. The determinant square-class map on $G_p$ preserves products and sends every element of $\Gamma_p$ to the class of a square. The Legendre symbol of the determinant therefore gives the well-defined function $\chi_p$ on $Y_p$. [math:prop-legendre-symbol-on-units-is-homomorphism](https://alphabetamath.cc/item/prop-legendre-symbol-on-units-is-homomorphism) [lem-projective-determinant-square-class](item-lem-projective-determinant-square-class) [lem-euler-hurwitz-determinant-character-well-defined](item-lem-euler-hurwitz-determinant-character-well-defined)

## Proof

**Given:** The Hamilton quotient, measure and invariant line above, and for the finite-level assertion the prime $p$ and level $U(p)$.

**Goal:** Obtain the norm factorization and determine the possible functions on $Y_p$ from the line when it contributes to the fixed space.

1.1 Apply [F3] to $M$ and let $\lambda(h)=\eta([N(\widetilde h)])$. This is a homomorphism on $H$ because product lifts give the norm product by [F1] and [F2]. Changing a lift by a scalar idele changes its norm by a square, which $\eta$ sends to $1$. The representatives $f_c(\Gamma g)=c\,\lambda(g)$ from [F3] satisfy $f_c(\Gamma gh)=\lambda(h)f_c(\Gamma g)$, giving the asserted right action. [A1, F1, F2, F3]

1.2 Write $\operatorname{red}$ for the first residue map $\mathbb Z_p\to\mathbb F_p$. To compute its kernel, suppose the first component of a compatible system $x$ vanishes. Dividing its component modulo $p^{n+1}$ by $p$ gives a residue modulo $p^n$, independent of the integer representative. These residues are compatible since the original representatives at successive levels agree modulo the smaller power. They define $y\in\mathbb Z_p$ with $x=py$. Conversely every multiple of $p$ has zero first residue, so the kernel is $p\mathbb Z_p$. The restriction of $\operatorname{red}$ to units is onto $\mathbb F_p^\times$. A unit reduces to a nonzero residue by reducing the equation with its inverse. For a nonzero residue $r$, take integer representatives $a$ of $r$ and $b$ of $r^{-1}$. The polynomial $aT-1$ vanishes at $b$ modulo $p$ and its derivative $a$ has nonzero residue. By [F7] it has a root in $\mathbb Z_p$, so $a$ is a unit lifting $r$. [F6, F7]

2.1 If $M$ has a nonzero vector fixed by $G(\mathbb R)\times U(p)$, the scalar formula forces $\lambda=1$ on this subgroup. Thus $f_c$ is constant on the fibers of the quotient map in [F4]. Indeed, if the finite components satisfy $g_f'=a_f g_f u$ with $a\in\Gamma$ and $u\in U(p)$, then $(g_\infty',g_f')=a(g_\infty,g_f)(v,u)$ for $v=(a_\infty g_\infty)^{-1}g_\infty'$. The left factor does not change the coset in $X$ and the right factor fixes $f_c$. For any $\Gamma_p g\in Y_p$ choose $k_p\in K_p$ with $r_p(k_p)=g$. Taking identity components at the real place and all other primes gives a representative of this point by [F4]. Write $\eta_p(t)$ for $\eta$ on the idele class with component $t\in\mathbb Q_p^\times$ at $p$ and $1$ elsewhere. This is a homomorphism to the signs because this insertion and the quotient map preserve multiplication. A lift with $\beta\in\mathcal H_p^\times$ at $p$ representing $k_p$ and $1$ elsewhere then gives the value $c\,\eta_p(N(\beta))$ on $Y_p$. [F2, F4, step 1.1]

3.1 Write $A=\Phi_p(\beta)=\begin{pmatrix}a&b\\c'&d\end{pmatrix}$, with $\Phi_p$ the fixed splitting. Since $\bar\beta=2\beta_0 1-\beta$, where $\beta_0$ is the coefficient of $1$ in $\beta$, [F1] gives $2\beta_0A-A^2=N(\beta)I_2$. Entrywise multiplication gives $(a+d)A-A^2=(ad-bc')I_2$. If $A$ is nonscalar, subtracting gives $(2\beta_0-a-d)A=(N(\beta)-\det A)I_2$. A nonzero coefficient on the left would make $A$ scalar over $\mathbb Q_p$, so the coefficient is zero and $N(\beta)=\det A$. If $A=sI_2$, injectivity and preservation of scalars give $\beta=s1$, and both expressions are $s^2$. In particular $N(\beta)=\det A$ is a unit in $\mathbb Z_p$, and its first residue is $\det(\bar A)$ because the first residue map preserves sums and products. [F1, F5, F6, step 2.1]

3.2 For $u\in\mathbb Z_p^\times$ of residue $1$, the polynomial $T^2-u$ vanishes at $1$ modulo $p\mathbb Z_p$ by step 1.2 and its derivative there is $2$, which has nonzero residue because $p$ is odd. By [F7] there is $s\in\mathbb Z_p$ with $s^2=u$ and residue $1$. This gives $\eta_p(u)=\eta_p(s)^2=1$. If two units have the same residue, their quotient has residue $1$, so their values under $\eta_p$ agree. Surjectivity in step 1.2 now defines a sign homomorphism on $\mathbb F_p^\times$ by the common value on unit lifts. It preserves products because a product of lifts lifts the product. By [F8] this homomorphism is trivial or the Legendre symbol. [F6, F7, F8, step 2.1, step 1.2]

4.1 By steps 2.1 and 3.1, the value on $\Gamma_p[\bar A]$ is $c\,\eta_p(\det A)$ with $\det A$ an integral unit of residue $\det(\bar A)$. Step 3.2 therefore makes the function either $c\,\mathbf1$ or $c\,\chi_p$. Each formula depends only on the square class of $\det(\bar A)$, since a sign homomorphism is trivial on squares. By [F8], multiplication on the left by an element of the subgroup $\Gamma_p$ leaves the determinant square class unchanged. Since every point of $Y_p$ has such a representative, all the one-dimensional fixed vectors give functions in the asserted span. [F4, F8, step 2.1, step 3.1, step 3.2] ∎
