---
id: def-euler-hurwitz-adelic-level
kind: definition
title: Projective quaternion group and finite adelic level
status: draft
domain: mathematics
deps:
  - math:def-prime
  - def-euler-prime-classes
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - thm-hurwitz-order-integral-structure
  - math:def-field-of-p-adic-numbers
  - math:lem-p-adic-valuation-on-q
  - math:thm-p-adic-completion-is-a-field
  - math:def-p-adic-integers-as-compatible-residue-classes
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - math:def-tensor-product-of-modules-by-generators-and-relations
  - math:thm-tensor-product-of-algebras-over-a-commutative-ring
  - def-author-6f52147f3ab3-hamilton-order-completions
  - def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles
  - def-finite-quaternion-adeles-and-projective-units
  - def-degree-two-projective-linear-group
  - thm-hurwitz-integral-splitting-at-odd-primes
  - def-euler-hurwitz-projective-reduction
  - math:def-local-ring
  - math:def-kernel-and-image-of-group-homomorphism
  - math:def-subgroup
  - math:thm-inverse-limit-topology-equals-the-p-adic-metric-topology
  - math:def-product-topology
  - math:def-compact-space
  - math:thm-closed-subspace-of-a-compact-space-is-compact
  - math:cor-square-matrix-invertible-iff-determinant-is-a-unit
  - math:def-relative-projective-space-standard-charts
  - math:def-group-scheme-over-a-field
  - math:def-affine-scheme
  - math:def-scheme-over-base
  - math:def-addition-and-multiplication-modulo-n
  - math:thm-integers-modulo-n-basic-algebra
  - math:def-subspace-topology-top
  - def-author-6f52147f3ab3-finite-quaternion-ideles
  - math:def-algebra-over-a-commutative-ring
  - math:thm-affine-scheme-ring-anti-equivalence
  - math:lem-group-homomorphism-basic-properties
formulation_deps:
  - math:def-prime
  - def-euler-prime-classes
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - thm-hurwitz-order-integral-structure
  - math:def-field-of-p-adic-numbers
  - math:lem-p-adic-valuation-on-q
  - math:thm-p-adic-completion-is-a-field
  - math:def-p-adic-integers-as-compatible-residue-classes
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - math:def-tensor-product-of-modules-by-generators-and-relations
  - math:thm-tensor-product-of-algebras-over-a-commutative-ring
  - def-author-6f52147f3ab3-hamilton-order-completions
  - def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles
  - def-finite-quaternion-adeles-and-projective-units
  - def-degree-two-projective-linear-group
  - thm-hurwitz-integral-splitting-at-odd-primes
  - def-euler-hurwitz-projective-reduction
  - math:def-kernel-and-image-of-group-homomorphism
  - math:def-subgroup
  - math:def-product-topology
  - math:def-compact-space
  - math:def-relative-projective-space-standard-charts
  - math:def-group-scheme-over-a-field
  - math:def-affine-scheme
  - math:def-scheme-over-base
  - math:def-addition-and-multiplication-modulo-n
  - math:thm-integers-modulo-n-basic-algebra
  - math:def-subspace-topology-top
  - math:def-algebra-over-a-commutative-ring
  - math:thm-affine-scheme-ring-anti-equivalence
