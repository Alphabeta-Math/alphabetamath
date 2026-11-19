---
title: Weight-two discrete series at the real place
status: draft
research_item: def-author-34e2e6a0519f-real-weight-two-discrete-series
dependency_level: 1
---

## Prerequisites

- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)
- [math:def-holomorphic-and-antiholomorphic-discrete-series-models](https://alphabetamath.cc/item/def-holomorphic-and-antiholomorphic-discrete-series-models)
- [math:thm-irreducibility-and-k-types-of-the-discrete-series](https://alphabetamath.cc/item/thm-irreducibility-and-k-types-of-the-discrete-series)
- [math:thm-square-integrability-of-sl2-r-discrete-series-matrix-coefficients](https://alphabetamath.cc/item/thm-square-integrability-of-sl2-r-discrete-series-matrix-coefficients)
- [math:def-matrix-coefficient-of-a-unitary-representation](https://alphabetamath.cc/item/def-matrix-coefficient-of-a-unitary-representation)
- [math:ex-general-and-special-linear-lie-groups](https://alphabetamath.cc/item/ex-general-and-special-linear-lie-groups)
- [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)
- [math:thm-quotient-manifold-by-a-closed-lie-subgroup](https://alphabetamath.cc/item/thm-quotient-manifold-by-a-closed-lie-subgroup)
- [math:thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group](https://alphabetamath.cc/item/thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group)
- [math:def-k-finite-and-smooth-vectors-for-sl2-r](https://alphabetamath.cc/item/def-k-finite-and-smooth-vectors-for-sl2-r)
- [math:lem-kak-integration-formula-for-k-bi-invariant-functions-on-sl2-r](https://alphabetamath.cc/item/lem-kak-integration-formula-for-k-bi-invariant-functions-on-sl2-r)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:def-hilbert-direct-sum-of-unitary-representations](https://alphabetamath.cc/item/def-hilbert-direct-sum-of-unitary-representations)
- [math:def-iwasawa-and-minimal-parabolic-data-for-sl2-r](https://alphabetamath.cc/item/def-iwasawa-and-minimal-parabolic-data-for-sl2-r)
- [math:thm-iwasawa-decomposition-for-sl2-r](https://alphabetamath.cc/item/thm-iwasawa-decomposition-for-sl2-r)
- [math:def-complex-haar-lp-spaces-and-compactly-supported-functions](https://alphabetamath.cc/item/def-complex-haar-lp-spaces-and-compactly-supported-functions)


## Definition

Assume the Axiom of Choice. Write $G=\mathrm{GL}_2(\mathbb R)$ for the group of invertible real two-by-two matrices and $S=\mathrm{SL}_2(\mathbb R)$ for its subgroup of determinant-one matrices. Give both groups the subspace topology from the Euclidean space of real two-by-two matrices. Write $q:G\to\mathrm{PGL}_2(\mathbb R)$ for the quotient by nonzero scalar matrices and give $\mathrm{PGL}_2(\mathbb R)$ the quotient topology induced by $q$.

Let $\rho$ be a strongly continuous unitary representation of $G$ with trivial central character, so every scalar matrix acts as the identity. It has **weight-two discrete-series type** if its restriction to $S$ is unitarily equivalent to the unitary direct sum of the holomorphic and antiholomorphic weight-two discrete-series models. In the holomorphic model the space consists of holomorphic $u$ on the upper half-plane $\mathfrak H$ with $\int_{\mathfrak H}|u(x+iy)|^2\,dx\,dy<\infty$. For $g\in S$ and $g^{-1}=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ the action sends $u(z)$ to $(cz+d)^{-2}u((az+b)/(cz+d))$. The other model is obtained by complex conjugating functions and action. The unitary direct sum uses the sum of the two squared norms and acts on each summand separately.

A strongly continuous unitary representation $\bar\rho$ of $\mathrm{PGL}_2(\mathbb R)$ has weight-two discrete-series type if its pullback $\bar\rho\circ q$ has this type.

## Definition references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)

[math:ex-general-and-special-linear-lie-groups](https://alphabetamath.cc/item/ex-general-and-special-linear-lie-groups)

[math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)

[math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)

[math:def-holomorphic-and-antiholomorphic-discrete-series-models](https://alphabetamath.cc/item/def-holomorphic-and-antiholomorphic-discrete-series-models)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[math:def-hilbert-direct-sum-of-unitary-representations](https://alphabetamath.cc/item/def-hilbert-direct-sum-of-unitary-representations)

## Facts & Assumptions

[A1] The Axiom of Choice applies in particular to countable families. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] With the stated Euclidean subspace topologies, $G$ and $S$ are real Lie groups. The scalar subgroup is central, and $q$ is the algebraic quotient homomorphism. [math:ex-general-and-special-linear-lie-groups](https://alphabetamath.cc/item/ex-general-and-special-linear-lie-groups) [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group) The subspace topology $S$ inherits from the Euclidean matrix space agrees with the one it inherits from $G$, so the inclusion $S\hookrightarrow G$ is continuous. [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[F2] The group quotient by a closed normal subgroup of a finite-dimensional real Lie group is a Lie group with the quotient topology under countable choice. The quotient topology makes the projection continuous. [math:thm-quotient-manifold-by-a-closed-lie-subgroup](https://alphabetamath.cc/item/thm-quotient-manifold-by-a-closed-lie-subgroup) [math:thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group](https://alphabetamath.cc/item/thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group) [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)

[F3] Strong continuity means norm-continuity of every orbit map, and unitary equivalence is given by a unitary intertwiner. [math:def-strongly-continuous-unitary-representation](https://alphabetamath.cc/item/def-strongly-continuous-unitary-representation)

[F4] For the rotation subgroup $K=\mathrm{SO}(2)\subset S$, use $k_\theta=\begin{pmatrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{pmatrix}$. A vector $v$ is $K$-finite for a model action $\sigma$ if the span of $\{\sigma(k)v:k\in K\}$ is finite-dimensional. The two displayed models at weight two are irreducible strongly continuous unitary representations. On $k_\theta$ the holomorphic characters are $e^{-i(2+2j)\theta}$ and the antiholomorphic characters are $e^{i(2+2j)\theta}$ for integers $j\geq0$. [math:def-k-finite-and-smooth-vectors-for-sl2-r](https://alphabetamath.cc/item/def-k-finite-and-smooth-vectors-for-sl2-r) [math:def-holomorphic-and-antiholomorphic-discrete-series-models](https://alphabetamath.cc/item/def-holomorphic-and-antiholomorphic-discrete-series-models) [math:thm-irreducibility-and-k-types-of-the-discrete-series](https://alphabetamath.cc/item/thm-irreducibility-and-k-types-of-the-discrete-series)

[F5] Let $dg$ be the fixed left Haar measure on $S$ used in the KAK integration formula. Write $g=n_xa_sk$ with $n_x=\begin{pmatrix}1&x\\0&1\end{pmatrix}$, $a_s=\operatorname{diag}(e^{s/2},e^{-s/2})$, $x,s\in\mathbb R$ and $k\in K$. In these NAK coordinates it is $e^{-s}\,dx\,ds\,dk$, with $dk$ the Haar probability measure on $K$. [math:def-iwasawa-and-minimal-parabolic-data-for-sl2-r](https://alphabetamath.cc/item/def-iwasawa-and-minimal-parabolic-data-for-sl2-r) [math:thm-iwasawa-decomposition-for-sl2-r](https://alphabetamath.cc/item/thm-iwasawa-decomposition-for-sl2-r) [math:lem-kak-integration-formula-for-k-bi-invariant-functions-on-sl2-r](https://alphabetamath.cc/item/lem-kak-integration-formula-for-k-bi-invariant-functions-on-sl2-r)

[F6] The complex Haar space $L^2(S,dg)$ consists of almost-everywhere classes of measurable complex functions with finite squared-modulus integral against $dg$. [Complex Haar $L^p$ spaces and compactly supported functions](https://alphabetamath.cc/item/def-complex-haar-lp-spaces-and-compactly-supported-functions) For either model action $\sigma$ at weight two, the continuous matrix coefficient $g\mapsto\langle\sigma(g)v,w\rangle$ on $S$ represents a class in $L^2(S,dg)$ when both $v$ and $w$ are $K$-finite. [math:def-matrix-coefficient-of-a-unitary-representation](https://alphabetamath.cc/item/def-matrix-coefficient-of-a-unitary-representation) [math:thm-square-integrability-of-sl2-r-discrete-series-matrix-coefficients](https://alphabetamath.cc/item/thm-square-integrability-of-sl2-r-discrete-series-matrix-coefficients)

[F7] Under the Axiom of Choice, the Hilbert direct sum of two strongly continuous unitary representations of a topological group is again strongly continuous and unitary, with componentwise action and the sum of the two squared norms. [math:def-hilbert-direct-sum-of-unitary-representations](https://alphabetamath.cc/item/def-hilbert-direct-sum-of-unitary-representations)

## Justification

**Given:** The groups and topologies above, the Axiom of Choice and a representation of either input kind in the definition.

1.1 The scalar subgroup is closed in $G$ since the off-diagonal entries are zero and the two diagonal entries are equal, all closed conditions on the entries. It is normal by centrality. Thus $\mathrm{PGL}_2(\mathbb R)$ is a topological group for the indicated quotient topology, and $q$ is a continuous homomorphism. Every orbit map of $\bar\rho\circ q$ is the composition of $q$ with a norm-continuous orbit map of $\bar\rho$. The pullback is unitary and trivial on scalars because $q$ sends them to the identity. [A1, F1, F2, F3]

1.2 Both weight-two model actions are strongly continuous and unitary by [F4]. With the Axiom of Choice and the topological group $S$, [F7] gives those same properties for their Hilbert direct sum. In the holomorphic formula, $-I$ sends $z$ to $z$ and has multiplier $(-1)^{-2}=1$, so $-I$ acts as the identity in both models. Their rotation weights have opposite signs, and replacing $k_\theta$ by $k_{-\theta}$ reverses both signs while preserving the least absolute weight two. Thus the test specifies the same weight under either angle convention. [A1, F1, F4, F7, algebra]

2.1 Each restricted orbit map is the corresponding orbit map on $G$ composed with the continuous inclusion $S\hookrightarrow G$. Restriction along it preserves strong continuity and unitarity. A unitary intertwiner remains an intertwiner on restriction and on pullback, so the test depends only on the unitary equivalence class of either input. [F1, F3, step 1.1]

3.1 For either model action on $S$, apply [F6] at weight two to the matrix coefficient of two $K$-finite vectors. The resulting continuous function represents a class in $L^2(S,dg)$ for the fixed left Haar measure in [F5]. [F4, F5, F6] ∎
