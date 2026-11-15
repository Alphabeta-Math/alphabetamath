---
id: lem-author-cf389990237c-constant-gravity-horizon-komar-integral
title: Constant surface gravity gives the normalized horizon integral
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-cf389990237c-normalized-horizon-komar-data
  - lem-author-cf389990237c-horizon-killing-binormal-contraction
  - math:def-riemannian-volume-form-on-an-oriented-manifold
  - math:prop-linearity-and-additivity-of-integration-over-disjoint-oriented-components
dependency_roles:
  def-author-cf389990237c-normalized-horizon-komar-data: mathematical-premise
  lem-author-cf389990237c-horizon-killing-binormal-contraction: mathematical-premise
  math:def-riemannian-volume-form-on-an-oriented-manifold: mathematical-premise
  math:prop-linearity-and-additivity-of-integration-over-disjoint-oriented-components: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 4
---

## Statement

If the section data in [[def-author-cf389990237c-normalized-horizon-komar-data]] have constant $\kappa$, the local Komar functional is $Q_C[T]=\kappa A_C/(4\pi)$, where $A_C=\int_CdA$. This follows from the binormal contraction in [[lem-author-cf389990237c-horizon-killing-binormal-contraction]] and the induced area convention of [[math:def-riemannian-volume-form-on-an-oriented-manifold]]. No exterior mass identification is asserted.

## Facts & Assumptions

[F1] The functional has factor $-(8\pi)^{-1}$, the integrand equals $-2\kappa$, and $\kappa$ is constant on the compact section. [[def-author-cf389990237c-normalized-horizon-komar-data]] [[lem-author-cf389990237c-horizon-killing-binormal-contraction]] [[math:def-riemannian-volume-form-on-an-oriented-manifold]]

[F2] The area convention is the intrinsic integral of smooth top forms on oriented $C$. The forms $\operatorname{vol}_q$ and $(-2\kappa)\operatorname{vol}_q$ are smooth with compact support because $C$ is compact. The form integral is real-linear on compactly supported smooth top forms, including scalar multiplication by any real constant. [[def-author-cf389990237c-normalized-horizon-komar-data]] [[math:def-riemannian-volume-form-on-an-oriented-manifold]] [[math:prop-linearity-and-additivity-of-integration-over-disjoint-oriented-components]]

## Proof

**Given:**The compact horizon section and constant surface gravity.

**Goal:** Evaluate its local normalized integral.

1.1 Substitute the contraction identity into the defining functional to obtain $Q_C[T]=-(8\pi)^{-1}\int_C(-2\kappa)\,dA$. [given, F1]

2.1 Apply real-linearity of the intrinsic top-form integral to $(-2\kappa)\operatorname{vol}_q$ on $C$, using its compact support and the constant scalar $-2\kappa$. Thus $\int_C(-2\kappa)\,dA=(-2\kappa)\int_CdA$, and step 1.1 gives $Q_C[T]=\kappa(4\pi)^{-1}\int_CdA=\kappa A_C/(4\pi)$. This is a calculation at the section and uses no Stokes theorem at an infinite end. [F1, F2, step 1.1] ∎
