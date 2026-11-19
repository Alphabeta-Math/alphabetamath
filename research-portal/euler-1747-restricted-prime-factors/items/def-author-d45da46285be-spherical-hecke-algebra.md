---
id: def-author-d45da46285be-spherical-hecke-algebra
kind: definition
title: Spherical Hecke algebra and action for a compact open subgroup
status: published
domain: mathematics
deps:
  - math:def-topological-group
  - math:def-hausdorff-space
  - math:def-compact-space
  - math:def-subgroup
  - math:def-coset
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-algebra-over-a-commutative-ring
  - math:def-left-haar-integral-and-left-haar-measure
  - math:def-borel-sigma-algebra
  - math:def-compactly-supported-convolution-on-a-group
  - math:def-vector-space
  - math:def-group
  - math:def-group-homomorphism
  - math:def-linear-map
  - math:def-linear-isomorphism-and-invertible-linear-map
  - math:def-linear-subspace
  - math:def-unital-associative-algebra-representation
  - math:lem-topological-group-translations-and-inversion
  - math:lem-coset-partition
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:thm-compactness-under-continuous-maps
  - math:def-locally-compact-space
  - math:def-continuous-map-top
  - math:def-ring-homomorphism
  - math:lem-finite-choice
  - math:def-compact-support-c-c-and-c-zero-on-an-lch-space
  - math:def-integral-of-a-nonnegative-simple-function
  - math:prop-the-nonnegative-integral-agrees-with-the-simple-integral
  - math:def-integrable-real-and-complex-functions-and-their-integrals
  - math:lem-group-homomorphism-basic-properties
  - math:def-topological-space
  - math:def-radon-measure-on-an-lch-space
  - math:thm-complex-numbers-form-a-field
  - math:def-ring
  - math:def-vector-space-of-linear-maps
  - math:def-endomorphism-ring-of-a-module
  - math:def-homeomorphism-and-open-maps
  - math:def-neighbourhood-top
  - math:def-interior-closure-boundary-top
  - math:def-complex-metric-convergence-and-continuity
  - math:def-metric-topology
  - math:lem-finite-sum-reindexing-and-fubini
  - math:lem-group-inverse-laws
  - math:def-left-and-right-modules
  - math:def-module-homomorphism-kernel-image-and-cokernel
  - math:prop-linear-maps-form-a-vector-space
  - math:prop-endomorphisms-form-a-ring
  - math:def-measurable-function-between-measurable-spaces
  - math:def-extended-real-valued-measurable-function
  - math:def-nonnegative-simple-measurable-function
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-measure
  - math:def-measure-space
  - math:def-measurable-space
  - math:def-countable
  - math:thm-subset-of-a-finite-set
  - math:lem-real-line-is-a-metric-space
  - math:def-extended-reals
  - math:def-order-topology-on-a-linearly-ordered-set
