---
title: Local conductor exponent from fixed vectors
status: draft
research_item: def-author-f98bf83ef432-local-conductor-exponent
dependency_level: 1
sources:
  references:
    - title: Andrew Corbett and Abhishek Saha, On the order of vanishing of newforms
        at cusps
      url: https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf
      locator: General notation and §2.1.1, p. 6, continuity and unit filtration.
        §2.1.3, p. 7, the fixed additive character. §2.1.4, equation (8), and
        §2.1.5, p. 8, the local conductor. §3.1, p. 16, the adelic product.
      statement: Inside $\mathrm{GL}_2(\mathfrak o)$, equation (8) defines $K_1(n)$ by
        $c\in\varpi^n\mathfrak o$ and $a\in U_n$, and $K'_1(n)$ by
        $c\in\varpi^n\mathfrak o$ and $d\in U_n$. Here $U_n=1+\varpi^n\mathfrak
        o$ for $n>0$ and $U_0=\mathfrak o^\times$. The absolute value is
        normalized by $|\varpi|=\#(\mathfrak o/\varpi\mathfrak o)^{-1}$. The
        authors fix a continuous additive character trivial on $\mathfrak o$ and
        nontrivial on $\varpi^{-1}\mathfrak o$. Section 2.1.5 defines the
        conductor exponent using the least nonnegative index at which $K_1(n)$
        fixes a nonzero vector. The local factors of the adelic congruence
        subgroup in §3.1 are $K_1(n)$ at positive index and
        $\mathrm{GL}_2(\mathbb Z_q)$ at index zero.
      hypotheses: The local passages use a nonarchimedean local field of
        characteristic zero with ring of integers $\mathfrak o$ and uniformizer
        $\varpi$. Section 2.1.5 treats irreducible, admissible, generic local
        representations. Section 3.1 works over $\mathbb Q$ with an irreducible
        unitary cuspidal automorphic representation whose central character is
        trivial on the positive reals and whose real factor has holomorphic
        discrete-series lowest weight $k\ge2$.
      reading_limits: Checked the stated passages for the normalization, the unit
        filtration, the fixed character, the matrix conditions, the local
        conductor and the adelic product. The comparison assumes existence of a
        qualifying index and uses the local subgroup argument.
    - title: J. S. Milne, Algebraic Number Theory
      url: https://www.jmilne.org/math/CourseNotes/ANT.pdf
      locator: Version 3.08, Chapter 7, paragraph after Proposition 7.5 (PDF page 109)
        and Proposition 7.46 and Definition 7.48 (PDF page 128).
      statement: An absolute value is discrete when the absolute values of the nonzero
        elements form a discrete multiplicative subgroup of the positive reals.
        For a field complete for a discrete absolute value, the ring of integers
        is compact if and only if its residue field is finite. A field with a
        nontrivial absolute value is a local field if it is locally compact in
        the induced topology, in which case it is also complete.
      hypotheses: The discreteness criterion uses the nonzero values in the positive
        reals with their usual topology. Proposition 7.46 assumes completeness
        for a discrete absolute value, with the ring of integers and its residue
        field taken for that absolute value. Definition 7.48 requires a field
        with a nontrivial absolute value and local compactness for the induced
        metric topology.
      reading_limits: Read the paragraph after Proposition 7.5, the statement and
        proof of Proposition 7.46, and Definition 7.48 in the PDF text. The
        argument uses the finite-residue-field direction and checks discreteness
        and local compactness for the q-adic field.
    - title: Torsten Wedhorn, The Local Langlands Correspondence for GL(n) over p-adic
        Fields
      url: https://arxiv.org/pdf/math/0011210
      locator: arXiv v2, Notations (PDF page 8), §2.1, (2.1.1)–(2.1.4) (PDF pages
        15–16), and §2.4, (2.4.1)–(2.4.3)(3) (PDF pages 28–29).
      statement: With its local group topology, $\mathrm{GL}_n(K)$ is a locally
        compact Hausdorff group. The compact open subgroups $I+\pi_K^m
        M_n(\mathcal O_K)$, $m\ge1$, form a neighbourhood basis at the identity.
        Admissibility requires open vector stabilizers and finite-dimensional
        spaces of fixed vectors for open subgroups. In the smooth category the
        finite-dimensional condition is equivalent to testing compact open
        subgroups. For a smooth irreducible representation of
        $\mathrm{GL}_n(K)$, genericity is nonvanishing of
        $\operatorname{Hom}_{U_n(K)}(V,\theta_\psi)$ for the upper unitriangular
        group, where $\theta_\psi(u)=\psi(\sum_{i=1}^{n-1}u_{i,i+1})$.
        Genericity is independent of the choice of nontrivial additive character
        $\psi$.
      hypotheses: The notations take $K$ to be a finite extension of $\mathbb Q_p$,
        $\mathcal O_K$ its ring of integers and $\pi_K$ a uniformizer. Section
        2.1 treats the group of points of a connected reductive group and
        explicitly includes $\mathrm{GL}_n(K)$. Section 2.4 uses a smooth
        irreducible complex representation of $\mathrm{GL}_n(K)$ and a
        nontrivial continuous additive character of $K$ into the unit circle.
      reading_limits: Checked the PDF text for the standing notation, the identity
        neighbourhood basis, admissibility, genericity and character
        independence. The entry topology and the unit modulus condition for
        characters of $\mathbb Q_q$ are checked locally.
