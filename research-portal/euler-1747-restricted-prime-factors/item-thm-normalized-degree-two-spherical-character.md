---
title: Normalized spherical character in degree two
status: draft
research_item: thm-normalized-degree-two-spherical-character
dependency_level: 3
sources:
  references:
    - title: Benedict H. Gross, On the Satake isomorphism
      url: https://people.math.harvard.edu/~gross/preprints/sat.pdf#page=6
      locator: §1, local setting and definition of the Weyl group on PDF page 2, and
        invariants after (1.4). §2, (2.1)–(2.5), the double-coset basis before
        Proposition 2.6, and (2.11)–(2.13). §3, (3.1)–(3.5) and Proposition 3.6.
        §6, the complex isomorphism preceding (6.3).
      statement: The integral spherical Hecke ring consists of locally constant,
        compactly supported, integer-valued bi-K-invariant functions. The
        double-coset indicators form its integral basis, and convolution for
        Haar measure giving K volume one is its multiplication, with the
        indicator of K as unit. The normalized Satake transform has value at
        each t in the diagonal torus equal to the positive square root of the
        modulus at t times the integral over N of n ↦ f(tn). After complex
        scalar extension it is a unital algebra isomorphism onto the
        Weyl-invariant group algebra of the diagonal torus modulo its
        intersection with K. For the split torus, quotient by its integral
        points gives the cocharacter lattice, where the cocharacters are
        algebraic group homomorphisms from the multiplicative group to the
        torus. Evaluation at the uniformizer followed by passage to the quotient
        inverts that identification. The Weyl group is the quotient of the
        normalizer of the torus by the torus.
      hypotheses: A nonarchimedean local field with finite residue field and a chosen
        uniformizer, and a connected split reductive group with an integral
        group scheme model of reductive special fiber. A split maximal torus is
        contained in a Borel, both defined over the valuation ring. The compact
        subgroup K consists of the integral points of the model, and N consists
        of the field points of the unipotent radical of the Borel. The Haar
        measures give K and N ∩ K volume one, respectively. The local
        application uses the standard degree-two matrix model.
      reading_limits: Read the cited setting, integral Hecke ring, torus
        identification, normalized isomorphism and its complex version. The
        example (3.7) assumes dominant cocharacters. The proof here computes the
        coefficients for all valuation pairs from (3.4) and identifies the
        complex source algebra.
    - title: Benedict H. Gross, On the Satake isomorphism
      url: https://people.math.harvard.edu/~gross/preprints/sat.pdf#page=11
      locator: §6, paragraph leading to (6.3)
      statement: In an irreducible smooth complex representation, the space fixed by
        the standard compact subgroup has dimension at most one. When nonzero,
        it carries a scalar character of the spherical Hecke algebra.
      hypotheses: Specialized to the same GL_2 and standard integral compact subgroup
        as the Satake isomorphism. The representation is smooth and
        algebraically irreducible over the complex numbers.
      reading_limits: Read the paragraph leading to (6.3). The proof uses the
        fixed-space bound as stated.
    - title: J. S. Milne, Algebraic Groups, version 2.00 (20 December 2015)
      url: https://www.jmilne.org/math/CourseNotes/iAG200.pdf#page=400
      locator: Proposition 1.59 (PDF page 33), Corollary 22.60 (PDF page 399) and
        Example 22.62 (PDF page 400).
      statement: For an algebraic subgroup H of G, the algebraic normalizer at a
        commutative base algebra R consists of elements of G(R) whose
        conjugation preserves the base change of H to R. Equivalently, this
        conjugation preserves H on points over every commutative R-algebra. For
        a split reductive group with its split maximal torus the Weyl group is
        constant. For GL_n and its diagonal torus, its members are represented
        by the permutation matrices, which act by permuting the diagonal
        entries.
      hypotheses: The normalizer criterion is over a field and applies to an algebraic
        subgroup of an algebraic group. The Weyl calculation uses the split
        group GL_n with its diagonal maximal torus.
      reading_limits: Read the normalizer criterion, the constancy assertion, and the
        GL_n example at the listed locations. The degree-two field-point
        calculation and action on valuation coordinates are supplied locally.
    - title: J. S. Milne, Algebraic Groups, version 2.00 (20 December 2015)
      url: https://www.jmilne.org/math/CourseNotes/iAG200.pdf#page=384
      locator: Examples 22.21 and 22.25 (PDF page 384), Definition 22.30 (page 385),
        §19(f) opening (page 346), Example 22.76 (page 404), and Theorem 22.85
        with the empty subset of simple roots (page 407).
      statement: Over a field, GL_n is connected reductive and its split diagonal
        torus is maximal. A reductive group with a split maximal torus is split.
        Over an algebraically closed field the invertible upper-triangular
        subgroup is a Borel. For that Borel in split GL_n, the groups for the
        positive roots are I+aE_ij for i<j and generate its unipotent radical.
        For n=2 there is one such group.
      hypotheses: The reductivity and split diagonal torus assertions apply to GL_n
        over a field. The Borel example is taken over algebraically closed
        fields. The root calculation uses the split pair (GL_n, D_n), with the
        positive roots from the upper-triangular Borel.
      reading_limits: Read the specified field-level examples and definitions and the
        statement of Theorem 22.85. The proof applies them to the matrix model
        and its geometric fibers.
    - title: The Stacks Project, General linear group scheme
      url: https://stacks.math.columbia.edu/tag/022W
      locator: Groupoid Schemes, Example 39.5.4 (Tag 022W), including its base-change
        formula.
      statement: The group functor of invertible n by n matrices is represented over
        the integers by the spectrum of the polynomial ring in the matrix
        entries with the determinant inverted, with group law given by matrix
        multiplication. Base change to any scheme represents the same functor on
        schemes over that base.
      hypotheses: The matrix size is at least one. For the base change the test
        schemes are over the chosen base scheme, and matrices are taken over
        their rings of global sections.
      reading_limits: Read the full example through the formula for the functor after
        base change. The application takes size two and base Spec O.
    - title: The Stacks Project, Smooth ring maps and smooth morphisms
      url: https://stacks.math.columbia.edu/tag/00T1
      locator: Commutative Algebra, Definition 10.137.5 with no equations and Lemma
        10.137.6(1) and (4), Tag 00T1. Morphisms of Schemes, Definition
        29.35.1(1)–(2), Tag 01V5.
      statement: A polynomial algebra over a commutative ring is standard smooth by
        the presentation with no equations. A standard smooth algebra is smooth,
        and a principal localization of a standard smooth algebra is standard
        smooth. The map of affine spectra of a smooth ring map is smooth.
      hypotheses: The polynomial ring has finitely many variables. Localization is at
        a single element, and the affine structure map is induced by the given
        ring map.
      reading_limits: Read the stated definition, the applicable parts of the standard
        smooth lemma, and the affine smoothness definition. The application uses
        the determinant and the product of the two diagonal coordinates as the
        localization elements.
    - title: Brian Conrad, Reductive Group Schemes
      url: https://math.stanford.edu/~conrad/papers/luminysga3smf.pdf
      locator: Definition 3.1.1 (printed p. 81), Definition 3.2.1 (p. 91), Definition
        5.2.1 (p. 151), Corollary 5.2.5 (p. 153), and Definition 5.2.10 (p.
        157).
      statement: A smooth relatively affine group scheme is reductive when its
        geometric fibers are connected reductive. In a smooth relatively affine
        group scheme a torus is maximal when maximal on every geometric fiber.
        In a reductive group scheme a smooth relatively affine subgroup with
        parabolic geometric fibers is parabolic and is a Borel if its fibers are
        Borels. A parabolic has a unique smooth closed normal subgroup with
        geometric fibers the fiberwise unipotent radicals.
      hypotheses: The base is a scheme. The maximal torus test is for a torus in a
        smooth relatively affine group scheme. The parabolic and relative
        radical statements are for subgroup schemes of a reductive group scheme.
      reading_limits: Read the cited definitions and the unipotent radical statement
        of Corollary 5.2.5. The proof checks the relative criteria using the
        explicit matrix scheme and its fibers.
