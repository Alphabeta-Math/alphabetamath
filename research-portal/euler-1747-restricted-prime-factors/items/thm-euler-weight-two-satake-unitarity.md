---
id: thm-euler-weight-two-satake-unitarity
kind: theorem
title: Ramanujan–Petersson bound in Satake normalization
status: published
domain: mathematics
deps:
  - math:thm-complete-subspace-iff-closed
  - math:def-quotient-topology
  - math:def-radon-measure-on-an-lch-space
  - math:def-countable-choice
  - math:def-strongly-continuous-unitary-representation
  - def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles
  - def-degree-two-projective-linear-group
  - math:def-prime
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - def-author-d45da46285be-spherical-hecke-algebra
  - def-author-d45da46285be-satake-transform
  - thm-normalized-degree-two-spherical-character
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - def-author-f98bf83ef432-local-conductor-exponent
  - def-author-f98bf83ef432-local-k-one-subgroup
  - def-author-f98bf83ef432-finite-conductor
  - lem-author-f98bf83ef432-unramified-iff-prime-avoids-conductor
  - math:def-divides-in-z
  - def-author-e2fc0f4318ab-weight-two-cusp-form
  - def-author-e2fc0f4318ab-normalized-weight-two-newform
  - thm-weight-two-newform-euler-root-bound
  - lem-author-d45da46285be-triangular-cosets
  - math:def-dirichlet-character-modulo-q
  - math:thm-of-square-roots
  - def-author-34e2e6a0519f-split-adelic-matrix-groups
  - math:lem-dirichlet-character-values
  - lem-author-e2fc0f4318ab-spherical-trace-and-product
  - lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars
  - math:thm-chinese-remainder-theorem
  - math:thm-determinant-multiplicative
  - def-author-24fda87362bc-local-adic-valuation
  - math:def-p-adic-integers-as-compatible-residue-classes
  - math:thm-fundamental-theorem-of-arithmetic
  - math:lem-complex-conjugation-and-modulus-laws
  - math:thm-finite-and-countable-subadditivity-of-measures
  - math:thm-nonnegative-integral-zero-iff-zero-almost-everywhere
  - lem-author-e2fc0f4318ab-classical-hecke-first-coefficient
  - math:def-product-topology
  - math:def-hausdorff-space
  - math:def-locally-compact-space
  - math:def-compact-space
  - math:def-hilbert-space
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:thm-extension-of-a-bounded-map-from-a-dense-subspace
  - math:def-borel-sigma-algebra
  - math:thm-continuous-preimages-of-borel-sets-are-borel
  - math:thm-nonnegative-weighted-sums-of-measures
formulation_deps:
  - math:def-quotient-topology
  - math:def-radon-measure-on-an-lch-space
  - math:def-countable-choice
  - math:def-strongly-continuous-unitary-representation
  - def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles
  - def-degree-two-projective-linear-group
  - math:def-prime
  - math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp
  - def-author-d45da46285be-spherical-hecke-algebra
  - def-author-d45da46285be-satake-transform
  - thm-normalized-degree-two-spherical-character
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - lem-author-d45da46285be-triangular-cosets
  - def-author-34e2e6a0519f-split-adelic-matrix-groups
  - def-author-24fda87362bc-local-adic-valuation
  - math:def-hausdorff-space
  - math:def-locally-compact-space
  - math:def-compact-space
  - math:def-hilbert-space
  - math:def-borel-sigma-algebra
argument_deps:
  - math:thm-complete-subspace-iff-closed
  - math:def-quotient-topology
  - math:def-radon-measure-on-an-lch-space
  - math:def-countable-choice
  - def-author-f98bf83ef432-local-conductor-exponent
  - def-author-f98bf83ef432-local-k-one-subgroup
  - def-author-f98bf83ef432-finite-conductor
  - lem-author-f98bf83ef432-unramified-iff-prime-avoids-conductor
  - math:def-divides-in-z
  - def-author-e2fc0f4318ab-weight-two-cusp-form
  - def-author-e2fc0f4318ab-normalized-weight-two-newform
  - thm-weight-two-newform-euler-root-bound
  - math:def-strongly-continuous-unitary-representation
  - def-author-d45da46285be-spherical-hecke-algebra
  - thm-normalized-degree-two-spherical-character
  - math:def-dirichlet-character-modulo-q
  - math:thm-of-square-roots
  - def-degree-two-projective-linear-group
  - def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - def-author-34e2e6a0519f-split-adelic-matrix-groups
  - math:lem-dirichlet-character-values
  - lem-author-e2fc0f4318ab-spherical-trace-and-product
  - lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars
  - math:thm-chinese-remainder-theorem
  - math:thm-determinant-multiplicative
  - def-author-24fda87362bc-local-adic-valuation
  - math:def-p-adic-integers-as-compatible-residue-classes
  - math:thm-fundamental-theorem-of-arithmetic
  - math:lem-complex-conjugation-and-modulus-laws
  - math:thm-finite-and-countable-subadditivity-of-measures
  - math:thm-nonnegative-integral-zero-iff-zero-almost-everywhere
  - lem-author-e2fc0f4318ab-classical-hecke-first-coefficient
  - math:def-product-topology
  - math:def-hausdorff-space
  - lem-author-d45da46285be-triangular-cosets
  - math:def-locally-compact-space
  - math:def-compact-space
  - math:def-hilbert-space
  - math:lem-compactness-of-a-subspace-is-ambient
  - math:thm-extension-of-a-bounded-map-from-a-dense-subspace
  - math:def-borel-sigma-algebra
  - math:thm-continuous-preimages-of-borel-sets-are-borel
  - math:thm-nonnegative-weighted-sums-of-measures
