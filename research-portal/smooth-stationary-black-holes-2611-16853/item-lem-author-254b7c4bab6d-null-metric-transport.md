---
title: Metric transport along a null generator
status: draft
research_item: lem-author-254b7c4bab6d-null-metric-transport
dependency_level: 3
---

## Prerequisites

- [lem-author-254b7c4bab6d-null-form-screen-descent](item-lem-author-254b7c4bab6d-null-form-screen-descent)
- [lem-author-254b7c4bab6d-null-expansion-rescaling](item-lem-author-254b7c4bab6d-null-expansion-rescaling)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)
- [math:thm-lie-derivative-is-a-derivation-of-the-tensor-algebra](https://alphabetamath.cc/item/thm-lie-derivative-is-a-derivation-of-the-tensor-algebra)
- [math:prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields](https://alphabetamath.cc/item/prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields)
- [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)


## Statement

On the null branch with generator $L$ in [lem-author-254b7c4bab6d-null-form-screen-descent](item-lem-author-254b7c4bab6d-null-form-screen-descent), write $q=g|_{TH}$. For tangent fields $X,Y$, $(\mathcal L_Lq)(X,Y)=2B(X,Y)$. Thus vanishing $B$ means preservation of the degenerate tangent metric along the local generator flow. The zero-trace condition remains invariant under the rescalings in [lem-author-254b7c4bab6d-null-expansion-rescaling](item-lem-author-254b7c4bab6d-null-expansion-rescaling); no implication from zero trace to vanishing $B$ is asserted here. The Lie derivative and connection conventions are those of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

## Facts & Assumptions

[F1] The descended null form is symmetric; the ambient connection is torsion-free and metric-compatible. Positive rescaling multiplies the expansion. [lem-author-254b7c4bab6d-null-form-screen-descent](item-lem-author-254b7c4bab6d-null-form-screen-descent) [lem-author-254b7c4bab6d-null-expansion-rescaling](item-lem-author-254b7c4bab6d-null-expansion-rescaling) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] For any smooth tensor on a smooth manifold, its Lie derivative along a smooth vector field is the derivative at zero of pullback by its local flow. It obeys the tensor-product rule, commutes with contractions, acts on functions by directional differentiation, and acts on vector fields by the Lie bracket. Apply these facts on $H$ to the smooth covariant two-tensor $q$ and the tangent generator $L$; no nondegeneracy of $q$ is required. [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field) [math:thm-lie-derivative-is-a-derivation-of-the-tensor-algebra](https://alphabetamath.cc/item/thm-lie-derivative-is-a-derivation-of-the-tensor-algebra) [math:prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields](https://alphabetamath.cc/item/prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields)

[F3] On every common local flow domain, a smooth tensor has zero Lie derivative if and only if its pullback by each defined flow map equals the tensor. Apply this to $q$ and the local flow of $L$ on $H$; completeness of $L$ is not assumed. [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)

## Proof

**Given:** The branch, tangent metric and generator in the Statement.

**Goal:** Compute the Lie derivative and its stated consequence.

1.1 Regard $q(X,Y)$ as the contraction of $q\otimes X\otimes Y$. The derivation and contraction rules in F2 give $L(q(X,Y))=(\mathcal L_Lq)(X,Y)+q([L,X],Y)+q(X,[L,Y])$. Thus $(\mathcal L_Lq)(X,Y)=L(g(X,Y))-g([L,X],Y)-g(X,[L,Y])$. The brackets here are intrinsic to $H$; ambient extensions of tangent fields give the same brackets on $H$. Replacing each bracket by its torsion-free connection expression and expanding the first term by metric compatibility leaves $g(\nabla_XL,Y)+g(X,\nabla_YL)$. [given, F1, F2]

2.1 Symmetry of $B$ makes this sum $2B(X,Y)$. Hence $B=0$ gives $\mathcal L_Lq=0$. By F3, for the local generator flow $\Phi_t$ this implies $\Phi_t^*q=q$ on every common local flow domain, proving preservation of the degenerate tangent metric. The rescaling statement follows from F1 and asserts only invariance of zero trace. [F1, F3, step 1.1] ∎
