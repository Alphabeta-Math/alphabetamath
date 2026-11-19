---
id: lem-quadratic-field-normalizer-in-degree-two
kind: lemma
title: Normalizer of a quadratic field torus in degree two
status: draft
domain: mathematics
deps:
  - math:def-field
  - math:def-finite-field-and-its-order
  - math:def-field-extension-generated-subfields-and-simple-extension
  - math:def-extension-degree-and-finite-extension
  - math:def-linear-basis
  - math:def-dimension
  - math:thm-unique-coordinates-with-respect-to-an-ordered-basis
  - math:def-linear-map
  - math:def-vector-space-of-linear-maps
  - math:lem-of-zero-mult
  - math:def-linear-isomorphism-and-invertible-linear-map
  - math:def-coordinate-column-and-matrix-of-a-linear-map
  - math:thm-matrix-of-a-composite-is-the-product
  - math:thm-invertible-matrices-correspond-to-linear-isomorphisms
  - def-degree-two-projective-linear-group
  - math:def-quotient-group
  - math:thm-quotient-group-laws
  - math:def-normal-subgroup
  - math:def-subgroup
  - math:def-normalizer-of-a-subgroup
  - math:lem-centralizers-and-normalizers-are-subgroups
  - math:def-relative-field-automorphism-group
  - math:def-field-homomorphism
  - math:def-finite-galois-extension-and-galois-group
  - math:def-relative-frobenius-of-a-finite-field-extension
  - math:def-generated-subgroup
  - math:def-order-in-a-group
  - math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group
  - math:def-action-by-automorphisms
  - math:def-external-semidirect-product
  - math:thm-external-semidirect-product-is-a-group
  - math:def-group-isomorphism-and-automorphism
  - math:def-finite-cardinality
  - math:lem-cardinality-of-a-finite-dimensional-space-over-a-finite-field
  - math:thm-sum-rule
  - math:thm-subset-of-a-finite-set
  - math:thm-lagrange
  - math:lem-finite-coset-partition
  - math:thm-product-rule
formulation_deps:
  - math:def-field
  - math:def-finite-field-and-its-order
  - math:def-field-extension-generated-subfields-and-simple-extension
  - math:def-extension-degree-and-finite-extension
  - math:def-linear-basis
  - math:def-dimension
  - math:thm-unique-coordinates-with-respect-to-an-ordered-basis
  - math:def-linear-map
  - math:def-linear-isomorphism-and-invertible-linear-map
  - math:def-coordinate-column-and-matrix-of-a-linear-map
  - math:thm-invertible-matrices-correspond-to-linear-isomorphisms
  - def-degree-two-projective-linear-group
  - math:def-quotient-group
  - math:thm-quotient-group-laws
  - math:def-normal-subgroup
  - math:def-subgroup
  - math:def-normalizer-of-a-subgroup
  - math:lem-centralizers-and-normalizers-are-subgroups
  - math:def-relative-field-automorphism-group
  - math:def-field-homomorphism
  - math:def-finite-galois-extension-and-galois-group
  - math:def-relative-frobenius-of-a-finite-field-extension
  - math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group
  - math:def-action-by-automorphisms
  - math:def-external-semidirect-product
  - math:thm-external-semidirect-product-is-a-group
  - math:def-group-isomorphism-and-automorphism
  - math:def-finite-cardinality
argument_deps:
  - math:def-field
  - math:def-finite-field-and-its-order
  - math:def-field-extension-generated-subfields-and-simple-extension
  - math:def-extension-degree-and-finite-extension
  - math:def-linear-basis
  - math:def-dimension
  - math:thm-unique-coordinates-with-respect-to-an-ordered-basis
  - math:def-linear-map
  - math:def-vector-space-of-linear-maps
  - math:lem-of-zero-mult
  - math:def-linear-isomorphism-and-invertible-linear-map
  - math:def-coordinate-column-and-matrix-of-a-linear-map
  - math:thm-matrix-of-a-composite-is-the-product
  - math:thm-invertible-matrices-correspond-to-linear-isomorphisms
  - def-degree-two-projective-linear-group
  - math:def-quotient-group
  - math:thm-quotient-group-laws
  - math:def-normal-subgroup
  - math:def-subgroup
  - math:def-normalizer-of-a-subgroup
  - math:lem-centralizers-and-normalizers-are-subgroups
  - math:def-relative-field-automorphism-group
  - math:def-field-homomorphism
  - math:def-finite-galois-extension-and-galois-group
  - math:def-relative-frobenius-of-a-finite-field-extension
  - math:def-generated-subgroup
  - math:def-order-in-a-group
  - math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group
  - math:def-action-by-automorphisms
  - math:def-external-semidirect-product
  - math:thm-external-semidirect-product-is-a-group
  - math:def-group-isomorphism-and-automorphism
  - math:def-finite-cardinality
  - math:lem-cardinality-of-a-finite-dimensional-space-over-a-finite-field
  - math:thm-sum-rule
  - math:thm-subset-of-a-finite-set
  - math:thm-lagrange
  - math:lem-finite-coset-partition
  - math:thm-product-rule