dependency_roles:
  math:thm-complete-subspace-iff-closed: mathematical-premise
  math:def-quotient-topology: mathematical-premise
  math:def-radon-measure-on-an-lch-space: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-strongly-continuous-unitary-representation: mathematical-premise
  def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles: mathematical-premise
  def-degree-two-projective-linear-group: mathematical-premise
  math:def-prime: mathematical-premise
  math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp: mathematical-premise
  def-author-d45da46285be-spherical-hecke-algebra: mathematical-premise
  def-author-d45da46285be-satake-transform: mathematical-premise
  thm-normalized-degree-two-spherical-character: mathematical-premise
  math:def-complex-conjugate-real-imaginary-part-and-modulus: mathematical-premise
  def-author-f98bf83ef432-local-conductor-exponent: mathematical-premise
  def-author-f98bf83ef432-local-k-one-subgroup: mathematical-premise
  def-author-f98bf83ef432-finite-conductor: mathematical-premise
  lem-author-f98bf83ef432-unramified-iff-prime-avoids-conductor: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  def-author-e2fc0f4318ab-weight-two-cusp-form: mathematical-premise
  def-author-e2fc0f4318ab-normalized-weight-two-newform: mathematical-premise
  thm-weight-two-newform-euler-root-bound: mathematical-premise
  lem-author-d45da46285be-triangular-cosets: mathematical-premise
  math:def-dirichlet-character-modulo-q: mathematical-premise
  math:thm-of-square-roots: mathematical-premise
  def-author-34e2e6a0519f-split-adelic-matrix-groups: mathematical-premise
  math:lem-dirichlet-character-values: mathematical-premise
  lem-author-e2fc0f4318ab-spherical-trace-and-product: mathematical-premise
  lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars: mathematical-premise
  math:thm-chinese-remainder-theorem: mathematical-premise
  math:thm-determinant-multiplicative: mathematical-premise
  def-author-24fda87362bc-local-adic-valuation: mathematical-premise
  math:def-p-adic-integers-as-compatible-residue-classes: mathematical-premise
  math:thm-fundamental-theorem-of-arithmetic: mathematical-premise
  math:lem-complex-conjugation-and-modulus-laws: mathematical-premise
  math:thm-finite-and-countable-subadditivity-of-measures: mathematical-premise
  math:thm-nonnegative-integral-zero-iff-zero-almost-everywhere: mathematical-premise
  lem-author-e2fc0f4318ab-classical-hecke-first-coefficient: mathematical-premise
  math:def-product-topology: mathematical-premise
  math:def-hausdorff-space: mathematical-premise
  math:def-locally-compact-space: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:def-hilbert-space: mathematical-premise
  math:lem-compactness-of-a-subspace-is-ambient: mathematical-premise
  math:thm-extension-of-a-bounded-map-from-a-dense-subspace: mathematical-premise
  math:def-borel-sigma-algebra: mathematical-premise
  math:thm-continuous-preimages-of-borel-sets-are-borel: mathematical-premise
  math:thm-nonnegative-weighted-sums-of-measures: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, Lemma 3.2, opening of the Ramanujan–Petersson paragraph, and p.
        8, Reference [1]
    - title: Pierre Deligne, La conjecture de Weil. I
      url: https://doi.org/10.1007/BF02684373
      locator: Theorem (8.2), p. 302. The classical root bound is supplied by the
        linked theorem.
    - title: Andrew Corbett and Abhishek Saha, On the order of vanishing of newforms
        at cusps
      url: https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf#page=16
      locator: §2.1.1, definition of U₀ (p. 6), §§2.1.4–2.1.5, equation (8) and the
        least-exponent rule (p. 8), §2.1.8, Definition 2.9 (p. 10), §3.1,
        (20)–(22) (pp. 16–17), §§3.2.1–3.2.2, Lemma 3.1 and the normalization
        after (25) (pp. 17–18), and §3.2.3, (28) and the following sentence (p.
        19).
      statement: An irreducible unitary cuspidal representation of GL₂ over the
        rational adeles of the specified real type contains an adelic newform
        invariant by the product of its local K₁ groups at the least
        fixed-vector exponents. At positive exponent n, K₁(n) uses c ≡ 0 and a ≡
        1, while K′₁(n) uses c ≡ 0 and d ≡ 1. The literal local test in equation
        (8) at exponent zero uses U₀ equal to the unit group, so it requires a
        unit upper-left entry. The global level subgroup in §3.1 uses the full
        integral factor at unramified primes. The associated classical
        holomorphic newform has weight k and level given by the product of the
        prime powers of those exponents. Equation (22) gives the
        determinant-normalized restriction of the adelic newform to real
        matrices of positive determinant. Equation (21) prescribes the character
        exp(ikθ) for the rotation with first row (cos θ, sin θ). The
        normalization following (25) sets the first Fourier coefficient to one.
        The additive quotient of the adeles by Q is compact and uses invariant
        probability measure. The global Whittaker newform factors with a local
        Whittaker newform belonging to every finite factor. The smooth finite
        factors are thus generic, meaning they have a nonzero Whittaker
        functional. At each finite place the local newform is a nonzero fixed
        vector at the least congruence exponent.
      hypotheses: The global representation is irreducible unitary cuspidal over Q and
        its central character is trivial on the positive real scalars. The full
        real factor is the discrete series of lowest weight k, defined in §3.1
        as the unique irreducible subrepresentation of normalized induction from
        |·|^((k−1)/2) sgn^k and |·|^((1−k)/2). Here k=2, so the sign factor is
        trivial. The local conductor definition uses irreducible admissible
        generic smooth factors, as used for the given cuspidal representation in
        §3.1.
      reading_limits: Read the listed congruence, correspondence, normalization, and
        local and global Whittaker passages. The correspondence, genericity and
        local newvector existence are used as stated. Equality of the fixed
        spaces at zero, transport at positive exponents and the determinant
        twist are supplied locally.
    - title: Denis Trotabas, Modular Forms and Automorphic Representations
      url: https://math.stanford.edu/~conrad/conversesem/refs/trotabas.pdf#page=21
      locator: §4, Theorem 4.1 (p. 10), §4.2 (p. 13), §6.1 (pp. 19–21), restriction
        remark, and §6.2, Theorem 6.1 (p. 21).
      statement: An irreducible unitary representation of GL₂ of the rational adeles
        is the restricted Hilbert tensor product of irreducible unitary local
        factors with unit spherical reference vectors outside a finite set. The
        Hilbert space is the completion of the span of elementary tensors
        agreeing with the reference vectors outside finitely many places, with
        the product inner product on elementary tensors. Its restriction to a
        single place is a Hilbert direct sum of copies of that factor, which
        determines the local equivalence class. At a finite place an irreducible
        unitary representation has finite-dimensional fixed spaces for each
        compact open subgroup, and its smooth vectors form an irreducible
        admissible representation.
      hypotheses: The tensor-product assertion is for an irreducible unitary
        representation of GL₂ over the rational adeles. The local admissibility
        theorem is for an irreducible unitary representation of a reductive
        group over a local field, and the smooth-vector assertion uses the
        nonarchimedean case and admissibility. Here the local group is GL₂(Q_q).
      reading_limits: Read the tensor construction and restriction remark, the
        tensor-product theorem statement and the finite-place admissibility and
        smooth-vector passages. The representation-theoretic existence and
        admissibility results are used as stated.
    - title: Denis Trotabas, Modular Forms and Automorphic Representations
      url: https://math.stanford.edu/~conrad/conversesem/refs/trotabas.pdf#page=25
      locator: §§8.1–8.2 (pp. 25–27), especially the hypotheses of §8.1 and the
        pairing and continuity argument on p. 27.
      statement: The central-character Hilbert space consists of Borel representatives
        modulo almost-everywhere equality on the rational quotient, with Borel
        descended moduli and squared norm integrated on the central quotient.
        For GL₂ over the rational adeles the central quotient has finite volume.
        The cuspidal subspace is the intersection of the kernels of continuous
        linear functionals defined by compactly supported tests on the left
        quotient by the adelic upper unitriangular group. On a smooth
        representative the functional integrates the unipotent constant term
        against its test.
      hypotheses: The central-character model uses a locally compact unimodular group,
        closed unimodular subgroups for the measured quotients, and a unitary
        central character trivial on the rational scalars. The pairing example
        is for GL₂ over the rational adeles with the compact additive
        rational-to-adelic quotient and the finite-volume central quotient.
      reading_limits: Read the conventions in §8.1 and the pairing formula,
        finite-volume assertion, continuity statement and closed-kernel
        characterization in §8.2. The application uses the continuity and
        pairing identity and needs only inclusion of the smooth cuspidal
        closure.
    - title: Jayce R. Getz and Heekyoung Hahn, An Introduction to Automorphic
        Representations
      url: https://sites.duke.edu/jgetz/files/2022/04/Graduate_Text.pdf#page=88
      locator: §2.3, Proposition 2.3.1 and the preceding restricted-product
        construction (pp. 47–48), §§3.1–3.2 including Theorem 3.2.2 (p. 72), and
        §3.6, Lemma 3.6.4 and the paragraph following its proof (pp. 78–79).
        Also §4.4, the isotypic decomposition, Proposition 4.4.3 and Theorem
        4.4.6 (pp. 102, 104), §4.6, the construction around (4.15), Theorem
        4.6.1 and Proposition 4.6.2 (pp. 108–110), and §4.8, Definition 4.7 (p.
        112).
      statement: An affine algebraic group's adelic points form a locally compact
        Hausdorff group with the restricted-product topology, and its rational
        points form a closed discrete subgroup. The adelic group is unimodular
        for a reductive group. A closed subgroup whose modular function equals
        the restriction of the ambient modular function admits a nonzero
        right-invariant Radon measure on the left coset space, unique up to
        positive scale and induced by the quotient Haar integral formula. Every
        locally compact Hausdorff group has a nonzero positive Radon right Haar
        measure, unique up to positive scaling. Abelian and discrete locally
        compact groups are unimodular. For a unitary representation of a real
        reductive group, the Hilbert space is the orthogonal Hilbert sum of its
        compact isotypic subspaces. In a Hilbert representation the vectors that
        are both smooth and compact-finite are dense and stable under the Lie
        algebra. Irreducible unitary representations are unitarily equivalent if
        their underlying modules are isomorphic by a map intertwining both the
        Lie algebra and maximal compact group actions. For a complex reductive
        Lie algebra with a chosen Cartan subalgebra, a Harish–Chandra parameter
        evaluates the Cartan projection of a central enveloping-algebra element
        after the shift by the half-sum of positive roots. An essentially
        square-integrable representation has square-integrable coefficients on
        the subgroup cut out by absolute values of rational characters, which
        for real GL₂ is the group of matrices of absolute determinant one.
      hypotheses: The adelic assertions are over a global field, here Q. The topology
        and discreteness are used for GL₂ and GL₄, with the integral matrix
        groups as restricted-product factors, and reductivity is used for GL₂.
        The quotient theorem requires a locally compact group and a closed
        subgroup with matching modular functions. Haar existence applies to a
        locally compact Hausdorff group. The abelian and discrete cases apply to
        the center and the indicated rational and unipotent subgroups. The
        archimedean assertions concern real reductive groups and use a maximal
        compact subgroup. The unitary equivalence assertion requires irreducible
        unitary representations whose underlying modules are isomorphic for the
        joint Lie algebra and maximal compact group actions. The Harish–Chandra
        formula applies to a module with an infinitesimal character, with the
        diagonal Cartan subalgebra in the application to complexified real GL₂.
      reading_limits: Read the statements and restricted-product description at the
        stated locators. Haar existence, reductive unimodularity, rational
        discreteness and the quotient theorem are used as stated. The closedness
        and unimodularity of the product with the full adelic center are checked
        in the proof. Read Proposition 4.4.3, the statement of Theorem 4.4.6,
        the Cartan projection and root shift construction in §4.6 and its
        parameter-evaluation formula, and the definition of essential square
        integrability. The evaluation on the scalar generator and integration of
        its infinitesimal action are carried out below.
    - title: Peter Humphries, Archimedean Newform Theory for GLₙ
      url: https://doi.org/10.1017/S1474748024000227
      locator: §2.4.3 (p. 49), Lemma 6.9 and its proof (pp. 75–76), and Lemma 8.1(2)
        (pp. 85–86).
      statement: For an integer κ ≥ 2, the real essentially square-integrable
        representation Dκ twisted by |det|^t embeds in the normalized
        upper-triangular induction of |·|^(t+(κ−1)/2) and sgn^κ|·|^(t−(κ−1)/2).
        The smooth model acts by right translation with left diagonal covariance
        |a|^(t+κ/2) sgn(d)^κ |d|^(t−κ/2). Its O(2)-types have degrees κ, κ+2,
        κ+4, and so on, each once.
      hypotheses: The field is ℝ, the group is GL₂, κ is an integer at least two and t
        is complex. The application takes κ=2 and t=0, with trivial central
        character.
      reading_limits: Read the essential square-integrability assertion, the
        O(2)-restriction formula and the normalized induced-model statement.
        These are used as stated.
    - title: Toshiyuki Kobayashi and Birgit Speh, How does the restriction of
        representations change under translations? A story for the general
        linear groups and the unitary groups
      url: https://www.ms.u-tokyo.ac.jp/~toshi/texpdf/tk2025b-Restriction_of_A_q.pdf
      locator: §2.1, (2.1) (p. 6), §§6.1–6.2 (pp. 25–26), and §6.3, (6.2) (p. 26).
      statement: For a positive integer a, the irreducible unitary relative discrete
        series σ_a of GL₂(ℝ) has Harish–Chandra parameter (a/2,−a/2) and minimal
        O(2)-type of degree a+1. It restricts to SL₂(ℝ) as the direct sum of the
        holomorphic and antiholomorphic discrete series, with extremal rotation
        weights a+1 and −(a+1), respectively.
      hypotheses: The representation is the indicated relative discrete series of
        GL₂(ℝ) and the subgroup is SL₂(ℝ). Use a=1 and identify the positive
        weight convention by the rotation matrix in Corbett–Saha (21).
      reading_limits: Read the normalization of Harish–Chandra parameters, the
        relative discrete series parameters, the group restriction statement and
        the unitary assertion in (6.2) specialized to n=2 and ℓ=1. The proof
        below uses a=1.
    - title: Kimball Martin, A summary of local representation theory for GL(2)
      url: https://kimballmartin.github.io/autreps/ch3.pdf#page=10
      locator: §3.2, paragraph after Theorem 3.2.3 (printed p. 32).
      statement: For a fixed central character there is a unique real GL₂ discrete
        series type of weight k when the parity of k is compatible with the
        value of the character at −1. In particular for trivial central
        character this applies at even k≥2.
      hypotheses: The field is ℝ and the group is GL₂. The application is to relative
        discrete series of least absolute rotation weight two and trivial scalar
        character.
      reading_limits: Read the real classification statement and the paragraph
        explaining the fixed-central-character uniqueness and parity condition.
        Only the even, trivial-central-character case is used.
