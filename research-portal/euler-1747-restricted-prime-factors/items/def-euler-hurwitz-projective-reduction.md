---
id: def-euler-hurwitz-projective-reduction
kind: definition
title: The projective reduction quotient
status: draft
domain: mathematics
deps:
  - def-euler-prime-classes
  - def-euler-hurwitz-order
  - lem-rational-hamilton-norm-and-inverse
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - math:def-field-of-p-adic-numbers
  - math:thm-p-adic-completion-is-a-field
  - math:def-p-adic-integers-as-compatible-residue-classes
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - math:def-tensor-product-of-modules-by-generators-and-relations
  - math:thm-tensor-product-of-algebras-over-a-commutative-ring
  - lem-euler-hurwitz-odd-split-reduction
  - def-degree-two-projective-linear-group
  - math:lem-ring-units-form-a-group
  - math:def-coset
  - def-author-87b4d85727bc-counting-inner-product-on-finite-functions
  - math:thm-standard-representatives-modulo-n
  - math:cor-square-matrix-invertible-iff-determinant-is-a-unit
  - math:def-subgroup
  - lem-degree-two-projective-group-cardinality
  - math:lem-p-adic-valuation-on-q
  - math:def-p-adic-absolute-value-on-the-rationals
  - math:prop-integers-modulo-n-as-a-quotient-ring
formulation_deps:
  - def-euler-prime-classes
  - def-euler-hurwitz-order
  - lem-rational-hamilton-norm-and-inverse
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - math:thm-standard-representatives-modulo-n
  - math:def-field-of-p-adic-numbers
  - math:thm-p-adic-completion-is-a-field
  - math:def-p-adic-integers-as-compatible-residue-classes
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - math:def-tensor-product-of-modules-by-generators-and-relations
  - math:thm-tensor-product-of-algebras-over-a-commutative-ring
  - lem-euler-hurwitz-odd-split-reduction
  - def-degree-two-projective-linear-group
  - math:lem-ring-units-form-a-group
  - math:def-coset
  - def-author-87b4d85727bc-counting-inner-product-on-finite-functions
  - math:lem-p-adic-valuation-on-q
  - math:def-p-adic-absolute-value-on-the-rationals
  - math:prop-integers-modulo-n-as-a-quotient-ring
argument_deps:
  - def-euler-prime-classes
  - def-euler-hurwitz-order
  - lem-rational-hamilton-norm-and-inverse
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - math:thm-standard-representatives-modulo-n
  - lem-euler-hurwitz-odd-split-reduction
  - def-degree-two-projective-linear-group
  - math:cor-square-matrix-invertible-iff-determinant-is-a-unit
  - math:lem-ring-units-form-a-group
  - math:def-subgroup
  - math:def-coset
  - lem-degree-two-projective-group-cardinality
  - def-author-87b4d85727bc-counting-inner-product-on-finite-functions
  - math:lem-p-adic-valuation-on-q
  - math:def-p-adic-absolute-value-on-the-rationals
  - math:prop-integers-modulo-n-as-a-quotient-ring
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  lem-rational-hamilton-norm-and-inverse: mathematical-premise
  math:def-integers-modulo-n: mathematical-premise
  math:thm-z-mod-p-is-a-field: mathematical-premise
  math:def-field-of-p-adic-numbers: mathematical-premise
  math:thm-p-adic-completion-is-a-field: mathematical-premise
  math:def-p-adic-integers-as-compatible-residue-classes: mathematical-premise
  math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp: mathematical-premise
  math:def-tensor-product-of-modules-by-generators-and-relations: mathematical-premise
  math:thm-tensor-product-of-algebras-over-a-commutative-ring: mathematical-premise
  lem-euler-hurwitz-odd-split-reduction: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  math:lem-ring-units-form-a-group: mathematical-premise
  math:def-coset: mathematical-premise
  def-author-87b4d85727bc-counting-inner-product-on-finite-functions: mathematical-premise
  math:thm-standard-representatives-modulo-n: mathematical-premise
  math:cor-square-matrix-invertible-iff-determinant-is-a-unit: mathematical-premise
  math:def-subgroup: mathematical-premise
  lem-degree-two-projective-group-cardinality: mathematical-premise
  math:lem-p-adic-valuation-on-q: mathematical-premise
  math:def-p-adic-absolute-value-on-the-rationals: mathematical-premise
  math:prop-integers-modulo-n-as-a-quotient-ring: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: pp. 2–3, §3.1, final display on p. 2 and definitions surrounding (3.3)
        on p. 3
      reading_limits: Attribution for the definitions on PDF pages 2–3 of §3.1.