dependency_roles:
  math:def-field: mathematical-premise
  math:def-finite-field-and-its-order: mathematical-premise
  math:def-field-extension-generated-subfields-and-simple-extension: mathematical-premise
  math:def-extension-degree-and-finite-extension: mathematical-premise
  math:def-linear-basis: mathematical-premise
  math:def-dimension: mathematical-premise
  math:thm-unique-coordinates-with-respect-to-an-ordered-basis: mathematical-premise
  math:def-linear-map: mathematical-premise
  math:def-vector-space-of-linear-maps: mathematical-premise
  math:lem-of-zero-mult: mathematical-premise
  math:def-linear-isomorphism-and-invertible-linear-map: mathematical-premise
  math:def-coordinate-column-and-matrix-of-a-linear-map: mathematical-premise
  math:thm-matrix-of-a-composite-is-the-product: mathematical-premise
  math:thm-invertible-matrices-correspond-to-linear-isomorphisms: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  math:def-quotient-group: mathematical-premise
  math:thm-quotient-group-laws: mathematical-premise
  math:def-normal-subgroup: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:def-normalizer-of-a-subgroup: mathematical-premise
  math:lem-centralizers-and-normalizers-are-subgroups: mathematical-premise
  math:def-relative-field-automorphism-group: mathematical-premise
  math:def-field-homomorphism: mathematical-premise
  math:def-finite-galois-extension-and-galois-group: mathematical-premise
  math:def-relative-frobenius-of-a-finite-field-extension: mathematical-premise
  math:def-generated-subgroup: mathematical-premise
  math:def-order-in-a-group: mathematical-premise
  math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group: mathematical-premise
  math:def-action-by-automorphisms: mathematical-premise
  math:def-external-semidirect-product: mathematical-premise
  math:thm-external-semidirect-product-is-a-group: mathematical-premise
  math:def-group-isomorphism-and-automorphism: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:lem-cardinality-of-a-finite-dimensional-space-over-a-finite-field: mathematical-premise
  math:thm-sum-rule: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:thm-lagrange: mathematical-premise
  math:lem-finite-coset-partition: mathematical-premise
  math:thm-product-rule: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Let $F$ be a finite field with $q=|F|$ elements and let $E/F$ be an extension of degree two, so that $E$ has dimension two over $F$. For a field $L$, write $L^\times$ for its multiplicative group of nonzero elements. For $a\in E$ let $m_a:E\to E$ be multiplication by $a$, given by $m_a(x)=ax$. Choose an ordered $F$-basis of $E$. Write $[S]$ for the class in $G=\mathrm{PGL}_2(F)$ of the matrix of an invertible $F$-linear map $S:E\to E$. Two such maps have the same class exactly when they differ by a scalar in $F^\times$.

The map $aF^\times\mapsto[m_a]$ identifies $C=E^\times/F^\times$ with the subgroup $T=\{[m_a]:a\in E^\times\}$ of $G$, called the quadratic field torus here. Let $N_G(T)=\{g\in G:gTg^{-1}=T\}$ be its normalizer, and let $H=\operatorname{Gal}(E/F)$ be the group of field automorphisms of $E$ fixing $F$ pointwise, with composition as product. With the action $\alpha_\sigma(aF^\times)=\sigma(a)F^\times$ of $H$ on $C$, there is a group isomorphism
$$C\rtimes_\alpha H\longrightarrow N_G(T),\qquad (aF^\times,\sigma)\longmapsto[m_a\circ\sigma].$$
Here the semidirect product has underlying set $C\times H$ and product $(c,\sigma)(d,\tau)=(c\alpha_\sigma(d),\sigma\circ\tau)$.

The normalizer is the disjoint union $T\cup T[\sigma_q]$, where $\sigma_q(x)=x^q$ is the relative Frobenius. Each class in $T[\sigma_q]$ has a representative $S=m_a\circ\sigma_q$ with $a\in E^\times$. It is semilinear over $E$ with respect to $\sigma_q$, meaning it is additive and satisfies $S(bx)=\sigma_q(b)S(x)$ for all $b,x\in E$. Here $T[\sigma_q]=\{t[\sigma_q]:t\in T\}$. Conjugation by $S$ sends $m_b$ to $m_{\sigma_q(b)}$ for every $b\in E$. The order of the normalizer, meaning its number of elements, is $2(q+1)$.

