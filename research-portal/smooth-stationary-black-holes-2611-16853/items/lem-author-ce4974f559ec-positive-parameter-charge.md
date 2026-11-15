---
id: lem-author-ce4974f559ec-positive-parameter-charge
title: Positive-parameter Harrison charge limits in the original end chart
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-ce4974f559ec-killing-end-flux
  - lem-author-ce4974f559ec-harrison-end-restriction
  - def-harrison-electromagnetic-form
  - def-source-free-geometric-electrovacuum-data
  - math:prop-integration-over-an-oriented-embedded-submanifold
dependency_roles:
  lem-author-ce4974f559ec-killing-end-flux: mathematical-premise
  lem-author-ce4974f559ec-harrison-end-restriction: mathematical-premise
  def-harrison-electromagnetic-form: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  math:prop-integration-over-an-oriented-embedded-submanifold: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 4
---

## Statement

Under the hypotheses of the two end lemmas, with the same orientation and $0<q<1$, the original-coordinate end spheres satisfy $\lim_{R\to\infty}(4\pi)^{-1}\int_{S_R}F_q=0$ and $\lim_{R\to\infty}(4\pi)^{-1}\int_{S_R}\star_{g_q}F_q=\sqrt{1-q^2}$. These are flux integrals of forms on the original spheres; no asymptotically orthonormal change of the transformed time coordinate is required.

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The oriented seed flux and fixed-positive-parameter spatial error have been established. [[lem-author-ce4974f559ec-killing-end-flux]] [[lem-author-ce4974f559ec-harrison-end-restriction]]

[F2] The electromagnetic definition proves the exact identity star of the real form equals the imaginary part of the complex form, using the orientation-preserving Harrison bundle map. [[def-harrison-electromagnetic-form]]

[F3] Integration is by pullback of differential forms, with the geometric charge normalization. [[def-source-free-geometric-electrovacuum-data]] [[math:prop-integration-over-an-oriented-embedded-submanifold]]

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The oriented seed flux and fixed-positive-parameter spatial error have been established. [[lem-author-ce4974f559ec-killing-end-flux]] [[lem-author-ce4974f559ec-harrison-end-restriction]]

[F2] The electromagnetic definition proves the exact identity star of the real form equals the imaginary part of the complex form, using the orientation-preserving Harrison bundle map. [[def-harrison-electromagnetic-form]]

[F3] Integration is by pullback of differential forms, with the geometric charge normalization. [[def-source-free-geometric-electrovacuum-data]] [[math:prop-integration-over-an-oriented-embedded-submanifold]]



**Proof technique:** direct.

1.1 Restrict the error identity of the preceding lemma to $S_R$ and integrate. The two-form coefficient estimate gives $\int_{S_R}E_q=O_q(R^{-1})$ by the sphere rescaling argument. By the exact Hodge identity, $\int_{S_R}(F_q+i\star_{g_q}F_q)=\int_{S_R}\mathcal H_q=-a_q\int_{S_R}(F+i\star_gF)+O_q(R^{-1})$. This uses the actual metric $g_q$ on the left, not the original star. [F1, F2, F3]

2.1 Taking real and imaginary parts and using the seed limits gives magnetic limit zero and electric limit $-a_q(-4\pi)=4\pi a_q$. Dividing by the prescribed $4\pi$ proves the two charge limits. Pullback integrals need no metric-dependent sphere area factor in this calculation, since that information is already in the Hodge two-form. This proves the Statement. [F1, F3, step 1.1] ∎