argument_deps:
  - math:def-prime
  - def-euler-prime-classes
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - thm-hurwitz-order-integral-structure
  - math:def-field-of-p-adic-numbers
  - math:lem-p-adic-valuation-on-q
  - math:thm-p-adic-completion-is-a-field
  - math:def-p-adic-integers-as-compatible-residue-classes
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - math:def-integers-modulo-n
  - math:thm-z-mod-p-is-a-field
  - math:def-tensor-product-of-modules-by-generators-and-relations
  - math:thm-tensor-product-of-algebras-over-a-commutative-ring
  - def-author-6f52147f3ab3-hamilton-order-completions
  - def-finite-quaternion-adeles-and-projective-units
  - def-degree-two-projective-linear-group
  - thm-hurwitz-integral-splitting-at-odd-primes
  - def-euler-hurwitz-projective-reduction
  - math:def-local-ring
  - math:def-kernel-and-image-of-group-homomorphism
  - math:def-subgroup
  - math:thm-inverse-limit-topology-equals-the-p-adic-metric-topology
  - math:def-product-topology
  - math:def-compact-space
  - math:thm-closed-subspace-of-a-compact-space-is-compact
  - math:cor-square-matrix-invertible-iff-determinant-is-a-unit
  - math:def-relative-projective-space-standard-charts
  - math:def-group-scheme-over-a-field
  - math:def-affine-scheme
  - math:def-scheme-over-base
  - math:def-addition-and-multiplication-modulo-n
  - math:thm-integers-modulo-n-basic-algebra
  - math:def-subspace-topology-top
  - def-author-6f52147f3ab3-finite-quaternion-ideles
  - math:def-algebra-over-a-commutative-ring
  - math:thm-affine-scheme-ring-anti-equivalence
  - math:lem-group-homomorphism-basic-properties
dependency_roles:
  math:def-prime: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  thm-hurwitz-order-integral-structure: mathematical-premise
  math:def-field-of-p-adic-numbers: mathematical-premise
  math:lem-p-adic-valuation-on-q: mathematical-premise
  math:thm-p-adic-completion-is-a-field: mathematical-premise
  math:def-p-adic-integers-as-compatible-residue-classes: mathematical-premise
  math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp: mathematical-premise
  math:def-integers-modulo-n: mathematical-premise
  math:thm-z-mod-p-is-a-field: mathematical-premise
  math:def-tensor-product-of-modules-by-generators-and-relations: mathematical-premise
  math:thm-tensor-product-of-algebras-over-a-commutative-ring: mathematical-premise
  def-author-6f52147f3ab3-hamilton-order-completions: mathematical-premise
  def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles: mathematical-premise
  def-finite-quaternion-adeles-and-projective-units: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  thm-hurwitz-integral-splitting-at-odd-primes: mathematical-premise
  def-euler-hurwitz-projective-reduction: mathematical-premise
  math:def-local-ring: mathematical-premise
  math:def-kernel-and-image-of-group-homomorphism: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:thm-inverse-limit-topology-equals-the-p-adic-metric-topology: mathematical-premise
  math:def-product-topology: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:thm-closed-subspace-of-a-compact-space-is-compact: mathematical-premise
  math:cor-square-matrix-invertible-iff-determinant-is-a-unit: mathematical-premise
  math:def-relative-projective-space-standard-charts: mathematical-premise
  math:def-group-scheme-over-a-field: mathematical-premise
  math:def-affine-scheme: mathematical-premise
  math:def-scheme-over-base: mathematical-premise
  math:def-addition-and-multiplication-modulo-n: mathematical-premise
  math:thm-integers-modulo-n-basic-algebra: mathematical-premise
  math:def-subspace-topology-top: mathematical-premise
  def-author-6f52147f3ab3-finite-quaternion-ideles: mathematical-premise
  math:def-algebra-over-a-commutative-ring: mathematical-premise
  math:thm-affine-scheme-ring-anti-equivalence: mathematical-premise
  math:lem-group-homomorphism-basic-properties: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, Lemma 3.2, proof, definition of the compact open level
      reading_limits: Attribution for the local level and its product in the opening
        paragraph of the proof.
dependency_level: 5
---

## Definition

Let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$. A prime is an integer greater than $1$ with no positive divisors other than $1$ and itself. Let $B$ be the rational Hamilton quaternion algebra, with basis $1,i,j,k$ and products $i^2=j^2=-1$ and $ij=k=-ji$. Let $\mathcal H$ be its Hurwitz order, the subring whose four coordinates are either all integers or all in $\mathbb Z+\tfrac12$.