---

## Prerequisites

- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)
- [lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)
- [def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)
- [def-author-d45da46285be-satake-transform](item-def-author-d45da46285be-satake-transform)
- [def-author-d45da46285be-spherical-model](item-def-author-d45da46285be-spherical-model)
- [math:thm-fundamental-theorem-of-symmetric-polynomials](https://alphabetamath.cc/item/thm-fundamental-theorem-of-symmetric-polynomials)
- [math:thm-fundamental-theorem-of-algebra-minimum-modulus-proof](https://alphabetamath.cc/item/thm-fundamental-theorem-of-algebra-minimum-modulus-proof)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)
- [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)
- [math:def-banach-valued-simple-function-and-integral](https://alphabetamath.cc/item/def-banach-valued-simple-function-and-integral)
- [math:thm-complex-plane-is-complete](https://alphabetamath.cc/item/thm-complex-plane-is-complete)
- [math:def-measure](https://alphabetamath.cc/item/def-measure)
- [math:def-lie-algebra-of-a-group-scheme](https://alphabetamath.cc/item/def-lie-algebra-of-a-group-scheme)
- [math:def-upper-unitriangular-group-scheme](https://alphabetamath.cc/item/def-upper-unitriangular-group-scheme)
- [math:lem-lie-algebra-tangent-space-and-functoriality](https://alphabetamath.cc/item/lem-lie-algebra-tangent-space-and-functoriality)
- [math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra)
- [math:lem-topological-group-translations-and-inversion](https://alphabetamath.cc/item/lem-topological-group-translations-and-inversion)
- [math:def-locally-finite-type-and-finite-type-morphism](https://alphabetamath.cc/item/def-locally-finite-type-and-finite-type-morphism)
- [math:def-quasi-compact-and-quasi-separated-morphism](https://alphabetamath.cc/item/def-quasi-compact-and-quasi-separated-morphism)
- [math:def-finite-type-and-module-finite-algebras](https://alphabetamath.cc/item/def-finite-type-and-module-finite-algebras)
- [math:lem-distinguished-opens-cover-every-open](https://alphabetamath.cc/item/lem-distinguished-opens-cover-every-open)
- [math:cor-polynomial-ring-over-a-field-is-euclidean](https://alphabetamath.cc/item/cor-polynomial-ring-over-a-field-is-euclidean)
- [math:thm-euclidean-domain-is-a-pid](https://alphabetamath.cc/item/thm-euclidean-domain-is-a-pid)
- [math:def-morphism-affine-schemes-from-ring-map](https://alphabetamath.cc/item/def-morphism-affine-schemes-from-ring-map)
- [math:lem-spectrum-map-stalk-homomorphisms-local](https://alphabetamath.cc/item/lem-spectrum-map-stalk-homomorphisms-local)
- [math:def-determinant-of-a-linear-operator](https://alphabetamath.cc/item/def-determinant-of-a-linear-operator)
- [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)
- [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)
- [math:def-restriction-and-extension-of-scalars](https://alphabetamath.cc/item/def-restriction-and-extension-of-scalars)
- [math:thm-tensor-products-commute-with-arbitrary-direct-sums](https://alphabetamath.cc/item/thm-tensor-products-commute-with-arbitrary-direct-sums)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:def-prime-and-maximal-ideals](https://alphabetamath.cc/item/def-prime-and-maximal-ideals)
- [math:cor-maximal-ideals-are-prime](https://alphabetamath.cc/item/cor-maximal-ideals-are-prime)
- [math:thm-generated-ideal-description-in-a-commutative-ring](https://alphabetamath.cc/item/thm-generated-ideal-description-in-a-commutative-ring)
- [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)
- [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals)
- [math:def-affine-scheme-spectrum](https://alphabetamath.cc/item/def-affine-scheme-spectrum)
- [math:def-functor-of-points-affine-scheme](https://alphabetamath.cc/item/def-functor-of-points-affine-scheme)
- [math:def-morphism-and-closed-subgroup-scheme](https://alphabetamath.cc/item/def-morphism-and-closed-subgroup-scheme)
- [` Benedict H. Gross, On the Satake isomorphism · §1, local setting and definition of the Weyl group on PDF page 2, and invariants after (1.4). §2, (2.1)–(2.5), the double-coset basis before Proposition 2.6, and (2.11)–(2.13). §3, (3.1)–(3.5) and Proposition 3.6. §6, the complex isomorphism preceding (6.3). `](https://people.math.harvard.edu/~gross/preprints/sat.pdf#page=6)
- [` Benedict H. Gross, On the Satake isomorphism · §6, paragraph leading to (6.3) `](https://people.math.harvard.edu/~gross/preprints/sat.pdf#page=11)
- [` J. S. Milne, Algebraic Groups, version 2.00 (20 December 2015) · Proposition 1.59 (PDF page 33), Corollary 22.60 (PDF page 399) and Example 22.62 (PDF page 400). `](https://www.jmilne.org/math/CourseNotes/iAG200.pdf#page=400)
- [` J. S. Milne, Algebraic Groups, version 2.00 (20 December 2015) · Examples 22.21 and 22.25 (PDF page 384), Definition 22.30 (page 385), §19(f) opening (page 346), Example 22.76 (page 404), and Theorem 22.85 with the empty subset of simple roots (page 407). `](https://www.jmilne.org/math/CourseNotes/iAG200.pdf#page=384)
- [` The Stacks Project, General linear group scheme · Groupoid Schemes, Example 39.5.4 (Tag 022W), including its base-change formula. `](https://stacks.math.columbia.edu/tag/022W)
- [` The Stacks Project, Smooth ring maps and smooth morphisms · Commutative Algebra, Definition 10.137.5 with no equations and Lemma 10.137.6(1) and (4), Tag 00T1. Morphisms of Schemes, Definition 29.35.1(1)–(2), Tag 01V5. `](https://stacks.math.columbia.edu/tag/00T1)
- [` Brian Conrad, Reductive Group Schemes · Definition 3.1.1 (printed p. 81), Definition 3.2.1 (p. 91), Definition 5.2.1 (p. 151), Corollary 5.2.5 (p. 153), and Definition 5.2.10 (p. 157). `](https://math.stanford.edu/~conrad/papers/luminysga3smf.pdf)


## Statement

Assume countable choice, meaning that a sequence of nonempty sets has a choice function. Let $\ell$ be prime, $F=\mathbb Q_\ell$ the $\ell$-adic field, $O=\mathbb Z_\ell$ its ring of integers, $G=\mathrm{GL}_2(F)$ and $K=\mathrm{GL}_2(O)$. Give $G$ and $K$ the subspace topologies from $F^4$ with its product of $\ell$-adic metric topologies. Let $\pi$ be the restriction of a strongly continuous unitary representation of $G$ to its space $V$ of smooth vectors, those fixed by some open subgroup. A strongly continuous unitary representation acts by complex-linear isometries on a complex Hilbert space with continuous orbit maps. Suppose $V$ is irreducible, meaning it is nonzero and has no nonzero proper invariant linear subspace, and admissible, meaning its fixed space under every compact open subgroup is finite dimensional. Suppose $V^K\ne0$.

Then $V^K$ is one dimensional. There is a unique unordered pair of nonzero complex numbers $u,v$, counted with multiplicity, such that for every spherical Hecke function $f$, its operator acts on $V^K$ by the scalar $S(f)(u,v)$. The spherical Hecke algebra consists of compactly supported complex functions invariant on both sides by $K$. Here $S$ is the normalized Satake transform by triangular cosets. Haar measure is normalized by $\operatorname{vol}(K)=1$, so each contributing coset $xK=\{xk:k\in K\}$ has weight one.

For either ordering, the same Hecke character, meaning the same unital complex-algebra map to $\mathbb C$, acts on the normalized upper-triangular spherical vector $\Phi_{u,v}$. This is the right $K$-invariant vector of value one at the identity in the function model where left multiplication by a triangular matrix of diagonal valuations $(r,s)$ multiplies the value by $\ell^{(s-r)/2}u^rv^s$. Its value at an invertible upper-triangular matrix with diagonal $(\ell^r,\ell^s)$ is $\ell^{(s-r)/2}u^rv^s$.

If the central character is trivial, meaning all scalar matrices act as the identity, then $uv=1$. The representation and its fixed-space action descend to $G/(F^\times I)=\mathrm{PGL}_2(F)$ with the quotient topology and compact subgroup the image of $K$.

## Facts & Assumptions

[F1] The field has normalized absolute value $|a|_\ell=\ell^{-\nu(a)}$ on nonzero elements, where the valuation is additive on products. Its ring of integers is compact open with residue field of size $\ell$. Both $K$ and its projective image are compact open in their respective Hausdorff topological groups, and triangular representatives of cosets $xK$ have well-defined diagonal valuations ([lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets), [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)). The completion theorem makes $F$ a complete nonarchimedean valued field and the extension agrees with the rational absolute value on $\mathbb Q$ ([math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)). On the rationals the normalization gives $|\ell|_\ell=\ell^{-1}$ ([math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals)).

[F2] A unitary representation acts by complex-linear norm-preserving bijections with continuous orbit maps. The smooth vectors form a stable subspace: sums are fixed by intersections of their fixing subgroups, and translating a vector conjugates its fixing subgroup ([math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)).

[F3] The spherical Hecke algebra acts on any $K$-fixed space by the operators given by finite coset summation and its convolution product uses the same finite-coset convention with each $xK$ of weight one ([def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)).

[F4] The transform weights each coset with diagonal valuations $(r,s)$ by $\ell^{(s-r)/2}X^rY^s$. In the function model, the line of $K$-fixed vectors has normalized generator $\Phi_{u,v}$ with value $\ell^{(s-r)/2}u^rv^s$ on this coset ([def-author-d45da46285be-satake-transform](item-def-author-d45da46285be-satake-transform), [def-author-d45da46285be-spherical-model](item-def-author-d45da46285be-spherical-model)).

[F5] Every symmetric polynomial in two variables over $\mathbb C$ is a polynomial in $X+Y$ and $XY$. A nonconstant complex polynomial has a root ([math:thm-fundamental-theorem-of-symmetric-polynomials](https://alphabetamath.cc/item/thm-fundamental-theorem-of-symmetric-polynomials), [math:thm-fundamental-theorem-of-algebra-minimum-modulus-proof](https://alphabetamath.cc/item/thm-fundamental-theorem-of-algebra-minimum-modulus-proof)).

[F6] Use the normalized Satake isomorphism and its defining integral in Gross, §3, and the dimension bound for irreducible smooth representations in §6, with hypotheses recorded below. Use also Gross’s integral spherical Hecke ring from §2 and the description of the Weyl group in §1. Evaluation at the chosen uniformizer identifies the cocharacter lattice with the diagonal torus quotient by its integral points in §2.

[F7] A continuous image of a compact space is compact ([math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)). In a quotient topology a subset is open exactly when its preimage is open ([math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)). Left translations in a topological group are homeomorphisms ([math:lem-topological-group-translations-and-inversion](https://alphabetamath.cc/item/lem-topological-group-translations-and-inversion)).

[F8] Use the complex plane with its usual norm $|z|$, for which it is complete ([math:thm-complex-plane-is-complete](https://alphabetamath.cc/item/thm-complex-plane-is-complete)). The scalar case of the Banach-valued simple integral is a sum over the disjoint nonzero level sets. When each such set has finite measure, its contribution is the level value times its measure ([math:def-banach-valued-simple-function-and-integral](https://alphabetamath.cc/item/def-banach-valued-simple-function-and-integral)). A measure is finitely additive on disjoint measurable sets, by countable additivity with empty sets padding the finite family ([math:def-measure](https://alphabetamath.cc/item/def-measure)).

[F9] For a finite-type group scheme over $F$, the Lie algebra at the identity identifies with the kernel of reduction from its $F[\varepsilon]/(\varepsilon^2)$-points to its $F$-points ([math:def-lie-algebra-of-a-group-scheme](https://alphabetamath.cc/item/def-lie-algebra-of-a-group-scheme)). Over $F$, the group schemes $U_2$ and $D_2$ are the upper unitriangular and diagonal subgroups of the general linear group scheme. Their points over a commutative $F$-algebra are the matrices with those forms ([math:def-upper-unitriangular-group-scheme](https://alphabetamath.cc/item/def-upper-unitriangular-group-scheme)). A morphism of finite-type group schemes induces a linear map on Lie algebras, computed on the reduction kernels by applying the morphism to dual-number points. ([math:lem-lie-algebra-tangent-space-and-functoriality](https://alphabetamath.cc/item/lem-lie-algebra-tangent-space-and-functoriality))

[F10] A left Haar measure is a left-translation-invariant Borel measure. ([def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)) The Borel sigma-algebra is generated by the open sets, so it contains every open set. ([math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra))

[F11] The product of two-by-two matrices over a field or local ring has entries $(AB)_{ij}=\sum_{h=1}^2 A_{ih}B_{hj}$. ([def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group))

[F12] A scheme morphism is of finite type if it is locally of finite type and quasi-compact. On an affine chart over an affine base, a finitely generated coordinate algebra gives the local finite-type condition ([math:def-locally-finite-type-and-finite-type-morphism](https://alphabetamath.cc/item/def-locally-finite-type-and-finite-type-morphism), [math:def-finite-type-and-module-finite-algebras](https://alphabetamath.cc/item/def-finite-type-and-module-finite-algebras)). A morphism is quasi-compact when preimages of quasi-compact open subsets are quasi-compact ([math:def-quasi-compact-and-quasi-separated-morphism](https://alphabetamath.cc/item/def-quasi-compact-and-quasi-separated-morphism)).

[F13] The distinguished opens $D(f)$, consisting of primes omitting $f$, form a basis of an affine spectrum ([math:lem-distinguished-opens-cover-every-open](https://alphabetamath.cc/item/lem-distinguished-opens-cover-every-open)). A one-variable polynomial ring over a field is Euclidean, and every Euclidean domain is a principal ideal domain ([math:cor-polynomial-ring-over-a-field-is-euclidean](https://alphabetamath.cc/item/cor-polynomial-ring-over-a-field-is-euclidean), [math:thm-euclidean-domain-is-a-pid](https://alphabetamath.cc/item/thm-euclidean-domain-is-a-pid)).

[F14] A ring map induces a morphism of affine spectra in the opposite direction. Its maps on stalks are local, so it is a scheme morphism ([math:def-morphism-affine-schemes-from-ring-map](https://alphabetamath.cc/item/def-morphism-affine-schemes-from-ring-map), [math:lem-spectrum-map-stalk-homomorphisms-local](https://alphabetamath.cc/item/lem-spectrum-map-stalk-homomorphisms-local)).

[F15] The determinant of a linear operator in positive dimension is the determinant of its matrix in an ordered basis ([math:def-determinant-of-a-linear-operator](https://alphabetamath.cc/item/def-determinant-of-a-linear-operator)). The determinant of a one-by-one matrix is its sole entry, since only the identity permutation contributes ([math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)).

[F16] Matrix products over any commutative algebra use the row-by-column formula ([math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)). Use the algebraic normalizer criterion and the permutation representatives for the split general linear group recorded below.

[F17] Extension of scalars along a map of commutative rings $R\to A$ sends an $R$-module $M$ to $A\otimes_R M$ and sends inverse maps to inverse maps ([math:def-restriction-and-extension-of-scalars](https://alphabetamath.cc/item/def-restriction-and-extension-of-scalars)). Tensor products commute with direct sums. Thus each basis summand $R$ becomes a basis summand $A$ under scalar extension ([math:thm-tensor-products-commute-with-arbitrary-direct-sums](https://alphabetamath.cc/item/thm-tensor-products-commute-with-arbitrary-direct-sums)).

[F18] A space is quasi-compact when every open cover has a finite subcover ([math:def-compact-space](https://alphabetamath.cc/item/def-compact-space), where this property is called compactness). In a commutative ring, a maximal ideal is a proper ideal with no strictly larger proper ideal, and a prime ideal is a proper ideal containing a factor of every product it contains ([math:def-prime-and-maximal-ideals](https://alphabetamath.cc/item/def-prime-and-maximal-ideals)). Every maximal ideal in a commutative ring is prime ([math:cor-maximal-ideals-are-prime](https://alphabetamath.cc/item/cor-maximal-ideals-are-prime)). The ideal generated by a set consists of finite sums of ring multiples of elements of that set ([math:thm-generated-ideal-description-in-a-commutative-ring](https://alphabetamath.cc/item/thm-generated-ideal-description-in-a-commutative-ring)).

[F19] The points of an affine spectrum are the prime ideals of its coordinate ring ([math:def-affine-scheme-spectrum](https://alphabetamath.cc/item/def-affine-scheme-spectrum)). For an affine scheme over $F$, its points over a commutative $F$-algebra are the $F$-algebra homomorphisms from its coordinate ring to that algebra, by the affine functor of points ([math:def-functor-of-points-affine-scheme](https://alphabetamath.cc/item/def-functor-of-points-affine-scheme)). A morphism of finite-type group schemes over $F$ is an $F$-scheme morphism commuting with multiplication, identity and inverse ([math:def-morphism-and-closed-subgroup-scheme](https://alphabetamath.cc/item/def-morphism-and-closed-subgroup-scheme)).

[F20] Use the determinant-invertible general linear group scheme over the valuation ring and the fiberwise criteria for reductivity, maximal tori, Borel subgroups and unipotent radicals recorded below. Use the field-level general linear group and triangular Borel structure from Milne.

[F21] A polynomial algebra in finitely many variables and each of its principal localizations give smooth affine schemes over the coefficient ring, by the standard smooth criterion recorded below.

## External input

Gross’s integral spherical Hecke ring $\mathcal H_{\mathbb Z}$ consists of the locally constant, compactly supported, integer-valued bi-$K$-invariant functions. The double-coset indicators form its integral basis. Its product uses Haar convolution with $K$ of volume one, and the indicator of $K$ is its unit. [On the Satake isomorphism, §2](https://people.math.harvard.edu/~gross/preprints/sat.pdf#page=3)

For the standard integral compact subgroup and upper-triangular choice, Gross's formula (3.4) gives the value at every diagonal matrix $t$ as $S_{\mathrm{Gross}}(f)(t)=\delta(t)^{1/2}\int_N f(tn)\,dn$. Here $N=\mathbf N(F)$ for the upper unitriangular group scheme $\mathbf N=U_2$. For $t=\operatorname{diag}(\ell^r,\ell^s)$, formula (3.3) gives the half modulus as the positive square root of the absolute determinant of conjugation on $\operatorname{Lie}(\mathbf N)$. The subgroup $N\cap K$ has measure one. By Proposition 3.6 and (3.5), after extending scalars to $\mathbb C$ this transform is an algebra isomorphism onto the Weyl-invariant group algebra of the torus quotient. [On the Satake isomorphism, §3](https://people.math.harvard.edu/~gross/preprints/sat.pdf#page=6)

Gross's §1 defines the Weyl group of the algebraic diagonal torus $\mathbf T$ as its algebraic normalizer modulo $\mathbf T$. [On the Satake isomorphism, §1](https://people.math.harvard.edu/~gross/preprints/sat.pdf#page=2)

The separate fixed-space bound applies to an irreducible smooth complex representation of this group. [On the Satake isomorphism, §6](https://people.math.harvard.edu/~gross/preprints/sat.pdf#page=11)

By Milne’s normalizer criterion, a matrix over a field extension $E/F$ lies in the algebraic normalizer of $\mathbf T$ when its conjugation preserves the base-changed torus, equivalently when it preserves the diagonal subgroup over every commutative $E$-algebra. For the diagonal torus of split $\mathrm{GL}_n$ the Weyl group is constant, with its classes represented by the permutation matrices. [Milne, Algebraic Groups, Proposition 1.59](https://www.jmilne.org/math/CourseNotes/iAG200.pdf#page=33) and [Corollary 22.60 and Example 22.62](https://www.jmilne.org/math/CourseNotes/iAG200.pdf#page=400)

For the split torus in Gross’s setting, a cocharacter is a group-scheme homomorphism from $\mathbf G_m$ to the torus. Quotienting its field points by its integral points identifies the quotient with the cocharacter lattice. The inverse sends a cocharacter to the class of its value at the uniformizer, and the torus Hecke basis element for that class corresponds to the cocharacter basis element of the group algebra. [On the Satake isomorphism, §1 and (2.11)–(2.13)](https://people.math.harvard.edu/~gross/preprints/sat.pdf#page=5)

The general linear group scheme over a base ring is given by the polynomial ring in the entries with the determinant inverted. Its points over an algebra of the base ring are the invertible matrices of the given size over that algebra. [The Stacks Project, Example 39.5.4](https://stacks.math.columbia.edu/tag/022W)

Over a field the general linear group is connected reductive and its diagonal torus is split maximal. Over an algebraically closed field, the upper-triangular subgroup is a Borel. In the split general linear group, the positive root groups for this Borel generate its unipotent radical. In degree two the only positive root group is the upper unitriangular subgroup. [Milne, general linear groups and maximal tori](https://www.jmilne.org/math/CourseNotes/iAG200.pdf#page=384) and [Borels](https://www.jmilne.org/math/CourseNotes/iAG200.pdf#page=346), with [Example 22.76](https://www.jmilne.org/math/CourseNotes/iAG200.pdf#page=404) and [Theorem 22.85](https://www.jmilne.org/math/CourseNotes/iAG200.pdf#page=407)

A standard smooth algebra gives a smooth affine structure morphism. This applies to a polynomial algebra in finitely many variables and to its principal localizations. [The Stacks Project, §10.137](https://stacks.math.columbia.edu/tag/00T1) and [Definition 29.35.1](https://stacks.math.columbia.edu/tag/01V5)

A smooth affine group scheme over a base is reductive if all geometric fibers are connected reductive. Maximality of a torus is tested on geometric fibers. A smooth affine subgroup with Borel geometric fibers in a reductive group scheme is a Borel over the base, using the parabolic criterion on those fibers. Its unipotent radical is the unique smooth closed normal subgroup having the geometric fiber radicals. [Conrad, Reductive Group Schemes, Definitions 3.1.1, 3.2.1, 5.2.1 and 5.2.10 and Corollary 5.2.5](https://math.stanford.edu/~conrad/papers/luminysga3smf.pdf)

## Proof

**Given:** $\ell,\pi,V,K$ and the hypotheses in the statement.

**Goal:** Identify the Hecke character, its normalized function model and its projective descent.

1.1 By [F1], the absolute value on $F$ extends that on $\mathbb Q$, so $|\ell|_\ell=\ell^{-1}$ and $\nu(\ell)=1$. The integer values of $\nu$ therefore range over $\mathbb Z$, and the nonzero elements of positive valuation are divisible by $\ell$ in $O$. Thus $F$ is complete discretely valued, with uniformizer $\ell$ and residue field of size $\ell$. Take the affine group scheme $\mathbf G_O=\operatorname{Spec} O[x_{11},x_{12},x_{21},x_{22},d^{-1}]$ with $d=x_{11}x_{22}-x_{12}x_{21}$, as in [F20]. Its $O$-points are the invertible matrices $K$, and its generic and special fibers are the corresponding general linear groups over $F$ and $O/\ell O$. The determinant localization is smooth over $O$ by [F21]. The geometric fibers are connected reductive by the field result in [F20], so the integral model is reductive. The compact open subgroup $K$ is the one in [F1]. [F1, F20, F21]

2.1 Inside $\mathbf G_O$ take the diagonal subgroup $\mathbf T_O$ and the upper-triangular subgroup $\mathbf B_O$, defined by setting the off-diagonal entries and the lower-left entry to zero, respectively. These equations are stable under matrix multiplication and inversion over every $O$-algebra. For an upper-triangular matrix with diagonal $(a,d)$ and upper-right entry $b$, the product $ad$ is a unit, and its inverse has diagonal $(a^{-1},d^{-1})$ and upper-right entry $-a^{-1}bd^{-1}$. The diagonal subgroup is $\mathbf G_m^2$ and is maximal on all geometric fibers by [F20]. In particular the generic fiber of $\mathbf G_O$ is split. The upper-triangular subgroup is smooth and affine by [F21], since its coordinate ring is the polynomial ring on the two diagonal entries and the upper-right entry with the product of the diagonal entries inverted. It has Borel geometric fibers by [F20] and hence is a Borel over $O$. The upper unitriangular subgroup $\mathbf N_O$ is the closed normal kernel of the diagonal projection of $\mathbf B_O$ onto $\mathbf T_O$. It is smooth with coordinate ring $O[Z]$, and on each geometric fiber it is the unipotent radical by [F20]. The relative radical criterion identifies it with the unipotent radical over $O$. These data meet the field and group hypotheses in Gross’s local setting. [F1, F6, F20, F21, step 1.1]

3.1 The smooth complex representation on $V$ is irreducible by hypothesis, so the fixed-space bound from [F6] and the nonzero hypothesis yield $\dim_{\mathbb C}V^K=1$. Write $\lambda(f)$ for the scalar of $T_f$ on this line. The unital action in [F3] makes $\lambda$ a unital complex-algebra homomorphism. [F2, F3, F6, given, step 2.1]

3.2 Let $\mathbf T=D_2$ and $\mathbf N=U_2$ be the diagonal and upper unitriangular group schemes over $F$, and put $T=\mathbf T(F)$ and $N=\mathbf N(F)$. These group schemes are the generic fibers of $\mathbf T_O$ and $\mathbf N_O$ from step 2.1. Write $n(z)=\begin{pmatrix}1&z\\0&1\end{pmatrix}$ for an upper unitriangular matrix of size two. By [F9] the group scheme $\mathbf N$ has the polynomial coordinate ring $F[Z]$, generated over $F$ by $Z$. Thus the structure morphism is locally of finite type by [F12]. To check quasi-compactness, refine an open cover of $\operatorname{Spec} F[Z]$ by the distinguished opens $D(f)$ contained in its members. If their polynomials generated a proper ideal, it would be principal by [F13]. The zero ideal is prime by [F18] because the polynomial ring is a domain. For a proper nonzero principal ideal $(p)$, choose a divisor $h$ of $p$ of least positive degree. Such a divisor exists since $p$ is nonconstant. It is irreducible, since a factorization into two nonconstant factors would give a divisor of $p$ of smaller positive degree. A generator of any larger principal ideal divides $h$. If the larger ideal is proper, its generator is therefore a unit multiple of $h$, so the ideal is $(h)$. Thus $(h)$ is maximal, and it is prime by [F18]. In either case a prime containing all the covering polynomials would be in none of the distinguished opens. Thus the polynomials generate the unit ideal. By [F18] write $1$ as a finite sum of multiples of these polynomials. No proper prime ideal contains all polynomials in that expression, so their distinguished opens cover the spectrum. For each of those finitely many opens, choose a member of the original cover containing it, using countable choice with singleton sets padding the finite list of nonempty choices. The chosen members form a finite subcover, so the spectrum is quasi-compact by [F18]. By [F19], $\operatorname{Spec} F$ has just the point $(0)$ because $F$ is a field. The quasi-compactness of the source therefore gives quasi-compactness of the structure morphism, since the only opens of the target are the empty set and the singleton. This proves $\mathbf N$ is of finite type. [F9, F12, F13, F18, F19, given, step 2.1]

4.1 Reduction from the dual numbers sends $n(w+\varepsilon z)$ to $n(w)$. By [F9] the tangent vectors at $n(0)$ are parametrized by $n(\varepsilon z)$ with $z\in F$. The coefficient of $\varepsilon$ in the coordinate $Z$ identifies the tangent space with the one-dimensional vector space $F$. For $a,d\in F^\times$, substitution $Z\mapsto(a/d)Z$ in $F[Z]$ is a ring automorphism with inverse $Z\mapsto(d/a)Z$. It induces an automorphism of the affine scheme by [F14]. By [F19], a point $n(z)$ over a commutative $F$-algebra corresponds to the map sending $Z$ to $z$. Precomposing this map with the substitution sends $n(z)$ to $n((a/d)z)$. This equals conjugation by $\operatorname{diag}(a,d)$ by entrywise multiplication. The multiplication map pulls $Z$ back to $Z_1+Z_2$, the identity sends it to zero, and inversion sends it to $-Z$. Writing $c=a/d$, the two compositions for compatibility with multiplication pull $Z$ back to $c(Z_1+Z_2)$ and $cZ_1+cZ_2$, which agree. Both identity compositions send $Z$ to zero, and both inverse compositions send $Z$ to $-cZ$. These equalities on the generator verify the group-scheme morphism conditions in [F19]. The same identities with $c^{-1}$ verify them for the inverse, so this is a group-scheme automorphism. On the dual-number points this sends $n(\varepsilon z)$ to $n(\varepsilon(a/d)z)$. By functoriality in [F9], the induced map on $\operatorname{Lie}(\mathbf N)$ is this map on the reduction kernel. On the tangent line this is multiplication by $a/d$. Its matrix in the basis corresponding to $n(\varepsilon)$ has the single entry $a/d$, so [F15] gives determinant $a/d$. By Gross's formula (3.3), the positive half modulus at $t=\operatorname{diag}(\ell^r,\ell^s)$ is $|\ell^{r-s}|_\ell^{1/2}=\ell^{(s-r)/2}$. The subgroup $T\cap K$ consists of diagonal matrices with unit entries. Each nonzero diagonal entry $a$ is $\ell^{\nu(a)}$ times a unit, so the quotient $T/(T\cap K)$ has coordinates $(r,s)\in\mathbb Z^2$ and group-algebra monomial $X^rY^s$. By the uniformizer identification in [F6], the cocharacter $x\mapsto\operatorname{diag}(x^r,x^s)$ maps to this quotient class. This is a group-scheme homomorphism since the powers are Laurent monomials and preserve multiplication. Its value at $\ell$ is the diagonal representative with valuations $(r,s)$, because $\nu(\ell)=1$. Evaluation is bijective by Gross’s identification, so these cocharacters exhaust the lattice and have the same monomials in the group algebra. [F1, F4, F6, F9, F14, F15, F16, F19, step 1.1, step 3.2]

5.1 Fix any integer pair $(r,s)$ and its diagonal representative $t$ from step 4.1. Each $tn$ has diagonal valuations $(r,s)$, so a coset with a different pair has empty preimage under $n\mapsto tn$. If the pair of $xK$ is $(r,s)$, choose an upper-triangular representative of $xK$ with diagonal $(\ell^r\epsilon_1,\ell^s\epsilon_2)$, where $\epsilon_1,\epsilon_2$ are units in $O$. Right multiplication by $\operatorname{diag}(\epsilon_1^{-1},\epsilon_2^{-1})\in K$ yields a representative with diagonal $(\ell^r,\ell^s)$. It has the form $tn_0$ with $n_0\in N$, since left multiplication by $t^{-1}$ gives an upper unitriangular matrix. Thus $tn\in xK$ exactly when $n_0^{-1}n\in N\cap K$, making its preimage $n_0(N\cap K)$. The preimage is open in $N$ because the map $n\mapsto tn$ is continuous in the inherited topology and $xK$ is open in $G$ by the translation property in [F7]. By [F10] the open preimage is Borel and therefore measurable for the Haar measure on $N$. Its measure is one by left invariance and the normalization in [F6]. [F1, F6, F7, F10, step 4.1]

6.1 The function $n\mapsto f(tn)$ is constant with value $f(x)$ on the preimage of each $xK$. These preimages are disjoint, and only finitely many from cosets where $f(x)\ne0$ can contribute. A nonzero level set for $f(tn)$ is the disjoint union of the contributing preimages with its level value. Each preimage is measurable and has measure one by step 5.1. By [F8] each nonzero level set has finite measure, equal to the number of its contributing preimages. The zero level set is the complement of the union of the nonzero level sets and is measurable as well. Thus the integrand is an integrable complex simple function. Its integral is therefore the sum of $f(x)$ over the contributing cosets with pair $(r,s)$. Multiplication by $\ell^{(s-r)/2}$ gives the coefficient of $X^rY^s$ in [F4]. This agrees with Gross’s coefficient formula on each integral input and at every pair. [F3, F4, F6, F8, step 4.1, step 5.1]

7.1 Each $f\in\mathcal H(G,K)$ is locally constant because it is constant on the open cosets $xK$. It is constant on double cosets and is nonzero on only finitely many of them because only finitely many cosets $xK$ contribute. The indicators of double cosets therefore span the complex algebra and are linearly independent by disjointness. By [F17], sending each integral basis indicator to the same function identifies $\mathbb C\otimes_{\mathbb Z}\mathcal H_{\mathbb Z}$ with $\mathcal H(G,K)$ as complex vector spaces. For convolution at $z\in G$, the integrand $f(x)h(x^{-1}z)$ is constant on each $xK$ by right invariance of $f$ and left invariance of $h$. Every such coset has Haar measure one, so Gross’s convolution on integral inputs gives exactly the coset-sum product in [F3]. Extending by complex bilinearity matches multiplication, and the indicator of $K$ is the unit of both algebras. With this identification, the coefficient agreement in step 6.1 extends from the integral basis to all complex inputs. [F1, F3, F6, F7, F17, step 6.1]

8.1 Use the normalizer quotient of [F6] and the criterion in [F16]. For any field extension $E/F$, including $F$, write $T_E=\mathbf T(E)$. An $E$-point $g=(g_{ij})$ of the algebraic normalizer preserves the base-changed torus over every commutative $E$-algebra, so in particular $gT_Eg^{-1}=T_E$. Then $D=\operatorname{diag}(1,\ell)$ lies in $T_E$ and its conjugate $gDg^{-1}$ is diagonal, say $\operatorname{diag}(b_1,b_2)$. The equation $gD=(gDg^{-1})g$ gives $(\lambda_j-b_i)g_{ij}=0$ by [F11], where $\lambda_1=1$ and $\lambda_2=\ell$. Because $1\ne\ell$ in $E$, each row has at most one nonzero entry. Invertibility forces exactly one nonzero entry per row, with the two entries in distinct columns. Thus $g$ is diagonal or a diagonal matrix times $w=\begin{pmatrix}0&1\\1&0\end{pmatrix}$. Each of these two matrix forms normalizes the diagonal torus over every commutative $E$-algebra, since diagonal matrices commute and $w$ interchanges the two entries. The two cosets modulo $T_E$ are distinct. Milne’s identification of the split Weyl quotient with the permutation matrices gives exactly these two geometric classes, both represented over $F$. Conjugation by $w$ swaps the diagonal entries and acts by $(r,s)\mapsto(s,r)$ on the torus quotient. Under Gross’s uniformizer identification in step 4.1, conjugation by $w$ sends the cocharacter $x\mapsto\operatorname{diag}(x^r,x^s)$ to $x\mapsto\operatorname{diag}(x^s,x^r)$. Hence the same swap acts on Gross’s cocharacter group algebra. Its invariants consist of Laurent polynomials with coefficients constant on the swap orbits. The orbit sums are a basis over the integral coefficient ring and over $\mathbb C$. Extending the coefficient ring $\mathbb Z[\sqrt{\ell},1/\sqrt{\ell}]$ to $\mathbb C$ therefore gives the symmetric Laurent algebra by [F17]. Scalar extension preserves Gross’s isomorphism and its inverse, and step 7.1 identifies the resulting transform with $S$. [F1, F4, F6, F9, F11, F16, F17, step 4.1, step 7.1]

9.1 Transfer $\lambda$ through $S$ to the unital character $\eta=\lambda\circ S^{-1}$ of the symmetric Laurent polynomials. This algebra is generated by $X+Y$, $XY$ and $(XY)^{-1}$, because multiplying any symmetric Laurent polynomial by a sufficiently high power of $XY$ gives a symmetric polynomial, to which [F5] applies. Set $a=\eta(X+Y)$ and $b=\eta(XY)$. The value $b$ is nonzero because $XY$ is invertible. The polynomial $t^2-at+b$ has a complex root $u$, which is nonzero since $b\ne0$. Put $v=b/u$. The root equation gives $u+v=a$, so $t^2-at+b=(t-u)(t-v)$. Evaluation at $(u,v)$ agrees with $\eta$ on the three generators and hence everywhere. Any pair giving the scalars for every $f$ must give $a$ and $b$ upon evaluation of $X+Y$ and $XY$, since $S$ is surjective onto the symmetric Laurent algebra. Its entries are therefore the roots of $t^2-at+b$ counted with multiplicity. [F5, step 3.1, step 8.1]

10.1 In the function model, the Hecke operator preserves the fixed line. Its scalar is its value on $\Phi_{u,v}$ evaluated at the identity, since $\Phi_{u,v}(1)=1$. Right translation and the coset action give $\sum_{xK}f(x)\Phi_{u,v}(x)$ for that scalar. Substituting the triangular values gives precisely $S(f)(u,v)$. This also gives the stated triangular value and identifies the same Hecke character for either ordering. [F3, F4, step 9.1]

10.2 Put $z=\ell I$. Centrality gives $k_1zk k_2=z k_1k k_2$ for $k,k_1,k_2\in K$, so the indicator of $zK$ is invariant on both sides by $K$. The set $zK$ is compact as the image of the compact subgroup $K$ by the continuous translation $k\mapsto zk$. The indicator is zero outside that compact coset, so it belongs to the spherical Hecke algebra. Its transform is $XY$ because there is one coset, of diagonal valuations $(1,1)$, and its action on $V^K$ is $\pi(z)$ by the coset sum. If the central character is trivial this operator is the identity, giving $uv=1$. [F1, F3, F4, F7, step 9.1]

11.1 Under this triviality, the lifts of a projective element act by the same operator on $V$, so $\bar\pi([g])=\pi(g)$ is a well-defined representation with $\bar K$-fixed space $V^K$. Write $q(g)=[g]$ and $\bar K=q(K)$. Each orbit map of $\bar\pi$ on $V$ is continuous for the induced norm topology since its composite with $q$ is the continuous orbit map of $\pi$ and $q$ has the quotient topology. For an open subgroup $U$ fixing a vector, $q(U)$ fixes it, and $q^{-1}(q(U))$ is the union of the scalar translates of $U$. Each translate is open by the homeomorphism assertion in [F7], so the quotient-topology criterion in [F7] makes $q(U)$ open. Thus the descended representation is smooth. [F1, F2, F7, step 10.2]

12.1 For any projective spherical Hecke function, each coset of $\bar K$ acts in its finite sum via any one lift, with the same operator on $V^K$ for all lifts and representatives because scalar matrices act trivially and $K$ fixes those vectors. For $f\in\mathcal H(G,K)$, sum the finitely many nonzero values $f(x)$ in each fiber of $xK\mapsto q(x)\bar K$ to define a function $\bar f$ on the projective cosets. Left multiplication by $K$ permutes the corresponding fibers and preserves $f$, so $\bar f$ is invariant on both sides by $\bar K$. Take a compact set $C\subseteq G$ outside which $f$ is zero. If $\bar f(\bar g)\ne0$, some coset $xK$ with $q(x)\bar K=\bar g\bar K$ has $f(x)\ne0$. There is then $k\in K$ with $q(xk)=\bar g$. Right $K$-invariance gives $f(xk)=f(x)\ne0$, so $xk\in C$ and $\bar g\in q(C)$. Thus $\bar f$ is zero outside the compact set $q(C)$, which is compact by continuity of the quotient map and [F7]. Grouping the formula for $T_f$ by these fibers gives $T_f=T_{\bar f}$ on the identified fixed spaces. This gives the descended action with the same volume-one convention. [F1, F3, F7, step 11.1] ∎