dependency_roles:
  math:def-topological-group: mathematical-premise
  math:def-hausdorff-space: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:def-algebra-over-a-commutative-ring: mathematical-premise
  math:def-left-haar-integral-and-left-haar-measure: mathematical-premise
  math:def-borel-sigma-algebra: mathematical-premise
  math:def-compactly-supported-convolution-on-a-group: mathematical-premise
  math:def-vector-space: mathematical-premise
  math:def-group: mathematical-premise
  math:def-group-homomorphism: mathematical-premise
  math:def-linear-map: mathematical-premise
  math:def-linear-isomorphism-and-invertible-linear-map: mathematical-premise
  math:def-linear-subspace: mathematical-premise
  math:def-unital-associative-algebra-representation: mathematical-premise
  math:lem-topological-group-translations-and-inversion: mathematical-premise
  math:lem-coset-partition: mathematical-premise
  math:lem-compactness-of-a-subspace-is-ambient: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:def-locally-compact-space: mathematical-premise
  math:def-continuous-map-top: mathematical-premise
  math:def-ring-homomorphism: mathematical-premise
  math:lem-finite-choice: mathematical-premise
  math:def-compact-support-c-c-and-c-zero-on-an-lch-space: mathematical-premise
  math:def-integral-of-a-nonnegative-simple-function: mathematical-premise
  math:prop-the-nonnegative-integral-agrees-with-the-simple-integral: mathematical-premise
  math:def-integrable-real-and-complex-functions-and-their-integrals: mathematical-premise
  math:lem-group-homomorphism-basic-properties: mathematical-premise
  math:def-topological-space: mathematical-premise
  math:def-radon-measure-on-an-lch-space: mathematical-premise
  math:thm-complex-numbers-form-a-field: mathematical-premise
  math:def-ring: mathematical-premise
  math:def-vector-space-of-linear-maps: mathematical-premise
  math:def-endomorphism-ring-of-a-module: mathematical-premise
  math:def-homeomorphism-and-open-maps: mathematical-premise
  math:def-neighbourhood-top: mathematical-premise
  math:def-interior-closure-boundary-top: mathematical-premise
  math:def-complex-metric-convergence-and-continuity: mathematical-premise
  math:def-metric-topology: mathematical-premise
  math:lem-finite-sum-reindexing-and-fubini: mathematical-premise
  math:lem-group-inverse-laws: mathematical-premise
  math:def-left-and-right-modules: mathematical-premise
  math:def-module-homomorphism-kernel-image-and-cokernel: mathematical-premise
  math:prop-linear-maps-form-a-vector-space: mathematical-premise
  math:prop-endomorphisms-form-a-ring: mathematical-premise
  math:def-measurable-function-between-measurable-spaces: mathematical-premise
  math:def-extended-real-valued-measurable-function: mathematical-premise
  math:def-nonnegative-simple-measurable-function: mathematical-premise
  math:def-complex-conjugate-real-imaginary-part-and-modulus: mathematical-premise
  math:def-measure: mathematical-premise
  math:def-measure-space: mathematical-premise
  math:def-measurable-space: mathematical-premise
  math:def-countable: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:lem-real-line-is-a-metric-space: mathematical-premise
  math:def-extended-reals: mathematical-premise
  math:def-order-topology-on-a-linearly-ordered-set: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
formulation_deps:
  - math:def-topological-group
  - math:def-hausdorff-space
  - math:def-compact-space
  - math:def-subgroup
  - math:def-coset
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-algebra-over-a-commutative-ring
  - math:def-left-haar-integral-and-left-haar-measure
  - math:def-borel-sigma-algebra
  - math:def-compactly-supported-convolution-on-a-group
  - math:def-vector-space
  - math:def-group
  - math:def-group-homomorphism
  - math:def-linear-map
  - math:def-linear-isomorphism-and-invertible-linear-map
  - math:def-linear-subspace
  - math:def-unital-associative-algebra-representation
  - math:def-topological-space
  - math:def-radon-measure-on-an-lch-space
  - math:thm-complex-numbers-form-a-field
  - math:def-ring
  - math:def-vector-space-of-linear-maps
  - math:def-endomorphism-ring-of-a-module
  - math:def-measure
  - math:def-countable
