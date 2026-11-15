---
id: def-author-310ff0f53b38-stationary-flow-exterior
title: Complete stationary flow and its exterior region
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-killing-field
  - math:def-local-and-global-flow
  - physics:def-gr-causal-curves-and-reachability
  - def-author-310ff0f53b38-asymptotically-flat-spacelike-end
  - math:def-interior-closure-boundary-top
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-killing-field: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  def-author-310ff0f53b38-asymptotically-flat-spacelike-end: mathematical-premise
  math:def-interior-closure-boundary-top: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Definition

Let $(M,g,N)$ be a time-oriented Lorentzian four-manifold and $T$ a smooth Killing field. Completeness means that the flow $\phi:\mathbb R\times M\to M$ of $T$ is defined for every real time and every point, with $\phi_0$ the identity and $\phi_{s+t}=\phi_s\circ\phi_t$. 

A specified spacelike end $S_{\rm ext}$ has the end-chart data of the spacelike-end interface: a spacelike embedded hypersurface without manifold boundary and a specified diffeomorphism $\chi:\{x\in\mathbb R^3:|x|>R_0\}\to S_{\rm ext}$, where $R_0>0$. Its radius is $r(\chi(x))=|x|$. Only these end-chart data are used here; no asymptotic decay condition is required. Require a specified $R_1>R_0$ such that $T$ is future timelike on $\chi(\{x:|x|\ge R_1\})$. The set $\{x:|x|\ge R_1\}$, including its finite-radius sphere, lies inside the original open chart domain. Restrict the chart to this tail and denote its image again by $S_{\rm ext}$; only this subset is used in the flow saturation $M_{\rm ext}=\bigcup_{t\in\mathbb R}\phi_t(S_{\rm ext})$. All subsequent sets are relative to this specified restricted end.

All chronological relations here are computed in $M$: $I^+(A)=\{q:\exists p\in A,\ p\ll_Mq\}$ and $I^-(A)=\{p:\exists q\in A,\ p\ll_Mq\}$. Define $D=I^+(M_{\rm ext})\cap I^-(M_{\rm ext})$, and define $\mathcal E^+=\partial_M D\cap I^+(M_{\rm ext})$ and $\mathcal E^-=\partial_M D\cap I^-(M_{\rm ext})$. The subscript on $\partial_M$ specifies the ambient topological boundary: for $A\subseteq M$, $\partial_M A=\overline A^{\,M}\setminus\operatorname{int}_M(A)$, with closure and interior taken in the manifold topology of $M$. These are the future and past portions of the boundary of the domain of outer communications; the full future event boundary is instead $\partial_M I^-(M_{\rm ext})$. These expressions define separate sets; no equality between them is built into their names.

## Definition references

[[physics:def-gr-smooth-lorentzian-objects]]

[[physics:def-gr-killing-field]]

[[math:def-local-and-global-flow]]

[[physics:def-gr-causal-curves-and-reachability]]

[[def-author-310ff0f53b38-asymptotically-flat-spacelike-end]]

[[math:def-interior-closure-boundary-top]]

## Facts & Assumptions

[F1] Lorentzian causal character, the Killing-field predicate and the global-flow laws are supplied interfaces. [[physics:def-gr-smooth-lorentzian-objects]] [[physics:def-gr-killing-field]] [[math:def-local-and-global-flow]]

[F2] The relation $\ll_M$ is chronological reachability by future timelike curves in $M$. [[physics:def-gr-causal-curves-and-reachability]]

[F3] The supplied end-chart interface specifies a spacelike embedded hypersurface without manifold boundary and its open exterior chart. Only these end-chart data are used; its additional asymptotic decay predicate is not assumed. The closed tail at $R_1>R_0$ is the specified restriction inside that chart. [[def-author-310ff0f53b38-asymptotically-flat-spacelike-end]]

[F4] In any topological space, the boundary of a subset is its closure minus its interior. Apply this definition to the manifold topology of $M$. [[math:def-interior-closure-boundary-top]]

## Justification

**Given:**The objects and specified data in the Definition.

**Goal:** Verify that the displayed conditions define unambiguous objects and predicates on these data.

1.1 Since $R_1>R_0$, every point with $|x|\ge R_1$ belongs to the original open chart domain. Restricting the specified chart therefore determines the closed tail, including its sphere, as a subset of $M$ without any extension of the chart. Globality of the supplied flow makes $\phi_t(S_{\rm ext})$ defined for every real $t$, so its union specifies a subset of $M$. The flow law gives $\phi_s(M_{\rm ext})=M_{\rm ext}$, since $t\mapsto t+s$ permutes $\mathbb R$. [F1, F3]

2.1 The chronological predicates then specify the two subsets $I^\pm(M_{\rm ext})$. Their intersection, its boundary in $M$, and the indicated intersections determine all the named sets. This construction needs no theorem identifying their topology or smoothness. [F2, F4, step 1.1] ∎