---

## Prerequisites

- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)
- [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)
- [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:def-vector-space](https://alphabetamath.cc/item/def-vector-space)
- [math:def-linear-map](https://alphabetamath.cc/item/def-linear-map)
- [math:def-linear-isomorphism-and-invertible-linear-map](https://alphabetamath.cc/item/def-linear-isomorphism-and-invertible-linear-map)
- [math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-group-action](https://alphabetamath.cc/item/def-group-action)
- [math:def-fixed-point-sets-of-a-group-action](https://alphabetamath.cc/item/def-fixed-point-sets-of-a-group-action)
- [def-author-f98bf83ef432-local-k-one-subgroup](item-def-author-f98bf83ef432-local-k-one-subgroup)
- [math:def-int-order](https://alphabetamath.cc/item/def-int-order)
- [math:def-linear-subspace](https://alphabetamath.cc/item/def-linear-subspace)
- [math:lem-group-homomorphism-basic-properties](https://alphabetamath.cc/item/lem-group-homomorphism-basic-properties)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:def-natural-numbers](https://alphabetamath.cc/item/def-natural-numbers)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)
- [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)
- [math:lem-monoid-units-form-a-group](https://alphabetamath.cc/item/lem-monoid-units-form-a-group)
- [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals)
- [math:cor-maximal-ideal-and-residue-field-of-zp](https://alphabetamath.cc/item/cor-maximal-ideal-and-residue-field-of-zp)
- [math:def-locally-compact-metric-space](https://alphabetamath.cc/item/def-locally-compact-metric-space)
- [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)
- [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:def-dimension](https://alphabetamath.cc/item/def-dimension)
- [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)
- [math:def-algebraic-dual-and-linear-functional](https://alphabetamath.cc/item/def-algebraic-dual-and-linear-functional)
- [math:def-orbit-and-stabilizer](https://alphabetamath.cc/item/def-orbit-and-stabilizer)
- [math:def-complex-metric-convergence-and-continuity](https://alphabetamath.cc/item/def-complex-metric-convergence-and-continuity)
- [math:def-ring-characteristic](https://alphabetamath.cc/item/def-ring-characteristic)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:thm-compactness-agrees-with-metric-compactness](https://alphabetamath.cc/item/thm-compactness-agrees-with-metric-compactness)
- [math:lem-rational-power-monotone](https://alphabetamath.cc/item/lem-rational-power-monotone)
- [math:lem-geometric-sequence-null](https://alphabetamath.cc/item/lem-geometric-sequence-null)
- [math:lem-complex-conjugation-and-modulus-laws](https://alphabetamath.cc/item/lem-complex-conjugation-and-modulus-laws)
- [math:def-metric-convergence](https://alphabetamath.cc/item/def-metric-convergence)
- [math:def-field-homomorphism](https://alphabetamath.cc/item/def-field-homomorphism)
- [math:def-field-extension-generated-subfields-and-simple-extension](https://alphabetamath.cc/item/def-field-extension-generated-subfields-and-simple-extension)
- [math:def-extension-degree-and-finite-extension](https://alphabetamath.cc/item/def-extension-degree-and-finite-extension)
- [math:def-linear-basis](https://alphabetamath.cc/item/def-linear-basis)
- [math:def-topological-group](https://alphabetamath.cc/item/def-topological-group)
- [math:lem-topological-group-translations-and-inversion](https://alphabetamath.cc/item/lem-topological-group-translations-and-inversion)
- [math:def-neighbourhood-top](https://alphabetamath.cc/item/def-neighbourhood-top)
- [` Andrew Corbett and Abhishek Saha, On the order of vanishing of newforms at cusps · General notation and §2.1.1, p. 6, continuity and unit filtration. §2.1.3, p. 7, the fixed additive character. §2.1.4, equation (8), and §2.1.5, p. 8, the local conductor. §3.1, p. 16, the adelic product. `](https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf)
- [` J. S. Milne, Algebraic Number Theory · Version 3.08, Chapter 7, paragraph after Proposition 7.5 (PDF page 109) and Proposition 7.46 and Definition 7.48 (PDF page 128). `](https://www.jmilne.org/math/CourseNotes/ANT.pdf)
- [` Torsten Wedhorn, The Local Langlands Correspondence for GL(n) over p-adic Fields · arXiv v2, Notations (PDF page 8), §2.1, (2.1.1)–(2.1.4) (PDF pages 15–16), and §2.4, (2.4.1)–(2.4.3)(3) (PDF pages 28–29). `](https://arxiv.org/pdf/math/0011210)


## Definition

For a prime $q$, let $\mathbb Q_q$ be the $q$-adic field obtained by metric completion and identify $\mathbb Z_q$ with its canonically embedded ring of integers. Write $G=\mathrm{GL}_2(\mathbb Q_q)$ for the group of invertible two-by-two matrices over $\mathbb Q_q$. Let $V$ be a complex vector space of arbitrary dimension. A complex representation $\rho$ of $G$ on $V$ is a group homomorphism into the group of invertible complex-linear maps $V\to V$ under composition. For a subgroup $J$ of $G$, write $V^J=\{v\in V:\rho(j)v=v\text{ for all }j\in J\}$ for its fixed space.

For each nonnegative integer $n$, let $K_{1,q}(n)$ consist of the matrices in $\mathrm{GL}_2(\mathbb Z_q)$ whose bottom row is congruent to $(0,1)$ modulo $q^n\mathbb Z_q$. In particular the matrices and their inverses are integral, and $K_{1,q}(0)=\mathrm{GL}_2(\mathbb Z_q)$.

Suppose $V^{K_{1,q}(n)}\ne\{0\}$ for at least one nonnegative integer $n$. The conductor exponent $a(\rho)$ is the least such integer.

## Definition references

[Prime integers](https://alphabetamath.cc/item/def-prime)

[The metric completion defining the local field](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)

[Field operations on the completion](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)

[Canonical embedding of the integral ring](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)

[General linear group](item-def-degree-two-projective-linear-group)

[Complex scalar field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

[Vector spaces and their zero vectors](https://alphabetamath.cc/item/def-vector-space)

[Linear maps](https://alphabetamath.cc/item/def-linear-map)

[Invertible linear maps](https://alphabetamath.cc/item/def-linear-isomorphism-and-invertible-linear-map)

[Group homomorphisms](https://alphabetamath.cc/item/def-group-homomorphism)

[Subgroups](https://alphabetamath.cc/item/def-subgroup)

[Left group actions](https://alphabetamath.cc/item/def-group-action)

[Fixed-point sets of an action](https://alphabetamath.cc/item/def-fixed-point-sets-of-a-group-action)

[Local congruence subgroups](item-def-author-f98bf83ef432-local-k-one-subgroup)

[Order on the integers](https://alphabetamath.cc/item/def-int-order)

[Associative composition with identity](https://alphabetamath.cc/item/def-semigroup-and-monoid)

[The group of invertible self-maps](https://alphabetamath.cc/item/lem-monoid-units-form-a-group)

## Facts & Assumptions

[F1] A group homomorphism preserves the identity and the group product, so $(g,v)\mapsto\rho(g)v$ is a left action. The space $V^J$ is the fixed-point set for its restriction to $J$. [Identity and product for a group homomorphism](https://alphabetamath.cc/item/lem-group-homomorphism-basic-properties) [Left action](https://alphabetamath.cc/item/def-group-action) [Fixed-point set](https://alphabetamath.cc/item/def-fixed-point-sets-of-a-group-action)

[F2] Invertible linear maps have two-sided linear inverses. A linear subspace is a subset containing zero and closed under addition and scalar multiplication. [Linearity](https://alphabetamath.cc/item/def-linear-map) [Linear inverses](https://alphabetamath.cc/item/def-linear-isomorphism-and-invertible-linear-map) [Subspace criterion](https://alphabetamath.cc/item/def-linear-subspace)

[F3] The order on the integers is a total order. The natural embedding $\iota:\mathbb N\to\mathbb Z$ identifies the natural numbers in order with the nonnegative integers. Every nonempty subset of $\mathbb N$ has a least element. [Integer order](https://alphabetamath.cc/item/def-int-order) [Total order of the integers](https://alphabetamath.cc/item/thm-int-ordered-ring) [The natural numbers including zero](https://alphabetamath.cc/item/def-natural-numbers) [Ordered natural embedding](https://alphabetamath.cc/item/lem-nat-embeds-int) [Well-ordering](https://alphabetamath.cc/item/thm-well-ordering-principle)

[F4] The canonical embedding of the integral ring into the field embeds the integral matrix group in $G$, since a two-sided integral inverse remains a two-sided inverse over the field. The local congruence-subgroup argument identifies $q$ as a uniformizer and supplies the subgroup property. For $n>0$, it gives a bijection between the fixed spaces of the top-left group $K^{\mathrm{top}}_{1,q}(n)$ and the bottom-row group $K_{1,q}(n)$ under the action of $W_n=\begin{pmatrix}0&1\\-q^n&0\end{pmatrix}$. At zero, both groups are the full integral group. The same argument shows that the literal top-left unit condition at zero in equation (8) has the same fixed vectors as the full integral group. [Integral embedding](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp) [Two-sided matrix inverses](item-def-degree-two-projective-linear-group) [Subgroups, conjugacy, and the level-zero fixed vectors](item-def-author-f98bf83ef432-local-k-one-subgroup)

[F5] Corbett and Saha define the conductor of an irreducible, admissible, generic representation as the least nonnegative index at which their top-left group $K_1(n)$ fixes a nonzero vector. At positive index their $K'_1(n)$ is the bottom-row group, and at index zero the adelic product in §3.1 uses the full integral group. Their absolute value is normalized by $|\varpi|=\#(\mathfrak o/\varpi\mathfrak o)^{-1}$. They fix a continuous additive character trivial on $\mathfrak o$ and nontrivial on $\varpi^{-1}\mathfrak o$. [Corbett and Saha, §§2.1.1, 2.1.3–2.1.5, and 3.1](https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf#page=8)

[F6] A monoid is a set with an associative operation and a two-sided identity. Its elements with two-sided inverses form a group under that operation. [Monoid axioms](https://alphabetamath.cc/item/def-semigroup-and-monoid) [Group of units](https://alphabetamath.cc/item/lem-monoid-units-form-a-group)

[F7] The constant-sequence embedding identifies $\mathbb Q$ with a dense subfield of $\mathbb Q_q$, and $\mathbb Q_q$ is complete for the extended nonarchimedean absolute value. On nonzero rationals this absolute value takes values in $q^{\mathbb Z}$, and $|q|_q=q^{-1}$. The ring of integers is the closed unit ball $\mathbb Z_q$. Its maximal ideal is $q\mathbb Z_q$, with residue field of order $q$. [The dense rational embedding](https://alphabetamath.cc/item/def-field-of-p-adic-numbers) [The extended absolute value and field operations](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field) [Rational absolute values](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals) [The closed unit ball](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp) [Maximal ideal and residue field](https://alphabetamath.cc/item/cor-maximal-ideal-and-residue-field-of-zp) [Count of representatives modulo $q$](item-def-author-f98bf83ef432-local-k-one-subgroup)

[F8] Milne calls an absolute value discrete when its nonzero values form a discrete subgroup of the positive reals under multiplication. A field complete for a discrete absolute value has a compact ring of integers when the residue field is finite. A metric space is locally compact when every point has a compact neighbourhood. A field with a nontrivial absolute value is a local field in Milne’s convention if it is locally compact for the induced metric topology. [Local compactness](https://alphabetamath.cc/item/def-locally-compact-metric-space) [Milne, after Proposition 7.5](https://www.jmilne.org/math/CourseNotes/ANT.pdf#page=109) [Milne, Proposition 7.46 and Definition 7.48](https://www.jmilne.org/math/CourseNotes/ANT.pdf#page=128)

[F9] Give $G$ the subspace topology from the four entries with their $q$-adic metric topology. The stabilizer of a vector $v$ is $\{g\in G:\rho(g)v=v\}$ for the left action in [F1]. A representation is smooth when every vector stabilizer is open in $G$. It is admissible when it is smooth and $V^J$ is finite-dimensional for every compact open subgroup $J$ of $G$. It is irreducible when $V\ne\{0\}$ and no nonzero proper linear subspace is invariant under every $\rho(g)$. Write $\mathbb C^\times=\mathbb C\setminus\{0\}$. By the field axioms, $(\mathbb Q_q,+)$ is an additive group and $(\mathbb C^\times,\cdot)$ is a multiplicative group. In the smooth irreducible class, genericity means that for some nontrivial continuous homomorphism $\psi:(\mathbb Q_q,+)\to(\mathbb C^\times,\cdot)$ there is a nonzero complex-linear functional $\lambda:V\to\mathbb C$ satisfying
$$\lambda\left(\rho\left(\begin{pmatrix}1&x\\0&1\end{pmatrix}\right)v\right)=\psi(x)\lambda(v)\qquad(x\in\mathbb Q_q,\ v\in V).$$
Give $\mathbb C^\times$ the subspace topology from the Euclidean metric on $\mathbb C$. Wedhorn’s compact open subgroup test is equivalent to his open subgroup test for admissibility in the smooth category. His genericity test is independent of the nontrivial additive character. [Metric topologies](https://alphabetamath.cc/item/def-metric-topology) [Euclidean metric on the complex plane](https://alphabetamath.cc/item/def-complex-metric-convergence-and-continuity) [Vector stabilizers for the representation action](https://alphabetamath.cc/item/def-orbit-and-stabilizer) [Product of the four entry topologies](https://alphabetamath.cc/item/def-product-topology) [Subspace topology](https://alphabetamath.cc/item/def-subspace-topology-top) [Compactness](https://alphabetamath.cc/item/def-compact-space) [Finite-dimensional spaces](https://alphabetamath.cc/item/def-dimension) [Linear subspaces](https://alphabetamath.cc/item/def-linear-subspace) [Continuity](https://alphabetamath.cc/item/def-continuous-map-top) [Group homomorphisms](https://alphabetamath.cc/item/def-group-homomorphism) [Additive and multiplicative groups from the field axioms](https://alphabetamath.cc/item/def-field) [The q-adic field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field) [The complex field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field) [Linear functional](https://alphabetamath.cc/item/def-algebraic-dual-and-linear-functional) [Wedhorn, arXiv v2, §§2.1 and 2.4](https://arxiv.org/pdf/math/0011210)

[F10] A field has characteristic zero when $n\cdot1$ is nonzero for every positive integer $n$. [Characteristic of a ring](https://alphabetamath.cc/item/def-ring-characteristic)

[F11] The traces of ambient open balls form a basis for the subspace topology of a metric space. A subspace is compact when every cover by relatively open sets has a finite subcover. [Open balls and the metric topology](https://alphabetamath.cc/item/def-metric-topology) [Traces in a subspace](https://alphabetamath.cc/item/def-subspace-topology-top) [Finite subcovers](https://alphabetamath.cc/item/def-compact-space) A subset of a metric space is compact for the restricted metric exactly when it is compact for the subspace topology of the ambient metric topology. [Compact subsets in the metric and subspace topology](https://alphabetamath.cc/item/thm-compactness-agrees-with-metric-compactness)

[F12] For Wedhorn, $K$ is a finite extension of $\mathbb Q_p$ and $\pi_K$ generates the maximal ideal of its ring of integers $\mathcal O_K$. He gives $\mathrm{GL}_n(K)$ a locally compact Hausdorff group topology. Its identity neighbourhood basis consists of the compact open subgroups $I+\pi_K^m M_n(\mathcal O_K)$, with $m\ge1$. His additive characters are continuous homomorphisms into the unit circle. [Wedhorn, Notations and §2.1, (2.1.1)–(2.1.2)](https://arxiv.org/pdf/math/0011210#page=15)

[F13] For a positive real base larger than one, its powers increase strictly with the rational exponent. The geometric sequence with real ratio of absolute value less than one tends to zero. Complex modulus is multiplicative and subadditive. [Monotonicity of powers](https://alphabetamath.cc/item/lem-rational-power-monotone) [Decay of a geometric sequence](https://alphabetamath.cc/item/lem-geometric-sequence-null) [Complex modulus laws](https://alphabetamath.cc/item/lem-complex-conjugation-and-modulus-laws)

[F14] A sequence $(x_m)$ converges to $x$ in a metric space with metric $d$ exactly when $d(x_m,x)\to0$. [Metric convergence](https://alphabetamath.cc/item/def-metric-convergence)

[F15] A field extension specifies an embedding of the base field into the extension field. A basis is a linearly independent spanning set. An extension has finite degree when the extension field has a finite basis over the base field, and its degree is the dimension over that field. [Field embeddings](https://alphabetamath.cc/item/def-field-homomorphism) [Field extensions](https://alphabetamath.cc/item/def-field-extension-generated-subfields-and-simple-extension) [Linear bases](https://alphabetamath.cc/item/def-linear-basis) [Finite extensions and degree](https://alphabetamath.cc/item/def-extension-degree-and-finite-extension) [Finite dimension](https://alphabetamath.cc/item/def-dimension)

[F16] Left translation by a fixed group element is continuous with continuous inverse in a topological group. Every neighbourhood at a point contains a member of any neighbourhood basis there. A set is open exactly when it is a neighbourhood of each of its points. [Topological groups](https://alphabetamath.cc/item/def-topological-group) [Left translations and their inverses](https://alphabetamath.cc/item/lem-topological-group-translations-and-inversion) [Neighbourhood bases and open sets](https://alphabetamath.cc/item/def-neighbourhood-top)

## Justification

**Given:** The prime $q$ and the complex representation $\rho$ with a nonzero $K_{1,q}(n)$-fixed vector for some nonnegative integer $n$.

1.1 The identity map on $V$ is linear, and a composition of linear self-maps preserves linear combinations by applying linearity twice. Composition is associative since both bracketings of three maps send $v$ to $T(S(R(v)))$, and the identity is two-sided. Thus these self-maps form a monoid by [F6]. Its units are exactly the invertible linear self-maps by [F2]. By [F6] they form the codomain group in the definition, for every $V$. [F2, F6]

1.2 For every positive integer $n$, the embedding of $\mathbb Q$ in [F7] sends the nonzero rational $n$ to $n\cdot1$ in $\mathbb Q_q$. Thus $\mathbb Q_q$ has characteristic zero by [F10]. If $x\ne0$, the isometric density in [F7] supplies a rational $r$ with $|x-r|_q<|x|_q$. The nonarchimedean inequality applied to $x=r+(x-r)$ and $r=x+(r-x)$ gives $|x|_q=|r|_q$. The nonzero values therefore lie in $q^{\mathbb Z}$, and the powers of $q$ in the rational subfield attain all these values. Since $q>1$, the interval $(q^{k-1},q^{k+1})$ meets $q^{\mathbb Z}$ only at $q^k$ by [F13]. Hence the nonzero value group is discrete in the positive reals, so the absolute value is discrete by [F8]. With the finite residue field in [F7], [F8] gives compactness of $\mathbb Z_q$. Write $d_q(y,z)=|y-z|_q$ for the metric on $\mathbb Q_q$. For $x\in\mathbb Q_q$, the map $t_x:y\mapsto x+y$ is a bijection from $\mathbb Z_q$ onto $x+\mathbb Z_q$. It preserves the $q$-adic distance because $d_q(t_x(y),t_x(z))=|(x+y)-(x+z)|_q=|y-z|_q=d_q(y,z)$. By [F11], the preimage of a relatively open set in $x+\mathbb Z_q$ is relatively open in $\mathbb Z_q$: the trace of a ball about $x+y$ pulls back to the trace of the ball of the same radius about $y$. Pull back any open cover of $x+\mathbb Z_q$ along $t_x$. Compactness of $\mathbb Z_q$ gives a finite subcover of the pullback cover, and its images under $t_x$ give a finite subcover of the original cover. Thus the translate is compact for the subspace topology and hence for the restricted metric by [F11]. It contains the open ball of radius one about $x$, since $|z-x|_q<1$ puts $z-x$ in $\mathbb Z_q$ by [F7]. Since $q>1$ and $|q|_q=q^{-1}$, the absolute value is nontrivial. By [F8] this makes $\mathbb Q_q$ a characteristic-zero nonarchimedean local field. By [F4] and [F7], the source can take $\mathfrak o=\mathbb Z_q$ and $\varpi=q$, with residue cardinality $q$ and the normalization in [F5]. [given, F4, F5, F7, F8, F10, F11, F13]

1.3 For a continuous additive homomorphism $\chi:\mathbb Q_q\to\mathbb C^\times$ and $x\in\mathbb Q_q$, the identity $|q^m x|_q=q^{-m}|x|_q$ and [F13] give $|q^m x|_q\to0$. Hence $q^m x\to0$ in the $q$-adic metric by [F14]. Fix $\varepsilon>0$. The trace in $\mathbb C^\times$ of the open ball of radius $\varepsilon$ about $\chi(0)=1$ is an open neighbourhood by [F9] and [F11]. By continuity in [F9], its preimage contains a $q$-adic ball about $0$. Thus all sufficiently late $q^m x$ belong to that preimage, so $\chi(q^m x)\to1$ by [F14]. The homomorphism law in [F1] gives $\chi(q^m x)=\chi(x)^{q^m}$ because $q^m$ is a positive integer. Subadditivity gives $\bigl||z|-1\bigr|\le |z-1|$, so $|\chi(x)|^{q^m}\to1$. If $|\chi(x)|>1$, monotonicity gives $|\chi(x)|^{q^m}\ge |\chi(x)|>1$ for all $m$. If $|\chi(x)|<1$, then $|\chi(-x)|=|\chi(x)|^{-1}>1$, already ruled out. Thus the characters used in [F5] and [F9] take values in the unit circle and are continuous for its subspace topology. [F1, F5, F7, F9, F11, F12, F13, F14]

2.1 By [F4] each $K_{1,q}(n)$ is a subgroup of $G$. By [F1] its fixed space is taken for the restricted action. Every operator of this action fixes the zero vector by linearity. If two vectors are fixed by every operator, so is each of their linear combinations, by applying linearity to each operator. Hence the fixed space is a linear subspace by [F2]. [F1, F2, F4, step 1.1]

2.2 In Wedhorn’s notation set $p=q$ and take $K=\mathbb Q_q$ with the identity embedding of $\mathbb Q_q$. The identity preserves addition, multiplication and one, so it gives a field extension by [F15]. As a vector space over itself, $\mathbb Q_q$ has basis $\{1\}$ because every $x$ is $x\cdot1$ and $c\cdot1=0$ implies $c=0$. Thus the extension has degree one by [F15]. Here $\mathcal O_K=\mathbb Z_q$ and $\pi_K=q$ by step 1.2. His groups from [F12] become $C_m=I+q^m M_2(\mathbb Z_q)$. By multiplicativity of the absolute value, $q^m\mathbb Z_q=\{x:|x|_q\le q^{-m}\}=\{x:|x|_q<q^{1-m}\}$, where the second equality uses the nonzero values from step 1.2. Consequently $C_m$ is the trace in $G$ of the product of the four entry balls of radius $q^{1-m}$ about the entries of $I$. These traces form a basis at $I$ in the entry topology by [F9], since $q^{1-m}\to0$ by [F13]. For fixed $g\in G$ and any $A,B\in G$, each entry of $gB-gA$ has absolute value at most $\max_{i,j}|g_{ij}|_q\max_{i,j}|B_{ij}-A_{ij}|_q$ by [F7]. Using the entry balls in [F9], this bound gives continuity of left translation, and the same bound with $g^{-1}$ gives continuity of its inverse. In Wedhorn’s group topology, left translation and its inverse are continuous by [F12] and [F16]. In either topology, the preimage under left translation of a neighbourhood of $g$ is a neighbourhood of $I$ and contains some $C_m$. The image $gC_m$ is itself a neighbourhood of $g$ by continuity of the inverse translation. Thus the sets $gC_m$ form a neighbourhood basis at each $g$ in both topologies. In either topology a set is open exactly when it contains one of these basic neighbourhoods about each of its points, by [F16]. Therefore the two topologies agree. [F7, F9, F12, F13, F15, F16, step 1.2]

3.1 Let $S$ be the set of nonnegative integers with nonzero $K_{1,q}(n)$-fixed space. It is nonempty by the hypothesis. By [F3] its inverse image under $\iota$ is nonempty and has a least element $k$. Since $\iota$ preserves order and maps this inverse image onto $S$, $\iota(k)$ is the least element of $S$. The least element is unique by antisymmetry. [given, F3, step 2.1]

4.1 Let $\rho'$ be another complex representation of $G$, on a complex vector space $V'$. An isomorphism from $\rho$ to $\rho'$ is an invertible complex-linear map $T:V\to V'$ such that $T\rho(g)v=\rho'(g)Tv$ for every $g\in G$ and $v\in V$. For such an isomorphism, $T$ sends vectors fixed by $K_{1,q}(n)$ to vectors fixed by that subgroup in $\rho'$. The same identity rearranged with $T^{-1}$ gives the reverse map. Since the restrictions are linear inverses and preserve zero, the two sets of qualifying indices coincide and the exponent is invariant under representation isomorphism. [F1, F2, step 2.1, step 3.1]

5.1 At every positive index the bijection in [F4] identifies the nonzero fixed-vector tests for the two conventions. It is induced by an invertible linear map $\rho(W_n)$, so it preserves nonzero vectors in both directions. At zero the full integral fixed space gives the same test, including for the literal unit condition in [F4]. If $\rho$ meets the conditions in [F9], it is irreducible and satisfies Wedhorn’s admissibility test by (2.1.3)–(2.1.4) in the common topology of step 2.2. For $\mathrm{GL}_2$, the sum in Wedhorn’s genericity test (2.4.2) is just the upper-right entry $x$. The character meets Wedhorn’s unit modulus condition by step 1.3, so the functional in [F9] gives genericity. By (2.4.3)(3) in [F9], genericity also holds for the nontrivial additive character fixed in [F5]. Under these conditions the conductor definition in [F5] applies over the field from step 1.2. The source uses exactly the indices in $S$ and its least index is $a(\rho)$. [F2, F4, F5, F9, step 1.2, step 3.1, step 2.2, step 1.3] ∎