## Facts & Assumptions

[F1] A field has commutative, distributive multiplication and $0\ne1$. Its nonzero elements form a commutative group under multiplication. A finite field has a finite underlying set. In an extension $E/F$ we identify $F$ with its image in $E$, and the degree is the dimension of $E$ over $F$. ([[math:def-field]], [[math:def-finite-field-and-its-order]], [[math:def-field-extension-generated-subfields-and-simple-extension]], [[math:def-extension-degree-and-finite-extension]]).

[F2] A space of dimension two has a two-element basis, which can be ordered. Any ordered basis is an injective list whose image is a finite basis, so it also has two vectors by uniqueness of the size of a finite basis. In such a basis every vector has exactly one pair of coordinates. An $F$-linear map preserves $F$-linear combinations. It is invertible if it has an $F$-linear inverse. The columns of its matrix are the coordinate columns of the images of the basis vectors, and composition gives matrix multiplication. For finite-dimensional spaces with ordered bases, invertible linear maps have invertible matrices. Conversely, an invertible matrix acts invertibly and linearly on coordinate columns. ([[math:def-dimension]], [[math:def-linear-basis]], [[math:thm-unique-coordinates-with-respect-to-an-ordered-basis]], [[math:def-linear-map]], [[math:def-linear-isomorphism-and-invertible-linear-map]], [[math:def-coordinate-column-and-matrix-of-a-linear-map]], [[math:thm-matrix-of-a-composite-is-the-product]], [[math:thm-invertible-matrices-correspond-to-linear-isomorphisms]]).

[F3] The projective group is the quotient of the invertible matrices by the nonzero scalar matrices, with $[A][B]=[AB]$. A subgroup $D$ is normal if each conjugation $d\mapsto ada^{-1}$ in the ambient group sends $D$ onto itself. For normal $D$, the left cosets $aD=\{ad:d\in D\}$ form a group under the well-defined product $(aD)(bD)=abD$. A subset containing the identity and closed under products and inverses is a subgroup. For a subgroup $T$ of $G$, the set of $g$ with $gTg^{-1}=T$ is a subgroup of $G$. ([[def-degree-two-projective-linear-group]], [[math:def-quotient-group]], [[math:thm-quotient-group-laws]], [[math:def-normal-subgroup]], [[math:def-subgroup]], [[math:def-normalizer-of-a-subgroup]], [[math:lem-centralizers-and-normalizers-are-subgroups]]).

[F4] An $F$-automorphism of $E$ is a bijective field map fixing $F$ pointwise, with field maps preserving addition, multiplication and $1$. For an extension of finite fields of degree $n$ over a field of $q$ elements, the extension is Galois and its group of $F$-automorphisms is cyclic with $n$ elements under composition, generated by the relative Frobenius $x\mapsto x^q$. To say that an element generates the group means that the smallest subgroup containing that element is the whole group. The element order of an automorphism in this finite group is the least positive $k$ for which its $k$-fold iterate is the identity. ([[math:def-relative-field-automorphism-group]], [[math:def-field-homomorphism]], [[math:def-finite-galois-extension-and-galois-group]], [[math:def-relative-frobenius-of-a-finite-field-extension]], [[math:thm-extensions-of-finite-fields-are-galois-with-cyclic-frobenius-group]], [[math:def-generated-subgroup]], [[math:def-order-in-a-group]]).

[F5] An action of a group $H$ on a group $C$ by automorphisms assigns each $h$ an invertible product-preserving map $\alpha_h:C\to C$, with $\alpha_1=\mathrm{id}_C$ and $\alpha_{h k}=\alpha_h\circ\alpha_k$. For such an action the pair law $(c,h)(d,k)=(c\alpha_h(d),hk)$ makes $C\rtimes_\alpha H$ a group. A bijective product-preserving map between groups is an isomorphism. ([[math:def-action-by-automorphisms]], [[math:def-external-semidirect-product]], [[math:thm-external-semidirect-product-is-a-group]], [[math:def-group-isomorphism-and-automorphism]]).

[F6] Finite cardinality $|X|$ is the number of elements of $X$ and is unchanged by bijections. A $d$-dimensional space over a field with $q$ elements has $q^d$ elements. Every subset of a finite set is finite. Cardinalities add for disjoint finite sets. ([[math:def-finite-cardinality]], [[math:lem-cardinality-of-a-finite-dimensional-space-over-a-finite-field]], [[math:thm-subset-of-a-finite-set]], [[math:thm-sum-rule]]).

