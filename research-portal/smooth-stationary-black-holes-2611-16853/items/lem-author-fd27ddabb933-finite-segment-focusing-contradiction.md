---
id: lem-author-fd27ddabb933-finite-segment-focusing-contradiction
title: A sufficiently long focal-free boundary segment contradicts negative
  outgoing expansion
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-fd27ddabb933-source-normal-null-generator
  - lem-author-fd27ddabb933-outward-null-affine-normalization
  - lem-null-optics-jacobian-comparison-input
  - physics:thm-gr-local-geodesics-and-exponential-map
  - def-null-screen-expansion-and-focal-data
  - math:def-axiom-of-choice
  - physics:def-gr-metric-selected-connection
dependency_roles:
  lem-author-fd27ddabb933-source-normal-null-generator: mathematical-premise
  lem-author-fd27ddabb933-outward-null-affine-normalization: mathematical-premise
  lem-null-optics-jacobian-comparison-input: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 8
---

## Statement

Work in ZFC. Use the full data and hypotheses of the source-normal null-generator construction on the smooth globally hyperbolic time-oriented Lorentzian four-manifold $(\mathcal E,g,N)$ of signature $(-,+,+,+)$, with compact spacelike source $A\subset\tau^{-1}(0)$ and earliest cylinder contact $p_R$. Identify $A=S_\epsilon$ with the source graph in the outward affine-normalization lemma and assume that lemma's full hypotheses on the same exterior and segment, including $p_R\notin K$. Let $\gamma:[0,\ell]\to\mathcal E$ be the generator from $A$ to $p_R$ supplied by the source-normal construction, after the positive affine rescaling supplied by the normalization lemma. Thus its initial tangent is exactly the smooth outgoing null field $L_\epsilon$ at its source point.

Suppose $\delta_*>0$, the outgoing source expansion in this gauge satisfies $\theta_{L_\epsilon}\le-\delta_*$, the affine length satisfies $\ell>2/\delta_*$, and $\operatorname{Ric}(\dot\gamma,\dot\gamma)\ge0$ along the segment. Then the source-normal focal exclusion and Raychaudhuri are incompatible. The requisite local normal geodesic family exists through the focal bound because this finite segment exists beyond it; no null-completeness assumption is used.

## Statement references

[[lem-author-fd27ddabb933-source-normal-null-generator]]

[[lem-author-fd27ddabb933-outward-null-affine-normalization]]

[[def-null-screen-expansion-and-focal-data]]

[[physics:def-gr-metric-selected-connection]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

[F1] Under its full hypotheses, the source-normal generator construction supplies this segment from $A$ to its earliest contact $p_R$, with no focal point to $A$ strictly before $p_R$, measured from $A$ toward $p_R$. Its positive affine reparametrizations preserve that focal exclusion. [[lem-author-fd27ddabb933-source-normal-null-generator]]

[F2] The affine source scale is exactly the outgoing null field for which the negative expansion bound is supplied. [[lem-author-fd27ddabb933-outward-null-affine-normalization]]

[F3] Null Raychaudhuri gives a focal point by two divided by the absolute negative initial expansion if the smooth normal congruence exists through that parameter. [[lem-null-optics-jacobian-comparison-input]]

[F4] For the metric-selected connection on a smooth time-oriented Lorentzian four-manifold, the maximal geodesic parameter interval is open and the geodesic evaluation domain is open with smooth evaluation. In particular, nearby initial data have a common smooth flow through any compact parameter interval of an existing segment. [[physics:thm-gr-local-geodesics-and-exponential-map]]

[F5] Focal points are loss of rank of the normal screen Jacobi map. [[def-null-screen-expansion-and-focal-data]]

[F6] The metric-selected connection is metric-compatible and torsion-free: $Xg(Y,Z)=g(\nabla_XY,Z)+g(Y,\nabla_XZ)$ and $\nabla_XY-\nabla_YX=[X,Y]$. Its coordinate coefficients are symmetric in their two lower indices. The supplier has domain mathematics. [[physics:def-gr-metric-selected-connection]]

[A1] Work in ZFC, including the countable and dependent choice required by the invoked geodesic, compactness and causal interfaces. [[math:def-axiom-of-choice]]

## Proof

**Given:** The assumptions in the Statement.

**Goal:** Establish the stated conditional claim.

1.1 Let $a=\gamma(0)$ and use the smooth outgoing null normal field $L_\epsilon$ on a surface neighborhood of $a$ in $A$. The existing affine segment and its endpoint in the smooth open spacetime belong to a maximal geodesic defined on an open interval containing $[0,\ell]$. By [F4], openness of the flow domain and compactness of this parameter interval give a common surface neighborhood $U$ of $a$ and an open interval $J\supset[0,\ell]$ on which $F(y,\lambda)=\gamma_{y,L_\epsilon(y)}(\lambda)$ is smooth. Its central generator is the given $\gamma$ by uniqueness. Every parameter curve is affine, and metric compatibility gives $\partial_\lambda g(L,L)=2g(\nabla_LL,L)=0$, where $L=\partial_\lambda F$. Its initially nonzero future null tangent therefore remains future null; it cannot vanish at a later time by geodesic uniqueness. [A1, F2, F4, F6, given, construct, algebra]

2.1 For a source-coordinate variation let $V=\partial_sF$. The parameter derivatives commute. In any ambient chart, the mixed second derivatives of $F$ agree and the symmetric connection coefficients in [F6] give $D_\lambda V=D_sL$ along the map, including at rank loss. Since $D_\lambda L=0$, metric compatibility yields $\partial_\lambda g(L,V)=g(L,D_\lambda V)=g(L,D_sL)=\tfrac12\partial_s g(L,L)=0$. The initial value is zero because $L_\epsilon$ is normal to $A$, so every variation field is orthogonal to $L$. Before screen rank loss, the two source variation fields are independent modulo $L$; together with the nonzero $L$ they span the three-dimensional space $L^\perp$. Thus the family is locally an immersed null hypersurface congruence on the regular interval, as required by [F3]. Its initial optical expansion is precisely $\theta_{L_\epsilon}$ by [F2] and [F5]. [F2, F3, F5, F6, step 1.1, algebra]

3.1 Apply [F3] with nonnegative null Ricci curvature and $\theta(0)=\theta_{L_\epsilon}(a)\le-\delta_*<0$. It forces a focal instant no later than $2/|\theta(0)|\le2/\delta_*<\ell$. This is strictly before the endpoint, contradicting [F1]. The smooth normal geodesic family is defined through that bound by step 1.1 and has the required null hypersurface structure wherever its screen map is regular by step 2.1; no existence past the bound was inferred from the focusing inequality. [F1, F3, F5, step 1.1, step 2.1, given, contradiction] ∎
