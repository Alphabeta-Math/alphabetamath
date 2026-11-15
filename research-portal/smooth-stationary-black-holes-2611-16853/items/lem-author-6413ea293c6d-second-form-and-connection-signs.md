---
id: lem-author-6413ea293c6d-second-form-and-connection-signs
title: Agreement of expansion and normal-connection conventions
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-surface-area-flux-and-null-variation-data
  - def-null-screen-expansion-and-focal-data
  - lem-author-6413ea293c6d-null-variation-normalization
dependency_roles:
  def-surface-area-flux-and-null-variation-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  lem-author-6413ea293c6d-null-variation-normalization: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Andersson–Mars–Simon, Stability of marginally outer trapped surfaces and
        existence of marginally outer trapped tubes
      url: https://arxiv.org/pdf/0704.2889
      locator: Sections 2–3, printed pages 5–8
dependency_level: 7
---

## Statement

Use the smooth surface and null pair of [[def-surface-area-flux-and-null-variation-data]] and [[def-null-screen-expansion-and-focal-data]]. Define the vector second fundamental form $\mathbf K(X,Y)=-(\nabla_XY)^\perp$ and $H=\operatorname{tr}_q\mathbf K$, where projection is onto the Lorentzian normal plane. Then $g(\mathbf K(X,Y),l)=\chi_l(X,Y)$ and $g(H,l)=\theta_l$. With $k=2\underline L$ as in [[lem-author-6413ea293c6d-null-variation-normalization]], the one-form $s(X)=-g(k,\nabla_Xl)/2$ equals $\zeta(X)=-g(\underline L,\nabla_XL)$.

## Facts & Assumptions

[F1] The surface expansion is the trace of the null second form and the null gauge specifies ζ. [[def-surface-area-flux-and-null-variation-data]] [[def-null-screen-expansion-and-focal-data]] [[lem-author-6413ea293c6d-null-variation-normalization]]

## Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Establish its identities with the indicated normalizations.

1.1 Since $g(Y,l)=0$ on the surface, metric compatibility gives $-g(\nabla_XY,l)=g(Y,\nabla_Xl)=\chi_l(X,Y)$. Projection of $\nabla_XY$ onto the normal plane leaves its pairing with the normal $l$ unchanged. [given, F1, algebra]

2.1 Taking the $q$-trace proves $g(H,l)=\theta_l$. Substituting $k=2\underline L$ and $l=L$ into the displayed definition of $s$ gives $s=\zeta$, including its sign. [step 1.1, F1, algebra] ∎