dependency_level: 4
---

## Definition

Let $p\in\mathcal P_3$, where $\mathcal P_3$ is the set of primes congruent to $3$ modulo $4$. Write $\mathbb F_p=\mathbb Z/p\mathbb Z$ for the field of integer residue classes modulo $p$, with addition and multiplication on representatives. Let $B$ be the rational Hamilton quaternion algebra, with coordinates in the basis $1,i,j,k$ where $i^2=j^2=-1$ and $k=ij=-ji$. Its Hurwitz order $\mathcal H$ is the subring with coordinates either all in $\mathbb Z$ or all in $\mathbb Z+\tfrac12$. For $\alpha=a+bi+cj+dk$, write $\operatorname{nrd}(\alpha)=a^2+b^2+c^2+d^2$ for the reduced norm.

Write $\mathbb Q_p$ for the field obtained by completing $\mathbb Q$ for the $p$-adic distance $d_p(x,y)=|x-y|_p$, with field operations extending those of $\mathbb Q$. For nonzero $z$, $|z|_p=p^{-v_p(z)}$, with $v_p(z)$ the exponent of $p$ in the numerator minus that in the denominator, and $|0|_p=0$. The ring $\mathbb Z_p$ of $p$-adic integers consists of tuples of residues modulo $p^n$ for $n\ge1$, with each residue reducing to the preceding one. Addition and multiplication are coordinatewise, and reduction modulo $p$ takes the first component. Use the canonical embedding $\iota_p:\mathbb Z_p\hookrightarrow\mathbb Q_p$ that sends a compatible tuple $(s_n)_{n\ge1}$ to the Cauchy class of the sequence of its standard integer representatives $b_n\in\{0,\ldots,p^n-1\}$.

The tensor products extend coefficients from $\mathbb Q$ to $\mathbb Q_p$ for $B$ and from $\mathbb Z$ to $\mathbb Z_p$ for $\mathcal H$. In each tensor product, multiplication on elementary tensors is $(x\otimes s)(y\otimes t)=xy\otimes st$, the identity is $1\otimes1$, and a coefficient $s$ acts by multiplication by $1\otimes s$. The inclusions $\mathcal H\subseteq B$ and $\iota_p$ induce the map $\jmath_p:\mathcal H\otimes_{\mathbb Z}\mathbb Z_p\to B\otimes_{\mathbb Q}\mathbb Q_p$ given by $x\otimes s\mapsto x\otimes\iota_p(s)$.

Fix one integral splitting $\Phi_p:B\otimes_{\mathbb Q}\mathbb Q_p\to M_2(\mathbb Q_p)$. Here $M_2(R)$ denotes the two-by-two matrices over $R$, with entrywise addition, row-by-column multiplication and scalars acting by scalar matrices. The splitting is an isomorphism preserving addition, multiplication, identity and the $\mathbb Q_p$-scalar action, taking the image of $\jmath_p$ onto $M_2(\mathbb Z_p)$ inside $M_2(\mathbb Q_p)$ via $\iota_p$.

Use this same splitting to define $\bar\Phi_p:\mathcal H/p\mathcal H\to M_2(\mathbb F_p)$ by reducing the entries of $\Phi_p(\alpha\otimes1)$ modulo $p$ on the additive coset $\alpha+p\mathcal H=\{\alpha+p\beta:\beta\in\mathcal H\}$. The quotient ring uses addition and multiplication of representatives.

Set $G_p=\mathrm{PGL}_2(\mathbb F_p)$. Its elements are classes $[A]=\{tA:t\in\mathbb F_p,\ t\ne0\}$ of invertible two-by-two matrices, where invertibility means having a two-sided matrix inverse. The group law is $[A][B]=[AB]$, with identity $[I_2]$ given by the matrix $I_2$ with diagonal entries $1$ and off-diagonal entries $0$. The domain $D_p=\{\alpha\in\mathcal H:p\nmid\operatorname{nrd}(\alpha)\}$ consists of elements whose integer reduced norm has nonzero residue modulo $p$. Define the projective reduction map by
$$\rho_p:D_p\to G_p,\qquad \rho_p(\alpha)=[\bar\Phi_p(\alpha+p\mathcal H)].$$

Write $\mathcal H^\times$ for the group of units of $\mathcal H$, the elements having a two-sided inverse in $\mathcal H$. Put $\Gamma_p=\rho_p(\mathcal H^\times)$ and define the quotient set of right cosets by
$$Y_p=\Gamma_p\backslash G_p=\{\Gamma_p g:g\in G_p\},\qquad \Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}.$$

