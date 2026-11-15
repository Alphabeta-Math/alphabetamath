---
id: lem-author-66066dbaeb16-boundary-spacelike-tangency-comparison
title: Strict mean-curvature barriers cannot have ordered boundary tangency
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-66066dbaeb16-half-domain-contact-hessian
  - lem-author-66066dbaeb16-spacelike-common-graph-curvature-jet
  - lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency
  - lem-author-66066dbaeb16-timelike-flow-ordering
  - def-spacelike-maximal-hypersurface-data
  - def-normal-graph-and-mean-curvature-data
  - physics:def-gr-smooth-lorentzian-objects
  - math:def-axiom-of-choice
  - physics:def-gr-metric-selected-connection
  - math:def-local-and-global-flow
  - math:thm-fundamental-theorem-on-flows
  - math:cor-finite-dimensional-inner-product-spaces-have-orthonormal-bases
dependency_roles:
  lem-author-66066dbaeb16-half-domain-contact-hessian: mathematical-premise
  lem-author-66066dbaeb16-spacelike-common-graph-curvature-jet: mathematical-premise
  lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency: mathematical-premise
  lem-author-66066dbaeb16-timelike-flow-ordering: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-normal-graph-and-mean-curvature-data: mathematical-premise
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  math:cor-finite-dimensional-inner-product-spaces-have-orthonormal-bases: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Work under the inherited ZFC convention. Let $(M,\gamma,N)$ be a smooth time-oriented Lorentzian four-manifold without boundary, of signature $(-,+,+,+)$, with its Levi–Civita connection $\nabla$. Let $\Sigma_1,\Sigma_2$ be smooth embedded spacelike hypersurfaces meeting at $q$, with the same tangent hyperplane there. In the boundary case assume both are smooth embedded hypersurfaces up to a common smooth boundary surface near $q$, with positive definite induced metric on their full tangent spaces at the boundary, and that their projected interiors select the same side of the common projected boundary in a common scalar-graph chart. Use future unit normals $n_i$ and $H_i=\operatorname{tr}_{h_i}\gamma(\nabla n_i,\cdot)=\operatorname{div}_\gamma n_i$, with divergence computed using a local unit timelike extension; maximal means $H_i=0$.

At an interior contact, or at a boundary contact under these common-boundary conditions, suppose $\Sigma_1$ lies to the future of $\Sigma_2$ on their common local neighborhood. Precisely, in a common scalar-graph chart with future timelike time direction, the first graph height is at least the second on the common spatial neighborhood, a closed half-neighborhood at the boundary. Then $H_1(q)\ge H_2(q)$. Consequently a strictly negative-mean-curvature spacelike hypersurface cannot touch a maximal one from the future; a strictly positive-mean-curvature hypersurface cannot touch it from the past.

For the $K$-flow application, let $U\subseteq M$ be open, let $K$ be a smooth vector field on $U$, and let $C\subseteq U$ be a smooth embedded three-dimensional collar with boundary the smooth surface $S$, with $K|_S=0$. Let $\phi:\mathcal D\to U$ be the maximal flow of $K$, with open domain $\mathcal D\subseteq\mathbb R\times U$. Let $f,g:C\to\mathbb R$ be smooth up to $S$, with $(h(x),x)\in\mathcal D$ for every $x\in C$ and $h\in\{f,g\}$. Define $F_h(x)=\phi(h(x),x)$ directly, and assume both maps are smooth embeddings up to $S$ with spacelike images on their full tangent spaces, including the boundary. Assume $K$ is future timelike on the exterior collar saturation $\{\phi(t,x):x\in C\setminus S,\ (t,x)\in\mathcal D\}$. These variable-time maps specify the boundary-compatible flow graphs; no transversality of $K$ at $S$ is imposed.

If $f\ge g$ on this collar and $f(p)=g(p)$ at $p\in S$, both graph images pass through $p$, have the same tangent hyperplane and inward tangent half-space, and the $f$-graph lies to the future of the $g$-graph on a common local half-neighborhood. Thus the comparison gives $H(F_f(C))(p)\ge H(F_g(C))(p)$, and both strict-barrier exclusions apply. Equal boundary heights supply tangency without equality of $df_p$ and $dg_p$. The comparison uses only finite flow intervals near the common time at each contact; it requires no estimate uniform over unbounded times. For $f\le g$, interchange the two graphs.

## Statement references

[[lem-author-66066dbaeb16-half-domain-contact-hessian]]

[[lem-author-66066dbaeb16-spacelike-common-graph-curvature-jet]]

[[lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency]]

[[lem-author-66066dbaeb16-timelike-flow-ordering]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-normal-graph-and-mean-curvature-data]]

[[physics:def-gr-smooth-lorentzian-objects]]

[[math:def-axiom-of-choice]]

[[physics:def-gr-metric-selected-connection]]

[[math:def-local-and-global-flow]]

[[math:thm-fundamental-theorem-on-flows]]

## Facts & Assumptions

[F1] A nonnegative $C^2$ graph difference on a closed smooth one-sided neighborhood, with zero value and first derivative at contact and a local $C^2$ extension, has positive semidefinite Hessian. The same holds at an interior minimum. [[lem-author-66066dbaeb16-half-domain-contact-hessian]]

