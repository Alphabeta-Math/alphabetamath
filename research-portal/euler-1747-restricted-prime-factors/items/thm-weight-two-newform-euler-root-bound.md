---
id: thm-weight-two-newform-euler-root-bound
kind: theorem
title: Ramanujan–Petersson for weight-two Euler roots
status: draft
domain: mathematics
deps:
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:thm-compact-subset-of-a-hausdorff-space-is-closed
  - math:prop-measure-monotonicity
  - math:cor-p-adic-field-is-locally-compact-and-totally-disconnected
  - math:lem-geometric-sequence-null
  - math:lem-coset-partition
  - math:thm-closed-subspace-of-a-compact-space-is-compact
  - math:def-topological-space
  - math:def-order-topology-on-a-linearly-ordered-set
  - math:thm-p-adic-completion-is-a-field
  - math:thm-finite-and-countable-subadditivity-of-measures
  - math:def-borel-sigma-algebra
  - math:thm-generating-family-criterion-for-measurable-functions
  - math:thm-nonnegative-integral-zero-iff-zero-almost-everywhere
  - math:thm-unit-group-chinese-remainder-decomposition
  - math:thm-fundamental-theorem-of-arithmetic
  - def-author-24fda87362bc-local-adic-valuation
  - math:lem-p-adic-valuation-on-q
  - math:cor-cauchy-reals-lub-complete
  - math:def-countable-choice
  - def-author-e2fc0f4318ab-weight-two-cusp-form
  - def-author-e2fc0f4318ab-normalized-weight-two-newform
  - math:def-prime
  - math:def-dirichlet-character-modulo-q
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:thm-of-square-roots
  - lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars
  - thm-normalized-degree-two-spherical-character
  - math:def-strongly-continuous-unitary-representation
  - lem-author-e2fc0f4318ab-classical-hecke-first-coefficient
  - lem-author-e2fc0f4318ab-spherical-trace-and-product
  - math:lem-complex-conjugation-and-modulus-laws
  - def-degree-two-projective-linear-group
  - def-author-34e2e6a0519f-split-adelic-matrix-groups
  - lem-author-d45da46285be-triangular-cosets
  - def-author-d45da46285be-satake-transform
  - def-author-d45da46285be-spherical-hecke-algebra
  - lem-author-c3a9b9243c74-fixed-space-of-tensor-factor
  - math:def-radon-measure-on-an-lch-space
  - math:def-quotient-topology
  - math:lem-nrqm-composites-hilbert-tensor-construction
  - math:thm-extension-of-a-bounded-map-from-a-dense-subspace
  - def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles
  - math:thm-determinant-multiplicative
  - math:lem-dirichlet-character-values
formulation_deps:
  - math:thm-unit-group-chinese-remainder-decomposition
  - math:thm-fundamental-theorem-of-arithmetic
  - def-author-24fda87362bc-local-adic-valuation
  - math:def-radon-measure-on-an-lch-space
  - math:def-countable-choice
  - def-author-e2fc0f4318ab-weight-two-cusp-form
  - def-author-e2fc0f4318ab-normalized-weight-two-newform
  - math:def-prime
  - math:def-dirichlet-character-modulo-q
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:thm-of-square-roots
  - lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars
  - thm-normalized-degree-two-spherical-character
  - math:def-strongly-continuous-unitary-representation
  - def-degree-two-projective-linear-group
  - def-author-34e2e6a0519f-split-adelic-matrix-groups
  - lem-author-d45da46285be-triangular-cosets
  - def-author-d45da46285be-satake-transform
  - math:def-quotient-topology
  - def-author-d45da46285be-spherical-hecke-algebra
argument_deps:
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:thm-compact-subset-of-a-hausdorff-space-is-closed
  - math:prop-measure-monotonicity
  - math:cor-p-adic-field-is-locally-compact-and-totally-disconnected
  - math:lem-geometric-sequence-null
  - math:lem-coset-partition
  - math:thm-closed-subspace-of-a-compact-space-is-compact
  - math:def-topological-space
  - math:def-order-topology-on-a-linearly-ordered-set
  - math:thm-p-adic-completion-is-a-field
  - math:thm-finite-and-countable-subadditivity-of-measures
  - math:def-borel-sigma-algebra
  - math:thm-generating-family-criterion-for-measurable-functions
  - math:thm-nonnegative-integral-zero-iff-zero-almost-everywhere
  - math:thm-unit-group-chinese-remainder-decomposition
  - math:thm-fundamental-theorem-of-arithmetic
  - def-author-24fda87362bc-local-adic-valuation
  - math:lem-p-adic-valuation-on-q
  - math:cor-cauchy-reals-lub-complete
  - lem-author-e2fc0f4318ab-classical-hecke-first-coefficient
  - lem-author-e2fc0f4318ab-spherical-trace-and-product
  - math:lem-complex-conjugation-and-modulus-laws
  - math:def-countable-choice
  - def-author-e2fc0f4318ab-weight-two-cusp-form
  - def-author-e2fc0f4318ab-normalized-weight-two-newform
  - math:def-prime
  - math:def-dirichlet-character-modulo-q
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:thm-of-square-roots
  - lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars
  - thm-normalized-degree-two-spherical-character
  - math:def-strongly-continuous-unitary-representation
  - def-degree-two-projective-linear-group
  - def-author-34e2e6a0519f-split-adelic-matrix-groups
  - lem-author-d45da46285be-triangular-cosets
  - def-author-d45da46285be-satake-transform
  - def-author-d45da46285be-spherical-hecke-algebra
  - lem-author-c3a9b9243c74-fixed-space-of-tensor-factor
  - math:def-radon-measure-on-an-lch-space
  - math:def-quotient-topology
  - math:lem-nrqm-composites-hilbert-tensor-construction
  - math:thm-extension-of-a-bounded-map-from-a-dense-subspace
  - def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles
  - math:thm-determinant-multiplicative
  - math:lem-dirichlet-character-values
