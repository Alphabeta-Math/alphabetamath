---
title: Definite quaternion transfer to cuspidal weight two
status: published
research_item: thm-definite-quaternion-jacquet-langlands-weight-two
dependency_level: 7
sources:
  references:
    - title: The Jacquet–Langlands Correspondence for GL2 (Stanford seminar notes)
      url: https://math.stanford.edu/~conrad/JLseminar/Notes/L20.pdf
      locator: §2, Theorem 2.1, pp. 2–3, with the local correspondence in Theorem 1.2
      statement: For a quaternion algebra over a global field of characteristic
        different from two and a fixed smooth idele class character, the
        irreducible quaternion automorphic representations of dimension greater
        than one with that central character inject into the irreducible
        cuspidal automorphic representations of the split adelic GL(2) with the
        same central character. The paired factors are equivalent at each split
        place and related by local Jacquet–Langlands at each ramified place.
      hypotheses: Use the number field Q, its rational Hamilton division algebra and
        the trivial central character. The quaternion representation must be
        irreducible automorphic and have dimension greater than one.
      reading_limits: Checked the forward theorem and its local compatibility
        conditions. The global proof and the characterization of the image are
        outside this use.
    - title: Ioan Alexandru Badulescu and David Renard, Unitary Dual of GL(n) at
        Archimedean Places and Global Jacquet–Langlands Correspondence
      url: https://arxiv.org/pdf/0905.4143
      locator: §1.5, p. 5, paragraph before Theorem 1.4, and §16, p. 41, finite local
        factors and spherical vectors
      statement: A discrete automorphic representation of the adelic unit group of a
        central simple algebra over a number field, or of the split form, is a
        restricted Hilbert tensor product of irreducible unitary local
        representations. Its local factors are determined by the discrete
        representation, and the finite factors have maximal-compact fixed
        vectors at almost all places.
      hypotheses: The global representation is an irreducible subrepresentation of
        square-integrable right translation with a fixed unitary central
        character trivial on rational central points. Apply this to the full
        Hamilton units and the split GL(2).
      reading_limits: Checked the fixed-character discrete-spectrum definition, the
        Hilbert tensor-product statement and the assertion of sphericality at
        almost all finite places. The referenced factorization proof is
        imported.
    - title: The Jacquet–Langlands Correspondence for GL2 (Stanford seminar notes)
      url: https://math.stanford.edu/~conrad/JLseminar/Notes/L20.pdf
      locator: §1.3, p. 1, real parametrizations and local transfer formula
      statement: The real local correspondence pairs the Hamilton representation with
        positive-scalar character ω+ and norm-one factor Sym^n(C²) with the real
        GL(2) discrete series having positive-scalar character ω+ and lowest
        absolute rotation weight n+2. The latter restricts to the holomorphic
        and antiholomorphic discrete series of that weight on SL(2,R).
      hypotheses: The quaternion algebra is the real Hamilton algebra. For a fixed
        central character, the parity of n is determined by its value at −1. Use
        the trivial positive-scalar character and n=0.
      reading_limits: Checked the parametrization and restriction formula. Only the
        trivial Hamilton representation is used in this application.
    - title: A. Raghuram and Naomi Tanabe, Notes on the Arithmetic of Hilbert Modular
        Forms
      url: https://tildesites.bowdoin.edu/~ntanabe/hilbert_arithmetic.pdf
      locator: (4.1)–(4.4), pp. 26–27, §4.1.3, p. 28, Theorem 4.9, p. 30, and §4.3,
        (4.13)–(4.14), Theorem 4.15 and the prime-eigenform and normalization
        paragraphs, pp. 32–33
      statement: From a cuspidal GL(2) representation with the prescribed real
        discrete-series weights, conductor and adelized central character, §4.3
        constructs a holomorphic Hilbert cusp form whose lift belongs to that
        representation. The constructed form has ideal coefficient c(O,f)=1 and
        is an eigenform for the prime operators away from the level and
        different. Formula (4.4) on the decomposition (4.2) gives the lift.
        Section 4.1.3 gives the degeneracy translates and Petersson pairing.
        Theorem 4.9 gives irreducible admissible local factors.
      hypotheses: Use the rational field, whose narrow class group and different are
        trivial, weight two, and trivial adelic central character. The real
        discrete series has lowest absolute weight two. Over Q the level ideal
        has a unique positive generator.
      reading_limits: Use the decomposition and lift, degeneracy and pairing formulas,
        irreducible admissible factorization, and §4.3 construction with
        first-coefficient normalization and the prime-eigenform conclusion. The
        classical newness argument uses proper lower levels and the Corbett–Saha
        inverse lift. The finite all-index operator and its action on the
        newform line are derived locally.
    - title: Peter Humphries, Archimedean Newform Theory for GL(n)
      url: https://www.cambridge.org/core/services/aop-cambridge-core/content/view/5B8EF22457D0AAB4E6282B6ABEAC5032/S1474748024000227a.pdf/archimedean_newform_theory_for_operatorname_mathrm_gln.pdf
      locator: §5.2.4, p. 68, paragraph at the global Whittaker coefficient, §2.2.4,
        p. 46, and §3.1, p. 51, congruence subgroup, Theorem 3.1 and Definition
        3.2
      statement: The finite smooth local factors of a cuspidal automorphic GL(n)
        representation are generic, irreducible and admissible. A generic
        irreducible admissible smooth representation over a nonarchimedean local
        field is isomorphic to an irreducible induced representation of
        Langlands type. For an induced representation of Langlands type, Theorem
        3.1 gives a least nonnegative index with nonzero fixed vectors for the
        last-row congruence subgroup K1. Definition 3.2 defines the local
        conductor ideal as the maximal ideal of the valuation ring raised to
        that index.
      hypotheses: For local genericity use a cuspidal automorphic representation over
        a number field. The local newvector theorem uses an induced
        representation of Langlands type over a nonarchimedean local field. Here
        n=2 and the fields are Q_q.
      reading_limits: Checked finite local genericity, the Langlands classification
        implication and the nonarchimedean fixed-vector and conductor
        definitions. This application uses the minimal index and its conductor
        interpretation in degree two.
    - title: Andrew Corbett and Abhishek Saha, On the Order of Vanishing of Newforms
        at Cusps
      url: https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf
      locator: §2.1.1, p. 6, the definition of U₀, §§2.1.4–2.1.5, p. 8, equation (8)
        and the definition of a(π), and §3.1, pp. 16–17, the definitions of N
        and K1(N) and equations (21)–(22)
      statement: For an irreducible unitary cuspidal GL(2) representation over Q with
        real discrete series of lowest weight k≥2 and central character trivial
        on the positive reals, the associated holomorphic newform has level N
        equal to the product of the local conductor prime powers. The local
        exponent is the least index with a nonzero fixed space for the test in
        (8). At positive index it requires the upper left entry congruent to one
        and the lower left entry congruent to zero. At zero the literal local
        formula requires a unit upper left entry. The global product K1(N) in
        §3.1 uses the full integral group at primes not dividing N. The smooth
        automorphic vectors fixed by K1(N) and transforming by exp(ikθ) in (21)
        form a one-dimensional space. Equation (22) recovers the classical
        newform of weight k, level N and the Dirichlet character associated to
        the central character.
      hypotheses: Use the rational unitary cuspidal representation whose real GL(2)
        factor is the discrete series of lowest weight two with trivial central
        character. The local test concerns irreducible admissible generic finite
        factors.
      reading_limits: Use the literal local test, the global congruence product,
        uniqueness with the stated rotation character, and the inverse lift. The
        equivalence of the finite fixed-space tests and the identification of
        the lifted vector are proved locally.
    - title: Bachir Bekka, Pierre de la Harpe and Alain Valette, Kazhdan’s Property
        (T)
      url: https://ncatlab.org/nlab/files/BekkaHarpeValetteOnKashdanPropertyT.pdf
      locator: Appendix B, §B.1, Corollary B.1.7, printed p. 349
      statement: If a homogeneous space G/H admits a nonzero invariant measure, that
        measure is unique up to multiplication by a positive constant.
      hypotheses: A locally compact group G and a closed subgroup H under the
        conventions of Appendix B. Use the quotients of the full adelic unit
        groups by the closed subgroups generated by rational points and central
        ideles. Inversion identifies their right actions on left cosets with
        left actions on right cosets.
      reading_limits: Checked the uniqueness clause of Corollary B.1.7. Existence of
        the quotient measures is supplied by the two local automorphic-space
        definitions.
    - title: William Casselman, Introduction to the Theory of Admissible
        Representations of p-adic Reductive Groups
      url: https://www.math.utah.edu/~ptrapa/math-library/casselman/casselman-p-adic-book.pdf
      locator: §2.1, Proposition 2.1.15, p. 23 of the 1 May 1995 draft
      statement: An irreducible unitary admissible smooth representation has a unique
        invariant Hermitian inner product up to scalar multiplication.
      hypotheses: A smooth irreducible admissible representation of a reductive group
        over a nonarchimedean local field with a positive invariant Hermitian
        inner product. Use the split finite GL(2) factors before quotienting by
        scalars.
      reading_limits: Checked the stated uniqueness proposition. Only the comparison
        of the two existing invariant inner products is used.
    - title: Neven Grbac and Joachim Schwermer, An Exercise in Automorphic Cohomology
        – The Case GL2 over a Quaternion Algebra
      url: https://www.math.uniri.hr/~ngrbac/GS_Kudla_revised.pdf
      locator: Chapter I, §§1.4–1.8, pp. 5–6, especially the last paragraph of §1.8
      statement: The smooth K-finite model of an irreducible constituent of the
        fixed-character cuspidal Hilbert spectrum consists of cuspidal
        automorphic forms, square-integrable modulo the center. Such forms have
        identically zero constant term along every proper standard rational
        parabolic, with Haar probability on the unipotent quotient.
      hypotheses: A connected reductive group over Q, an irreducible cuspidal
        constituent and a unitary central character trivial on the rational
        center. Apply this to split GL(2), the trivial character and the upper
        triangular parabolic.
      reading_limits: Checked the smooth function convention, constant term, and
        identification of cuspidal automorphic representations with smooth
        K-finite models in the cuspidal Hilbert spectrum. Only one nonzero
        vector in this model is used. The closed-span argument and the passage
        to the projective quotient are proved locally.