dependency_level: 6
---

## Statement

Assume countable choice, meaning that a sequence of nonempty sets has a choice function. Write $\mathbb A=\mathbb R\times\mathbb A_f$, where $\mathbb A_f$ consists of tuples of $q$-adic numbers integral at all but finitely many primes $q$. Put $G=\mathrm{GL}_2(\mathbb A)$, the invertible two-by-two matrices over this ring. Give $G$ the restricted-product topology of the real and local matrix groups with respect to the finite-place subgroups $K_q=\mathrm{GL}_2(\mathbb Z_q)$. Thus a basic open box has local open factors and uses $K_q$ at all but finitely many $q$. Local matrix groups carry the subspace topology from the four matrix entries. Embed $\mathrm{GL}_2(\mathbb Q)$ diagonally, and let $Z=\{aI:a\in\mathbb A^\times\}$ be the scalar subgroup.

Let $\Pi$ be an irreducible unitary cuspidal automorphic representation of $G$ with central character trivial on the positive real scalars. Here unitary means a strongly continuous action by complex-linear Hilbert space isometries, and irreducible means there is no proper nonzero closed invariant subspace. The action is by right translation on a closed invariant subspace of the cuspidal Hilbert space with unitary central character $\omega$. Vectors in this model are square-integrable classes of Borel representatives on $Y=\mathrm{GL}_2(\mathbb Q)\backslash G$, modulo equality almost everywhere for the Haar-induced measure on $Y$. Their moduli descend to Borel functions on the norm quotient. On both quotients the Borel sigma-algebra is generated by the open sets in the quotient topology. The smooth representatives used to define the cuspidal subspace satisfy left rational invariance and $\phi(zg)=\omega(z)\phi(g)$ for $z\in Z$, with $\omega$ a continuous character trivial on rational scalars and of absolute value one. Thus $|\phi|^2$ descends to the locally compact Hausdorff space $X=(\mathrm{GL}_2(\mathbb Q)Z)\backslash G$ with the quotient topology. The squared norm uses the Haar-induced measure on $X$, equivalently any nonzero right-$G$-invariant Radon measure on $X$. A Radon measure here is a Borel measure finite on compact sets, inner regular on open sets and outer regular on Borel sets. The cusp space is the closure in the square-integral norm of smooth square-integrable functions whose constant term vanishes at every $g$. The constant term is
$$\int_{\mathbb Q\backslash\mathbb A}\phi\left(\begin{pmatrix}1&x\\0&1\end{pmatrix}g\right)\,dx,$$
where $dx$ is Haar probability on the compact additive quotient and the rationals are diagonal. The integrand is well defined there because adding a rational to $x$ left multiplies the upper unitriangular matrix by a rational matrix. Smooth functions here are differentiable to all orders in the real variables and invariant under right translation by some compact open subgroup of the finite adelic group, so they are locally constant in the finite variables.

Use the irreducible unitary local factors $\pi_v$ of $\Pi$ at the places $v$ of $\mathbb Q$. Fix a unit $K_q$-fixed reference vector at each finite place outside a finite exceptional set. The restricted Hilbert tensor product is the completion of the span of elementary tensors that agree with this reference family outside finitely many places. The inner product on elementary tensors is the product of the local inner products, with only finitely many factors different from one. Each local matrix group embeds by placing its matrix at that place and the identity elsewhere. The restriction to this embedded group is a Hilbert direct sum of copies of $\pi_v$, which determines that factor up to unitary equivalence.