dependency_roles:
  math:lem-compactness-of-a-subspace-is-ambient: mathematical-premise
  math:thm-compact-subset-of-a-hausdorff-space-is-closed: mathematical-premise
  math:prop-measure-monotonicity: mathematical-premise
  math:cor-p-adic-field-is-locally-compact-and-totally-disconnected: mathematical-premise
  math:lem-geometric-sequence-null: mathematical-premise
  math:lem-coset-partition: mathematical-premise
  math:thm-closed-subspace-of-a-compact-space-is-compact: mathematical-premise
  math:def-topological-space: mathematical-premise
  math:def-order-topology-on-a-linearly-ordered-set: mathematical-premise
  math:thm-p-adic-completion-is-a-field: mathematical-premise
  math:thm-finite-and-countable-subadditivity-of-measures: mathematical-premise
  math:def-borel-sigma-algebra: mathematical-premise
  math:thm-generating-family-criterion-for-measurable-functions: mathematical-premise
  math:thm-nonnegative-integral-zero-iff-zero-almost-everywhere: mathematical-premise
  math:thm-unit-group-chinese-remainder-decomposition: mathematical-premise
  math:thm-fundamental-theorem-of-arithmetic: mathematical-premise
  def-author-24fda87362bc-local-adic-valuation: mathematical-premise
  math:lem-p-adic-valuation-on-q: mathematical-premise
  math:cor-cauchy-reals-lub-complete: mathematical-premise
  math:def-countable-choice: mathematical-premise
  def-author-e2fc0f4318ab-weight-two-cusp-form: mathematical-premise
  def-author-e2fc0f4318ab-normalized-weight-two-newform: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-dirichlet-character-modulo-q: mathematical-premise
  math:def-complex-conjugate-real-imaginary-part-and-modulus: mathematical-premise
  math:thm-of-square-roots: mathematical-premise
  lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars: mathematical-premise
  thm-normalized-degree-two-spherical-character: mathematical-premise
  math:def-strongly-continuous-unitary-representation: mathematical-premise
  lem-author-e2fc0f4318ab-classical-hecke-first-coefficient: mathematical-premise
  lem-author-e2fc0f4318ab-spherical-trace-and-product: mathematical-premise
  math:lem-complex-conjugation-and-modulus-laws: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  def-author-34e2e6a0519f-split-adelic-matrix-groups: mathematical-premise
  lem-author-d45da46285be-triangular-cosets: mathematical-premise
  def-author-d45da46285be-satake-transform: mathematical-premise
  def-author-d45da46285be-spherical-hecke-algebra: mathematical-premise
  lem-author-c3a9b9243c74-fixed-space-of-tensor-factor: mathematical-premise
  math:def-radon-measure-on-an-lch-space: mathematical-premise
  math:def-quotient-topology: mathematical-premise
  math:lem-nrqm-composites-hilbert-tensor-construction: mathematical-premise
  math:thm-extension-of-a-bounded-map-from-a-dense-subspace: mathematical-premise
  def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles: mathematical-premise
  math:thm-determinant-multiplicative: mathematical-premise
  math:lem-dirichlet-character-values: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: "La conjecture de Weil : I"
      url: https://www.numdam.org/item/PMIHES_1974__43__273_0.pdf#page=31
      locator: Pierre Deligne, §8, Théorème (8.2), printed p. 302
      statement: For a normalized primitive holomorphic cusp form of integral weight k
        at least two, the two roots of X^2−a_p X+ε(p)p^(k−1) at a prime p not
        dividing the level each have absolute value p^((k−1)/2).
      hypotheses: Level N at least one, a Dirichlet character ε modulo N, a cusp form
        new at level N with first Fourier coefficient one, and a prime p not
        dividing N. The modular transformation factor ε(a)^−1 equals ε(d) for a
        determinant-one matrix in Γ_0(N).
      reading_limits: Checked the printed theorem statement, including the
        top-left-entry character convention, primitive-form condition,
        polynomial and modulus of both roots. The proof from purity is imported.
    - title: Eigenspaces of Newforms with Nontrivial Character
      url: https://arxiv.org/pdf/2307.07804#page=12
      locator: M. Karameris, arXiv:2307.07804v7, §3 opening, p. 12
      statement: Every element of GL₂(A) is a product of a diagonal rational matrix,
        an inserted real matrix of positive determinant and an element of K₀(N).
      hypotheses: Rational adeles and a positive integral level N. The local factors
        of K₀(N) are the full integral matrix groups away from N and the
        subgroups with lower left entry divisible by the local level at primes
        dividing N.
      reading_limits: Checked the displayed strong approximation formula and local
        level subgroups in v7. Strong approximation is imported.
    - title: Modular Forms and Automorphic Representations
      url: https://math.stanford.edu/~conrad/conversesem/refs/trotabas.pdf#page=15
      locator: D. Trotabas, §§1 and 2.1, pp. 1–2 (classical character), §5.1
        Definition 5.1 and lift properties, pp. 15–17, §5.2 Definition 5.2, p.
        17, Appendix §§8.1–8.2, pp. 25–27, and §§6.1–6.2 and Theorem 6.1, pp.
        19–21
      statement: The classical transformation factor on Γ₀(N) is χ(a) for upper left
        entry a after extracting the weight factor. The adelization of a
        classical holomorphic cusp form is continuous, has central covariance by
        a finite-order idele class character and lies in the corresponding
        cuspidal space with norm squared given by integrating the absolute
        square on the quotient by the rational group and center. It has the
        normalized real restriction and its finite right K₀(N) covariance is
        through the lower right unit class. Its unitary representation is the
        closed span of right translates. An irreducible unitary representation
        of GL₂(A) is a restricted Hilbert tensor product of irreducible local
        unitary representations, built with spherical unit reference vectors
        outside a finite set. Local inserted elements act on their own factors.
      hypotheses: The lift uses a classical holomorphic cuspidal modular form of
        integral weight and Dirichlet nebentypus χ modulo N evaluated on the
        upper left entry of Γ₀(N). The application takes χ to be ε⁻¹ on unit
        classes. The tensor product theorem assumes a strongly continuous
        irreducible unitary representation of GL₂ over the rational adeles.
      reading_limits: Checked the classical character in §§1 and 2.1, the
        determinant-normalized formula in Definition 5.1 and its continuity,
        central covariance and cuspidal Hilbert realization, as well as the
        tensor construction and factorization statement. Their proofs are
        imported. The finite character calculation, regrouping of the tensor
        factors and passage to pointwise equality are argued locally.
    - title: Average Values of Modular L-Series via the Relative Trace Formula
      url: https://arxiv.org/pdf/math/0510113#page=24
      locator: D. Ramakrishnan and J. Rogawski, §4, printed p. 724, paragraph defining
        the adelic scalar product
      statement: For GL₂ over the rational adeles, the adelic scalar product uses the
        measure on Z(A)GL₂(Q)\GL₂(A) induced by Haar measure, normalized to give
        the quotient mass one.
      hypotheses: The group is GL₂ over the rational adeles and Z is its scalar
        center. The authors use the scalar product there for trivial central
        character. The quotient Haar measure itself depends on the groups, and
        the absolute square descends for any unitary central character.
      reading_limits: Checked the scalar-product and quotient-measure normalization.
        Use the quotient Haar measure as a nonzero invariant Radon measure. Full
        support is proved locally.
    - title: On the order of vanishing of newforms at cusps
      url: https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf#page=17
      locator: A. Corbett and A. Saha, §2.1.4, equation (8), p. 8, and §3.1, equations
        (20)–(22) and the paragraph following (22), pp. 16–17
      statement: A holomorphic classical newform of weight k, level N and character χ
        adelizes to a K₁(N)-invariant adelic newform in an irreducible unitary
        cuspidal representation of GL₂(A). On positive-determinant real matrices
        the lift is det(h)^(k/2)(ci+d)^(-k)f(hi). Their K₁(N) is the product of
        local subgroups with lower left entry zero and upper left entry one
        modulo the local level, and the full integral matrix group at primes
        away from N.
      hypotheses: A holomorphic classical newform over Q of integral weight k ≥ 2,
        level N and Dirichlet character χ. The unitary correspondence uses a
        central character trivial on positive real scalars and holomorphic
        discrete series at the real place.
      reading_limits: Checked the definition of K₁(N), equations (20)–(22) and the
        converse adelization of a classical newform. The correspondence is
        imported. The determinant twist from the upper-left congruence
        convention to the lower-right covariance is derived locally.
    - title: Automorphic Representations and L-functions for GL(n)
      url: https://www.math.columbia.edu/~goldfeld/LanglandsBookChapter.pdf#page=3
      locator: D. Goldfeld and H. Jacquet, §2.1 (Smooth representations), pp. 2–3,
        paragraph beginning “If π is a unitary (topologically) irreducible
        representation”
      statement: For a topologically irreducible unitary Hilbert-space representation
        of GL(n,F), the vectors fixed by some compact open subgroup form an
        invariant subspace on which the restricted action is algebraically
        irreducible and admissible. Admissibility means finite-dimensional fixed
        spaces for all compact open subgroups.
      hypotheses: F is a nonarchimedean local field and the given representation of
        GL(n,F) is unitary and topologically irreducible on a complex Hilbert
        space. Here F is Q_ℓ, n is 2 and the representation is the local factor
        of the restricted Hilbert tensor product.
      reading_limits: Checked the smoothness convention, admissibility definition and
        Hilbert-to-smooth irreducibility statement in §2.1. The result is
        imported. Equivalence with the open-subgroup convention is checked
        locally.