argument_deps:
  - math:lem-topological-group-translations-and-inversion
  - math:lem-coset-partition
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:thm-compactness-under-continuous-maps
  - math:def-locally-compact-space
  - math:def-continuous-map-top
  - math:def-algebra-over-a-commutative-ring
  - math:def-ring-homomorphism
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-finite-choice
  - math:def-hausdorff-space
  - math:def-left-haar-integral-and-left-haar-measure
  - math:def-compactly-supported-convolution-on-a-group
  - math:def-compact-support-c-c-and-c-zero-on-an-lch-space
  - math:def-borel-sigma-algebra
  - math:def-integral-of-a-nonnegative-simple-function
  - math:prop-the-nonnegative-integral-agrees-with-the-simple-integral
  - math:def-integrable-real-and-complex-functions-and-their-integrals
  - math:def-group-homomorphism
  - math:lem-group-homomorphism-basic-properties
  - math:def-linear-map
  - math:def-linear-subspace
  - math:def-unital-associative-algebra-representation
  - math:def-group
  - math:def-linear-isomorphism-and-invertible-linear-map
  - math:def-topological-group
  - math:def-compact-space
  - math:def-coset
  - math:def-subgroup
  - math:def-vector-space
  - math:def-topological-space
  - math:def-radon-measure-on-an-lch-space
  - math:thm-complex-numbers-form-a-field
  - math:def-ring
  - math:def-vector-space-of-linear-maps
  - math:def-endomorphism-ring-of-a-module
  - math:def-homeomorphism-and-open-maps
  - math:def-neighbourhood-top
  - math:def-interior-closure-boundary-top
  - math:def-complex-metric-convergence-and-continuity
  - math:def-metric-topology
  - math:lem-finite-sum-reindexing-and-fubini
  - math:lem-group-inverse-laws
  - math:def-left-and-right-modules
  - math:def-module-homomorphism-kernel-image-and-cokernel
  - math:prop-linear-maps-form-a-vector-space
  - math:prop-endomorphisms-form-a-ring
  - math:def-measurable-function-between-measurable-spaces
  - math:def-extended-real-valued-measurable-function
  - math:def-nonnegative-simple-measurable-function
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-measure
  - math:def-measure-space
  - math:def-measurable-space
  - math:def-countable
  - math:thm-subset-of-a-finite-set
  - math:lem-real-line-is-a-metric-space
  - math:def-extended-reals
  - math:def-order-topology-on-a-linearly-ordered-set
dependency_level: 0
---

## Definition

