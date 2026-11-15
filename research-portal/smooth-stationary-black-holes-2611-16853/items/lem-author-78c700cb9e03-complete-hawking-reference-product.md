---
id: lem-author-78c700cb9e03-complete-hawking-reference-product
title: A complete timelike collar flow is a reference product
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-killing-field
  - def-spacelike-maximal-hypersurface-data
  - physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets
  - math:def-local-and-global-flow
  - lem-author-78c700cb9e03-invariant-normal-boost-coordinates
  - lem-author-78c700cb9e03-bounded-rapidity-reference-graph
  - lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow
dependency_roles:
  physics:def-gr-killing-field: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  lem-author-78c700cb9e03-invariant-normal-boost-coordinates: mathematical-premise
  lem-author-78c700cb9e03-bounded-rapidity-reference-graph: mathematical-premise
  lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 5
---

## Statement

In the complete stationary-collar model, let $V^\circ$ be the original reference graph $\tau=a(r,y)$ for $0<r<r_0$. Suppose $K$ is future timelike on this graph for every metric in the family. Then $(s,x)\mapsto\phi_s^K(x)$ is a diffeomorphism from $\mathbb R\times V^\circ$ onto $D_0$. It is future timelike along every orbit for every metric in the family. If the original reference section is Cauchy in the original exterior, this product agrees with its unique Cauchy intersection; it does not require the deformed exteriors to be globally hyperbolic.

## Statement references

[[def-spacelike-maximal-hypersurface-data]]

[[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]

[[math:def-local-and-global-flow]]

[[physics:def-gr-killing-field]]

[[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]]

[[lem-author-78c700cb9e03-bounded-rapidity-reference-graph]]

[[lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow]]

## Facts & Assumptions

[F1] The complete boost/circle extension identifies $D_0$ with $(0,r_0)\times\mathbb R\times S$, with $K=\partial_\tau$ and the reference graph as stated. [[lem-author-78c700cb9e03-invariant-normal-boost-coordinates]] [[lem-author-78c700cb9e03-bounded-rapidity-reference-graph]] [[lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow]]

[F2] A spacelike reference section has a future normal. A Cauchy set meets every inextendible causal curve at exactly one parameter value in the original domain. [[def-spacelike-maximal-hypersurface-data]] [[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]

[F3] Complete field flows obey the flow law. [[math:def-local-and-global-flow]]

[F4] The complete-collar extension makes $K$ Killing for each $g_q$. A Killing field is defined by $\mathcal L_Kg_q=0$, where the Lie derivative is the derivative at zero of the metric pulled back by the local flow. [[lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow]] [[physics:def-gr-killing-field]]

[F5] In the stationary-saturation construction, $t_0(r,\tau,y)$ is the time at which the formal $T$ orbit meets the reference graph at $x_0\in C$, and $\mathcal F(r,\tau,y)=\phi^T_{-t_0}(x_0)$. The bounded-root estimate is $|\tau+t_0|\le A$. The original stationary-product time $t_D$, normalized by $t_D|_C=0$, is its elapsed $T$-flow time. [[lem-author-78c700cb9e03-stationary-saturation-complete-hawking-flow]] [[lem-author-78c700cb9e03-bounded-rapidity-reference-graph]]

## Proof

**Given:**The stated data and complete hypotheses.

**Goal:** Establish the conclusions on the domains and parameter ranges specified.

1.1 In the full model the reference-flow map is $(s,r,y)\mapsto(r,a(r,y)+s,y)$. Its smooth inverse is $(r,\tau,y)\mapsto(\tau-a(r,y),r,y)$, so it is a global diffeomorphism onto $D_0$, not just a local transverse flow map. For each $q$, the flow definition in [F4] and the translation form of the $K$ flow give $0=(\mathcal L_Kg_q)_{\tau\tau}=\partial_\tau(g_q)_{\tau\tau}$. Hence $g_q(K,K)$ is constant along each orbit and is negative by its value at the reference point. Continuity in the given time orientation keeps $K$ future-directed along this connected timelike orbit. [given, F1, F3, F4]

2.1 In the original stationary product, [F5] gives $t_D(\mathcal F(r,\tau,y))=-t_0(r,\tau,y)$, since $x_0\in C$ has time zero and $\mathcal F$ is obtained by flowing it for time $-t_0$. Thus the bounded-root estimate gives $|t_D-\tau|=|t_0+\tau|\le A$. Along a $K$ orbit $\tau$ tends to both infinities, so $t_D$ does too. As $t_D$ is a continuous real coordinate on the entire original exterior, the orbit can have no endpoint there in either direction and is therefore inextendible there. By step 1.1 it is timelike for the original metric, so the original Cauchy condition [F2] makes its displayed reference intersection the unique one. This comparison uses only the original metric; no analogous causal-completeness property of a deformed metric has been assumed. [F1, F2, F5, step 1.1] ∎