dependency_level: 5
---

## Statement

Assume countable choice, meaning a sequence of nonempty sets has a choice function. Let $f$ be a normalized primitive holomorphic cusp form of weight two, level $N$ and Dirichlet character $\epsilon$. This means that $f$ is new at level $N$, is a simultaneous eigenfunction of the classical Hecke operators and has first Fourier coefficient one. For a prime $\ell\nmid N$ let $a_\ell$ be its classical Hecke eigenvalue at $\ell$. Then each root of the Hecke polynomial
$$P_\ell(X)=X^2-a_\ell X+\ell\epsilon(\ell)$$
has complex absolute value $\sqrt\ell$, the positive square root of $\ell$.

Write $L=\mathrm{GL}_2(\mathbb A)$ for the general linear group over the rational adeles, with its restricted-product topology, and $Z$ for its scalar subgroup. The continuous adelization $\Phi_f:L\to\mathbb C$ is uniquely determined by left invariance under the diagonally embedded $\mathrm{GL}_2(\mathbb Q)$, the finite right covariance $\Phi_f(gk)=\epsilon(d(k))^{-1}\Phi_f(g)$ for $g\in L$ and $k\in K_0(N)$, and the real restriction $\Phi_f(h_\infty)=(f|_2h)(i)$ for positive-determinant real $h$, inserted at the real place with identity at every finite place. Here $K_0(N)$ is the subgroup of finite tuples $k=(k_p)_p$ in $\prod_p\mathrm{GL}_2(\mathbb Z_p)$ with lower left entry in $N\mathbb Z_p$ at every $p$, embedded with real component the identity. For each maximal prime power $p^{e_p}$ dividing $N$, reduce the lower right entry of $k_p$ modulo $p^{e_p}$. The Chinese remainder map combines these residues into the unit class $d(k)$ modulo $N$. At $N=1$ this is the sole unit class.