For each prime $\ell$, let $\mathbb Q_\ell$ be the field obtained by completing $\mathbb Q$ for the distance $d_\ell(x,y)=\ell^{-v_\ell(x-y)}$ for $x\ne y$ and $d_\ell(x,x)=0$. Here $v_\ell$ counts the exponent of $\ell$ in the numerator minus that in the denominator. Its subring $\mathbb Z_\ell$ consists of compatible tuples of residues modulo $\ell^n$ for $n\ge1$, with each residue reducing to the preceding one and with componentwise arithmetic. In each ring $\mathbb Z/\ell^n\mathbb Z$, addition and multiplication are induced by those on integer representatives. Put $B_\ell=B\otimes_{\mathbb Q}\mathbb Q_\ell$ and $\mathcal H_\ell=\mathcal H\otimes_{\mathbb Z}\mathbb Z_\ell\subset B_\ell$. These tensor products extend coefficients and multiply elementary tensors by $(x\otimes a)(y\otimes b)=xy\otimes ab$. A superscript $\times$ denotes elements with a two-sided multiplicative inverse in the indicated ring.

Write $G=PB^\times$ for the algebraic group of projective quaternion units over $\mathbb Q$. The standard affine chart of $\mathbb P^3_{\mathbb Q}$ indexed by $i$ has normalized coordinate $x_i=1$ and three coordinates $x_j/x_i$ for $j\ne i$. Two charts overlap where the new denominator is a unit, and their coordinates there are related by division by that denominator. On each chart take the open where the reduced norm $N(x)=x_0^2+x_1^2+x_2^2+x_3^2$ of the normalized tuple is a unit. These opens agree on overlaps because rescaling multiplies the norm by the square of a unit. They form the open subscheme $D_+(N)$, with group law induced by the Hamilton product.

A commutative unital $\mathbb Q$-algebra $R$ is a commutative unital ring with a unital ring homomorphism $\eta_R:\mathbb Q\to R$. The group $G(R)$ consists of $\mathbb Q$-scheme morphisms $\operatorname{Spec}R\to G$, where $\operatorname{Spec}R$ is the affine scheme of $R$. Such morphisms commute with the structure maps to $\operatorname{Spec}\mathbb Q$. The structure map of $\operatorname{Spec}R$ is $\operatorname{Spec}(\eta_R)$. The group structure on $G$ gives multiplication on these points. Over a field, a projective point is a nonzero tuple up to common nonzero scaling, and any nonzero coordinate can be the normalization denominator. In particular $G(\mathbb Q_\ell)=B_\ell^\times/\mathbb Q_\ell^\times$, with scalars embedded as $a1$ and multiplication on representatives. Let $\mathbb A_f$ be the finite adele ring, whose elements are tuples in $\prod_\ell\mathbb Q_\ell$ integral in $\mathbb Z_\ell$ at all but finitely many primes, with coordinatewise operations. Give $\mathbb A_f$ its $\mathbb Q$-algebra structure via the diagonal map $\eta_{\mathbb A_f}:a\mapsto(\iota_\ell(a))_\ell$, where $\iota_\ell:\mathbb Q\to\mathbb Q_\ell$ is the canonical embedding into the completion.

Let $K_\ell$ be the image of $\mathcal H_\ell^\times$ under the projective quotient map $q_\ell:B_\ell^\times\to G(\mathbb Q_\ell)$. Each projection $\pi_\ell:\mathbb A_f\to\mathbb Q_\ell$ is a $\mathbb Q$-algebra map since $\pi_\ell\circ\eta_{\mathbb A_f}=\iota_\ell$. The induced maps on points identify $G(\mathbb A_f)$ with the tuples of local projective classes in $K_\ell$ at all but finitely many primes, with coordinatewise multiplication. Its basic open sets are products of open local sets equal to $K_\ell$ at all but finitely many primes. The local topology is the quotient topology from $B_\ell^\times$, where $B_\ell^\times$ has the subspace topology from the product of the four $\ell$-adic coordinates of $B_\ell$. In the quotient topology a set is open exactly when its preimage is open.

Write $M_2(R)$ for the ring of two-by-two matrices over $R$ with row-by-column multiplication and $I_2$ for the identity matrix. The group $\mathrm{GL}_2(R)=M_2(R)^\times$ of invertible matrices gives the projective group $\mathrm{PGL}_2(R)=\mathrm{GL}_2(R)/(R^\times I_2)$, whose elements $[A]$ identify matrices differing by multiplication by a unit scalar. At $p$ use the integral splitting $\Phi_p:B_p\to M_2(\mathbb Q_p)$ fixed for $\rho_p$. An integral splitting is an algebra isomorphism that carries $\mathcal H_p$ onto $M_2(\mathbb Z_p)$, preserving addition, multiplication, identity and scalar action. It identifies $K_p$ with $\mathrm{PGL}_2(\mathbb Z_p)$.