Equip $\mathbb C[Y_p]$, the space of complex-valued functions on $Y_p$ with pointwise vector operations, with the counting inner product
$$\langle f,h\rangle_p=\sum_{y\in Y_p} f(y)\overline{h(y)}.$$
Each coset has weight $1$ in this finite sum. The bar denotes complex conjugation, which sends $a+bi$ to $a-bi$ for real $a,b$ and the complex imaginary unit $i$.

## Definition references

[[def-euler-prime-classes]]

[[def-euler-hurwitz-order]]

[[lem-rational-hamilton-norm-and-inverse]]

[[math:def-integers-modulo-n]]

[[math:thm-z-mod-p-is-a-field]]

[[math:thm-standard-representatives-modulo-n]]

[[math:def-field-of-p-adic-numbers]]

[[math:thm-p-adic-completion-is-a-field]]

[[math:def-p-adic-integers-as-compatible-residue-classes]]

[[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp]]

[[math:def-tensor-product-of-modules-by-generators-and-relations]]

[[math:thm-tensor-product-of-algebras-over-a-commutative-ring]]

[[lem-euler-hurwitz-odd-split-reduction]]

[[def-degree-two-projective-linear-group]]

[[math:lem-ring-units-form-a-group]]

[[math:def-coset]]

[[def-author-87b4d85727bc-counting-inner-product-on-finite-functions]]

[[math:lem-p-adic-valuation-on-q]]

[[math:def-p-adic-absolute-value-on-the-rationals]]

[[math:prop-integers-modulo-n-as-a-quotient-ring]]

## Facts & Assumptions

[F1] A prime in $\mathcal P_3$ is congruent to $3$ modulo $4$. [[def-euler-prime-classes]] The field $\mathbb F_p$ consists of congruence classes of integers modulo $p$, where $r$ and $s$ have the same class when $p$ divides $r-s$. Primality makes every nonzero class invertible. There are $p$ classes represented by $0,\ldots,p-1$. [[math:def-integers-modulo-n]] [[math:thm-z-mod-p-is-a-field]] [[math:thm-standard-representatives-modulo-n]]

[F2] The Hurwitz order is a subring of $B$ with the coordinate set above, and the reduced norm on $B$ is the displayed sum of squares. [[def-euler-hurwitz-order]] [[lem-rational-hamilton-norm-and-inverse]]

[F3] For every odd prime there is an integral splitting as specified above. It induces a unital algebra isomorphism on the quotient ring $\mathcal H/p\mathcal H$ and gives $\det\bar\Phi_p(\alpha+p\mathcal H)=\operatorname{nrd}(\alpha)\bmod p$ for every $\alpha\in\mathcal H$, with $\operatorname{nrd}(\alpha)\in\mathbb Z$. Here $\det$ is the determinant $ad-bc$ for a matrix with rows $(a,b)$ and $(c,d)$. [[lem-euler-hurwitz-odd-split-reduction]]

[F4] A square matrix of positive size over a commutative ring is invertible exactly when its determinant is a unit. [[math:cor-square-matrix-invertible-iff-determinant-is-a-unit]] Over a field the invertible two-by-two matrices form a group under matrix multiplication, and their projective classes form a group with the product and identity specified above. [[def-degree-two-projective-linear-group]]

[F5] The units of a ring form a group under its multiplication. A subgroup is a subset of a group containing the identity and closed under products and inverses. For such a subgroup $H$ of $G$, $Hg=\{hg:h\in H\}$ is its right coset represented by $g$. [[math:lem-ring-units-form-a-group]] [[math:def-subgroup]] [[math:def-coset]]

[F6] For a finite field $F$ with $q$ elements, $\mathrm{PGL}_2(F)$ has $q(q^2-1)$ elements and its set of right cosets by any subgroup is finite, with cardinality the group size divided by the subgroup size. [[lem-degree-two-projective-group-cardinality]]

[F7] On the complex functions on any nonempty finite set, the pointwise operations and the finite sum of products with conjugated second values define a complex inner product space, with the inner product linear in the first variable. [[def-author-87b4d85727bc-counting-inner-product-on-finite-functions]]

[F8] For a prime $p$ and nonzero rational $z$, the exponent of $p$ in the numerator minus that in the denominator is independent of the fraction representing $z$. [[math:lem-p-adic-valuation-on-q]] The $p$-adic absolute value is $p^{-v_p(z)}$ for $z\ne0$ and $0$ at zero. [[math:def-p-adic-absolute-value-on-the-rationals]]