Assume the real factor is the full $\mathrm{GL}_2(\mathbb R)$ weight-two discrete series, the unitary type of the unique irreducible subrepresentation of normalized upper-triangular induction from the diagonal characters $|\cdot|^{1/2}$ and $|\cdot|^{-1/2}$. In the induced model, smooth functions transform on the left under upper-triangular matrices of diagonal $(a,d)$ by $|a|^{1/2}|d|^{-1/2}$ times the half modulus $|a/d|^{1/2}$, and the group acts by right translation. The type is square-integrable modulo the real center. On the positive-determinant group its holomorphic constituent has rotation weights $2,4,6,\ldots$. The other constituent has weights $-2,-4,-6,\ldots$, obtained by conjugating rotations by a negative-determinant reflection. A rotation of angle $\theta$ has rows $(\cos\theta,\sin\theta)$ and $(-\sin\theta,\cos\theta)$, with weight $j$ meaning multiplication by $e^{ij\theta}$.

For a prime $\ell$, let $\pi_\ell$ be the factor at $\mathrm{GL}_2(\mathbb Q_\ell)$, the group of invertible two-by-two matrices over the $\ell$-adic field. Suppose $\pi_\ell$ is unramified, meaning that $K=K_\ell=\mathrm{GL}_2(\mathbb Z_\ell)$ fixes a nonzero vector, where $\mathbb Z_\ell$ is the ring of integers of $\mathbb Q_\ell$. The normalized Satake parameters $u_\ell,v_\ell$ are the unordered pair of nonzero complex numbers, counted with multiplicity, giving the scalar of each spherical Hecke operator on the $K$-fixed line by evaluation of its normalized Satake transform. The transform sums one term per coset $xK$ and weights diagonal valuations $(r,s)$ of an upper-triangular representative by $\ell^{(s-r)/2}X^rY^s$. The valuation of a nonzero local entry is its exponent of $\ell$ after removing an invertible integral factor. The spherical Hecke functions are compactly supported and invariant on both sides under $K$.

Then $|u_\ell|=|v_\ell|=1$, where $|z|$ is complex modulus. If every local scalar matrix acts trivially on $\pi_\ell$, let $p:\mathrm{GL}_2(\mathbb Q_\ell)\to\mathrm{PGL}_2(\mathbb Q_\ell)$ be the quotient by the local scalar subgroup. The descended representation $\bar\pi_\ell$ is defined by $\bar\pi_\ell(p(g))=\pi_\ell(g)$, so its pullback is $\pi_\ell$. The same bound applies to the projective representation in the Satake normalization of that pullback, with the $p(K)$-fixed line identified with the $K$-fixed line.

## Statement references

[[math:def-countable-choice|Countable choice]]

[[def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles|The finite adele ring]]

[[def-author-34e2e6a0519f-split-adelic-matrix-groups|The topology and scalar subgroup of the adelic matrix group]]

[[def-degree-two-projective-linear-group|Degree-two linear and projective groups]]

[[math:def-strongly-continuous-unitary-representation|Unitary representations]]

[[math:def-prime|Prime integers]]

[[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp|The local field and its integral subring]]

[[def-author-d45da46285be-spherical-hecke-algebra|Spherical Hecke algebra and fixed spaces]]

[[def-author-d45da46285be-satake-transform|Coset weights in the normalized Satake transform]]

[[lem-author-d45da46285be-triangular-cosets|Triangular representatives and their diagonal valuations]]

[[thm-normalized-degree-two-spherical-character|The Satake parameters of the fixed line and projective descent]]

[[math:def-complex-conjugate-real-imaginary-part-and-modulus|Complex modulus]]

[[math:def-quotient-topology|Quotient topology]]

[[math:def-radon-measure-on-an-lch-space|Radon measure]]

[[math:def-borel-sigma-algebra|Borel sigma-algebra]]

[[def-author-24fda87362bc-local-adic-valuation|Normalized local valuation]]

[[math:def-hausdorff-space|Hausdorff separation]]

[[math:def-locally-compact-space|Locally compact spaces]]

[[math:def-compact-space|Compact subsets and finite subcovers]]

[[math:def-hilbert-space|Hilbert spaces]]

## Facts & Assumptions

[F1] Use the adelic-to-classical newform correspondence described below with its upper-left congruence convention. For $n>0$ its group $K^{\mathrm{top}}_{1,q}(n)$ is defined by $c\equiv0$ and $a\equiv1$ modulo $q^n$, and our group $K_{1,q}(n)$ by $c\equiv0$ and $d\equiv1$. The global level subgroup uses the full integral group at exponent zero. The literal local test in equation (8) at zero uses matrices with unit upper-left entry. Their common fixed space equals the full integral fixed space, by the zero-exponent calculation in the cited congruence-group definition. The local exponent in our convention is the least $n\ge0$ such that $K_{1,q}(n)$ fixes a nonzero vector. The finite conductor is the product of the corresponding prime powers. [[def-author-f98bf83ef432-local-k-one-subgroup|The two congruence groups and their comparison]] [[def-author-f98bf83ef432-local-conductor-exponent|Local conductor exponent]] [[def-author-f98bf83ef432-finite-conductor|Finite conductor]]

[F2] For a family with finite conductor $C$, a local factor is unramified at $\ell$ exactly when $\ell\nmid C$, meaning $C$ is not a multiple of $\ell$. [[lem-author-f98bf83ef432-unramified-iff-prime-avoids-conductor|Unramified primes of the finite conductor]] [[math:def-divides-in-z|Integer divisibility]]

[F3] A normalized holomorphic weight-two newform is a cusp form in the new subspace, the orthogonal complement of the span of lower-level images, with first Fourier coefficient one and on which each classical Hecke operator acts by a scalar. Its transformation law is $f|_2\gamma=\epsilon(d_\gamma)f$ for $\gamma\in\Gamma_0(N)$, the group of integral determinant-one matrices with $N\mid c_\gamma$. The Dirichlet character $\epsilon$ is a homomorphism from the units modulo $N$ to $\mathbb C^\times$ extended by zero on other residue classes. It has absolute value one on units. The weight-two action for a positive-determinant real matrix $h$ with lower row $(c,d)$ is $(f|_2h)(z)=\det(h)(cz+d)^{-2}f(hz)$, where the matrix acts on the upper half-plane by its fractional linear map. For $\ell\nmid N$ and $T_\ell f=\lambda_\ell f$, the roots of the classical Hecke polynomial $X^2-\lambda_\ell X+\ell\epsilon(\ell)$ both have modulus $\sqrt\ell$, the positive square root of $\ell$. Complex modulus is multiplicative. [[math:lem-complex-conjugation-and-modulus-laws|Modulus of a product]] [[def-author-e2fc0f4318ab-weight-two-cusp-form|Weight-two holomorphic cusp forms]] [[def-author-e2fc0f4318ab-normalized-weight-two-newform|Classical normalized newforms]] [[thm-weight-two-newform-euler-root-bound|The classical weight-two Euler-root bound]] [[math:def-dirichlet-character-modulo-q|Dirichlet characters]] [[math:lem-dirichlet-character-values|Unit modulus of character values]] [[math:thm-of-square-roots|Nonnegative square roots]]

[F4] By the local representation results below, the smooth vectors of an irreducible unitary finite factor, those fixed by some open subgroup, are irreducible and admissible. Admissibility means that the fixed spaces for compact open subgroups are finite dimensional. On the nonzero $K$-fixed line, each spherical Hecke operator is a finite sum of translates with one term per coset. The indicators of $K\operatorname{diag}(\ell,1)K$ and $(\ell I)K$ give operators $\mathcal T_\ell,\mathcal R_\ell$ with respective scalars $\sqrt\ell(u_\ell+v_\ell)$ and $u_\ell v_\ell$. The determinants in the first support have valuation one and those in the second have valuation two. [[math:def-strongly-continuous-unitary-representation|Unitary actions and intertwining isomorphisms]] [[def-author-d45da46285be-spherical-hecke-algebra|Hecke operators as finite sums]] [[thm-normalized-degree-two-spherical-character|The fixed line and normalized parameter pair]] [[lem-author-e2fc0f4318ab-spherical-trace-and-product|The two spherical scalars]]