[F7] For a subgroup $D$ of a finite group $U$, the set $U/D$ of left cosets is finite and its cardinality is the index $[U:D]$. Lagrange's theorem gives $|U|=[U:D]\,|D|$. Two finite sets have a Cartesian product whose cardinality is the product of their cardinalities. ([[math:lem-finite-coset-partition]], [[math:thm-lagrange]], [[math:thm-product-rule]]).

[F8] For linear maps $A,B:E\to E$ and $c\in F$, the pointwise operations satisfy $(A+B)(x)=A(x)+B(x)$ and $(cA)(x)=cA(x)$ for each $x\in E$. The zero map $0$ sends each $x$ to $0$ in $E$. Multiplication by zero in a field gives $0x=0$. ([[math:def-vector-space-of-linear-maps]], [[math:lem-of-zero-mult]]).

## Proof

**Given:** A finite field $F$ of order $q$, an extension $E/F$ of degree two, and an ordered $F$-basis of $E$.

**Goal:** Identify the projective multiplication subgroup and its normalizer, prove the semidirect product and Frobenius descriptions, and compute the normalizer order.

1.1 By dimension two the chosen ordered basis has two vectors. Its coordinates identify invertible $F$-linear maps on $E$ with invertible two-by-two matrices. The scalar map $x\mapsto cx$ has matrix $cI$ for $c\in F^\times$. For $a,b\in E$, distributivity and commutativity show that $m_a$ is $F$-linear, and evaluation at each $x\in E$ gives $m_a+m_b=m_{a+b}$, $c m_b=m_{cb}$ for $c\in F$, and $m_a\circ m_b=m_{ab}$. Also $m_1=\mathrm{id}_E$, and $0x=0$ gives $m_0=0$. Evaluation at $1$ distinguishes the maps $m_a$. For $a\ne0$, $m_{a^{-1}}$ is the inverse of $m_a$. The inclusion of fields identifies $F^\times$ with a subgroup of the commutative group $E^\times$, since the inclusion preserves $1$, products and inverses. Every conjugation in $E^\times$ acts as the identity, so $F^\times$ is normal. The quotient group laws therefore apply to $C$. For $a,b\in E^\times$, $[m_a]=[m_b]$ holds exactly when $m_a=c m_b$ for some $c\in F^\times$, or equivalently $a=cb$. If the cosets agree then $a\in bF^\times$, and conversely $a=cb$ gives $aF^\times=bF^\times$ because multiplication by $c$ permutes $F^\times$. Thus $aF^\times\mapsto[m_a]$ is well defined and injective, and $m_a\circ m_b=m_{ab}$ proves it preserves the quotient product. The image contains the identity and is closed under products and inverses, so this is an isomorphism onto the subgroup $T$. [F1, F2, F3, F5, F8]

2.1 Take $g\in N_G(T)$ and an invertible $F$-linear map $S$ representing it. For every $b\in E^\times$ there is a $d\in E^\times$ with $[S\circ m_b\circ S^{-1}]=[m_d]$. Equality of projective classes gives $S\circ m_b\circ S^{-1}=c m_d=m_{cd}$ for some $c\in F^\times$. Applying the same argument to $g^{-1}$ shows that conjugation by $S$ maps the nonzero multiplication maps onto themselves. It fixes the zero map because $S(0)=0$, so it permutes all the maps $m_b$ for $b\in E$. [F2, F3, F8, step 1.1]

2.2 By the cardinality formula for a two-dimensional space, $|E|=q^2$. Apply the finite-field theorem with degree two. It gives $|H|=2$ and says that $\sigma_q$ generates $H$. The identity generates only the trivial subgroup, so $\sigma_q$ is the unique nonidentity element of $H$, and $H=\{\mathrm{id}_E,\sigma_q\}$. Its inverse is also a nonidentity element because the inverse of the identity is the identity. Thus $\sigma_q^{-1}=\sigma_q$, and $\sigma_q\circ\sigma_q=\mathrm{id}_E$ gives element order two. For any $\sigma\in H$, both $\sigma$ and its inverse preserve addition and fix $F$ and hence are $F$-linear by multiplicativity. For $b,x\in E$, $(\sigma\circ m_b\circ\sigma^{-1})(x)=\sigma(b)x$. In particular $[\sigma]$ normalizes $T$ since $\sigma$ permutes $E^\times$. Each $[m_a]\in T$ normalizes $T$ as well, and consequently every $[m_a\circ\sigma]$ belongs to $N_G(T)$. [given, F1, F2, F3, F4, F6, step 1.1]

