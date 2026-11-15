---
id: lem-author-64ac0bd1fcc4-orbit-metric-reconstruction
title: Algebraic reconstruction from orbit and horizontal metric data
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-64ac0bd1fcc4-orthogonal-orbit-projection
  - lem-author-64ac0bd1fcc4-orbit-gram-determinant
  - def-stationary-lorentzian-data
  - physics:def-gr-tensor-fields-and-components
  - math:def-tensor-product-of-multilinear-tensors
  - math:lem-matrix-inversion-preserves-ck-regularity
  - math:thm-ck-euclidean-maps-closed-under-algebra-and-composition
dependency_roles:
  lem-author-64ac0bd1fcc4-orthogonal-orbit-projection: mathematical-premise
  lem-author-64ac0bd1fcc4-orbit-gram-determinant: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  physics:def-gr-tensor-fields-and-components: mathematical-premise
  math:def-tensor-product-of-multilinear-tensors: mathematical-premise
  math:lem-matrix-inversion-preserves-ck-regularity: mathematical-premise
  math:thm-ck-euclidean-maps-closed-under-algebra-and-composition: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 9
---

## Statement

For the projection data of [[lem-author-64ac0bd1fcc4-orthogonal-orbit-projection]], define one-forms $\sigma^i(V)=H^{ij}g(X_j,V)$. Then the full metric is $g=H_{ij}\sigma^i\otimes\sigma^j+q$. Thus agreement of $H$, the one-forms $\sigma^i$ and $q$ on a common domain implies agreement of the full metric there. The Gram-matrix and tensor conventions are those of [[lem-author-64ac0bd1fcc4-orbit-gram-determinant]] and [[def-stationary-lorentzian-data]]. This is an algebraic reconstruction identity, not an assertion that an Ernst-map uniqueness theorem alone supplies the global one-forms or identifies the domains.

## Facts & Assumptions

[F1] The inverse Gram matrix defines $P$ and $q$ as in the projection lemma, and every vector decomposes as $V=X_i\sigma^i(V)+PV$. [[lem-author-64ac0bd1fcc4-orthogonal-orbit-projection]] [[lem-author-64ac0bd1fcc4-orbit-gram-determinant]] [[def-stationary-lorentzian-data]]

[F2] A one-form is a smooth covector field, of type $(0,1)$, and a covariant two-tensor field assigns a bilinear form to each tangent space. Equality of such fields is pointwise equality of these multilinear maps. Smoothness of a covector or covariant two-tensor field is tested by smooth component functions in each chart. [[physics:def-gr-tensor-fields-and-components]]

[F3] For covectors $\alpha,\beta$ on the same tangent space, the tensor-product definition gives $(\alpha\otimes\beta)(V,W)=\alpha(V)\beta(W)$. We apply this definition pointwise to the one-forms in the Statement. [[math:def-tensor-product-of-multilinear-tensors]]

[F4] For each finite $r\in\mathbb N$, if a real matrix-valued function on an open Euclidean domain has $C^r$ entries and nonzero determinant everywhere, its inverse has $C^r$ entries. We use this with chart dimension four and matrix size two. [[math:lem-matrix-inversion-preserves-ck-regularity]]

[F5] For every finite $r\in\mathbb N$, finite componentwise sums and products of $C^r$ Euclidean maps are $C^r$; hence the same finite operations preserve smoothness. [[math:thm-ck-euclidean-maps-closed-under-algebra-and-composition]]

## Proof

**Given:**The pointwise tensors and decomposition in the Statement.

**Goal:** Recover the full metric from these data.

1.1 Inserting the vector decompositions into $g(V,W)$, both mixed terms vanish because $PV$ and $PW$ are orthogonal to the generators. The orbit term is $H_{ij}\sigma^i(V)\sigma^j(W)$ and the remaining term is $g(PV,PW)=q(V,W)$. [given, F1]

1.2 In a smooth coordinate chart, $H_{ij}=g_{ab}X_i^aX_j^b$ is a finite sum of products of smooth component functions of the metric and generators. Thus $H_{ij}$ and $\det H=H_{11}H_{22}-H_{12}H_{21}$ are smooth. The nonzero determinant locus is open by continuity. On the chart portion of that locus, apply the matrix-inversion result for every finite $r$ to obtain smooth $H^{ij}$. Each $\sigma^i$ is pointwise linear in its vector argument and has components $\sigma^i_a=H^{ij}g_{ba}X_j^b$, smooth by the finite-operation result. The component criterion makes these covectors smooth one-forms. The formula for $q$ in the projection input also has smooth components by the same finite-operation argument. [F1, F2, F4, F5, algebra]

2.1 The tensor-product evaluation rule gives $(H_{ij}\sigma^i\otimes\sigma^j+q)(V,W)=H_{ij}\sigma^i(V)\sigma^j(W)+q(V,W)$. The equality in step 1.1 holds at every point for every pair of tangent vectors, so pointwise equality of bilinear maps gives the asserted covariant-tensor identity. Equal tensors on its right side therefore give equal metrics on a common domain. It gives no mechanism for constructing that domain or controlling boundary conditions, which remain part of the external global classification input. [F1, F2, F3, step 1.1, step 1.2] ∎