The closed span of right translates of $\Phi_f$ in the cuspidal $L^2$ space with its unitary central character gives the irreducible unitary adelic representation of $f$. In this model the squared norm integrates the absolute square on $Z\mathrm{GL}_2(\mathbb Q)\backslash L$ with its quotient topology and a nonzero right-$L$-invariant Radon measure. Let $\pi_\ell$ be the factor at $G_\ell=\mathrm{GL}_2(\mathbb Q_\ell)$, where $\mathbb Q_\ell$ is the $\ell$-adic field. It is unramified, meaning it has a nonzero vector fixed by the compact open subgroup $K=\mathrm{GL}_2(\mathbb Z_\ell)$, where $\mathbb Z_\ell$ is the local integer ring. The two roots of $P_\ell$, divided by $\sqrt\ell$, are its unit-normalized Satake parameters. These are the unordered pair of nonzero complex numbers, counted with multiplicity, giving the scalar of each spherical Hecke operator on the $K$-fixed line by evaluation of its normalized Satake transform. In particular each parameter has absolute value one.

## Statement references

[[def-author-e2fc0f4318ab-normalized-weight-two-newform|Classical normalized newform]]

[[lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars|Weight-two adelic conventions]]

[[thm-normalized-degree-two-spherical-character|Normalized spherical character and Satake parameters]]

[[def-author-34e2e6a0519f-split-adelic-matrix-groups|Adelic matrix group and its topology]]

[[def-degree-two-projective-linear-group|General linear groups of degree two]]

[[lem-author-d45da46285be-triangular-cosets|Local field, integral subgroup and topology]]

[[def-author-d45da46285be-satake-transform|Normalized Satake transform]]

[[def-author-d45da46285be-spherical-hecke-algebra|Spherical Hecke operators]]

[[math:def-quotient-topology|Quotient topology]]

[[math:def-radon-measure-on-an-lch-space|Radon measure]]

[[math:thm-fundamental-theorem-of-arithmetic|Prime powers of the level]]

[[def-author-24fda87362bc-local-adic-valuation|Local integer rings and their residue classes]]

[[math:thm-unit-group-chinese-remainder-decomposition|Chinese remainder isomorphism on units]]

## Facts & Assumptions

[F1] The Fourier coefficient indexed by $\ell$ equals the classical $T_\ell$ eigenvalue, since $f$ has first Fourier coefficient one and $\ell\nmid N$ ([[def-author-e2fc0f4318ab-weight-two-cusp-form]], [[def-author-e2fc0f4318ab-normalized-weight-two-newform]], [[lem-author-e2fc0f4318ab-classical-hecke-first-coefficient]]).

[F2] Each of the two spherical Hecke operators is a finite sum of translates, one per contributing coset $xK$. Evaluation of the normalized Satake transform at the pair $(u,v)$ gives the scalar on the fixed line. For the two operators $\mathcal T_\ell$ and $\mathcal R_\ell$ of the trace and product calculation these scalars are $\sqrt\ell(u+v)$ and $uv$ on an irreducible admissible smooth local representation with a nonzero $K$-fixed space and unitary realization. In the spherical-character theorem, a vector is smooth if it is fixed by an open subgroup. On the weight-two adelization, once these operators act by scalars, those scalars are $a_\ell$ and $\epsilon(\ell)$, respectively ([[def-author-d45da46285be-spherical-hecke-algebra]], [[def-author-d45da46285be-satake-transform]], [[thm-normalized-degree-two-spherical-character]], [[lem-author-e2fc0f4318ab-spherical-trace-and-product]], [[lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars]]).

[F3] Complex absolute value is multiplicative and agrees with the usual positive real value on positive reals. Complex absolute value also satisfies the triangle inequality and is unchanged by negation. The positive square root of $\ell$ exists and is nonzero since the real numbers form a complete ordered field and $\ell>0$ ([[math:def-complex-conjugate-real-imaginary-part-and-modulus]], [[math:lem-complex-conjugation-and-modulus-laws]], [[math:thm-of-square-roots]], [[math:cor-cauchy-reals-lub-complete]], [[math:def-prime]]).

[F4] Use the adelization and representation results below for strong approximation, the continuous lift, the cuspidal Hilbert space, the quotient Haar measure, the newform correspondence, the restricted tensor product and the local smooth representation.

[F5] Deligne’s theorem gives the absolute values of both roots in the stated classical normalization.

[F6] The local matrix group and integral subgroup use the entry topologies, and $K$ is compact and open. For every finite prime $p$, the ring $\mathbb Z_p$ is open in $\mathbb Q_p$. The adelic group uses coordinatewise multiplication and the restricted-product topology. Each place embeds by inserting the identity at every other place ([[def-degree-two-projective-linear-group]], [[lem-author-d45da46285be-triangular-cosets]], [[def-author-34e2e6a0519f-split-adelic-matrix-groups]]). The adelic and local matrix groups are topological groups, so left and right translations by fixed elements are homeomorphisms ([[def-author-34e2e6a0519f-split-adelic-matrix-groups]]).

[F7] In the quotient topology a set is open if its preimage is open. A nonzero Radon measure is inner regular on open sets, so the whole space contains a compact subset of positive measure ([[math:def-quotient-topology]], [[math:def-radon-measure-on-an-lch-space]]). Measures are finitely subadditive. A nonnegative measurable function of zero integral vanishes almost everywhere ([[math:thm-finite-and-countable-subadditivity-of-measures]], [[math:thm-nonnegative-integral-zero-iff-zero-almost-everywhere]]). The open sets generate the Borel sigma-algebra of a topological space. A map is measurable if the preimage of each set in a generating family for the target sigma-algebra is measurable. [[math:def-borel-sigma-algebra]] [[math:thm-generating-family-criterion-for-measurable-functions]] The open rays of a linear order generate its order topology ([[math:def-order-topology-on-a-linearly-ordered-set]]). A cover of a compact subset by ambient open sets has a finite subcover. [[math:lem-compactness-of-a-subspace-is-ambient]] A compact subset of a Hausdorff space is closed and hence Borel. [[math:thm-compact-subset-of-a-hausdorff-space-is-closed]] [[math:def-borel-sigma-algebra]] A measure is monotone under inclusion of measurable sets. [[math:prop-measure-monotonicity]]