[F2] Tangent spacelike hypersurfaces have common scalar-graph charts. When their boundary images and projected interior sides agree, their graphs have extensions across a common projected boundary and can be put on one half-neighborhood. At the shared first jet their mean-curvature difference is the contraction of the Hessian difference with a positive definite matrix. In Lorentzian normal coordinates with time vector the common future normal at contact, that matrix is the identity. [[lem-author-66066dbaeb16-spacelike-common-graph-curvature-jet]]

[F3] For the smooth collar, fixed-surface field, open maximal-flow domain and variable-time embeddings specified in the Statement, both maps fix $S$. Equal boundary heights give equal differentials on the full collar tangent space and the same inward image half-space, without equality of height derivatives. [[lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency]]

[F4] For these boundary-compatible spacelike embeddings, future timelikeness of $K$ on the exterior collar saturation makes ordered flow heights give future-side scalar-graph ordering near equal-height contact, including a common half-neighborhood at $S$. Only finite intervals near the common time are used. [[lem-author-66066dbaeb16-timelike-flow-ordering]]

[F5] Spacelikeness, the future unit normal, the induced metric and maximality have the stated hypersurface meanings, with $H=\operatorname{div}_\gamma n$ for a unit timelike extension. [[def-spacelike-maximal-hypersurface-data]]

[F6] The graph mean-curvature convention is the trace of $(V,W)\mapsto\gamma(\nabla_Vn,W)$, equivalently the unit-extension divergence. The $K$-maps in the Statement are specified directly as in [F3]; they do not require $K$ transverse to $C$ at $S$. [[def-normal-graph-and-mean-curvature-data]] [[lem-author-66066dbaeb16-fixed-surface-flow-graph-tangency]]

[F7] The metric signature, time orientation and future timelike directions are the mathematical Lorentzian conventions. [[physics:def-gr-smooth-lorentzian-objects]]

[F8] Every finite-dimensional real or complex inner product space has an orthonormal basis. This applies to the real three-dimensional tangent space with its positive definite induced metric $h$ at contact. [[math:cor-finite-dimensional-inner-product-spaces-have-orthonormal-bases]]

[A1] The geometric suppliers retain their inherited Axiom of Choice convention; this local composition adds no choice assumption beyond ZFC. [[math:def-axiom-of-choice]]

## Proof

**Given:** The ambient, contact and ordering hypotheses in the Statement; for the $K$-flow conclusion, its explicit collar, flow-domain, embedding and exterior-timelikeness hypotheses.

**Goal:** Prove the oriented mean-curvature comparison, its strict-barrier consequences, and its boundary-compatible $K$-flow application.

1.1 Write the two hypersurfaces as scalar graphs $t=a(z)$ and $t=b(z)$ in the common future-timelike chart in the ordering hypothesis. In the boundary case their boundary images agree and their projected interiors select the same side by hypothesis; [F2] supplies $C^2$ extensions of the graph functions across the common projected boundary. Their common domain is thus a smooth one-sided neighborhood. Tangency gives $(a-b)(q)=0$ and $D(a-b)(q)=0$, while the given future-side ordering gives $a-b\ge0$ on this common domain. [given, F2, F5, F6, F7]

2.1 Apply [F1] to $w=a-b$, using its extension in the boundary case. Its Hessian $B=D^2w(q)$ is positive semidefinite. At the shared first jet, [F2] gives $H_1(q)-H_2(q)=\alpha h^{ij}B_{ij}$ with $\alpha=-\gamma(n,\partial_t)>0$ and positive definite induced metric $h$. In an $h$-orthonormal basis $e_1,e_2,e_3$, whose existence follows from [F8] for this real three-dimensional inner product space, this contraction is $\alpha\sum_{i=1}^3 B(e_i,e_i)\ge0$. This proves the comparison on the actual one-sided domain without assuming a minimum on its exterior. [F1, F2, F8, step 1.1, algebra]

3.1 If the first surface is a future barrier with strictly negative mean curvature and the second is maximal, step 2.1 contradicts $H_1<0=H_2$. If the barrier lies to the past, take the maximal surface as the first surface: step 2.1 gives $0\ge H_{\rm barrier}$, contradicting its strict positive sign. [F5, step 2.1, algebra]

4.1 In the $K$-flow application all the hypotheses of [F3] and [F4] are explicitly assumed. For $p\in S$ with equal heights, [F3] gives $F_f(p)=F_g(p)=p$, a common tangent hyperplane and inward tangent half-space; both images have boundary $S$ locally. Their projected interiors therefore choose the same side. Since $f\ge g$ and $K$ is future timelike on the exterior saturation, [F4] supplies their future-side ordering on a common scalar-graph half-neighborhood, using only a finite time interval near $f(p)=g(p)$. Steps 1.1 and 2.1 give the claimed curvature inequality, and step 3.1 gives both barrier exclusions; interchanging $f,g$ gives the reversed-order version. [given, F3, F4, step 1.1, step 2.1, step 3.1] ∎