Let $\mathbb F_p=\mathbb Z/p\mathbb Z$ be the field of residues modulo $p$ and $G_p=\mathrm{PGL}_2(\mathbb F_p)$. For $R=\mathbb Z_p$ write $\bar A$ for the matrix obtained by applying the first residue map to each entry of $A$. Define $r_p:K_p\to G_p$ by $[A]\mapsto[\bar A]$ in the above identification. Its domain $K_p$ is the **projective integral subgroup** at $p$ in $\mathrm{PGL}_2(\mathbb Q_p)$, and its target $G_p$ is $\mathrm{PGL}_2(\mathbb F_p)$. In the projective reduction $\rho_p$, the same formula is applied to $\Phi_p(\alpha\otimes1)$ for $\alpha\in\mathcal H$ whose reduced norm is not divisible by $p$.

The **finite adelic level** at $p$ is
$$U(p)=\{(g_\ell)\in G(\mathbb A_f):g_\ell\in K_\ell\text{ for }\ell\ne p,\quad g_p\in\ker r_p\}.$$
Here $\ker r_p$ is the subset of $K_p$ mapping to $[I_2]$. A level here is a compact open subgroup, meaning it contains the identity, is closed under multiplication and inversion, is open in $G(\mathbb A_f)$, and every open cover in its subspace topology from $G(\mathbb A_f)$ has a finite subcover.

## Definition references

[[math:def-prime]]

[[def-euler-prime-classes]]

[[def-euler-hamilton-quaternions]]

[[def-euler-hurwitz-order]]

[[thm-hurwitz-order-integral-structure]]

[[math:def-field-of-p-adic-numbers]]

[[math:lem-p-adic-valuation-on-q]]

[[math:thm-p-adic-completion-is-a-field]]

[[math:def-p-adic-integers-as-compatible-residue-classes]]

[[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp]]

[[math:def-integers-modulo-n]]

[[math:def-addition-and-multiplication-modulo-n]]

[[math:thm-integers-modulo-n-basic-algebra]]

[[math:thm-z-mod-p-is-a-field]]

[[math:def-tensor-product-of-modules-by-generators-and-relations]]

[[math:thm-tensor-product-of-algebras-over-a-commutative-ring]]

[[def-author-6f52147f3ab3-hamilton-order-completions]]

[[def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles]]

[[math:def-relative-projective-space-standard-charts]]

[[math:def-group-scheme-over-a-field]]

[[math:def-algebra-over-a-commutative-ring]]

[[math:def-affine-scheme]]

[[math:thm-affine-scheme-ring-anti-equivalence]]

[[math:def-scheme-over-base]]

[[def-finite-quaternion-adeles-and-projective-units]]

[[def-degree-two-projective-linear-group]]

[[thm-hurwitz-integral-splitting-at-odd-primes]]

[[def-euler-hurwitz-projective-reduction]]

[[math:def-kernel-and-image-of-group-homomorphism]]

[[math:def-subgroup]]

[[math:def-product-topology]]

[[math:def-subspace-topology-top]]

[[math:def-compact-space]]

## Facts & Assumptions

[F1] A prime $p\in\mathcal P_3$ is odd. The rational Hamilton algebra and its Hurwitz order have the coordinates above. The order has integer basis $1,i,j,(-1+i+j+k)/2$, which is also a rational basis of $B$. [[math:def-prime]] [[def-euler-prime-classes]] [[def-euler-hamilton-quaternions]] [[def-euler-hurwitz-order]] [[thm-hurwitz-order-integral-structure]]

