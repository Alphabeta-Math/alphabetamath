---
title: Quantitative lapse and shift bounds force annular timelikeness
status: draft
research_item: lem-author-0a41d659d5ab-annular-timelike-gap
dependency_level: 4
sources:
  references:
    - title: S. Alexakis, A. D. Ionescu and S. Klainerman, Rigidity of stationary
        black holes with small angular momentum on the horizon
      url: https://arxiv.org/pdf/1304.0487v2
      locator: §2.2 Lemma 2.1, (2.9)–(2.10), PDF p. 7; Lemma 2.3, (2.15), PDF pp. 8–9
      statement: Under the source package and sup_{S0}|g(T,T)|<epsilon^2, with epsilon
        sufficiently small depending on A, 0<=n<1 and n>=C1(A)^-1(r-1)/r on
        Sigma1; moreover sup_{Sigma1 minus Sigma_R1}(sum_j|X_j|+sum_ij|nabla_i
        X_j|)<=epsilon^(1/30). The norms on X_j here are its covariant
        coordinate components as in the source transport formulas.
      hypotheses: The complete GR, SBS, maximality and quantitative bounds of
        §§1.1–1.2, with the horizon-smallness parameter sufficiently small
        depending on A. The covariant shift components are measured in the
        source section chart.
      reading_limits: Read Lemmas 2.1, 2.2 and 2.3 and their printed arguments on PDF
        pp. 7–9. The maximum-principle/Hopf estimates, weighted integral
        estimate, interpolation and transport bounds are imported rather than
        reconstructed. Reading the printed arguments is not an independent proof
        review or verification of their cited PDE inputs.
---

## Prerequisites

- [def-author-0a41d659d5ab-aik-quantitative-package](item-def-author-0a41d659d5ab-aik-quantitative-package)
- [lem-author-0a41d659d5ab-horizon-field-norm](item-lem-author-0a41d659d5ab-horizon-field-norm)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:cor-real-spectral-theorem-for-self-adjoint-endomorphisms](https://alphabetamath.cc/item/cor-real-spectral-theorem-for-self-adjoint-endomorphisms)
- [physics:def-causal-classification-of-lorentz-vectors](https://alphabetamath.cc/physics/item/def-causal-classification-of-lorentz-vectors)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Rigidity of stationary black holes with small angular momentum on the horizon · §2.2 Lemma 2.1, (2.9)–(2.10), PDF p. 7; Lemma 2.3, (2.15), PDF pp. 8–9 `](https://arxiv.org/pdf/1304.0487v2)


## Statement

For the AIK quantitative package and $\sup_{S_0}|g(T,T)|<\epsilon^2$, let $C_1=C_1(A)$ be the lapse constant from the explicit external estimate. For all sufficiently small $0<\epsilon<1$ depending only on $A$, the stationary field is strictly timelike on $1+\epsilon^{1/100}\le r\le R_1$ in $\Sigma_0$. More explicitly, once the imported estimates hold, $\epsilon^{7/150}<(8A_1C_1^2)^{-1}$ suffices for this assertion.

## Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The quantitative package includes $A_1^{-1}I\le(h_{ij})\le A_1I$ and the source section coordinates. [def-author-0a41d659d5ab-aik-quantitative-package](item-def-author-0a41d659d5ab-aik-quantitative-package)

[F2] The norm identity and exact horizon-smallness translation are those of [lem-author-0a41d659d5ab-horizon-field-norm](item-lem-author-0a41d659d5ab-horizon-field-norm).

[F3] Lapse and shift components use the hypersurface definitions in [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data).

[F4] The explicit External input supplies $n\ge C_1^{-1}(r-1)/r$ and $\sum_j|X_j|\le\epsilon^{1/30}$ on the bounded annulus, for the covariant shift components $X_j=h_{ji}X^i$.

[F5] A self-adjoint endomorphism of a finite-dimensional real inner product space admits an orthonormal eigenbasis. [math:cor-real-spectral-theorem-for-self-adjoint-endomorphisms](https://alphabetamath.cc/item/cor-real-spectral-theorem-for-self-adjoint-endomorphisms)

[F6] In signature $(-,+,+,+)$, a tangent vector is timelike exactly when its squared Lorentzian norm is negative. [physics:def-causal-classification-of-lorentz-vectors](https://alphabetamath.cc/physics/item/def-causal-classification-of-lorentz-vectors)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conditional conclusion.

1.1 Put $\delta=\epsilon^{1/100}<1$. For $r\ge1+\delta$, monotonicity of $(r-1)/r$ gives $n\ge C_1^{-1}\delta/(1+\delta)\ge\delta/(2C_1)$. Since $h^{-1}\le A_1I$, the covariant-component estimate gives $h(X,X)=h^{ij}X_iX_j\le A_1\sum_jX_j^2\le A_1\epsilon^{1/15}$. The symmetric matrix $H=(h_{ij})$ defines a self-adjoint endomorphism of Euclidean $\mathbb R^3$, since $u^{\mathsf T}Hv=(Hu)^{\mathsf T}v$. By [F5] it has an orthonormal eigenbasis. Applying [F1] to each unit eigenvector puts its eigenvalue in $[A_1^{-1},A_1]$, so the eigenvalues of $H^{-1}$ are the reciprocals of those of $H$ and are therefore at most $A_1$, proving the inverse-metric bound. [F1, F3, F4, F5, algebra]

2.1 The norm identity now yields $g(T,T)\le-(4C_1^2)^{-1}\epsilon^{1/50}+A_1\epsilon^{1/15}$. Since $1/15-1/50=7/150$, the threshold in the Statement bounds the second term by $(8C_1^2)^{-1}\epsilon^{1/50}$, and hence $g(T,T)\le-(8C_1^2)^{-1}\epsilon^{1/50}<0$. By [F6], this strict negativity makes $T$ timelike throughout the stated annulus. All constants in this condition depend only on the fixed source bounds. [step 1.1, F1, F2, F6, algebra] ∎

## External input

Import the source lapse lower bound (2.10) and shift estimate (2.15), with exactly the GR/SBS/maximal and quantitative assumptions stated in the package and the source horizon bound. Only these inequalities are used here; their elliptic, integral, interpolation and transport proofs remain external. The norm estimate uses covariant shift components and the inverse induced metric, avoiding an implicit identification with contravariant components.
