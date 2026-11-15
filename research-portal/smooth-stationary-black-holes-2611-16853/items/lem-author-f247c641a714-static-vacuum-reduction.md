---
id: lem-author-f247c641a714-static-vacuum-reduction
title: Vacuum curvature of a globally static product
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-f247c641a714-regular-static-exterior-data
  - def-stationary-lorentzian-data
  - math:prop-gradient-hessian-and-divergence-connection-formulas
  - math:prop-christoffel-formula-for-the-levi-civita-connection
  - physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative
  - math:def-scalar-curvature
  - math:def-ricci-curvature
dependency_roles:
  def-author-f247c641a714-regular-static-exterior-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  math:prop-gradient-hessian-and-divergence-connection-formulas: mathematical-premise
  math:prop-christoffel-formula-for-the-levi-civita-connection: mathematical-premise
  physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative: mathematical-premise
  math:def-scalar-curvature: mathematical-premise
  math:def-ricci-curvature: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

For the static product of the regular exterior data, the equation $\operatorname{Ric}(g)=0$ on $\mathbb R\times X$ is equivalent to
$$\Delta_hV=0,\qquad D^2V=V\operatorname{Ric}(h).$$
When these equivalent conditions hold, the scalar curvature of $h$ is zero. The displayed spatial equations then extend continuously to $B$ when $h,V$ are $C^2$ there, in the multiplication form displayed above.

## Statement references

[[def-author-f247c641a714-regular-static-exterior-data]]

[[def-stationary-lorentzian-data]]

[[math:prop-gradient-hessian-and-divergence-connection-formulas]]

[[math:def-scalar-curvature]]

[[math:def-ricci-curvature]]

## Facts & Assumptions

[F1] The formulation and calculations use the following exact object, operator and earlier-result interfaces: [[def-author-f247c641a714-regular-static-exterior-data]] [[def-stationary-lorentzian-data]] [[math:prop-gradient-hessian-and-divergence-connection-formulas]]

[F2] On the smooth interior, the Riemannian Christoffel formula applies to the positive-definite metric $h$, and the nondegenerate four-metric Christoffel formula applies to $g=-V^2dt^2+h$ because $V>0$ there. The ZFC convention of [F1] includes the countable choice assumed by the latter supplier. [[math:prop-christoffel-formula-for-the-levi-civita-connection]] [[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative]]

[F3] For the smooth Riemannian metric $h$ on $X$, scalar curvature is the metric trace of its Ricci tensor: $\operatorname{Scal}(h)=h^{ij}\operatorname{Ric}_{ij}(h)$. The ZFC convention of [F1] includes the countable choice assumed by this definition. [[math:def-scalar-curvature]]

[F4] On the smooth Riemannian interior, $\operatorname{Ric}(h)(A,C)=\operatorname{tr}(Z\mapsto R_h(Z,A)C)$, with $R_h(A,C)E=D_AD_CE-D_CD_AE-D_{[A,C]}E$. This curvature sign agrees with the Lorentzian convention in [F1]. [[math:def-ricci-curvature]]

## Proof

**Given:** The static product of [F1], its Levi–Civita curvature conventions and coordinate Hessian formula, the Christoffel formulas in [F2], the scalar-curvature definition in [F3], and the Riemannian Ricci definition in [F4].

**Goal:** Derive the spatial equations, rather than presume a static vacuum reduction.

1.1 In product coordinates, $g_{tt}=-V^2$, $g_{ti}=0$ and $g_{ij}=h_{ij}$. The Christoffel formulas of [F2] give $\Gamma^t{}_{ti}=V^{-1}\partial_iV$, $\Gamma^i{}_{tt}=Vh^{ij}\partial_jV$, $\Gamma^i{}_{jk}=\Gamma^i{}_{jk}(h)$, with all other mixed Christoffel symbols zero. Substituting into $\operatorname{Ric}_{ab}=\partial_c\Gamma^c{}_{ab}-\partial_b\Gamma^c{}_{ac}+\Gamma^c{}_{cd}\Gamma^d{}_{ab}-\Gamma^c{}_{bd}\Gamma^d{}_{ac}$ yields $\operatorname{Ric}_{tt}(g)=V\Delta_hV$, $\operatorname{Ric}_{ti}(g)=0$, and $\operatorname{Ric}_{ij}(g)=\operatorname{Ric}_{ij}(h)-V^{-1}(\partial_i\partial_jV-\Gamma^k{}_{ij}(h)\partial_kV)$. For the last formula, the extra terms are $-\partial_j(V^{-1}\partial_iV)+V^{-1}\Gamma^k{}_{ij}(h)\partial_kV-V^{-2}\partial_iV\partial_jV=-V^{-1}(D^2V)_{ij}$. [given, F1, F2, F4]

2.1 Since $V>0$ in $X$, vanishing of these components is precisely the two equations in the Statement. Their spatial trace, using [F3], is $V\operatorname{Scal}(h)=\Delta_hV=0$, giving zero scalar curvature. At $B$ all quantities in the multiplication form $D^2V=V\operatorname{Ric}(h)$ and in $\Delta_hV=0$ are continuous under the stated $C^2$ hypotheses, so their zero identities have the continuous boundary limits. This extension does not divide by the vanishing lapse. [given, F1, F3, step 1.1] ∎