[F8] The Hilbert tensor product completes the span of elementary tensors with the product pairing. Under countable choice a bounded linear map on a dense linear subspace extends to the completion when the target is complete. For the action of a group on the first tensor factor, the fixed space is the tensor product of the first factor's fixed space with the second factor. A scalar action by a finite linear combination of group operators on the local fixed space gives the same scalar on the tensor fixed space ([[math:lem-nrqm-composites-hilbert-tensor-construction]], [[math:thm-extension-of-a-bounded-map-from-a-dense-subspace]], [[lem-author-c3a9b9243c74-fixed-space-of-tensor-factor]]).

[F9] The group $K_0(N)$ is defined by the lower left entry condition at the finite places. The maps $a(k),d(k)$ take the upper left and lower right unit classes modulo $N$ by combining local reductions at the maximal prime powers of $N$. Prime factorization makes these moduli pairwise coprime, and the Chinese remainder isomorphism on unit groups applies, including the empty list for $N=1$. These classes multiply under products, since the reductions are upper triangular. The finite part of a rational matrix in $\Gamma_0(N)$ gives its ordinary residue classes. The weight-two slash action composes in the order of matrix multiplication. Dirichlet character values on units have modulus one, and $\epsilon(-1)=1$ by the weight-two transformation at $-I$. [[lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars]] [[def-author-e2fc0f4318ab-weight-two-cusp-form]] [[math:def-dirichlet-character-modulo-q]] [[math:lem-dirichlet-character-values]] [[def-author-24fda87362bc-local-adic-valuation]] [[math:thm-fundamental-theorem-of-arithmetic]] [[math:thm-unit-group-chinese-remainder-decomposition]]

[F10] An idele is a tuple of nonzero local scalars that are units at all but finitely many finite places. The valuation $v_p$ is additive under multiplication, with $v_p(p)=1$ and $v_p(q)=0$ for any other prime $q$. On a nonzero rational $m/n$ it is the difference of the integer valuations of $m$ and $n$. Determinant is multiplicative, and the determinant of an adelic invertible matrix is an idele. [[def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles]] [[lem-author-d45da46285be-triangular-cosets]] [[math:thm-determinant-multiplicative]] [[def-author-24fda87362bc-local-adic-valuation]] [[math:lem-p-adic-valuation-on-q]] The absolute value on the completion $\mathbb Q_p$ is nonarchimedean ([[math:thm-p-adic-completion-is-a-field]]). Under countable choice $\mathbb Q_p$ is locally compact in its $p$-adic topology. [[math:cor-p-adic-field-is-locally-compact-and-totally-disconnected]] For a real $r$ with $|r|<1$, the powers $r^n$ converge to zero. [[math:lem-geometric-sequence-null]]

[F11] The entrywise formula $ad-bc$ for the determinant is continuous on each local matrix group because field addition, negation and multiplication are continuous. The entry-topology argument is in step 1.2 of the split group construction [[def-author-34e2e6a0519f-split-adelic-matrix-groups]]. A unitary representation is a homomorphism into the bijective complex-linear isometries of a complex Hilbert space with norm-continuous vector orbits [[math:def-strongly-continuous-unitary-representation]].

[F12] The distinct left cosets of a subgroup partition its ambient group. [[math:lem-coset-partition]] An arbitrary union of open sets is open. [[math:def-topological-space]] A closed subspace of a compact space is compact. [[math:thm-closed-subspace-of-a-compact-space-is-compact]]

## External input