[F9] For each positive integer $m$, the classes in $\mathbb Z/m\mathbb Z$ form a ring with $[a]_m+[b]_m=[a+b]_m$, $[a]_m[b]_m=[ab]_m$, and identity $[1]_m$. [[math:prop-integers-modulo-n-as-a-quotient-ring]]

## Justification

By [F8], changing a fraction representing a nonzero rational leaves the difference of the two exponents unchanged. The resulting absolute value is therefore independent of that choice, and its value at zero is given separately.

For $n\ge1$, the transition sends $[a]_{p^{n+1}}$ to $[a]_{p^n}$. If two representatives differ by a multiple of $p^{n+1}$, they differ by a multiple of $p^n$, so this map is well defined. The representative operations of [F9] show that the map preserves addition, multiplication and identity. Thus the componentwise sum, additive inverse and product of compatible tuples are compatible, and the tuple of identity classes is compatible. The ring laws hold in each component, and taking the first component $\mathbb Z_p\to\mathbb F_p$ preserves addition, multiplication and identity.

The chosen integral splitting fixes the matrix $\bar\Phi_p(\alpha+p\mathcal H)$ for every $\alpha\in\mathcal H$. The determinant criterion makes this matrix invertible on the specified domain, and the right cosets of the image subgroup supply the index set of the counting pairing.

## Proof

**Given:** $p\in\mathcal P_3$, the Hurwitz order $\mathcal H$ and the integral splitting from [F3] chosen once at $p$.

**Goal:** Verify the projective reduction, the quotient set, and its counting inner product.

1.1 Since $p$ is congruent to $3$ modulo $4$, it is odd, so [F3] applies. The quotient map $\alpha\mapsto\alpha+p\mathcal H$ preserves multiplication and identity by the operations of the quotient ring. Composing it with $\bar\Phi_p$, which is determined by the chosen splitting, gives the map $A_p(\alpha)=\bar\Phi_p(\alpha+p\mathcal H)$ with $A_p(\alpha\beta)=A_p(\alpha)A_p(\beta)$ and $A_p(1)=I_2$. [F1, F2, F3]

2.1 By the congruence of [F3], $\alpha\in D_p$ precisely when $\det A_p(\alpha)$ is nonzero in the field $\mathbb F_p$. By [F1] and [F4] this is equivalent to $A_p(\alpha)$ being invertible. Thus $1\in D_p$, and if $\alpha,\beta\in D_p$ then $A_p(\alpha\beta)$ is a product of two invertible matrices and hence is invertible. Therefore $\alpha\beta\in D_p$. Taking projective classes gives $\rho_p(1)=[I_2]$ and $\rho_p(\alpha\beta)=\rho_p(\alpha)\rho_p(\beta)$. [F1, F3, F4, step 1.1]

3.1 For $u\in\mathcal H^\times$, its inverse $v$ lies in $\mathcal H$. The equations $uv=vu=1$ give $A_p(u)A_p(v)=A_p(v)A_p(u)=I_2$. Hence both $u$ and $v$ belong to $D_p$. The unit group contains $1$ and is closed under products. By step 2.1 its image $\Gamma_p$ contains $[I_2]$, contains the product of any two of its elements, and contains the inverse $\rho_p(v)$ of every $\rho_p(u)$. Thus $\Gamma_p$ is a subgroup of $G_p$. [F5, step 1.1, step 2.1]

4.1 By [F5], the sets $\Gamma_p g$ are right cosets. Equality $\Gamma_p h=\Gamma_p g$ implies $h=\gamma g$ for some $\gamma\in\Gamma_p$ since $h\in\Gamma_p h$. Conversely, if $h=\gamma g$ with $\gamma\in\Gamma_p$, then $\Gamma_p h=(\Gamma_p\gamma)g=\Gamma_p g$, because right multiplication by $\gamma$ permutes the subgroup, with inverse right multiplication by $\gamma^{-1}$. The coset of $[I_2]$ belongs to $Y_p$, and $Y_p$ is finite by [F6] applied to the field of $p$ elements from [F1] and the subgroup of step 3.1. [F1, F5, F6, step 3.1]

5.1 By [F7] on the nonempty finite set $Y_p$, the pointwise operations give the complex function space and the displayed counting pairing gives its inner product. Each summand uses the value at a coset, so replacing any representative by one giving the same coset leaves that summand unchanged. This verifies the constructions in the definition. [F7, step 4.1] ∎
