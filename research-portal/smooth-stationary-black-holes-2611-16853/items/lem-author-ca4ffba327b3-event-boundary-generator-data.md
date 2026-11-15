---
id: lem-author-ca4ffba327b3-event-boundary-generator-data
title: Smooth event-boundary branches are achronal null geodesic sheets
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-bifurcate-killing-horizon-data
  - physics:def-gr-metric-selected-connection
  - physics:def-gr-future-and-past-sets
  - math:def-axiom-of-choice
  - math:def-integral-curve-of-a-vector-field
  - math:def-geodesic-of-an-affine-connection
  - math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves
  - math:thm-smooth-inverse-function-theorem-on-manifolds
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  physics:def-gr-future-and-past-sets: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-integral-curve-of-a-vector-field: mathematical-premise
  math:def-geodesic-of-an-affine-connection: mathematical-premise
  math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Work in ZFC on a smooth time-oriented Lorentzian four-manifold $(M,g)$. Let $E\subseteq M$ be a specified open end and let $O\subseteq M$ be a specified open set. Suppose $H_+=O\cap\partial I^-(E)$ and $H_-=O\cap\partial I^+(E)$ are smooth null hypersurfaces meeting transversely in an embedded spacelike two-surface $S$. Each branch is achronal in $O$. Its nonzero null radical fields have null geodesic integral curves up to reparametrization. Near $S$ these generators meet $S$ transversely and are orthogonal to it. These conclusions do not, by themselves, assert equality with the entire local causal boundary of $S$.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-bifurcate-killing-horizon-data]]

[[physics:def-gr-metric-selected-connection]]

[[physics:def-gr-future-and-past-sets]]

[[math:def-axiom-of-choice]]

[[math:def-integral-curve-of-a-vector-field]]

[[math:def-geodesic-of-an-affine-connection]]

[[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]]

[[math:thm-smooth-inverse-function-theorem-on-manifolds]]

## Facts & Assumptions

[F1] Chronological futures are future sets and chronological pasts are past sets; their boundaries are achronal, including after time reversal. [[physics:def-gr-future-and-past-sets]]

[F2] The Lorentzian, null-hypersurface and connection conventions define the radical line and a metric-compatible torsion-free connection. Only these geometric conventions are used; no Killing field on the branches is assumed. [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]] [[physics:def-gr-metric-selected-connection]]

[F3] An integral curve of a smooth field $L$ satisfies $\dot\gamma=L\circ\gamma$; such curves exist locally, are unique and depend smoothly on their initial point. An affinely parametrized geodesic satisfies $D_s\dot\gamma=0$ for the specified affine connection. [[math:def-integral-curve-of-a-vector-field]] [[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]] [[math:def-geodesic-of-an-affine-connection]]

[F4] A smooth map whose differential is an isomorphism at a point restricts to a diffeomorphism between neighborhoods of that point and its image. [[math:thm-smooth-inverse-function-theorem-on-manifolds]]

[A1] ZFC includes the choice assumptions inherited through the causal-calculus interfaces. [[math:def-axiom-of-choice]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conclusions without an additional rigidity assumption.

1.1 Apply [F1] to $I^+(E)$ and its time-reversed past counterpart $I^-(E)$. Their ambient boundaries are achronal. Restricting to the specified open set $O$ cannot introduce a timelike curve between branch points, so each branch is achronal in $O$. [F1, A1, given]

1.2 Work locally on either branch $H$ with a nonzero smooth radical field $L$; such local sections exist because the radical is a smooth line subbundle. For every smooth tangent field $Y$, metric compatibility and torsion freedom give $g(\nabla_LL,Y)=-g(L,\nabla_LY)=-g(L,\nabla_YL+[L,Y])=-\tfrac12Yg(L,L)=0$, because $[L,Y]$ is tangent to $H$. Thus $\nabla_LL$ lies in the normal line, which equals the radical line, so $\nabla_LL=aL$. The coefficient $a$ is smooth: locally divide a component of $\nabla_LL$ by a nonvanishing component of $L$. [F2, given, algebra]

2.1 By [F3], $L$ has local integral curves. On any such curve $\gamma:I\to H$, fix $t_0\in I$ and put $b(t)=\exp(-\int_{t_0}^t a(\gamma(u))\,du)$ and $s(t)=\int_{t_0}^t b(u)^{-1}\,du$. Differentiation gives $b'=-a(\gamma)b$ and $s'=b^{-1}>0$, so $s$ is a smooth strictly increasing reparametrization with smooth inverse onto its interval image by [F4]. The rescaled velocity is $d\gamma/ds=bL$, and $D_s(d\gamma/ds)=b(b'+a(\gamma)b)L=0$. Its norm is zero since $L$ is null, proving the geodesic assertion. This is a rescaling along the curve, not an assertion of a single affine scale on the entire branch. [F3, F4, step 1.2, algebra]

3.1 At $p\in S$, the null radical is orthogonal to $T_pS$. It cannot belong to $T_pS$ because that space has positive definite induced metric. Thus it is transverse to $S$ within either three-dimensional branch $H$. Choose a local smooth nonzero radical field $L$ near $p$ in $H$. By [F3], after shrinking, its local flow defines a smooth map $F:(-\varepsilon,\varepsilon)\times W\to H$, $F(t,q)=\Phi(t,q)$, where $W$ is an open neighborhood of $p$ in $S$. Its differential at $(0,p)$ sends $(c,v)\in\mathbb R\oplus T_pS$ to $cL_p+v$, an isomorphism onto $T_pH$ by transversality and dimension. By [F4], shrinking to a smaller product neighborhood makes $F$ a diffeomorphism onto an open branch neighborhood. This supplies the local sheets from $S$; their curves are the null geodesics up to reparametrization from step 2.1. Orthogonality at $S$ and step 1.1 give the remaining claims. Nothing in this construction identifies the branches with the entire local causal boundary of $S$. [F2, F3, F4, step 1.1, step 2.1] ∎