[F2] The valuation $v_\ell$ on a nonzero rational is the exponent difference specified above. For a prime $\ell$, the metric completion $\mathbb Q_\ell$ is a field with a multiplicative absolute value extending the rational one, so $|\ell|_\ell=\ell^{-1}$. The compatible residue ring $\mathbb Z_\ell$ embeds in it as its closed unit ball. The tensor product is generated by elementary tensors subject to additivity in each entry and the relation $(cx)\otimes a=x\otimes(ca)$ for original scalars $c$. For algebras over a commutative ring its multiplication is the formula given above. [[math:lem-p-adic-valuation-on-q]] [[math:def-field-of-p-adic-numbers]] [[math:thm-p-adic-completion-is-a-field]] [[math:def-p-adic-integers-as-compatible-residue-classes]] [[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp]] [[math:def-tensor-product-of-modules-by-generators-and-relations]] [[math:thm-tensor-product-of-algebras-over-a-commutative-ring]]

[F3] For an order with an integer basis that is also a rational basis of $B$, its local completion is the set of tuples of $\ell$-adic integer coefficients in that basis. The change between the Hamilton basis and the order basis is continuous in both directions on $B_\ell$, so either basis gives the same product topology. The order $\mathcal H_\ell$ corresponds to $\mathbb Z_\ell^4$ in order coordinates. Its local unit group is open in $B_\ell^\times$ for the topology on the four coordinates. [[def-author-6f52147f3ab3-hamilton-order-completions]]

[F4] The group of finite adelic projective units for such an order has the restricted product description above. Each local quotient map $q_\ell$ is open, and $\prod_\ell K_\ell$ is a compact open subgroup of $G(\mathbb A_f)$ in the indicated topology. [[def-finite-quaternion-adeles-and-projective-units]]

[F5] The odd-prime splitting of the Hurwitz order takes its local order onto $M_2(\mathbb Z_p)$ and the reduced matrix of $\alpha\in\mathcal H$ has determinant $N(\alpha)\bmod p$. In the definition of $G_p$ and $\rho_p$, an integral splitting at $p$ is fixed, with $\rho_p(\alpha)=[\overline{\Phi_p(\alpha\otimes1)}]$ when $\alpha\in\mathcal H$ and $p$ does not divide its reduced norm. [[thm-hurwitz-integral-splitting-at-odd-primes]] [[def-euler-hurwitz-projective-reduction]]

[F6] For positive $m$, addition and multiplication on integer representatives are well defined in $\mathbb Z/m\mathbb Z$ and satisfy the commutative ring laws, with zero $[0]$, identity $[1]$ and additive inverse $-[a]=[-a]$. For a prime $p$, $\mathbb F_p$ is a field. A local ring is a nonzero commutative ring with a unique maximal ideal, a proper ideal contained in no larger proper ideal. An ideal contains zero and is closed under differences and multiplication by arbitrary ring elements. [[math:def-integers-modulo-n]] [[math:def-addition-and-multiplication-modulo-n]] [[math:thm-integers-modulo-n-basic-algebra]] [[math:thm-z-mod-p-is-a-field]] [[math:def-local-ring]] [[def-degree-two-projective-linear-group]]

[F7] Over a field or local ring the matrix groups and projective classes have the above descriptions. A ring map preserving $1$ from one such ring to another induces a homomorphism on projective classes by applying it to matrix entries. Over a commutative ring a square matrix is invertible exactly when its determinant is a unit. For a two-by-two matrix with rows $(a,b)$ and $(c,d)$ the determinant is $ad-bc$. [[def-degree-two-projective-linear-group]] [[math:cor-square-matrix-invertible-iff-determinant-is-a-unit]] [[thm-hurwitz-integral-splitting-at-odd-primes]]

[F8] The sets fixing the residue modulo $p^n$ for $n\ge1$ are basic neighborhoods in the inverse-limit topology on $\mathbb Z_p$. Under the unit-ball embedding $\mathbb Z_p\hookrightarrow\mathbb Q_p$, each such fiber is a translate of $p^n\mathbb Z_p$, a closed ball of radius $p^{-n}$ that is also open in $\mathbb Q_p$. These radii tend to zero, so the fibers also form a basis for the topology inherited from $\mathbb Q_p$. The product topology has a basis of boxes restricting finitely many coordinates. The subspace topology consists of the intersections with ambient open sets. [[math:thm-inverse-limit-topology-equals-the-p-adic-metric-topology]] [[def-author-6f52147f3ab3-finite-quaternion-ideles]] [[math:def-product-topology]] [[math:def-subspace-topology-top]]