Let $G$ be a Hausdorff topological group, a Hausdorff space with a group law and inversion both continuous, and let $K$ be a compact open subgroup. Write $G/K$ for the set of cosets $xK=\{xk:k\in K\}$. The spherical Hecke algebra $\mathcal H(G,K)$ consists of complex functions $f$ invariant on both sides under $K$, meaning $f(kxk')=f(x)$ for $k,k'\in K$, and zero outside a compact subset. It has pointwise vector-space operations over the field $\mathbb C$, unit $\mathbf 1_K$ (one on $K$, zero elsewhere), and multiplication
$$(f*h)(z)=\sum_{xK\in G/K} f(x)h(x^{-1}z).$$
The sum uses only the finitely many cosets where $f$ is nonzero. The scalar structure map is $c\mapsto c\mathbf 1_K$. When a left Haar measure assigns $K$ volume one, this multiplication is convolution for that measure. Here a left Haar measure is a nonzero left-translation-invariant Borel measure, finite on compact sets, outer regular on Borel sets and inner regular on open sets.

A complex representation on a complex vector space $V$ is a group homomorphism $\pi$ from $G$ to the group of invertible complex-linear maps $V\to V$ under composition. The fixed subspace is $V^K=\{w\in V:\pi(k)w=w\text{ for all }k\in K\}$. The Hecke operator of $f$ on this space is
$$T_f w=\sum_{xK\in G/K} f(x)\pi(x)w.$$
Again the sum uses only the cosets where $f$ is nonzero. The assignment $f\mapsto T_f$ gives a unital representation of the algebra on $V^K$. It takes values in $\operatorname{End}_{\mathbb C}(V^K)$, the complex-linear self-maps of $V^K$ with pointwise addition and scalar multiplication, composition as multiplication, and the identity map as unit.

## Facts & Assumptions

[F1] Left translations in a topological group are homeomorphisms. A homeomorphism and its inverse are continuous. The cosets $xK$ of a subgroup partition the group. Unions of open sets are open, complements of open sets are closed, and a closed set equals its closure ([[math:lem-topological-group-translations-and-inversion]], [[math:def-homeomorphism-and-open-maps]], [[math:lem-coset-partition]], [[math:def-topological-space]], [[math:def-interior-closure-boundary-top]]).

[F2] Any cover of a compact subset by ambient open sets admits a finite subcover. A continuous image of a compact subset is compact. A space is locally compact if each point has a compact neighborhood. Continuity at a point follows if every open neighborhood of its image contains the image of an open neighborhood of the point. On $\mathbb C$ use the topology of the metric $d(z,w)=|z-w|$ ([[math:lem-compactness-of-a-subspace-is-ambient]], [[math:thm-compactness-under-continuous-maps]], [[math:def-locally-compact-space]], [[math:def-neighbourhood-top]], [[math:def-continuous-map-top]], [[math:def-complex-metric-convergence-and-continuity]], [[math:def-metric-topology]]).

[F3] The complex numbers form a field, and vector addition in a complex vector space is an abelian group operation. A unital ring has abelian-group addition, associative unital multiplication, and both distributive laws. A complex algebra is a unital ring with a unital structure map from $\mathbb C$ into its center. Finite sums in an additive commutative monoid are invariant under reindexing. Representatives of a finite family of nonempty sets can be picked by enumerating the family and using finite choice ([[math:thm-complex-numbers-form-a-field]], [[math:def-vector-space]], [[math:def-ring]], [[math:def-algebra-over-a-commutative-ring]], [[math:def-ring-homomorphism]], [[math:def-finite-sum-in-a-commutative-monoid]], [[math:lem-finite-choice]]).

[F4] On a locally compact Hausdorff group with left Haar measure $\mu$, convolution of continuous compactly supported functions is $(f*h)(z)=\int_G f(x)h(x^{-1}z)\,d\mu(x)$. Borel sets include open sets, and left invariance gives $\mu(xK)=\mu(K)$ for Borel $K$. The regularity conditions on the Haar measure are the Radon conditions given in the definition. A Borel measure $\mu$ on $G$ means a measure on the Borel sigma-algebra $\mathcal B(G)$, so $(G,\mathcal B(G),\mu)$ is a measure space. ([[math:def-measure]], [[math:def-measure-space]], [[math:def-radon-measure-on-an-lch-space]], [[math:def-compactly-supported-convolution-on-a-group]], [[math:def-compact-support-c-c-and-c-zero-on-an-lch-space]], [[math:def-borel-sigma-algebra]], [[math:def-left-haar-integral-and-left-haar-measure]]).

[F5] The Lebesgue integral of a nonnegative simple function is the sum of its coefficients times the measures of its pairwise disjoint measurable pieces. The integral of a real function is the difference of the integrals of its positive and negative parts when both are finite. The complex integral uses the integrals of the real and imaginary parts, with integrability determined by the integral of the modulus ([[math:def-integral-of-a-nonnegative-simple-function]], [[math:prop-the-nonnegative-integral-agrees-with-the-simple-integral]], [[math:def-integrable-real-and-complex-functions-and-their-integrals]]).

[F6] A group homomorphism respects products and identity. A linear map respects linear combinations. A subset of a vector space is a linear subspace if it contains zero and is closed under linear combinations. A unital algebra representation on a vector space is a linear map to its linear endomorphisms preserving multiplication and unit ([[math:def-group-homomorphism]], [[math:lem-group-homomorphism-basic-properties]], [[math:def-linear-map]], [[math:def-linear-subspace]], [[math:def-unital-associative-algebra-representation]]).

[F7] A group has an associative operation, a two-sided identity and two-sided inverses. In a group, $(ab)^{-1}=b^{-1}a^{-1}$. Invertibility of a linear map means it has a two-sided linear inverse. A subgroup contains the group identity and is closed under products and inverses ([[math:def-group]], [[math:lem-group-inverse-laws]], [[math:def-linear-isomorphism-and-invertible-linear-map]], [[math:def-subgroup]]).

[F8] Finite sums in an additive commutative monoid split over disjoint index sets and can be interchanged on a product of finite index sets ([[math:lem-finite-sum-reindexing-and-fubini]]).

[F9] Every complex vector space is a left $\mathbb C$-module by the vector-space axioms. A map between such spaces is complex-linear exactly when it is additive and commutes with complex scalar multiplication, so the linear self-maps are the module endomorphisms. Linear self-maps form a complex vector space under pointwise operations and a unital ring under pointwise addition and composition, with identity the identity map ([[math:def-vector-space]], [[math:def-left-and-right-modules]], [[math:def-linear-map]], [[math:def-module-homomorphism-kernel-image-and-cokernel]], [[math:def-vector-space-of-linear-maps]], [[math:prop-linear-maps-form-a-vector-space]], [[math:def-endomorphism-ring-of-a-module]], [[math:prop-endomorphisms-form-a-ring]]).

[F10] Measurability means that preimages of measurable sets are measurable, using the Borel sets on the real, extended real, or complex codomain as applicable. A nonnegative simple measurable function is measurable and has finite range in $[0,\infty)$. On $\mathbb R$ use the metric topology of $d_{\mathbb R}(s,t)=|s-t|$. On $\overline{\mathbb R}=\mathbb R\cup\{-\infty,+\infty\}$ use the order topology generated by the open rays of the order extending the real order with $-\infty$ least and $+\infty$ greatest. For a complex value $a+ib$ with $a,b$ real its real part is $a$, imaginary part is $b$, and modulus is $\sqrt{a^2+b^2}$ ([[math:def-measurable-space]], [[math:def-measurable-function-between-measurable-spaces]], [[math:def-extended-real-valued-measurable-function]], [[math:def-borel-sigma-algebra]], [[math:def-nonnegative-simple-measurable-function]], [[math:def-complex-conjugate-real-imaginary-part-and-modulus]], [[math:lem-real-line-is-a-metric-space]], clause 1, [[math:def-metric-topology]], [[math:def-extended-reals]], [[math:def-order-topology-on-a-linearly-ordered-set]]).

[F11] A finite set is in bijection with a finite initial segment of the natural numbers, so its elements admit a finite list without repetitions. Every subset of a finite set is finite. ([[math:def-countable]], [[math:thm-subset-of-a-finite-set]]).

## Justification

**Given:** $G,K$ and $\pi$ as in the definition. For the integral formula assume a left Haar measure $\mu$ with $\mu(K)=1$.

**Goal:** Verify the finite-sum algebra, its action and the normalization.

1.1 Each coset $xK$ is open because it is the preimage of $K$ under the continuous inverse of left translation by $x$. It is compact as a continuous image of $K$ under left translation. It is closed because its complement is a union of other open cosets. The coset $xK$ is a compact neighborhood of $x$, so $G$ is locally compact. By compactness, finitely many cosets cover any given compact subset of $G$. Disjointness implies that every coset meeting the subset belongs to this finite subcover. [F1, F2, given]

1.2 Distributivity gives $(0+0)a=0a+0a$ and $a(0+0)=a0+a0$ for $a\in\mathbb C$. The vector-space distributive laws give $(0+0)v=0v+0v$ and $a(0_V+0_V)=a0_V+a0_V$ for $v\in V$. In each equality the left side equals either summand on the right. Adding the additive inverse of that summand to both sides gives $0a=a0=0$ and $0v=a0_V=0_V$. For any complex-linear map $L:V\to V$, additivity gives $L(0_V)=L(0_V+0_V)=L(0_V)+L(0_V)$, so the same calculation gives $L(0_V)=0_V$. [F3, F6, F7]

2.1 Invertible complex-linear self-maps form a group under composition. The composite is linear and has the composite of the two inverses in reverse order as its inverse. Composition is associative, the identity is linear, and each inverse is linear by invertibility. The subset $V^K$ contains $0_V$ because each $\pi(k)$ is linear and sends $0_V$ to $0_V$ by step 1.2. If $u,v\in V^K$ then $\pi(k)(au+bv)=a\pi(k)u+b\pi(k)v=au+bv$ for all $k\in K$ and $a,b\in\mathbb C$. Thus $V^K$ is a linear subspace. [F6, F7, given, step 1.2]

2.2 Right $K$-invariance makes each input constant on every open coset. The cosets on which an input is nonzero form a subset of the finite set of cosets meeting a compact set outside which the input vanishes. This subset is finite. The coset through a point maps to the value at that point, so it maps into every open neighborhood of that value in $\mathbb C$ with its usual metric topology. This gives continuity. The nonzero set of each input is a finite union of compact closed cosets by step 1.1. A finite union of compact sets is compact because the union of finite subcovers of the individual sets is a finite subcover of the union. The nonzero set is closed, so it equals the support, defined as its closure. Thus the inputs meet the support and continuity requirements of the Haar convolution definition. [F1, F2, F4, F11, step 1.1]

3.1 Write $S_f$ for the finite set of cosets where $f$ is nonzero. For $k\in K$, replacing $x$ by $xk$ leaves $f(x)$ unchanged, sends $x^{-1}z$ to $(xk)^{-1}z=k^{-1}x^{-1}z$ and sends $\pi(x)w$ to $\pi(x)\pi(k)w=\pi(x)w$ for $w\in V^K$. Left $K$-invariance of $h$ thus gives representative independence for convolution, and fixedness of $w$ gives it for the action. In calculations we may choose representatives from the finite sets of contributing cosets. [F3, F6, F7, step 2.2]

4.1 Use the measure space $(G,\mathcal B(G),\mu)$ from [F4] and the measurable spaces $(G,\mathcal B(G))$ and $(Y,\mathcal B(Y))$ for $Y=\mathbb C$, $\mathbb R$, or $\overline{\mathbb R}$ as appropriate. Use the topology from [F2] on $\mathbb C$ and the topologies from [F10] on $\mathbb R$ and $\overline{\mathbb R}$. For fixed $z$, the Haar integrand is $\sum_{xK\in S_f} f(x)h(x^{-1}z)\mathbf 1_{xK}$, with disjoint Borel pieces of measure one. The integrand, its real and imaginary parts, their positive and negative parts, and the modulus are all constant on those pieces and zero on their Borel complement, which is open as a union of the other cosets. A preimage of a Borel set under any of these functions is a union of the pieces whose value belongs to that set, including the complement if the set contains zero. Each such union is open by [F1] and hence Borel. Thus all these functions are measurable. The modulus and the four nonnegative parts are simple with finite integrals because only the finitely many measure-one pieces can contribute. Applying the simple integral formula to the four parts, then subtracting and recombining using the finite sums, gives the complex integral $\sum_{xK\in S_f} f(x)h(x^{-1}z)\mu(xK)=(f*h)(z)$. [F1, F2, F3, F4, F5, F10, step 1.1, step 2.2, step 3.1, step 1.2]

4.2 The zero function belongs to $\mathcal H(G,K)$. A linear combination of two inputs is $K$-invariant on both sides and vanishes outside the union of their two compact supports. This gives a vector space under the pointwise operations, with the vector-space laws holding at each point. In the multiplication formula, replacing $z$ by $zk$ for $k\in K$ leaves each term unchanged, and replacing $z$ by $kz$ reindexes the sum by $xK\mapsto k^{-1}xK$ using left invariance of $f$. For each representative $x$ in $S_f$, the term $f(x)h(x^{-1}z)$ vanishes outside $x\operatorname{supp}h$. The finite union of these translated supports is compact, giving closure under convolution. When combining two first inputs, take the union of their two coset sets as the common index set. Concatenate the two finite lists and discard repeated entries, keeping the first occurrence of each coset. The remaining finite list enumerates the common index set. Terms added to an individual sum have zero coefficient, so the disjoint splitting law preserves its value. Scalar multiplication and addition distribute through the finite sums by starting with the empty sum and using the binary distributive laws when adjoining each term. Applying this to each factor gives bilinearity. [F1, F2, F3, F7, F8, F11, step 2.2, step 3.1, step 1.2]

5.1 For $k\in K$, applying $\pi(k)$ to the term $f(x)\pi(x)w$ gives $f(kx)\pi(kx)w$ by left invariance and the representation law. By linearity applied successively to the finite sum, these transformed terms sum to $\pi(k)T_fw$. The map $xK\mapsto kxK$ permutes $S_f$, so the sum is fixed by $K$. The sum is linear in $w$ because each $\pi(x)$ is linear and scalar multiplication distributes through the sum by the same finite recursion. A linear combination of coefficients also distributes through the sum, using the union of the two finite sets of contributing cosets and extending the sums by zero as in step 4.2. The resulting identities hold at each $w\in V^K$, so $f\mapsto T_f$ is linear for the pointwise vector-space operations on $\operatorname{End}_{\mathbb C}(V^K)$. [F1, F3, F6, F8, F9, step 1.2, step 2.1, step 3.1, step 4.2]

5.2 For a third function $j$, both $(f*h)*j$ and $f*(h*j)$ at $z$ expand to $\sum_{xK\in S_f,\,yK\in S_h} f(x)h(y)j(y^{-1}x^{-1}z)$. In the first product fix representatives $x$ for $S_f$. Take the outer sum over the finite set $U=\bigcup_{xK\in S_f} xS_h$, where $xS_h=\{xyK:yK\in S_h\}$. To see that $U$ is finite, go through the finite list of $xK\in S_f$ and for each $x$ list the cosets $xyK$ for the finite list of $yK\in S_h$. Discard repetitions as in step 4.2 to obtain a finite list of $U$. Every expanded term vanishes outside $U$ because then $h(x^{-1}z')=0$ for each $x$ at the outer coset $z'K$. Expanding the coefficient and interchanging the sums over $U$ and $S_f$ makes $x$ the outer variable. For each fixed $x$, the terms for $z'K\in U\setminus xS_h$ vanish by the same test, so disjoint splitting restricts the inner sum to $xS_h$. Each term $f(x)h(x^{-1}z')j(z'^{-1}z)$ is independent of the representative $z'$ by right invariance of $h$ and left invariance of $j$, using the inverse product law. Thus reindex by $z'K=xyK$ and take $z'=xy$, so $(xy)^{-1}=y^{-1}x^{-1}$. For the second product the expansion already has $x$ as the outer variable. This proves associativity. [F1, F3, F7, F8, step 3.1, step 4.2, step 1.2]

6.1 For $k,k'\in K$, subgroup closure gives $kzk'\in K$ if $z\in K$. Conversely, if $kzk'\in K$, then $z=k^{-1}(kzk')(k')^{-1}\in K$ by closure under inverses and products. Hence $\mathbf 1_K$ is bi-$K$-invariant and it vanishes outside the compact set $K$, so $\mathbf 1_K\in\mathcal H(G,K)$. For $\mathbf 1_K*f$ the only contributing coset is $K$ and the representative $1\in K$ gives $f(z)$. For $f*\mathbf 1_K$, the condition $x^{-1}z\in K$ is equivalent to $z\in xK$. In one direction $k=x^{-1}z\in K$ gives $z=xk$. In the other direction $z=xk$ with $k\in K$ gives $x^{-1}z=k$. Since $z\in zK$ and the cosets partition $G$, the condition holds exactly when $xK=zK$. If $zK\in S_f$, the representative $z$ gives the value $f(z)$ and all other terms vanish. If $zK\notin S_f$, all terms vanish and $f(z)=0$. Pointwise addition is an abelian group law by step 4.2, convolution is associative by step 5.2, and its bilinearity supplies both distributive laws. Together with the two-sided unit these are the unital ring axioms. The unit and bilinearity give $(c\mathbf 1_K)*f=f*(c\mathbf 1_K)=cf$. The map $c\mapsto c\mathbf 1_K$ preserves addition by pointwise operations, preserves products by bilinearity and the unit law, and sends $1$ to the unit. It is therefore the central unital structure map inducing the pointwise scalars. [F1, F3, F7, F8, given, step 1.2, step 3.1, step 4.2, step 5.2]

7.1 In $T_{f*h}w$, sum over the same finite set $U$ as in step 5.2 and expand $f*h$. The additive group of $V$ admits finite-sum interchange, giving the outer sum over $S_f$. For each $x$, terms for cosets in $U\setminus xS_h$ vanish because $h(x^{-1}z')=0$. The expanded term at $z'K$ is independent of $z'$ by right invariance of $h$ and fixedness of $w$. Reindexing by $z'K=xyK$ now gives the terms $f(x)h(y)\pi(xy)w$. Since $T_hw$ is fixed, expanding $T_f(T_hw)$ gives these terms by $\pi(xy)=\pi(x)\pi(y)$, distributing each $\pi(x)$ through the finite linear combination by its linearity on binary combinations and iteration from $\pi(x)0=0$. Thus $T_{f*h}=T_f\circ T_h$ in the endomorphism ring. Also $T_{\mathbf 1_K}w=\pi(1)w=w$, so the unit maps to the identity endomorphism. With step 5.1 this proves the unital algebra action. [F3, F6, F8, F9, step 3.1, step 5.1, step 5.2, step 6.1, step 1.2] ∎