[F5] Let $K_0(N)$ consist of the finite integral invertible tuples with lower-left entry in $N\mathbb Z_q$ at each $q$. Write $a(k),d(k)$ for the unit classes modulo $N$ assembled from the upper-left and lower-right entries at the prime powers dividing $N$. For a maximal prime power $q^n$ dividing $N$, reduction $\mathbb Z_q\to\mathbb Z/q^n\mathbb Z$ is the coordinate homomorphism from the compatible residue tuples. It takes a diagonally embedded integer to its usual residue and takes units to units, preserving their inverses. The Chinese remainder ring isomorphism identifies unit classes modulo $N$ with tuples of unit classes at these prime powers. At $N=1$ the list is empty and there is one unit class. The fundamental theorem of arithmetic factors each positive integer into prime powers, with the empty product for one. Determinants multiply, and the valuation of a product of nonzero local scalars is the sum of valuations. On a nonzero rational $m/n$, the local valuation is $v_q(m)-v_q(n)$, where the integer valuations are the exponents of $q$ in the prime factorizations of the absolute values. [[lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars|Finite level and the weight-two scalar comparison]] [[def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles|Finite ideles and their unit components]] [[math:thm-chinese-remainder-theorem|Combine prime-power residues]] [[math:def-p-adic-integers-as-compatible-residue-classes|Compatible residue tuples]] [[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp|Identify the integral subring]] [[math:thm-fundamental-theorem-of-arithmetic|Prime factorization]] [[math:thm-determinant-multiplicative|Multiplicativity of the determinant]] [[lem-author-d45da46285be-triangular-cosets|Additivity on nonzero local scalars]] [[def-author-24fda87362bc-local-adic-valuation|The rational valuation formula]]

[F6] For a left rationally invariant function with real restriction $(f|_2h)(i)$ and right $K_0(N)$ covariance by $\epsilon(d(k))^{-1}$, if $\mathcal T_\ell,\mathcal R_\ell$ act by scalars at a prime $\ell\nmid N$, those scalars respectively are the Fourier coefficient $a_\ell$ of the normalized newform $f$ and $\epsilon(\ell)$. [[lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars|Scalar comparison for the lower-right covariance]]

[F7] A Radon measure approximates the measure of each open subset from within by compact subsets. A continuous function on $G$ constant on the fibers of the projection to $X$ is continuous as a function on $X$ in the quotient topology. Measures are finitely subadditive. A continuous map has Borel preimages of Borel sets, so it is measurable for the Borel sigma-algebras. A nonnegative measurable function with integral zero vanishes almost everywhere. [[math:def-radon-measure-on-an-lch-space|Radon measure on the orbit space]] [[math:def-quotient-topology|Continuity through the quotient]] [[math:thm-finite-and-countable-subadditivity-of-measures|Finite subadditivity]] [[math:thm-nonnegative-integral-zero-iff-zero-almost-everywhere|Vanishing almost everywhere]] [[math:thm-continuous-preimages-of-borel-sets-are-borel|Borel preimages under continuous maps]]

[F8] Use the locally compact adelic group topology, closed discreteness of rational points, reductive unimodularity and quotient measure theorem specified below. Every locally compact Hausdorff group has a nonzero Radon Haar measure. Abelian and discrete locally compact groups are unimodular. [[def-author-34e2e6a0519f-split-adelic-matrix-groups|Restricted adelic matrix-group topology]]

[F9] Use the continuous constant-term pairings and their closed kernels described below for the unitary central-character space.

[F10] In the product topology on two spaces, open rectangles form a basis. A space is Hausdorff if any two distinct points have disjoint open neighborhoods. [[math:def-product-topology|Product topology on two spaces]] [[math:def-hausdorff-space|Hausdorff separation]]

[F11] Use the real essentially square-integrable induced model and the restriction to the determinant-one group specified below. In the unitary model the compact types give an orthogonal Hilbert sum and the compact-finite vectors are dense. Use Getz–Hahn's Harish–Chandra evaluation rule and density of smooth compact-finite vectors as specified below. Corbett–Saha use the same full normalized induction at weight two and take the holomorphic lowest weight on the indicated rotations.

[F12] Under countable choice, the classical Hecke eigenvalue of a weight-two cuspidal newform with first Fourier coefficient one equals its Fourier coefficient at a prime not dividing the level. [[lem-author-e2fc0f4318ab-classical-hecke-first-coefficient|The first Hecke coefficient identity]]

[F13] A locally compact space has a compact neighborhood of each point. Every open cover of a compact space has a finite subcover. For a compact subset, the finite-subcover property also applies to covers by sets open in the ambient space. [[math:def-locally-compact-space|Compact neighborhoods]] [[math:def-compact-space|Compact spaces and subsets]] [[math:lem-compactness-of-a-subspace-is-ambient|Ambient open covers of compact subsets]]

[F14] Under countable choice, a bounded linear map from a dense normed subspace into a Banach space extends uniquely to a bounded linear map on the whole normed space. A Hilbert space is complete for its induced norm. [[math:thm-extension-of-a-bounded-map-from-a-dense-subspace|Extension from a dense subspace]] [[math:def-hilbert-space|Completeness of the Hilbert norm]]

[F15] The finite factors of the irreducible cuspidal representation have local Whittaker models by the factorization below. Their smooth representations are generic, and their least upper-left newvector exponents exist at every finite place.

[F16] Every finite or countable sum of measures on one measurable space with all weights equal to one is a measure. [[math:thm-nonnegative-weighted-sums-of-measures|Countable sums of measures]]

[F17] A closed subspace of a complete metric space is complete. Under countable choice, a complete subspace of any metric space is closed. [[math:thm-complete-subspace-iff-closed|Completeness and closedness]]

## External input

Corbett–Saha's correspondence applies to an irreducible unitary cuspidal automorphic representation of $\mathrm{GL}_2$ over the rational adeles, with the indicated discrete series of lowest weight $k\ge2$ and central character trivial on the positive real scalars. Their adelic newform $\Phi$ is a vector of the given representation and is right invariant by the product of their local $K_1$ groups at the conductor exponents. The classical holomorphic newform has level $N$ equal to the product of prime powers from those exponents. At $k=2$ the real restriction is $\Phi(h_\infty)=(f|_2h)(i)$, where $h$ is a real matrix of positive determinant and $h_\infty$ inserts it at the real place and the identity at every finite place. One can choose the newform with first Fourier coefficient one. The global Whittaker newform factors into local Whittaker newforms, one in the Whittaker model of each finite smooth factor. Thus each such factor has a nonzero linear functional on which the upper unitriangular subgroup acts by a nontrivial additive character. For an irreducible admissible smooth factor with this property, the least upper-left congruence exponent exists by the local newvector result. At exponent zero, the global level factor is the full integral group. Equation (8) for the local test uses $U_0=\mathbb Z_q^\times$, so its upper-left entry must be a unit. See also §§2.1.5 and 2.1.8 and equation (28). [On the order of vanishing of newforms at cusps](https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf#page=16)