Strong approximation expresses each element of $L$ as $q h_\infty k$ with $q\in\mathrm{GL}_2(\mathbb Q)$, $h\in\mathrm{GL}_2^+(\mathbb R)$ and $k\in K_0(N)$. [Eigenspaces of Newforms with Nontrivial Character](https://arxiv.org/pdf/2307.07804#page=12)

Trotabas evaluates his classical nebentypus $\chi$ on the upper left entry of a matrix in $\Gamma_0(N)$. His Definition 5.1 gives a left rational invariant lift with value $\det(h)^{k/2}(ci+d)^{-k}f(hi)$ at $h_\infty$ in weight $k$, and finite right covariance through $d(k)$. It is continuous and transforms under the center by a unitary character. The cuspidal $L^2$ model uses the squared norm in the statement and realizes the action by right translation. An irreducible unitary representation of $L$ is a restricted Hilbert tensor product of irreducible local unitary representations. It is built by enlarging finite tensor products with the specified unit reference vectors. An element inserted at one place acts on the factor there. [Modular Forms and Automorphic Representations](https://math.stanford.edu/~conrad/conversesem/refs/trotabas.pdf#page=15)

The $L^2$ integral uses the quotient of Haar measure on $Z\mathrm{GL}_2(\mathbb Q)\backslash L$, a nonzero right-invariant Radon measure. Its scale is immaterial to the norm-zero condition. [Average Values of Modular L-Series via the Relative Trace Formula](https://arxiv.org/pdf/math/0510113#page=24)

The adelic lift of a classical holomorphic newform lies in an irreducible unitary cuspidal representation. It has the real restriction in the statement and is fixed by Corbett and Saha’s $K_1(N)$, the subgroup of $K_0(N)$ with upper left entry congruent to one at each prime power in the level. [On the order of vanishing of newforms at cusps](https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf#page=17)

For a primitive normalized cusp form and a prime away from its level, Deligne's root theorem applies to the polynomial with linear coefficient given by the Fourier coefficient with a minus sign and constant coefficient $\epsilon(\ell)\ell^{k-1}$ in weight $k\ge2$. [La conjecture de Weil : I](https://www.numdam.org/item/PMIHES_1974__43__273_0.pdf#page=31)

For a topologically irreducible unitary Hilbert-space representation of $\mathrm{GL}_n(F)$ over a nonarchimedean local field $F$, the vectors fixed by some compact open subgroup form an invariant subspace with an algebraically irreducible admissible action. Admissibility means that the fixed space for each compact open subgroup is finite dimensional. [Automorphic Representations and L-functions for GL(n)](https://www.math.columbia.edu/~goldfeld/LanglandsBookChapter.pdf#page=3)

## Proof

**Given:** The normalized weight-two newform $f$, its character and level, and the prime $\ell\nmid N$.

**Goal:** Identify the two rescaled roots with the two Satake parameters and determine their absolute values.

1.1 Let $X=Z\mathrm{GL}_2(\mathbb Q)\backslash L$ with the quotient measure $\mu$ of [F4]. By [F6], right translation $R_x$ on $L$ is a homeomorphism. It descends to a map $\bar R_x$ on left cosets. For the quotient map $q:L\to X$ and any open $U\subset X$, the identity $q^{-1}(\bar R_x^{-1}(U))=R_x^{-1}(q^{-1}(U))$ gives continuity of $\bar R_x$ by [F7]. The same argument for $x^{-1}$ gives continuity of the inverse, so right translation on $X$ is a homeomorphism. Any nonempty open subset of $X$ has positive measure. Indeed its right translates are open and cover $X$ by transitivity. If the subset had measure zero, its translates would be null by right invariance. By [F7], finitely many of those ambient open translates cover the compact positive-measure subset $C$ from [F7]. Their union $B$ is open and hence Borel, and $C$ is Borel since the Radon measure is on a Hausdorff space. Finite subadditivity gives $\mu(B)=0$. As $C\subseteq B$, monotonicity gives $\mu(C)\le\mu(B)=0$, a contradiction. If a continuous function $D$ on $L$ is left rational invariant and has the unitary central covariance of $\Phi_f$, then $|D|^2$ is constant on the quotient fibers because the central character has modulus one. The triangle inequality and invariance under negation in [F3] give $\bigl||z|-|w|\bigr|\le |z-w|$ by writing $z=w+(z-w)$ and $w=z+(w-z)$. Factoring the difference of squares gives $\bigl||z|^2-|w|^2\bigr|\le (|z|+|w|)|z-w|$. For $|z-w|<1$ the factor $|z|+|w|$ is bounded by $2|w|+1$, proving continuity at each $w$. Thus $|D|^2$ is continuous and descends to a continuous function on $X$ with values in the usual real half-line by the quotient topology. Put $Y=[0,+\infty]$ with the order topology of [F7]. For a finite cut $a$, the two open rays in $Y$ restrict to $[0,a)$ and $(a,\infty)$ in the finite half-line. At the infinite cut the restrictions are the whole finite half-line and the empty set. These restrictions are relatively open and the rays generate the topology of $Y$. Every open set of $Y$ meets $[0,\infty)$ in a relatively open set, so the descended absolute square has open preimages for open sets of $Y$. These preimages belong to $\mathcal B(X)$, the sigma-algebra of the Radon measure. The open sets of $Y$ generate $\mathcal B(Y)$, so the generating-family criterion of [F7] applies to the descended absolute square as a map $(X,\mathcal B(X))\to(Y,\mathcal B(Y))$. If $D$ represents the zero $L^2$ class, the descended absolute square has integral zero. By [F7] it vanishes almost everywhere. Its positive set is open and null, so by full support it is empty. Thus $D$ vanishes everywhere. [F3, F4, F6, F7]

1.2 Since $a_1=1$, take $z=x+iy$ in the upper half-plane with $f(z)\ne0$. The real matrix $h=\begin{pmatrix}y&x\\0&1\end{pmatrix}$ has positive determinant, sends $i$ to $z$ and gives $(f|_2h)(i)\ne0$. For Trotabas's lift in [F4], take the Dirichlet character $\chi$ defined on units by $\chi(u)=\epsilon(u)^{-1}$ and extended by zero on nonunits. For every $\gamma\in\Gamma_0(N)$ with diagonal entries $a_\gamma,d_\gamma$, the determinant gives $a_\gamma d_\gamma\equiv 1\pmod N$. Thus $\chi(a_\gamma)=\epsilon(d_\gamma)$, so $f$ satisfies Trotabas's classical transformation law. For any unit class $d_0$ and integer representatives of it and its inverse $a_0$, the matrix $\gamma=\begin{pmatrix}a_0&(a_0d_0-1)/N\\N&d_0\end{pmatrix}$ belongs to $\Gamma_0(N)$. Its finite part $\gamma_f$ has lower right class $d_0$ and upper left class $a_0$. On this part, a left rational invariant lift with that real restriction satisfies $\Phi(h_\infty\gamma_f)=\Phi((\gamma^{-1}h)_\infty)=\epsilon(d_0)^{-1}(f|_2h)(i)$, by the slash composition and transformation laws. The lower right character of the continuous lift thus equals $\epsilon^{-1}$. Strong approximation makes left rational invariance, the real restriction and this covariance determine the lift uniquely: they give the value $\epsilon(d(k))^{-1}(f|_2 h)(i)$ at every $q h_\infty k$. The continuous lift supplied by Trotabas therefore gives the $\Phi_f$ in the statement. [F1, F4, F9, given]

2.1 Let $\Psi$ be Corbett and Saha’s adelic newform. For $k\in K_0(N)$, split off the finite scalar tuple whose component at each $p\mid N$ is the upper left entry of $k_p$ and is one elsewhere. The entries at $p\mid N$ are units. Dividing out this tuple leaves the lower left entries divisible by their local levels and makes the upper left entries one at $p\mid N$, so the quotient lies in Corbett and Saha’s $K_1(N)$ and fixes $\Psi$ by [F4]. Scalar unit tuples reducing to one at those prime powers belong to $K_1(N)$, so their central character is one. The central character therefore gives right covariance of $\Psi$ by a character $\xi(a(k))$ of the upper left residue class. Using $\gamma_f$ and the nonzero real restriction in step 1.2 gives $\xi(a_0)=\epsilon(d_0)^{-1}=\epsilon(a_0)$ for every unit class $a_0$. [F4, F9, step 1.2]

2.2 By steps 1.1 and 1.2 the class $[\Phi_f]$ is nonzero. Embed $G_\ell$ in $L$ by inserting the identity at every place other than $\ell$. This is a continuous homomorphism because multiplication is coordinatewise and the preimage of a basic restricted-product box is empty or its open $\ell$-component. Since $\ell\nmid N$, the embedded $K$ lies in $K_0(N)$ and has $d(k)=1$ modulo $N$. The finite right covariance fixes $\Phi_f$ under $K$ and therefore fixes its class. [F4, F6, F9, given, step 1.1, step 1.2]

3.1 For an idele $s$, put $r(s)=\prod_{p}p^{v_p(s_p)}\in\mathbb Q_{>0}$. This product has finitely many nontrivial factors, and $v_p(r(s))=v_p(s_p)$ by [F10], so $s_f/r(s)$ has finite unit components. Using the Chinese remainder isomorphism in [F9], define $\eta(s)=\epsilon((s_f/r(s))\bmod N)$ from the reductions of these units. Additivity of the valuations gives $r(st)=r(s)r(t)$, so multiplicativity of reduction and the unit character law make $\eta$ a unitary character. For $p\mid N$ write $e=e_p\ge1$. The projection to the $e$th coordinate of the compatible residue model in [F9] has kernel $p^e\mathbb Z_p$. Indeed, if $x_e=0$ for a compatible tuple $x=(x_n)_n$, then each $x_{n+e}$ is represented by a multiple of $p^e$. Dividing those representatives by $p^e$ gives well-defined classes modulo $p^n$, since changing a representative changes the quotient by a multiple of $p^n$. The resulting classes are compatible because reduction from modulus $p^{n+e+1}$ to $p^{n+e}$ becomes reduction from $p^{n+1}$ to $p^n$ after division. They define $y\in\mathbb Z_p$, and reduction of $x_{n+e}$ modulo $p^n$ gives $x_n$, so $x=p^e y$ in every coordinate. Conversely a multiple of $p^e$ projects to zero. Thus each fiber is a translate of $p^e\mathbb Z_p$. Multiplication by $p^e$ and translation are homeomorphisms of $\mathbb Q_p$ by continuity of field operations and their inverse maps, so the fibers are open by [F6]. At each nonunit finite place of $s$, the open ball of radius $|s_p|_p$ about $s_p$ fixes its valuation. If $|x-s_p|_p<|s_p|_p$, applying [F10] to $x=s_p+(x-s_p)$ gives $|x|_p\le |s_p|_p$. Applying it to $s_p=x+(s_p-x)$ gives $|s_p|_p\le \max(|x|_p,|x-s_p|_p)$, which forces $|x|_p\ge |s_p|_p$. Equality of absolute values gives $v_p(x)=v_p(s_p)$. In particular each unit has a radius-one ball of units, so the local unit group is open. Require units at all other finite places, which fixes $r(s)$. At each $p\mid N$, also restrict the entry divided by this fixed $r(s)$ to its residue fiber. These finitely many extra restrictions are open because scaling by $r(s)^{-1}$ is a homeomorphism. The resulting open box contains $s$ and $\eta$ is constant there. For a nonzero rational $m/n$ with $n>0$, factor $|m|$ and $n$ into primes by [F9]. Their exponents differ by $v_p(m/n)$ by [F10], so $r(m/n)=|m|/n$ for the diagonal idele. The finite quotient by $r(m/n)$ is the sign of $m/n$, and $\epsilon(-1)=1$. Thus $\eta$ is trivial on rational ideles and also on real insertions, where the finite tuple is the identity. The function $\eta(\det g)^{-1}\Psi(g)$ has left rational invariance and the same real restriction as $\Phi_f$. For $k\in K_0(N)$, its determinant has finite unit components and residue $a(k)d(k)$, so step 2.1 gives the twisted function finite right covariance by $\epsilon(d(k))^{-1}$. Strong approximation now identifies the twisted function with $\Phi_f$. Use the same quotient measure for both central characters. The map $M$ of multiplication by $\eta(\det g)^{-1}$ preserves the squared norm and obeys $R(x)M=\eta(\det x)^{-1}MR(x)$ for right translation by $x\in L$. It maps the span of right translates of $\Psi$ isometrically onto that of $\Phi_f$. By [F8], the map and its inverse extend to the two closed spans. Their compositions are identities on the dense spans and hence everywhere. The intertwining identity also holds on the closures by continuity. Therefore the cyclic unitary space of $\Phi_f$ is the determinant twist of the irreducible cyclic space of $\Psi$ and is irreducible, since multiplying the action by nonzero scalars preserves its invariant subspaces. [F4, F6, F8, F9, F10, F11, step 1.2, step 2.1]

4.1 The determinant map $L\to\mathbb A^\times$ is continuous. For a basic idele box, the local determinant preimages of its factors are open by [F11]. Outside the finitely many exceptional places, those factors contain $\mathrm{GL}_2(\mathbb Z_p)$, since an integral invertible matrix and its integral inverse have determinants whose product is $1$. At each point of the preimage, retain the local determinant preimages at the real place and at the finite exceptional places of the target box or the point. Use the integral matrix group at every other place. This gives a basic matrix neighborhood inside the preimage. Thus $\eta\circ\det$ is locally constant by step 3.1. Let $\pi_\Psi$ be the irreducible unitary right-translation action on the cyclic space of $\Psi$ supplied by [F4]. Its orbit maps are norm-continuous. By step 3.1, for every vector $w$ in that space the orbit map of $Mw$ is $x\mapsto\eta(\det x)^{-1}M\pi_\Psi(x)w$. Near any fixed $x_0\in L$ the scalar factor is constant, so this orbit map is norm-continuous there by continuity of $M$ and of the orbit of $w$. The twist acts by bijective complex-linear isometries and satisfies the right-translation group law. Therefore the action on the cyclic space of $\Phi_f$ is strongly continuous and unitary. [F4, F6, F10, F11, step 3.1]

5.1 By steps 3.1 and 4.1, the representation is irreducible and strongly continuous unitary, so the tensor product theorem in [F4] applies. Identify the adelic Hilbert space with $V_\ell\widehat\otimes W$, where $V_\ell$ is the space of $\pi_\ell$ and $W$ is the restricted Hilbert tensor product of the factors at the other places with the same reference vectors. To see the identification, take finite stages containing the exceptional places and $\ell$. Each such stage maps into $V_\ell\widehat\otimes W$ by grouping its elementary tensors into the $\ell$-component and the tensor of the remaining components, which maps into $W$. The product pairing makes this map an isometry on finite linear combinations, and the maps respect the inclusions that insert reference vectors. The union of these stages is dense in the global space because any finite stage can be enlarged to include $\ell$. The images span a dense subspace of $V_\ell\widehat\otimes W$ since the finite-stage tensors are dense in $W$. The isometry and its inverse on the dense image both extend by bounded linear extension. Their compositions equal the identities by continuity on the dense subspaces, so the extended map is onto. The finite-stage action gives $\pi_\ell(x)\otimes I_W$ for $x\in G_\ell$ on the dense span and hence everywhere by continuity. [F4, F8, step 2.2, step 3.1, step 4.1]

6.1 By [F10] and countable choice, $\mathbb Q_\ell$ is a locally compact nonarchimedean valued field in its $\ell$-adic topology. The nonzero elements $\ell^n$ have absolute values $\ell^{-n}\to0$ by the valuation and geometric limit in [F10], so the topology is nondiscrete. Thus $\mathbb Q_\ell$ is a nonarchimedean local field. Apply the local smooth representation result in [F4] with $F=\mathbb Q_\ell$, $n=2$ and the topologically irreducible unitary factor $\pi_\ell$ from step 5.1. Its vectors fixed by a compact open subgroup carry an algebraically irreducible admissible action. To compare with the smoothness convention in [F2], suppose a vector is fixed by an open subgroup $J$ of $G_\ell$. Then $J\cap K$ is open. The left cosets of $J\cap K$ in $K$ partition $K$ by [F12]. Each coset is open in $K$ by restriction of the corresponding translation homeomorphism from [F6]. The complement of $J\cap K$ in $K$ is a union of these open cosets, so it is open by [F12]. Thus $J\cap K$ is closed in the compact space $K$ and is compact by [F12]. The vector is fixed by this compact open subgroup. A vector fixed by a compact open subgroup is fixed by an open subgroup, so the two conventions give the same space. [F2, F4, F6, F10, F12, given, step 5.1]

7.1 The nonzero $K$-fixed class from step 2.2 and the fixed-space identity in [F8] imply $V_\ell^K\ne0$. Since $K$ is compact open, $V_\ell^K$ is also the $K$-fixed subspace of the smooth representation in step 6.1. With countable choice as assumed, the hypotheses of [F2] hold. The operators $\mathcal T_\ell$ and $\mathcal R_\ell$ act on $V_\ell^K$ by $\sqrt\ell(u+v)$ and $uv$. Each is a finite sum of operators from $G_\ell$, so [F8] transfers the same scalars to the tensor fixed space and thus to $[\Phi_f]$. [F2, F6, F8, given, step 2.2, step 5.1, step 6.1]

8.1 For either of the operators $T$ in step 7.1 with scalar $\lambda$, form the function $D=T\Phi_f-\lambda\Phi_f$ using the finite sum of right translates. Each translated function is continuous by composition with a right-translation homeomorphism from [F6]. Right translates preserve left rational invariance and left central covariance because left multiplication commutes with right translation. This sum represents the action on the class $[\Phi_f]$, so $D$ represents the zero class by step 7.1. Step 1.1 gives $T\Phi_f=\lambda\Phi_f$ at every argument. [F2, F4, F6, step 1.1, step 7.1]

9.1 Applying the weight-two comparison in [F2] to these pointwise scalar identities gives $\sqrt\ell(u+v)=a_\ell$ and $uv=\epsilon(\ell)$. Thus $\ell(Y-u)(Y-v)=\ell Y^2-\sqrt\ell a_\ell Y+\ell\epsilon(\ell)=P_\ell(\sqrt\ell Y)$. In particular the root multiset of $P_\ell$ is $\{\sqrt\ell u,\sqrt\ell v\}$, including multiplicities. [F2, F3, step 8.1]

10.1 The form is holomorphic, cuspidal, primitive and normalized, and the prime does not divide the level. By [F1], Deligne’s theorem in [F5] uses the same coefficient $a_\ell$ as in $P_\ell$. Its weight-two conclusion gives absolute value $\sqrt\ell$ for each root. By [F3] and step 9.1 this yields $|u|=|v|=1$, with the identification of the parameters already proved. [F1, F3, F5, given, step 9.1] ∎