[F9] The kernel of a group homomorphism consists of elements sent to the identity. A subgroup contains the identity and is closed under products and inverses. A group homomorphism $f:X\to Y$ sends the identity $e_X$ to $e_Y$ and satisfies $f(x^{-1})=f(x)^{-1}$. A compact subspace is one where every open cover has a finite subcover. A closed subspace of a compact space is compact, where closed means having open complement. [[math:def-kernel-and-image-of-group-homomorphism]] [[math:def-subgroup]] [[math:lem-group-homomorphism-basic-properties]] [[math:def-compact-space]] [[math:thm-closed-subspace-of-a-compact-space-is-compact]]

[F10] An element of the compatible residue ring $\mathbb Z_p$ is a unit exactly when its residue modulo $p$ is nonzero. [[def-author-6f52147f3ab3-finite-quaternion-ideles]], Justification, step 1.2.

## Justification

The standard charts and the group-scheme definition specify the norm open and its points over a ring. The construction of projective quaternion units supplies the Hamilton group law on this open and identifies its finite adelic points with the restricted product via the local projections. For these points, the source is the affine scheme of the ring and the morphism commutes with the maps to the base. [[math:def-relative-projective-space-standard-charts]] [[math:def-group-scheme-over-a-field]] [[math:def-affine-scheme]] [[math:def-scheme-over-base]] [[def-finite-quaternion-adeles-and-projective-units]]

Step 2.2 of the scalar-adele construction proves that the diagonal map is a unital ring homomorphism into $\mathbb A_f$. Each projection preserves sums, products and $1$ because these are coordinatewise. Its composite with the diagonal map is $\iota_\ell$ by evaluation at $\ell$, so it is a $\mathbb Q$-algebra map. Taking spectra gives $\mathbb Q$-morphisms $\operatorname{Spec}\mathbb Q_\ell\to\operatorname{Spec}\mathbb A_f$. Precomposing with them gives the maps $G(\mathbb A_f)\to G(\mathbb Q_\ell)$. [[def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles]] [[math:def-algebra-over-a-commutative-ring]] [[math:thm-affine-scheme-ring-anti-equivalence]] [[math:def-scheme-over-base]] [[math:def-group-scheme-over-a-field]]

The same integral splitting is used for the local level and for $\rho_p$. The proof identifies the integral projective classes with their images in the local projective quaternion group and checks that the reduction kernel cuts out a compact open subgroup.

## Proof

**Given:** $p\in\mathcal P_3$, the Hurwitz order $\mathcal H$ in $B$, and the integral splitting fixed for $\rho_p$.

**Goal:** Verify the projective reduction and the compact open level $U(p)$.

1.1 By [F1], [F2] and [F3] the Hurwitz basis defines the stated local orders inside $B_\ell$. For each prime $\ell$ and $n\ge1$, congruence modulo $\ell^{n+1}$ implies congruence modulo $\ell^n$. Reduction from $\mathbb Z/\ell^{n+1}\mathbb Z$ to $\mathbb Z/\ell^n\mathbb Z$ is therefore well defined and preserves sums, products and $1$ by the representative formulas in [F6]. At $p$, the first residue map $\epsilon:\mathbb Z_p\to\mathbb F_p$ is a ring homomorphism preserving $1$ by componentwise arithmetic. Every residue has an integer representative, whose compatible tuple maps to it. By [F10], the units of $\mathbb Z_p$ are exactly the elements outside the kernel of $\epsilon$. The subset mapping to zero contains $0$. Since $\epsilon$ is a ring homomorphism, for $x,y$ in the subset and any $z\in\mathbb Z_p$ we have $\epsilon(x-y)=0$ and $\epsilon(zx)=0$. Thus it is an ideal by [F6]. It is proper and contains every proper ideal, since an ideal containing a unit is the entire ring. Thus $\mathbb Z_p$ is local. [F1, F2, F3, F6, F10]