Every irreducible unitary representation of the rational adelic matrix group is a restricted Hilbert tensor product of irreducible unitary local factors, spherical at all but finitely many finite places. Restriction to a single embedded local group is a Hilbert sum of copies of its factor. For an irreducible unitary factor of $\mathrm{GL}_2(\mathbb Q_q)$, the smooth vectors form an irreducible admissible representation. [Modular Forms and Automorphic Representations, §§4–4.2 and 6](https://math.stanford.edu/~conrad/conversesem/refs/trotabas.pdf#page=21)

The central-character Hilbert model uses Borel representatives modulo almost-everywhere equality on the rational quotient, with Borel descended moduli and squared norm integrated on $X$. For the rational adelic group in degree two this central quotient has finite invariant volume. The standard cuspidal subspace is the intersection of the kernels of continuous linear functionals. The tests are continuous compactly supported functions on $U(\mathbb A)\backslash G$, where $U$ is the upper unitriangular subgroup. The functional associated to each test integrates the form against that test on $U(\mathbb Q)\backslash G$. On a smooth representative this is the integral of its constant term against the test on $U(\mathbb A)\backslash G$. The constant term is integration along the additive quotient of the adeles by the rationals. Use its translation-invariant probability normalization. [Modular Forms and Automorphic Representations, §§8.1–8.2](https://math.stanford.edu/~conrad/conversesem/refs/trotabas.pdf#page=25) [On the order of vanishing of newforms at cusps, §3.2.1](https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf#page=17)

The adelic matrix groups in degrees two and four are locally compact Hausdorff with the indicated restricted-product topologies, and the diagonal rational points are closed and discrete. The adelic group in degree two is unimodular. Every locally compact Hausdorff group has a nonzero positive Radon right Haar measure. Such a measure is also left invariant for abelian or discrete groups. When a closed subgroup of a locally compact group has the restriction of the ambient modular function as its own modular function, the left coset space has a nonzero right-invariant Radon measure given by the quotient Haar integral formula, unique up to positive scale. In particular this applies when both groups are unimodular, meaning their right Haar measures are also left invariant. [Getz–Hahn, Proposition 2.3.1, Theorem 3.2.2 and §3.6](https://sites.duke.edu/jgetz/files/2022/04/Graduate_Text.pdf#page=88)

For $\mathrm{GL}_2(\mathbb R)$, Humphries's smooth model for $D_2$ is a subrepresentation of the normalized induction from $|\cdot|^{1/2}$ and $|\cdot|^{-1/2}$. For a diagonal matrix with entries $a,d$ the left covariance is $|a/d|$. This type is essentially square-integrable and its $\mathrm O(2)$-types have degrees $2,4,6,\ldots$, each once. Each degree $j>0$ type has rotation weights $j,-j$. [Humphries, §2.4.3, Lemma 6.9 and Lemma 8.1(2)](https://doi.org/10.1017/S1474748024000227)

Kobayashi–Speh's real relative discrete series $\sigma_1$ has infinitesimal character $(1/2,-1/2)$ and minimal $\mathrm O(2)$-type of degree two. Its restriction to $\mathrm{SL}_2(\mathbb R)$ splits into the holomorphic and antiholomorphic discrete series with opposite extremal rotation weights of absolute value two. The series is irreducible and unitary, as also seen by taking $n=2$ and $\ell=1$ in (6.2). [Kobayashi–Speh, §§6.2–6.3](https://www.ms.u-tokyo.ac.jp/~toshi/texpdf/tk2025b-Restriction_of_A_q.pdf)

A unitary representation of a real reductive group is the orthogonal Hilbert sum of its compact isotypic subspaces and its compact-finite vectors are dense. The smooth compact-finite vectors of a Hilbert representation are dense and Lie algebra invariant. Infinitesimally equivalent irreducible unitary representations are unitarily equivalent. Infinitesimal equivalence means an isomorphism of the underlying modules intertwining both the Lie algebra and maximal compact group actions. For a module with an infinitesimal character, the action of an element of the center of the enveloping algebra is given by evaluating its Harish–Chandra image at the parameter. The image is obtained by projection to the enveloping algebra of the Cartan subalgebra and then applying the shift $X\mapsto X-\rho(X)$ on Cartan elements, with $\rho$ the half-sum of positive roots. [Getz–Hahn, Proposition 4.4.3 and Theorem 4.4.6](https://sites.duke.edu/jgetz/files/2022/04/Graduate_Text.pdf#page=118) [Getz–Hahn, §4.6](https://sites.duke.edu/jgetz/files/2022/04/Graduate_Text.pdf#page=124)

For a fixed central character and compatible weight, the real relative discrete-series type is unique. Corbett–Saha's equation (21) uses positive weight $k$ for the holomorphic lowest-weight vector in the rotation convention of the Statement. [Martin, §3.2](https://kimballmartin.github.io/autreps/ch3.pdf#page=10) [Corbett–Saha, equation (21)](https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf#page=16)

## Proof

**Given:** The cuspidal representation $\Pi$, countable choice and its unramified factor at $\ell$.

**Goal:** Determine the moduli of the two normalized Satake parameters of that factor, including the stated projective case.

1.1 Let $H=\mathrm{GL}_2(\mathbb Q)Z$. Conjugation on two-by-two matrices gives a continuous homomorphism $J:G\to\mathrm{GL}_4(\mathbb A)$ in the basis of four matrices $E_{ij}$ for $i,j\in\{1,2\}$, each having a one at $(i,j)$ and zeros elsewhere. Every matrix is the unique sum of its entries times these units. Its coordinates are continuous locally, and an integral invertible matrix and its inverse preserve the integral matrix lattice at every finite place, so the local maps carry the integral factors into the corresponding integral factors of the restricted products. The kernel is $Z$, since commuting with the diagonal matrix units forces a matrix to be diagonal, and commuting with the off-diagonal units forces its diagonal entries to agree. Consequently $H=J^{-1}(J(\mathrm{GL}_2(\mathbb Q)))$. The image of the rational subgroup is a subset of the closed discrete $\mathrm{GL}_4(\mathbb Q)$ in [F8], so it is itself closed and discrete. Thus $H$ is closed and its cosets of $Z$ are open in $H$. [F8]

1.2 Take $k=2$ in [F1]. The sign character raised to $k$ is trivial and the two inducing exponents are $1/2$ and $-1/2$. The half modulus gives left covariance $|a/d|$, exactly the model in the Statement and the $D_2$ model of [F11]. Thus the full given real type satisfies the archimedean induction hypothesis of the correspondence. All real scalars act trivially by this covariance. Essential square integrability gives square integrability modulo the full real center here. Indeed $g\mapsto|\det g|^{-1/2}g$ identifies the quotient by positive scalars with the group of matrices of absolute determinant one, and passing to the full scalar quotient also divides by the central finite subgroup $\{\pm I\}$. The squared modulus of each coefficient is invariant under this finite subgroup, so the integrals differ only by a positive normalization factor by the quotient Haar formula. [given, F1, F8, F11]

2.1 The minimal degree-two $\mathrm O(2)$-type of $\sigma_1$ has weights $2,-2$, so $-I=r_\pi$ acts as the identity there. Since $-I$ is central and $\sigma_1$ is irreducible, its fixed subspace is the whole representation. In the complexified Lie algebra, the scalar generator $I=\operatorname{diag}(1,1)$ is central and belongs to the diagonal Cartan subalgebra. The Cartan projection in [F11] fixes $I$. Both roots, which are the differences of the two diagonal coordinates, vanish on $I$, so the root shift leaves $I$ unchanged as well. A parameter $(\lambda_1,\lambda_2)$ evaluates $I$ as $\lambda_1+\lambda_2$. Thus $d\sigma_1(I)$ acts on the smooth compact-finite vectors by the scalar $1/2+(-1/2)=0$. For each such vector $v$, the derivative at $t$ of $\sigma_1(e^t I)v$ is $\sigma_1(e^t I)d\sigma_1(I)v=0$. Its value is therefore $v$ for every $t$, and density from [F11] and continuity of each unitary operator extend this identity to the Hilbert space. Thus $\sigma_1$ and $D_2$ have the same trivial central character and the same least absolute rotation weight. By the fixed-central-character uniqueness in [F11], their smooth compact-finite modules are of the same discrete-series type, so there is an isomorphism intertwining the Lie algebra and maximal compact group actions. The unitary equivalence theorem in [F11] then identifies the irreducible Hilbert models. The restriction in [F11] applies to the real factor in the Statement. [F11, step 1.2]

2.2 The left orbit projection $G\to X$ is open because the inverse image of the image of an open set is the union of its left translates by $H$. The relation of lying in the same left orbit is the preimage of the closed subgroup $H$ by the continuous map $(g,g')\mapsto g'g^{-1}$ on $G\times G$. For $g,g'$ with distinct images, take a basic open rectangle around $(g,g')$ disjoint from that relation by [F10]. The images of its two factors are open and disjoint, since any point in both images would give a related pair inside the rectangle. This proves Hausdorff separation. Write $p_X:G\to X$ for the projection. For a compact neighborhood $C$ of $g$ in $G$, any ambient open cover of $p_X(C)$ pulls back by continuity to an ambient open cover of $C$. A finite subcover of $C$ then gives a finite subcover of $p_X(C)$ by the corresponding original sets. By [F13] this proves that $p_X(C)$ is compact. It contains the open image of an open neighborhood of $g$ lying in $C$, so $X$ is locally compact. The open cosets of $Z$ cover $H$, and [F13] gives a finite subcover of any compact subset of $H$ by these disjoint cosets. Thus a compact set meets only finitely many cosets. The kernel description in step 1.1 makes $Z$ a closed subgroup of $G$, hence locally compact Hausdorff by intersecting compact neighborhoods with $Z$. By [F8] it has right Haar measure, which is also left invariant since $Z$ is abelian. The cosets are open and closed and at most countably many, with rational matrices as representatives. Choose the first representative in a fixed enumeration of the rational invertible matrices for each coset. For each coset $cZ$, extend its transported measure to Borel subsets $E$ of $H$ by $\nu_c(E)=\mu_Z(\{z\in Z:cz\in E\})$, where $\mu_Z$ is the Haar measure on $Z$. The map $z\mapsto cz$ is continuous into $H$, so [F7] gives Borel preimages, and preimages preserve empty sets and disjoint unions. All the $\nu_c$ are Borel measures on $H$, so [F16] gives countable additivity of $\nu=\sum_{cZ}\nu_c$. Its restriction to $Z$ is $\mu_Z$, so it is nonzero. Compact sets meet only finitely many cosets, so the measure is finite on compact sets. Inner regularity on open sets follows by compact approximation in finitely many cosets at a time. For a Borel set of finite measure, the given countable choice supplies open approximations in the cosets with summable errors, giving outer regularity. Left and right translation permute the cosets and act there by translations in the transported $Z$ coordinates, since $Z$ is central. Thus $H$ is unimodular. By [F8] the modular functions agree, so the quotient Haar theorem gives the nonzero right-invariant Radon measure on $X$, unique up to scale. [given, F7, F8, F10, F13, F16, step 1.1]

3.1 Every positive-determinant matrix is a positive scalar times a determinant-one matrix, by division by the positive square root of its determinant. The scalars act trivially by step 1.2. The group restriction in [F11], transported to the given real Hilbert representation by the unitary equivalence in step 2.1, splits the restriction to $\mathrm{SL}_2(\mathbb R)$ into the holomorphic and antiholomorphic discrete series. These are closed irreducible constituents for the positive-determinant group as well, since the additional scalar factor acts trivially. In the convention of [F11] all rotation weights of the holomorphic series are bounded below by $2$ and those of the antiholomorphic series are bounded above by $-2$. The full $\mathrm O(2)$-spectrum in [F11] gives one line of each nonzero even rotation weight and no other weights. The weights must therefore lie in the constituent of their sign, giving $2,4,6,\ldots$ and $-2,-4,-6,\ldots$, respectively. The two constituents are orthogonal by the Hilbert decomposition into rotation types in [F11]. The reflection $s=\operatorname{diag}(1,-1)$ conjugates $r_\theta$ to $r_{-\theta}$, so it exchanges the two closed constituents. [F11, step 1.2, step 2.1]

3.2 Let $U(\mathbb A)=\{u(x):x\in\mathbb A\}$ with $u(x)=\begin{pmatrix}1&x\\0&1\end{pmatrix}$, and let $U(\mathbb Q)$ use rational $x$. The equations $g_{11}=g_{22}=1$ and $g_{21}=0$ at each place define $U(\mathbb A)$ as a closed subgroup. The coordinate projections are continuous in the restricted-product topology. Its rational subgroup is the intersection with the closed discrete rational matrix group, hence is closed and discrete. Both unipotent groups are abelian by $u(x)u(y)=u(x+y)$. The same compact-neighborhood argument as in step 2.2 gives local compactness of these closed subgroups, and [F8] gives their unimodularity. Thus the quotient Haar theorem applies to $Y$, $U(\mathbb Q)\backslash G$ and $U(\mathbb A)\backslash G$, with the closed discrete rational matrix group supplying the subgroup for $Y$. Use the quotient measure on $Y$ for the almost-everywhere classes and the measure on $X$ of step 2.2 for the norm. In [F9] the central quotient has finite volume, and the measures on the two unipotent quotients can be normalized compatibly with the additive Haar probability in the constant term. The central character is unitary and trivial on rational scalars by hypothesis. These are the measured quotients and the character conditions for [F9]. [given, F8, F9, step 2.2]

4.1 Let $D$ be the subspace of smooth cuspidal classes used to generate the closure in the Statement. On $X$, the invariant measure giving the norm in the model of [F9] is $c>0$ times the measure defining the given norm by step 2.2. Thus the identity on smooth representatives defines a linear map $T$ on $D$ into that central-character Hilbert space, with $\|Tf\|_{\mathrm{std}}=\sqrt c\,\|f\|$ and hence the same norm-zero representatives. The domain $D$ is dense in the stated cuspidal closure by definition, and the target is Banach for its Hilbert norm. With the given countable choice, [F14] yields the unique bounded extension of $T$ to that closure. The norm equality extends by continuity, so the map scaled by $c^{-1/2}$ is an isometry onto its image. It intertwines right translations because the equality holds on $D$ and both actions and the extended map are continuous. Every smooth representative in the generating cuspidal space has zero constant term, so each pairing in [F9] vanishes on it. Each kernel is closed, hence the image of the square-integral closure in the Statement lies in the standard cuspidal subspace. The closed Hilbert subspace realizing $\Pi$ is complete by [F14] and [F17]. A Cauchy sequence in its image under the scaled isometry pulls back to a Cauchy sequence in $\Pi$ and therefore converges to an image point. Thus this image is complete and, under the given countable choice, closed by [F17]. The isometry intertwines the actions, so its image is an irreducible unitary subrepresentation of the standard cuspidal space with the stated central character and real type. [F9, F14, F17, step 3.2, given]

5.1 Apply the correspondence in [F1] to the subrepresentation from step 4.1, using the full inducing pair checked in step 1.2 and its given central character. It produces the normalized classical newform $f$ and its adelic newform $\Phi$ at level $N$. For each prime $q$ and each positive $n$ the comparison in [F1] uses conjugation by $W_n=\begin{pmatrix}0&1\\-q^n&0\end{pmatrix}$ from the upper-left group onto the bottom-row group. In fact the conjugate of a matrix with entries $a,b,c,d$ in row order has entries $d,-c/q^n,-q^n b,a$ in row order. The action of $W_n$ transports fixed spaces isomorphically. For each $q$, [F4] and [F15] give an irreducible admissible generic smooth factor and a nonzero fixed vector at its least upper-left exponent. A vector fixed by any of the congruence groups is smooth because the group is open. At positive exponents the displayed transport therefore identifies the relevant fixed spaces. At zero the bottom-row congruences are vacuous. By the zero-exponent calculation in the congruence-group definition cited in [F1], the integral matrices with unit upper-left entry generate the full integral group. Hence the source’s literal zero test fixes exactly the vectors fixed by $\mathrm{GL}_2(\mathbb Z_q)$. This is also the zero factor in its global level group. Thus the least exponents in the bottom-row convention exist and agree with those in the upper-left convention at every prime. They are zero outside finitely many primes because the tensor product has spherical reference vectors there. The finite conductor $C$ in our convention consequently equals $N$. Since $\pi_\ell$ is unramified, [F2] gives $\ell\nmid N$. [F1, F2, F4, F15, step 1.2, step 4.1, given]

6.1 The nonzero vector $\Phi$ lies in the given irreducible unitary representation, so the closed span of its right translates is that representation. The unitary equivalence between the representation generated by $\Phi$ and $\Pi$ restricts to the embedded local group. The isotypic restriction in the external input identifies its irreducible local factor with $\pi_\ell$ up to unitary equivalence. By [F4] its smooth vectors form an irreducible admissible representation. The integral subgroup $K$ is open in the local topology, so every Hilbert vector fixed by $K$ is smooth. Unramifiedness thus gives a nonzero smooth $K$-fixed space, which is a line by [F4] and the given countable choice. The Hilbert $K$-fixed space is this same line. The fixed space of the Hilbert sum is the Hilbert sum of these lines, since the coordinate projections commute with $K$. Each Hecke operator therefore acts on the global $K$-fixed space with the same scalar as on the local line. In particular this applies to the class of $\Phi$, which is $K$-fixed since $\ell\nmid N$. [given, F1, F4, step 5.1]

6.2 For $k\in K_0(N)$, split off the central finite unit tuple whose scalar at each $q\mid N$ is the upper-left entry of $k_q$ and is $1$ elsewhere. Dividing $k$ by this tuple leaves an element of the upper-left level group of [F1]. Every finite unit tuple of residue $1$ modulo $N$ gives a scalar in that level group, so its central character is one on the nonzero vector $\Phi$. Hence $\Phi(gk)=\chi(a(k))\Phi(g)$ for a character $\chi$ on the units modulo $N$, induced by $\omega$. For $\gamma\in\Gamma_0(N)$, left rational invariance gives $\Phi(\gamma_\infty h_\infty)=\Phi(h_\infty\gamma_f^{-1})$, with $\gamma_f$ denoting $\gamma$ at all finite places. By [F5] the residues of the entries of $\gamma_f$ agree with their ordinary integer residues. The upper-left residue of $\gamma_f^{-1}$ is the class of $d_\gamma$, by the determinant-one inverse formula. Using the real restriction in [F1] and composition of the slash action, this gives $((f|_2\gamma)|_2h)(i)=\chi(d_\gamma)(f|_2h)(i)$ for every positive-determinant $h$. By [F3] and the nonzero real restriction, $\chi(d_\gamma)=\epsilon(d_\gamma)$. Every unit class is realized by $d_\gamma$, since for integer representatives $d,a$ of that class and its inverse, the matrix with rows $(a,(ad-1)/N)$ and $(N,d)$ belongs to $\Gamma_0(N)$. Thus $\chi=\epsilon$. [F1, F3, F5, step 5.1]

7.1 Use the invariant quotient measure of step 2.2. Right translation on $X$ is a homeomorphism because it descends from right translation on $G$ through the quotient topology, with inverse given by translation by the inverse element. The right translates of any nonempty open set cover $X$ by transitivity. If the set were null, its translates would be null by invariance. For each compact subset of $X$, the ambient open cover by these translates has a finite subcover by [F13]. Finite subadditivity then makes the compact subset null. Inner regularity on the open space $X$ would then force the measure to be zero. For either of the two operators $T$ in [F4], let $s$ be its scalar from step 6.1. The function $D(g)=(T\Phi)(g)-s\Phi(g)$ is continuous because $\Phi$ is a smooth adelic newform and $T$ is a finite sum of translates. It is left rationally invariant and has central covariance by $\omega$ because right translations commute with both left actions. Thus $|D|^2$ descends to a continuous function on $X$ by [F7] and the unit modulus of $\omega$. By [F7] the continuous descended function is Borel measurable on $X$. The integral of this nonnegative function is the squared norm of the zero Hilbert class by step 6.1, so the function vanishes almost everywhere by [F7]. Its nonzero set would be an open set of positive measure if it were nonempty, so $T\Phi=s\Phi$ holds pointwise on $G$. [F1, F4, F7, F13, step 2.2, step 6.1]

7.2 For an idele $x\in\mathbb A^\times$, set $r(x)=\prod_q q^{v_q(x_q)}\in\mathbb Q_{>0}$ and $\eta(x)=\epsilon((x_f/r(x))\bmod N)$, reducing the finite tuple of units by [F5]. The product is finite because an idele has unit components outside a finite set. For each finite prime $q$, the rational valuation formula in [F5] gives $v_q(r(x))=v_q(x_q)$. Thus the quotient has unit components at every finite prime and reduction is defined. By additivity of local valuations in [F5], $v_q(x_q y_q)=v_q(x_q)+v_q(y_q)$, so $r(xy)=r(x)r(y)$. The residue map and the character law give $\eta(xy)=\eta(x)\eta(y)$, and these character values have modulus one. For a nonzero rational $t=m/n$ with $n>0$, factor $|m|$ and $n$ into primes using [F5]. The difference of their exponents at $q$ is $v_q(t)$, so $r(t)=|m|/n=|t|$ and the finite quotient is its sign. The identity $\epsilon(-1)=1$ follows from the weight-two transformation at $-I$ and $f\ne0$, so $\eta$ is trivial on rational scalars. It is trivial on ideles supported at the real place. Define $\Phi_b(g)=\eta(\det g)^{-1}\Phi(g)$. It is left rationally invariant and has the same real restriction as $\Phi$. For $k\in K_0(N)$, $\eta(\det k)=\epsilon(a(k)d(k))$, since all its local determinants are units and the lower-left entries of $k$ vanish upon reduction at the required prime powers. The covariance in step 6.2 gives $\Phi_b(gk)=\epsilon(d(k))^{-1}\Phi_b(g)$. [F3, F5, step 6.2]

8.1 For a matrix inserted at $\ell$ with determinant valuation $e$, $\eta$ on its determinant has value $\epsilon(\ell)^{-e}$. Indeed the rational factor is $\ell^e$, while the finite entries at $q\mid N$ are $1$ before division. As $\ell\nmid N$, at each such prime the residue of $\ell^{-e}$ is the inverse of the ordinary residue of $\ell^e$ by [F5]. All cosets in $\mathcal T_\ell$ have $e=1$, and the scalar coset in $\mathcal R_\ell$ has $e=2$. Thus each scalar on $\Phi_b$ is the corresponding scalar on $\Phi$ multiplied by $\epsilon(\ell)^e$, by the pointwise eigenvalue equation from step 7.1, the finite-translate formula and multiplicativity of $\eta\circ\det$. In particular both operators act by scalars on $\Phi_b$. Applying [F6] to its covariance and real restriction, and [F4] to the original scalars, gives $a_\ell=\epsilon(\ell)\sqrt\ell\,(u_\ell+v_\ell)$ and $\epsilon(\ell)=\epsilon(\ell)^2u_\ell v_\ell$. Consequently $\sqrt\ell\,\epsilon(\ell)u_\ell$ and $\sqrt\ell\,\epsilon(\ell)v_\ell$ have sum $a_\ell$ and product $\ell\epsilon(\ell)$. By [F12], $\lambda_\ell=a_\ell$ for this normalized newform at $\ell\nmid N$. Thus these are the roots of $X^2-\lambda_\ell X+\ell\epsilon(\ell)$, counted with multiplicity. By [F3] both have modulus $\sqrt\ell$, and $|\epsilon(\ell)|=1$ because $\ell\nmid N$. Dividing yields $|u_\ell|=|v_\ell|=1$. [F3, F4, F5, F6, F12, step 5.1, step 7.1, step 7.2]

9.1 Under the extra hypothesis of trivial local scalar action, two lifts in the local matrix group of the same projective element differ by a scalar matrix. They act identically on every Hilbert vector. Thus $\bar\pi_\ell(p(g))=\pi_\ell(g)$ defines an action on the local Hilbert space, with the product law inherited from multiplication of representatives. The orbit maps of $\bar\pi_\ell$ are continuous: their composites with $p$ are the continuous orbit maps of $\pi_\ell$, and $p$ has the quotient topology by [F7]. A vector fixed by $p(K)$ is exactly one fixed by $K$ after pullback, since every element of $p(K)$ has a lift in $K$. This line is the spherical line of [F4], and the Satake pair of the pullback is the pair bounded in step 8.1. [given, F4, F7, step 6.1, step 8.1] ∎