3.1 Define $\sigma:E\to E$ by $S\circ m_b\circ S^{-1}=m_{\sigma(b)}$. This map is bijective by the preceding permutation and evaluation at $1$. At each $x\in E$, linearity of $S$ gives $S((m_b+m_d)(S^{-1}(x)))=S(m_b(S^{-1}(x)))+S(m_d(S^{-1}(x)))$, so conjugation preserves these pointwise sums. It preserves compositions and the identity map by the inverse equations. The addition and multiplication formulas for $m_b$ therefore give $\sigma(b+d)=\sigma(b)+\sigma(d)$, $\sigma(bd)=\sigma(b)\sigma(d)$, and $\sigma(1)=1$. For $b\in F$, the map $m_b$ is scalar multiplication and commutes with $S$, so $\sigma(b)=b$. Thus $\sigma\in H$. Replacing $S$ by $cS$ for $c\in F^\times$ leaves conjugation unchanged because the scalar map commutes with every $F$-linear map. The intertwining equation $S\circ m_b=m_{\sigma(b)}\circ S$ at $1$ now gives $S(b)=\sigma(b)S(1)$ for every $b\in E$. Since $S$ is injective and $S(0)=0$, $a=S(1)$ is nonzero. Thus $S=m_a\circ\sigma$. [F1, F2, F4, F8, step 1.1, step 2.1]

3.2 For $\sigma\in H$, since $\sigma$ fixes $F$ pointwise, replacing $a$ by $ca$ with $c\in F^\times$ multiplies $\sigma(a)$ by the same $c$. Thus $\alpha_\sigma(aF^\times)=\sigma(a)F^\times$ is well defined and preserves the quotient product by multiplicativity of $\sigma$. Its inverse is $\alpha_{\sigma^{-1}}$. Evaluating on cosets gives $\alpha_{\mathrm{id}_E}=\mathrm{id}_C$ and $\alpha_{\sigma\circ\tau}=\alpha_\sigma\circ\alpha_\tau$. This supplies the action for $C\rtimes_\alpha H$. In the proposed map $\Phi(aF^\times,\sigma)=[m_a\circ\sigma]$, changing $a$ by a factor in $F^\times$ scales the representative by that factor. Moreover $(m_a\circ\sigma)\circ(m_b\circ\tau)=m_{a\sigma(b)}\circ(\sigma\circ\tau)$, by the conjugation formula. Hence $\Phi$ is well defined and preserves the semidirect product law. [F2, F3, F4, F5, F8, step 1.1, step 2.2]

4.1 The factorization of $S$ gives surjectivity of $\Phi$. If $[m_a\circ\sigma]=[m_b\circ\tau]$, then $m_a\circ\sigma=c(m_b\circ\tau)$ for some $c\in F^\times$. Evaluating at $1$ gives $a=cb$, and canceling multiplication by $a$ gives $\sigma=\tau$. This proves injectivity and the isomorphism. The two possible automorphisms give the disjoint sets $T$ and $T[\sigma_q]$. For $S=m_a\circ\sigma_q$ in the latter case, additivity follows from $F$-linearity, and $S(bx)=a\sigma_q(b)\sigma_q(x)=\sigma_q(b)S(x)$. Because the multiplication maps commute, conjugation by $m_a$ fixes $m_{\sigma_q(b)}$, so conjugation by $S$ sends $m_b$ to $m_{\sigma_q(b)}$. [F1, F2, F3, F5, F8, step 1.1, step 2.2, step 3.1, step 3.2]

5.1 Since $F$ and $E$ are finite, their subsets $F^\times$ and $E^\times$ are finite. In each field the zero singleton and the group of nonzero elements form a disjoint partition. Adding the cardinalities of the two parts gives $|F^\times|=q-1$ and $|E^\times|=q^2-1$. The finite coset partition lemma for $F^\times\le E^\times$ gives that $C$ is finite and $[E^\times:F^\times]=|C|$. Lagrange's theorem then gives $q^2-1=|C|(q-1)$. As $0\ne1$ in $F$, we have $q\ge2$, and division gives $|C|=q+1$. The isomorphism identifies the normalizer bijectively with the pairs in $C\times H$. The product rule and $|H|=2$ give $|N_G(T)|=2(q+1)$, completing the normalizer description. [F1, F3, F6, F7, step 1.1, step 2.2, step 4.1] ∎