2.1 By [F1] and [F5] the splitting identifies $\mathcal H_p^\times$ with $\mathrm{GL}_2(\mathbb Z_p)$ and takes scalars to scalar matrices. If two integral invertible matrices $A,A'$ satisfy $A'=cA$ with $c\in\mathbb Q_p^\times$, then $A'A^{-1}=cI_2$ and $AA'^{-1}=c^{-1}I_2$ both have integral entries. Thus $c\in\mathbb Z_p^\times$. Conversely a unit scalar in $\mathbb Z_p$ already gives the same class in $G(\mathbb Q_p)$. This identifies $K_p$ with $\mathrm{PGL}_2(\mathbb Z_p)$. By step 1.1 and [F7], $\epsilon$ induces the stated homomorphism $r_p$. For any invertible matrix over $\mathbb F_p$, lift its four entries to integers in $\mathbb Z_p$. The lifted determinant reduces to the original nonzero determinant, so it is a unit by step 1.1 and the lifted matrix is invertible by [F7]. Hence $r_p$ is surjective. If $u\in\mathcal H^\times$, then $\Phi_p(u\otimes1)$ and its inverse have integral entries, so its reduction is invertible. Its determinant is $N(u)\bmod p$ by [F5], so $u$ is in the domain of $\rho_p$. The two reductions then give the same projective class. [F1, F4, F5, F6, F7, step 1.1]

3.1 In the Hurwitz basis of [F1], the residues of the four coefficients of $x\in\mathcal H_p$ determine the matrix $\overline{\Phi_p(x)}$. The splitting is linear over $\mathbb Z_p$ on $\mathcal H_p$ and the basis images are integral, so reduction commutes with the linear combination. For an integer lift $c$ of a first residue, the fiber is $c+p\mathbb Z_p$ by [F8]. It is the ambient closed ball $|z-c|_p\le p^{-1}$ since $(z-c)/p$ must belong to the unit ball in [F2], and it is open by [F8]. The product of four such balls is open in $B_p$ in the order coordinates by [F3] and [F8]. Its trace on $\mathcal H_p$ is the subset specified by the four first residues. Its trace on $\mathcal H_p^\times$ is open in $B_p^\times$ because $\mathcal H_p^\times$ is itself open there by [F3]. For any $a\in G_p$, the subset of $\mathcal H_p^\times$ on which $r_p(q_p(x))=a$ is a union of these intersections. Its image under the open quotient map $q_p$ is $r_p^{-1}(\{a\})$, which is therefore open in $G(\mathbb Q_p)$. [F1, F2, F3, F4, F5, F8, step 2.1]

4.1 Put $K=\prod_\ell K_\ell$. The map $f:K\to G_p$ given by $f(g)=r_p(g_p)$ preserves products by step 2.1 and coordinatewise multiplication. Its kernel is $U(p)$ by [F9]. By [F9], the identity of $K$ maps to $[I_2]$. If $g,h\in U(p)$, then $f(gh)=f(g)f(h)=[I_2]$, and $f(g^{-1})=f(g)^{-1}=[I_2]$. Thus $U(p)$ is a subgroup of $K$ by [F9]. By step 3.1 the product defining $U(p)$ is a basic open set in $G(\mathbb A_f)$. Its complement in $K$ is a union, over $a\in G_p$ with $a\ne[I_2]$, of open boxes with $p$-factor $r_p^{-1}(\{a\})$ and other factors $K_\ell$. Thus $U(p)$ is closed in the compact group $K$, and the closed-subspace result in [F9] makes $U(p)$ compact in the subspace topology from $K$. By [F8], the open sets of $U(p)$ in that topology are $(V\cap K)\cap U(p)=V\cap U(p)$ with $V$ open in $G(\mathbb A_f)$. Thus the topology used for compactness is the subspace topology from the finite adelic group. This proves that the prescription defines the asserted compact open level. [F4, F8, F9, step 2.1, step 3.1] ∎

## Remarks

In the discussion of the [[def-euler-hurwitz-torus-normalizer|finite torus normalizer]], $K_p$ denotes the normalizer of $C_p$ in $G_p=\mathrm{PGL}_2(\mathbb F_p)$.
