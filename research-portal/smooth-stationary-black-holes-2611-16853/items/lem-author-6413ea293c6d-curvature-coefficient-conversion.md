---
id: lem-author-6413ea293c6d-curvature-coefficient-conversion
title: General curvature coefficient in the outward hypersurface gauge
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-6413ea293c6d-null-variation-normalization
  - lem-author-6413ea293c6d-second-form-and-connection-signs
  - def-surface-area-flux-and-null-variation-data
  - physics:def-gr-curvature-tensor-and-derived-tensors
dependency_roles:
  lem-author-6413ea293c6d-null-variation-normalization: mathematical-premise
  lem-author-6413ea293c6d-second-form-and-connection-signs: mathematical-premise
  def-surface-area-flux-and-null-variation-data: mathematical-premise
  physics:def-gr-curvature-tensor-and-derived-tensors: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 8
---

## Statement

In [[lem-author-6413ea293c6d-null-variation-normalization]] and [[lem-author-6413ea293c6d-second-form-and-connection-signs]], write $G=\operatorname{Ric}-\tfrac12\operatorname{Scal}_g g$ for the Einstein tensor, and define the scalar $Y:=V|\chi_l|_q^2+G(l,u)$. For the unit outward variation of [[def-surface-area-flux-and-null-variation-data]], $Y=\tfrac12|\chi_L|_q^2+G(L,n)=\tfrac12|\chi_L|_q^2+\tfrac12G(L,L)+G(L,\underline L)$. In particular, if $\chi_L=0$ and $G(L,L)=0$, then $Y=G(L,\underline L)$. Vanishing expansion alone is not substituted for these two conditions.

## Facts & Assumptions

[F1] The normalized null decomposition and second-form identifications hold under the declared surface hypotheses. [[lem-author-6413ea293c6d-null-variation-normalization]] [[lem-author-6413ea293c6d-second-form-and-connection-signs]] [[def-surface-area-flux-and-null-variation-data]]

[F2] Ricci curvature, scalar curvature and the Einstein tensor are the smooth metric-derived tensors of [[physics:def-gr-curvature-tensor-and-derived-tensors]], Definition (c), on the smooth time-oriented Lorentzian four-manifold of [F1]. In particular, $G$ is a covariant two-tensor and is bilinear on each tangent space.

## Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Establish its identities with the indicated normalizations.

1.1 The normalization lemma gives $V=1/2$, $u=n$ and $l=L$. Substitution into the defining scalar gives the first formula, using the same second fundamental form as the expansion. [given, F1, algebra]

2.1 The gauge identity $n=L/2+\underline L$ and bilinearity give the second formula. Setting the explicitly assumed $\chi_L$ and $G(L,L)$ to zero yields the final equality, without discarding either term otherwise. [step 1.1, F1, F2, algebra] ∎