---

## Prerequisites

- [math:thm-extension-of-a-bounded-map-from-a-dense-subspace](https://alphabetamath.cc/item/thm-extension-of-a-bounded-map-from-a-dense-subspace)
- [math:def-hilbert-space](https://alphabetamath.cc/item/def-hilbert-space)
- [def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)
- [math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring)
- [math:def-radon-measure-on-an-lch-space](https://alphabetamath.cc/item/def-radon-measure-on-an-lch-space)
- [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [def-author-5b8600b4f4af-full-adelic-hamilton-group](item-def-author-5b8600b4f4af-full-adelic-hamilton-group)
- [def-definite-quaternion-automorphic-fixed-space](item-def-definite-quaternion-automorphic-fixed-space)
- [def-author-34e2e6a0519f-split-adelic-matrix-groups](item-def-author-34e2e6a0519f-split-adelic-matrix-groups)
- [def-author-34e2e6a0519f-split-cuspidal-spectrum](item-def-author-34e2e6a0519f-split-cuspidal-spectrum)
- [def-author-34e2e6a0519f-real-weight-two-discrete-series](item-def-author-34e2e6a0519f-real-weight-two-discrete-series)
- [def-author-5b8600b4f4af-split-unramified-quaternion-representation](item-def-author-5b8600b4f4af-split-unramified-quaternion-representation)
- [thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character)
- [def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)
- [thm-hurwitz-integral-splitting-at-odd-primes](item-thm-hurwitz-integral-splitting-at-odd-primes)
- [def-author-e2fc0f4318ab-weight-two-cusp-form](item-def-author-e2fc0f4318ab-weight-two-cusp-form)
- [def-author-e2fc0f4318ab-normalized-weight-two-newform](item-def-author-e2fc0f4318ab-normalized-weight-two-newform)
- [math:def-dirichlet-character-modulo-q](https://alphabetamath.cc/item/def-dirichlet-character-modulo-q)
- [lem-author-34e2e6a0519f-projective-automorphic-passage](item-lem-author-34e2e6a0519f-projective-automorphic-passage)
- [lem-author-34e2e6a0519f-spherical-action-under-equivalence](item-lem-author-34e2e6a0519f-spherical-action-under-equivalence)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [def-author-6f52147f3ab3-finite-quaternion-ideles](item-def-author-6f52147f3ab3-finite-quaternion-ideles)
- [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)
- [math:lem-nrqm-composites-hilbert-tensor-construction](https://alphabetamath.cc/item/lem-nrqm-composites-hilbert-tensor-construction)
- [math:thm-metric-completion-carries-a-unique-banach-space-structure](https://alphabetamath.cc/item/thm-metric-completion-carries-a-unique-banach-space-structure)
- [math:thm-completion-of-an-inner-product-space-is-hilbert](https://alphabetamath.cc/item/thm-completion-of-an-inner-product-space-is-hilbert)
- [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)
- [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals)
- [math:thm-bezout-identity](https://alphabetamath.cc/item/thm-bezout-identity)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative)
- [math:cor-inverse-matrix-by-adjugate](https://alphabetamath.cc/item/cor-inverse-matrix-by-adjugate)
- [` The Jacquet–Langlands Correspondence for GL2 (Stanford seminar notes) · §2, Theorem 2.1, pp. 2–3, with the local correspondence in Theorem 1.2 `](https://math.stanford.edu/~conrad/JLseminar/Notes/L20.pdf)
- [` Ioan Alexandru Badulescu and David Renard, Unitary Dual of GL(n) at Archimedean Places and Global Jacquet–Langlands Correspondence · §1.5, p. 5, paragraph before Theorem 1.4, and §16, p. 41, finite local factors and spherical vectors `](https://arxiv.org/pdf/0905.4143)
- [` The Jacquet–Langlands Correspondence for GL2 (Stanford seminar notes) · §1.3, p. 1, real parametrizations and local transfer formula `](https://math.stanford.edu/~conrad/JLseminar/Notes/L20.pdf)
- [` A. Raghuram and Naomi Tanabe, Notes on the Arithmetic of Hilbert Modular Forms · (4.1)–(4.4), pp. 26–27, §4.1.3, p. 28, Theorem 4.9, p. 30, and §4.3, (4.13)–(4.14), Theorem 4.15 and the prime-eigenform and normalization paragraphs, pp. 32–33 `](https://tildesites.bowdoin.edu/~ntanabe/hilbert_arithmetic.pdf)
- [` Peter Humphries, Archimedean Newform Theory for GL(n) · §5.2.4, p. 68, paragraph at the global Whittaker coefficient, §2.2.4, p. 46, and §3.1, p. 51, congruence subgroup, Theorem 3.1 and Definition 3.2 `](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/5B8EF22457D0AAB4E6282B6ABEAC5032/S1474748024000227a.pdf/archimedean_newform_theory_for_operatorname_mathrm_gln.pdf)
- [` Andrew Corbett and Abhishek Saha, On the Order of Vanishing of Newforms at Cusps · §2.1.1, p. 6, the definition of U₀, §§2.1.4–2.1.5, p. 8, equation (8) and the definition of a(π), and §3.1, pp. 16–17, the definitions of N and K1(N) and equations (21)–(22) `](https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf)
- [` Bachir Bekka, Pierre de la Harpe and Alain Valette, Kazhdan’s Property (T) · Appendix B, §B.1, Corollary B.1.7, printed p. 349 `](https://ncatlab.org/nlab/files/BekkaHarpeValetteOnKashdanPropertyT.pdf)
- [` William Casselman, Introduction to the Theory of Admissible Representations of p-adic Reductive Groups · §2.1, Proposition 2.1.15, p. 23 of the 1 May 1995 draft `](https://www.math.utah.edu/~ptrapa/math-library/casselman/casselman-p-adic-book.pdf)
- [` Neven Grbac and Joachim Schwermer, An Exercise in Automorphic Cohomology – The Case GL2 over a Quaternion Algebra · Chapter I, §§1.4–1.8, pp. 5–6, especially the last paragraph of §1.8 `](https://www.math.uniri.hr/~ngrbac/GS_Kudla_revised.pdf)


## Statement

Assume the Axiom of Choice. Let $B$ be the rational Hamilton quaternion algebra with basis $1,i,j,k$ and the relations $i^2=j^2=-1$ and $ij=k=-ji$. Its scalar extension $B_{\mathbb R}=B\otimes_{\mathbb Q}\mathbb R$ is the real Hamilton division algebra. Let $G=PB^\times$ be its group of units modulo scalars. Let $\pi$ be a non-one-dimensional irreducible automorphic representation of $G(\mathbb A)$, meaning an irreducible unitary constituent of right translation on $L^2(G(\mathbb Q)\backslash G(\mathbb A))$ for a nonzero right-invariant Radon measure on the quotient. Here a Radon measure is a Borel measure finite on compact sets, outer regular on Borel sets and inner regular on open sets. Assume the real component $\pi_\infty$ is trivial, meaning the real projective units act as the identity.

Its global Jacquet–Langlands transfer is an irreducible cuspidal representation $\Pi$ of $\mathrm{PGL}_2(\mathbb A)$. Cuspidality means occurrence under right translation in the square-integral closure of the continuous square-integrable functions on the split automorphic quotient whose upper unipotent constant term vanishes at every translate. The constant term averages along the matrices with ones on the diagonal, zero below it and an upper right entry ranging over $\mathbb Q\backslash\mathbb A$ with Haar probability measure. The split quotient uses a nonzero right-invariant Radon measure. The real component of $\Pi$ has weight-two discrete-series type, with the holomorphic and antiholomorphic weight-two models on restriction to determinant-one real matrices.

At every split finite prime $\ell$, meaning $B\otimes_{\mathbb Q}\mathbb Q_\ell\simeq M_2(\mathbb Q_\ell)$, the local factors $\pi_\ell$ and $\Pi_\ell$ are unitarily equivalent under the resulting identification with $\mathrm{PGL}_2(\mathbb Q_\ell)$. Here local factors are the single-place representations on the Hilbert spaces in the restricted tensor product of the full-unit pullbacks. Choose a unit reference vector $e_v$ in each Hilbert space, fixed by the subgroup defining the restricted product of the adelic group at almost every finite place. The restricted Hilbert tensor product is the completion of the span of elementary tensors whose entries are $e_v$ outside a finite set. Finite sets of places give ordinary finite tensor products, identified by inserting the reference vectors at the added places. The pairing of elementary tensors $\bigotimes_v x_v$ and $\bigotimes_v y_v$ is the finite product of the local pairings $\langle x_v,y_v\rangle$ over the places where either entry differs from $e_v$. The action applies each local operator to its own entry and extends by continuity. The local factors are strongly continuous unitary representations. At split finite places their spaces of smooth vectors are irreducible and admissible. A split local factor is unramified when it has nonzero fixed vectors under the image of $\mathrm{GL}_2(\mathbb Z_\ell)$. The two factors are unramified at the same split primes and there their spherical Hecke eigencharacters agree. Such a character gives the scalar on the fixed line of each compactly supported function invariant on both sides under that subgroup, with one term per coset in its action. Every odd prime is split. At each odd prime use a splitting carrying the completed Hurwitz order onto $M_2(\mathbb Z_\ell)$ for both the local comparison and the unramified test. It identifies the projective image of the Hurwitz order's units with the image of $\mathrm{GL}_2(\mathbb Z_\ell)$.

The representation $\Pi$, viewed on $\mathrm{GL}_2(\mathbb A)$ by composition with the scalar quotient, is generated by the unitary adelic lift of a normalized holomorphic weight-two cuspidal newform $f$ on $\Gamma_0(N)$ for some positive integer $N$. Here $\Gamma_0(N)$ consists of determinant-one integral matrices with lower left entry divisible by $N$. The form is new in the sense of orthogonality to the lower-level forms pulled to level $N$, is an eigenform for the classical weight-two Hecke operator $T_m$ at every positive integer $m$ and has first coefficient one in its Fourier expansion in $q=\exp(2\pi i z)$. Its Dirichlet character is trivial, meaning it is one on the invertible classes modulo $N$.

For each finite prime $q$, let $a_q$ be the least integer $n\ge0$ for which the full matrix local factor has a nonzero vector fixed by $K_{1,q}(n)$, the subgroup of $\mathrm{GL}_2(\mathbb Z_q)$ with bottom row congruent to $(0,1)$ modulo $q^n\mathbb Z_q$. At $n=0$ this is the full integral group. The exact level is the finite conductor $N=\prod_q q^{a_q}$, with only finitely many $a_q>0$. At each split unramified prime $\ell$ one has $\ell\nmid N$.

For the lift, write $g=\gamma g_\infty k$, where the rational factor $\gamma$ is an element of $\mathrm{GL}_2(\mathbb Q)$ embedded diagonally by using the same matrix at every place. Here $g_\infty\in\mathrm{GL}_2(\mathbb R)$ has positive determinant and is supported at the real place, and $k\in K_0(N)$ is supported at the finite places. $K_0(N)$ is the product over primes $q$ of the subgroups of $\mathrm{GL}_2(\mathbb Z_q)$ with lower left entry in $q^{v_q(N)}\mathbb Z_q$, where $v_q$ is the normalized valuation on $\mathbb Q_q$ and $v_q(N)$ is the exponent of $q$ in $N$. The lift is the well-defined function $\phi_f(g)=(f|_2g_\infty)(i)$, with $i$ the imaginary unit and $(f|_2 A)(z)=\det(A)(cz+d)^{-2}f((az+b)/(cz+d))$ for a positive-determinant matrix $A$ with rows $(a,b)$ and $(c,d)$. Generation means taking the closed linear span of the right translates of $\phi_f$ in the cuspidal space.

## Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)

[math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring)

[math:def-radon-measure-on-an-lch-space](https://alphabetamath.cc/item/def-radon-measure-on-an-lch-space)

[def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)

[def-author-5b8600b4f4af-full-adelic-hamilton-group](item-def-author-5b8600b4f4af-full-adelic-hamilton-group)

[def-definite-quaternion-automorphic-fixed-space](item-def-definite-quaternion-automorphic-fixed-space)

[def-author-34e2e6a0519f-split-adelic-matrix-groups](item-def-author-34e2e6a0519f-split-adelic-matrix-groups)

[def-author-34e2e6a0519f-split-cuspidal-spectrum](item-def-author-34e2e6a0519f-split-cuspidal-spectrum)

[def-author-34e2e6a0519f-real-weight-two-discrete-series](item-def-author-34e2e6a0519f-real-weight-two-discrete-series)

[def-author-5b8600b4f4af-split-unramified-quaternion-representation](item-def-author-5b8600b4f4af-split-unramified-quaternion-representation)

[thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character)

[def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)

[thm-hurwitz-integral-splitting-at-odd-primes](item-thm-hurwitz-integral-splitting-at-odd-primes)

[def-author-e2fc0f4318ab-weight-two-cusp-form](item-def-author-e2fc0f4318ab-weight-two-cusp-form)

[def-author-e2fc0f4318ab-normalized-weight-two-newform](item-def-author-e2fc0f4318ab-normalized-weight-two-newform)

[math:def-dirichlet-character-modulo-q](https://alphabetamath.cc/item/def-dirichlet-character-modulo-q)

[math:lem-nrqm-composites-hilbert-tensor-construction](https://alphabetamath.cc/item/lem-nrqm-composites-hilbert-tensor-construction)

[math:thm-metric-completion-carries-a-unique-banach-space-structure](https://alphabetamath.cc/item/thm-metric-completion-carries-a-unique-banach-space-structure)

[math:thm-completion-of-an-inner-product-space-is-hilbert](https://alphabetamath.cc/item/thm-completion-of-an-inner-product-space-is-hilbert)

## Facts & Assumptions

[F1] The full quaternion adelic unit group is $B_{\mathbb R}^\times\times\widehat B^\times$, with the finite restricted product taken relative to the units of the completed Hurwitz orders. For the rational Hamilton units, the scalar-quotient identifications of adelic groups and rational orbits give the same irreducible constituents and fixed vectors on passing between projective units and full units with trivial scalar action. The same passage applies to split matrices. [def-author-6f52147f3ab3-finite-quaternion-ideles](item-def-author-6f52147f3ab3-finite-quaternion-ideles) [def-author-5b8600b4f4af-full-adelic-hamilton-group](item-def-author-5b8600b4f4af-full-adelic-hamilton-group) [def-definite-quaternion-automorphic-fixed-space](item-def-definite-quaternion-automorphic-fixed-space) [def-author-34e2e6a0519f-split-adelic-matrix-groups](item-def-author-34e2e6a0519f-split-adelic-matrix-groups) [lem-author-34e2e6a0519f-projective-automorphic-passage](item-lem-author-34e2e6a0519f-projective-automorphic-passage)

[F2] The classical degree-two global transfer sends a non-one-dimensional irreducible quaternion automorphic constituent to an irreducible cuspidal constituent with the same central character. It agrees with the quaternion factors at the split places and uses classical local transfer at the nonsplit places. With unitary central character these discrete constituents are restricted Hilbert tensor products of irreducible unitary local representations, with integral-subgroup-fixed reference vectors at almost all finite places. The split matrix factors have irreducible admissible smooth representations at the finite places. A smooth vector is fixed by some open subgroup, and admissibility means that the fixed space of each compact open subgroup is finite dimensional. The smooth cuspidal realization of the transferred constituent supplies a nonzero smooth cusp vector square-integrable modulo the center. Its upper unipotent constant term vanishes identically with Haar probability on the unipotent quotient. See the global transfer, Hilbert factorization, classical newform and smooth cuspidal realization inputs.

[F3] Scalar extension to $\mathbb R$ keeps the Hamilton basis and multiplication table. The resulting algebra is a division algebra by the inverse formula for nonzero real quaternions. [def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions) [math:thm-quaternions-form-a-division-ring](https://alphabetamath.cc/item/thm-quaternions-form-a-division-ring) For the real Hamilton algebra the local transfer takes the representation with positive-scalar character $\omega_+$ and norm-one factor $\operatorname{Sym}^n(\mathbb C^2)$ to the split discrete series with positive-scalar character $\omega_+$ and lowest absolute rotation weight $n+2$. The parity of $n$ is determined by the central character. The split partner restricts to determinant-one real matrices as the direct sum of the holomorphic and antiholomorphic models of that weight. See the real local transfer input and [def-author-34e2e6a0519f-real-weight-two-discrete-series](item-def-author-34e2e6a0519f-real-weight-two-discrete-series).

[F4] At a split prime let $J_\ell$ be the image of $\mathrm{GL}_2(\mathbb Z_\ell)$ under the projective identification. At every odd prime the chosen splitting carries the completed Hurwitz order onto $M_2(\mathbb Z_\ell)$, so its units map onto $\mathrm{GL}_2(\mathbb Z_\ell)$. Any two split algebra identifications differ by conjugation by an invertible matrix. The Axiom of Choice implies countable choice, as required by the spherical fixed-line theorem. An irreducible admissible smooth local factor of a unitary representation has a one-dimensional spherical fixed space if it is unramified. The normalization assigns volume one to the integral subgroup, equivalently one summand per coset. An intertwiner identifies the Hecke actions with this convention. [def-author-5b8600b4f4af-split-unramified-quaternion-representation](item-def-author-5b8600b4f4af-split-unramified-quaternion-representation) [thm-hurwitz-integral-splitting-at-odd-primes](item-thm-hurwitz-integral-splitting-at-odd-primes) [thm-normalized-degree-two-spherical-character](item-thm-normalized-degree-two-spherical-character) [lem-author-34e2e6a0519f-spherical-action-under-equivalence](item-lem-author-34e2e6a0519f-spherical-action-under-equivalence) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice) [def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)

[F5] The rational case of the classical newform input constructs a holomorphic weight-two cusp form of trivial character at the conductor level, with the lift in the given cuspidal representation. It has normalized ideal coefficient at $(1)$ and is an eigenform for the prime operators away from the level. For classical newness apply the inverse lift in [F7] to this same vector. The classical old subspace is the span of $g(tz)$ for $g$ a cusp form on $\Gamma_0(M)$, with $M$ a proper positive divisor of $N$ and $t$ a positive divisor of $N/M$. Newness is orthogonality to this span for the Petersson pairing. The adelic decomposition and slash-action formula in the Statement give the lift. The classical newform input also gives the lower-level degeneracy translates and the normalized Petersson pairing. Use the classical Hecke operators of the normalized-newform definition with the character extended by zero on nonunits. See [def-author-e2fc0f4318ab-weight-two-cusp-form](item-def-author-e2fc0f4318ab-weight-two-cusp-form), [def-author-e2fc0f4318ab-normalized-weight-two-newform](item-def-author-e2fc0f4318ab-normalized-weight-two-newform) and [math:def-dirichlet-character-modulo-q](https://alphabetamath.cc/item/def-dirichlet-character-modulo-q).

[F6] Every finite smooth local factor of a cuspidal matrix representation is irreducible, admissible and generic. Here genericity is the existence of a nonzero Whittaker functional, a linear functional transforming on the upper unipotent subgroup by a nontrivial additive character of the local field. The generic factor is isomorphic to an irreducible induced representation of Langlands type. The finite-place newvector theorem for such an induced representation gives the least congruence index with nonzero $K_{1,q}(n)$-fixed space and identifies the local conductor ideal as $q^{a_q}\mathbb Z_q$. See the finite newvector input.

[F7] The rational classical level is the product of the local conductor prime powers. The local test in Corbett–Saha requires the upper left entry congruent to one and the lower left entry congruent to zero at positive index. At index zero its literal upper-left condition requires a unit, while the global group $K_1(N)$ in their §3.1 uses the full integral group at primes not dividing $N$. In the smooth automorphic model the vectors fixed by this global group and transforming by $e^{ik\theta}$ under the rotations in (21) form a one-dimensional space. The inverse lift in (22) recovers a classical newform at that level, of weight $k$ and with the Dirichlet character attached to the central character. Use unique prime factorization for divisibility of the product. See the conductor product input and [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic).

[F8] The full adelic groups are locally compact Hausdorff, and the two orbit spaces modulo rational points and central ideles are Hausdorff. Their identity cosets are closed, so their inverse images are closed subgroups of the full groups. The orbit homeomorphisms preserve Borel sets, open sets and compact sets, hence preserve Radon regularity in the stated convention. [math:def-radon-measure-on-an-lch-space](https://alphabetamath.cc/item/def-radon-measure-on-an-lch-space) Nonzero invariant Radon measures on these quotients are unique up to positive scale, by inversion and the quotient measure input. Multiplication of the measure by a positive constant leaves the square-integrable classes and closed subspaces unchanged and rescales the norm uniformly. [lem-author-34e2e6a0519f-projective-automorphic-passage](item-lem-author-34e2e6a0519f-projective-automorphic-passage) [def-author-34e2e6a0519f-split-cuspidal-spectrum](item-def-author-34e2e6a0519f-split-cuspidal-spectrum)

[F9] An irreducible unitary admissible smooth representation of a split finite matrix group has only one invariant Hermitian inner product up to positive scale. See the local inner product input.

[F10] For complex Hilbert spaces under countable choice, the product pairing on the algebraic tensor product is an inner product and gives the elementary tensor norm as the product of the factor norms. A normed space has a Banach completion, and the completion of an inner-product space is Hilbert with the extended pairing. [math:lem-nrqm-composites-hilbert-tensor-construction](https://alphabetamath.cc/item/lem-nrqm-composites-hilbert-tensor-construction) [math:thm-metric-completion-carries-a-unique-banach-space-structure](https://alphabetamath.cc/item/thm-metric-completion-carries-a-unique-banach-space-structure) [math:thm-completion-of-an-inner-product-space-is-hilbert](https://alphabetamath.cc/item/thm-completion-of-an-inner-product-space-is-hilbert)

[F11] Fix a positive integer $m$. Use the set $X_m$ of finite adelic matrices consisting of the tuples $x=(x_p)_p$ in the finite adelic matrix group with integral entries everywhere and with $v_p(\det x_p)=v_p(m)$ at every prime $p$. At each $p\mid N$ require the upper left entry to be a unit and the lower left entry to lie in $N\mathbb Z_p$. The corresponding full adelic set is $\mathrm{GL}_2(\mathbb R)^+\times X_m$, where the real determinant is positive. The real group $\mathrm{GL}_2(\mathbb R)^+$ is also the real part of the subgroup acting on the left, so taking cosets there leaves just the finite cosets $K_0(N)x$, each represented with real component the identity. The valuation is additive on products, agrees with the rational valuation on $\mathbb Q^\times$ and vanishes exactly on $\mathbb Z_p^\times$. [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation) [def-author-34e2e6a0519f-split-adelic-matrix-groups](item-def-author-34e2e6a0519f-split-adelic-matrix-groups)

[F12] The ring $\mathbb Z_p$ is the unit ball of $\mathbb Q_p$, whose absolute value on nonzero rational $r$ is $|r|_p=p^{-v_p(r)}$. A rational number is integral if it belongs to every $\mathbb Z_p$, since a prime in the reduced denominator would give absolute value greater than one. Bézout's identity gives an integral linear combination equal to the positive greatest common divisor of two integers that are not both zero. Division by a positive integer has a unique remainder from zero up to one less than the divisor. [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp) [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals) [math:thm-bezout-identity](https://alphabetamath.cc/item/thm-bezout-identity) [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)

[F13] Under countable choice a bounded linear map from a dense normed subspace to a Banach space extends uniquely to a bounded linear map on the ambient normed space. A Hilbert space is Banach in its induced norm. [Extension from a dense subspace](https://alphabetamath.cc/item/thm-extension-of-a-bounded-map-from-a-dense-subspace) [Hilbert space completeness](https://alphabetamath.cc/item/def-hilbert-space)

[F14] The integral subgroup $\mathrm{GL}_2(\mathbb Z_\ell)$ in the split finite matrix group is compact open in its entrywise topology, as shown in the construction of the split cuspidal quotient. The ring $\mathbb Z_\ell$ is open in $\mathbb Q_\ell$, and field multiplication by a nonzero constant and addition by a constant are homeomorphisms. Give the local scalar quotient the quotient topology. [def-author-34e2e6a0519f-split-cuspidal-spectrum](item-def-author-34e2e6a0519f-split-cuspidal-spectrum) [def-author-34e2e6a0519f-split-adelic-matrix-groups](item-def-author-34e2e6a0519f-split-adelic-matrix-groups)

[F15] For matrices of the same size over a commutative ring the determinant is multiplicative. For an invertible matrix over a field its adjugate is the determinant times the inverse. In size two the adjugate sends $(a,b,c,d)$ in row order to $(d,-b,-c,a)$, so applying it twice gives the original matrix. [math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative) [math:cor-inverse-matrix-by-adjugate](https://alphabetamath.cc/item/cor-inverse-matrix-by-adjugate)

## Proof

**Given:** The projective Hamilton automorphic constituent $\pi$ and its trivial real action.

**Goal:** Obtain its cuspidal weight-two transfer, compare the split local actions and identify the corresponding classical newform.

1.1 Pull back $\pi$ along the quotient from the full quaternion adelic unit group in [F1]. The orbit identification places the pullback in the square-integrable full-unit space modulo rational units and scalar ideles. The transported measure is Radon under the orbit homeomorphism and differs from the invariant measure in the automorphic realization by a positive factor by [F8]. The pullback is irreducible and still has dimension greater than one, since invariant subspaces and the representation space are preserved. Its central character is trivial, and its real action is trivial because that action factors through the projective real action. [given, F1, F8]

1.2 For each family of local Hilbert spaces supplied by [F2], use the Axiom of Choice to select unit reference vectors with the stated tail invariance. Take the places in order, beginning with the real place and then the primes in increasing order. Form the finite Hilbert tensor products by iterating [F10] with the countable choice in [F4]. Passing to the next stage by tensoring with the next unit vector is an isometric linear embedding by the product pairing. Thus the compatible union has the product inner product, which gives the same pairing regardless of the stage where two elementary tensors are compared. Finite sums of elementary tensors are dense at each stage, and [F10] gives their span a Hilbert completion. For an adelic element, [F1] and the split matrix restricted product ensure that its entries fix the reference vectors outside a finite set. The coordinatewise action is defined on each finite tensor span by taking a stage containing that set and all the varying entries. Multilinearity defines the corresponding map on finite tensors, and the product pairing shows that it is an isometry. The inverse element gives its inverse and the local group laws give the action law, which extends by density to the completion. For an elementary tensor, near the identity the tail is fixed on a basic open box and continuity on the finitely many remaining entries follows from the local orbit maps and the product norm. Indeed, the difference of two finite elementary tensors expands into a sum replacing one factor at a time. Linearity, density and unitarity then give continuity on the completion. Inserting a vector at a single place and taking the reference vectors elsewhere gives an isometric embedding that intertwines the group supported at that place. [given, F1, F2, F4, F10]

2.1 Apply [F2] to the full-unit constituent of step 1.1 with the trivial unitary central character. This gives the full cuspidal matrix representation $\widetilde\Pi$ with trivial central character. Take a nonzero smooth cusp vector $u$ in its square-integrable realization from [F2]. It is invariant under left rational matrices and scalar ideles, so it defines a continuous function on the full-unit orbit space by the quotient topology. The upper unipotent quotient in [F2] identifies with $\mathbb Q\backslash\mathbb A$ via the upper right entry, with the same Haar probability as in the Statement. For every right translate $R(h)u$, its constant term at $g$ equals the constant term of $u$ at $gh$, and thus vanishes. These translates remain continuous by continuity of right translation and square-integrable by measure invariance. Their closed linear span is nonzero and invariant, hence equals $\widetilde\Pi$ by irreducibility. The quotient homeomorphism in [F1] preserves each unipotent average under pullback and identifies the two square-integral closures. It therefore realizes the projective constituent $\Pi$ in the specified cuspidal space, using the stated split quotient measure by [F8]. The real scalar extension in [F3] identifies the nonsplit real factor to which local transfer applies. The single-place embedding in step 1.2 identifies triviality of the global action of real quaternion units with triviality on the real factor. The trivial Hamilton representation has trivial positive-scalar character and norm-one part $\operatorname{Sym}^0(\mathbb C^2)$. Setting $n=0$ in [F3] gives both weight-two models on restriction to the determinant-one group. [F1, F2, F3, F8, step 1.1, step 1.2]

3.1 At a split finite prime $\ell$, [F2] identifies the smooth representations of the full local factors. If the split identification changes by conjugation by $C$ as in [F4], compose the intertwiner on the matrix side with the action of $C$. This intertwines the actions for the new identification. The cuspidal matrix factor has a nonzero smooth space by [F6], and the split smooth equivalence makes the quaternion smooth space nonzero as well. On either side the smooth vectors form a linear subspace because two open fixing subgroups have an open intersection. Translation by a group element carries vectors fixed by an open subgroup to vectors fixed by its conjugate, which is open. The closure of the smooth subspace is therefore nonzero and invariant, so irreducibility of the local unitary factor in [F2] makes that closure the whole Hilbert space. Pulling the target inner product back along the smooth intertwiner gives another invariant inner product on the source smooth space, a positive scalar multiple of its original inner product by [F9]. Rescale the smooth intertwiner to be isometric. Its inverse is also isometric on the other smooth space since the smooth intertwiner is bijective. The two smooth domains are dense by the preceding argument, and both target Hilbert spaces are Banach by [F13]. With countable choice from [F4], extend the rescaled map and its inverse using [F13]. Their compositions agree with the identities on dense subspaces, hence are the identities by continuity. Norm preservation and equivariance pass from the dense smooth space to the whole space by continuity. This gives the split unitary intertwiner. [F2, F4, F6, F9, F13, step 2.1]

3.2 The cuspidality from step 2.1 gives finite local genericity by [F6], so each smooth local factor is of Langlands type and the finite-place newvector theorem applies. The congruence groups $K_{1,q}(n)$ are open, since the entry conditions use the open sets $q^n\mathbb Z_q$ and $1+q^n\mathbb Z_q$ inside the open integral matrix group. Their Hilbert fixed vectors are therefore smooth, so the smooth test gives the stated $a_q$. For almost all primes the reference vectors in [F2] are fixed by the whole integral group $K_{1,q}(0)$, so $a_q=0$ there. For positive $n$, conjugation by $W=\begin{pmatrix}0&1\\-q^n&0\end{pmatrix}$ sends the entries $(a,b,c,d)$ from the convention in [F7] to $(d,-c/q^n,-q^nb,a)$ in row order. These entries are integral, the determinant is still a unit, and the bottom row is congruent to $(0,1)$. Since $W^2=-q^n I$, conjugation is its own inverse and carries the bottom-row subgroup back to the upper-left subgroup by the same entry computation. The action of $W$ thus identifies the two fixed spaces. At zero let $S_q$ be the set of integral invertible matrices with unit upper left entry, the literal local test in [F7]. If $g$ in the full integral group has nonunit upper left entry, its lower left entry is a unit because its first column is nonzero modulo $q$. With $E=\begin{pmatrix}1&1\\0&1\end{pmatrix}$, both $E$ and $Eg$ belong to $S_q$, since adding a unit to a nonunit gives a unit in $\mathbb Z_q$. Hence a vector fixed by every element of $S_q$ is fixed by $E^{-1}(Eg)=g$ as well. The two zero-index fixed spaces coincide, and the positive-index comparison then gives the same exponent at every prime. [F2, F6, F7, F11, F14, step 2.1]

4.1 At a split prime $\ell$, a local scalar embeds as a central idele supported at $\ell$. By step 1.2 its global action intertwines its local action under the corresponding isometric embedding. It acts trivially on both global representations, so injectivity of the embeddings forces trivial action on both local factors. Thus the equivalence descends to the projective group. The local projection is open because the preimage of the image of an open set is a union of its scalar translates, which are open. The orbit maps of the descended actions are continuous because their pullbacks are continuous. Since the projection is surjective, invariant subspaces are exactly the same for the two actions. A fixing subgroup that is open pulls back to an open fixing subgroup, and an open fixing subgroup upstairs projects to an open fixing subgroup downstairs, so the smooth spaces agree. For a compact open subgroup $J$ of the projective group, intersect its open preimage with $\mathrm{GL}_2(\mathbb Z_\ell)$. The intersection is an open subgroup of the full matrix group and is closed in the compact integral group because its other cosets there are open. It is therefore compact open, and its fixed space contains the $J$-fixed space. Admissibility in [F2] bounds that space by a finite dimension. Via the split equivalence this proves smooth irreducibility and admissibility for both projective factors. The full integral subgroup and its projective image have the same fixed vectors. The full integral subgroup is open, so its fixed vectors belong to the smooth local factors. Under [F4] the nonzero fixed spaces are lines and the split intertwiner identifies all normalized spherical Hecke scalars on them. At odd primes the same integral splitting from [F4] identifies the projective images of the Hurwitz units and the integral matrix units. [F1, F2, F4, F14, step 1.1, step 1.2, step 2.1, step 3.1]

5.1 By step 2.1 the full matrix representation is cuspidal of real weight-two type with trivial central character. By [F7] and step 3.2 its conductor level is $N=\prod_q q^{a_q}$. Use [F5] to obtain the holomorphic weight-two cusp form $f$ and its lift $\phi_f$ in this constituent. The ideal coefficient at $(1)$ is the coefficient of $q^1$, since the rational narrow class representative can be taken to be $1$. The lift is fixed by $K_0(N)$, hence by the product of the upper-left congruence subgroups in [F7]. For the rotation $k_\theta=\begin{pmatrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{pmatrix}$, one has $k_\theta i=i$ and the slash factor at $i$ is $(\cos\theta-i\sin\theta)^{-2}=e^{2i\theta}$. Applying the lift formula gives $\phi_f(gk_\theta)=e^{2i\theta}\phi_f(g)$. The restriction of the lift formula to the real group is inverse to (22), so [F7] identifies this same $f$ as a classical newform. For each proper divisor $M$ of $N$ and each $t\mid N/M$, rational left invariance turns the finite right translate by $\operatorname{diag}(t^{-1},1)$ of a lower-level lift into the real slash by $\operatorname{diag}(t,1)$. In the degeneracy formula of [F5] the multiplier $t^{-1}$ cancels the weight-two slash factor $t$, giving $g(z)\mapsto g(tz)$. Thus the proper-level degeneracy images give precisely the old space in [F5]. At weight two the Petersson integrand uses $y^2\,dx\,dy/y^2=dx\,dy$, so the positive volume normalization in that formula leaves orthogonality unchanged. Consequently $f$ is orthogonal to the old subspace in the stated convention. The lift belongs to the one-dimensional space in [F7]. The closed span of the right translates of $\phi_f$ is the whole constituent by irreducibility. At a split unramified prime $\ell$, step 4.1 gives a nonzero full integral fixed space, so $a_\ell=0$. Unique prime factorization gives $\ell\nmid N$, including when the product of the positive-exponent factors is empty and $N=1$. [F5, F7, step 2.1, step 3.2, step 4.1]

6.1 Fix $m\ge1$. For the finite cosets in [F11], take $x\in X_m$ and apply the adelic decomposition in [F5] to the adele with finite part $x^{-1}$ and real part the identity. The rational factor $\gamma$ has the same matrix at every place and satisfies $\gamma g_\infty=I$ at the real place, so $A=\gamma^{-1}$ has positive determinant. Inverting the finite equation gives $x=k^{-1}A_f$, with $A_f$ the finite tuple consisting of that same rational matrix $A$ at every prime. Multiplication by $K_0(N)$ on either side preserves $X_m$. The entries stay integral. By determinant multiplicativity in [F15] the determinant is multiplied at each prime by a local unit of valuation zero, so additivity preserves the determinant ideal. At a level prime the lower left entry stays in $N\mathbb Z_p$ and the upper left entry is multiplied modulo $p$ by a unit. The upper left entry of an element of $K_0(N)$ is a unit there by its unit determinant and its zero lower left entry modulo $p$. Both matrices are upper triangular modulo $N\mathbb Z_p$ there. By [F12] the entries of $A$ are therefore integers, its lower left entry is divisible by $N$ by applying the same test after dividing by $N$, and its upper left entry is coprime to $N$. The normalized local valuations on the rational determinant of $A$ agree with its rational prime exponents. These exponents are those of $m$, so its positive determinant is $m$ by prime factorization. Two such rational matrices give the same coset exactly when they differ by left multiplication by $\Gamma_0(N)$. Indeed their rational left multiplier then belongs at every finite prime to the local level group, so its entries are integral, its lower left entry is divisible by $N$ and its positive determinant is a unit at every prime, hence is one. Conversely every such $\Gamma_0(N)$ multiplier has its finite part in $K_0(N)$. [F5, F7, F11, F12, F15, step 5.1]

7.1 For a rational representative in step 6.1 let $(u,w)$ be its integral first column and $a=\gcd(u,w)>0$. The conditions on this column give $(a,N)=1$. By [F12] choose integers $s,t$ with $su+tw=a$. The matrix with rows $(s,t)$ and $(-w/a,u/a)$ has determinant one and belongs to $\Gamma_0(N)$, as follows. Bézout gives integers $r,v$ with $ra+vN=1$ from $(a,N)=1$. Multiplying by $w/a$ gives $w/a=rw+vN(w/a)$, so $N\mid w/a$. Left multiplication sends the first column to $(a,0)$, so the lower right entry is $d=m/a>0$. Adding an integral multiple of the second row to the first gives the unique upper right entry $b$ in $0\le b<d$. The representatives are thus the finite components of $A=\begin{pmatrix}a&b\\0&d\end{pmatrix}$ with $ad=m$, $a,d>0$, $(a,N)=1$ and $0\le b<d$. Each satisfies the local conditions. A determinant-one integral row operation preserves the first-column greatest common divisor, so equivalent representatives have the same $a$ and hence the same $d$. For two such representatives their left multiplier is upper unipotent with upper right entry $(b'-b)/d$. This is integral only when the two residues coincide. [F7, F12, step 6.1]

8.1 For the now finite set of cosets $K_0(N)x$ define $H_m\phi_f(g)$ to be the sum of $\phi_f(g(1,x^\iota))$ over one representative $x$ of each coset, where $\iota$ is the componentwise adjugate. The adjoined real component in $(1,x^\iota)$ is the identity. By [F15] the adjugate reverses products of invertible matrices. For $k\in K_0(N)$, its adjugate $k^\iota$ also belongs to $K_0(N)$, by the two-by-two formula and the unit determinant. Replacing $x$ by $kx$ leaves the summand unchanged since $(kx)^\iota=x^\iota k^\iota$ and $\phi_f$ is fixed on the right by $K_0(N)$. For $h\in K_0(N)$, evaluating at $g(1,h)$ replaces $x^\iota$ by $h x^\iota=(x h^\iota)^\iota$. Right multiplication by $h^\iota$ permutes the finite left-level cosets by step 6.1. Thus $H_m\phi_f$ is fixed by $K_0(N)$. Real rotations commute with the finite translations and preserve the same rotation character in the sum. The sum belongs to the smooth automorphic model of the constituent because it is a finite sum of right translates of $\phi_f$. It is fixed by the global $K_1(N)$ and has the rotation character in [F7], so it is a scalar multiple of $\phi_f$ by uniqueness, with zero allowed. [F5, F7, F11, F15, step 5.1, step 6.1, step 7.1]

9.1 For $z=x+iy$ with $y>0$, evaluate $H_m$ at the adele supported at the real place with component $h_z=\begin{pmatrix}y&x\\0&1\end{pmatrix}$. For each representative from step 7.1, its adjugate $A^\iota=mA^{-1}$ from [F15] contributes $\phi_f(h_z(A^\iota)_f)$. The argument equals the rational matrix $A^\iota$ embedded at every place times the adele supported at the real place with component $(A^\iota)^{-1}h_z$. Formula [F5] and the weight-two slash composition rule give $((f|_2(A^\iota)^{-1})|_2h_z)(i)=y(f|_2 A)(z)$, since $(A^\iota)^{-1}=A/m$ and the numerator determinant and the squared denominator in the slash action both scale by the square of the scalar. Divide the eigenfunction equation by $y$ using $\phi_f(h_z)=yf(z)$. Each summand on the classical side is $(f|_2 A)(z)=md^{-2}f((az+b)/d)$. By step 7.1 the sum precisely matches the classical $T_m$ in [F5], including its restriction to $(a,N)=1$ from the Dirichlet character extended by zero on nonunits. This applies also when $m$ has a prime divisor of $N$. Thus $f$ satisfies the classical eigenform condition at every positive index and is a normalized weight-two cuspidal newform. [F5, F15, step 5.1, step 7.1, step 8.1] ∎

## External input

The global transfer input gives the forward correspondence for quaternion automorphic constituents of dimension greater than one at fixed central character, including the split and nonsplit comparisons.

The Hilbert factorization input gives the restricted Hilbert tensor product for both full-unit discrete automorphic constituents.

The real local transfer input relates the Hamilton symmetric-power index to the split lowest absolute rotation weight and supplies the two models on the determinant-one group.

The classical newform input constructs the cusp form and its lift at the conductor level, with the stated character, Fourier normalization and prime eigenform properties away from the level. It also supplies the irreducible admissible split local factors.

The finite newvector input gives local genericity, the implication to Langlands-type induction and the least congruence index giving the local conductor ideal.

The conductor product input identifies the rational newform level with the product of local conductor prime powers. Its subgroup and rotation conditions specify the one-dimensional adelic newform line, and its inverse lift recovers the classical newform.

The quotient measure input gives uniqueness up to positive scale for invariant Radon measures on the full-unit orbit spaces.

The local inner product input gives uniqueness up to positive scale of the invariant Hermitian inner product on each smooth split local factor.

The smooth cuspidal realization input supplies a nonzero smooth square-integrable cusp vector with identically vanishing upper unipotent constant term.
