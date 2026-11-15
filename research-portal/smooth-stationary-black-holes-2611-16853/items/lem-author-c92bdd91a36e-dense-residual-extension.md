---
id: lem-author-c92bdd91a36e-dense-residual-extension
title: Extending smooth equation residuals from a dense nonzero-field locus
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-source-free-geometric-electrovacuum-data
  - physics:lem-emg-lorentz-hodge-calculus
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - physics:def-gr-curvature-tensor-and-derived-tensors
  - math:cor-two-continuous-maps-into-a-hausdorff-space-agreeing-on-a-dense-set-are-equal
  - math:def-axiom-of-choice
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  physics:lem-emg-lorentz-hodge-calculus: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  physics:def-gr-curvature-tensor-and-derived-tensors: mathematical-premise
  math:cor-two-continuous-maps-into-a-hausdorff-space-agreeing-on-a-dense-set-are-equal: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references: []
dependency_level: 1
---

## Statement

Work in ZFC, including the Axiom of Choice. Let $U$ be an open region of a smooth Hausdorff second-countable four-manifold without boundary, equipped with a smooth Lorentzian metric $h$ of signature $(-,+,+,+)$, an independently specified orientation $o$, and a smooth $h$-timelike vector field $N$ selecting a time orientation. Let $T$ be a smooth vector field on $U$ (a section of $TU$), and let $H$ be a smooth real two-form there. Suppose $D:=\{x\in U:T_x\ne0\}$ is dense in $U$ and the source-free geometric electrovacuum equations hold on $D$. Then they hold on all of $U$, including the zeros of $T$. The Hodge star uses $h$ and $o$, and all raised indices use $h^{-1}$. Density is a required hypothesis; smoothness alone does not imply it for an arbitrary vector field. No Killing-field or stationarity condition on $T$ is required.

## Facts & Assumptions

[A1] Use [[math:def-axiom-of-choice]], as in the geometric electrovacuum interface. This includes the countable choice assumed in the smooth Lorentzian and Hodge suppliers; the dense-set argument below makes no sequence choices.

[F1] Use the signature, index and curvature conventions of [[def-stationary-lorentzian-data]] only. The lemma does not assume that $(h,T)$ is stationary; the regularity suppliers below apply to the specified Lorentzian metric without a Killing field.

[F2] The equations and metric-specific Hodge star have the meanings in [[def-source-free-geometric-electrovacuum-data]], applied to $(U,h,N,o,H)$. Write their residuals as

$$\mathcal R_{ab}:=\operatorname{Ric}(h)_{ab}-2\left(H_{ac}H_b{}^c-\frac14h_{ab}H_{cd}H^{cd}\right),\qquad P:=\mathrm dH,\qquad Q:=\mathrm d(\star_hH).$$

The equations are exactly $\mathcal R=0$, $P=0$ and $Q=0$.

[F3] On an oriented, time-oriented smooth Lorentzian four-manifold, [[physics:lem-emg-lorentz-hodge-calculus]] supplies the smooth Hodge bundle map and the exterior derivative of smooth forms, including its local coordinate formula.

[F4] [[physics:def-gr-inverse-metric-and-musical-isomorphisms]] supplies the smooth inverse metric and index raising. [[physics:def-gr-curvature-tensor-and-derived-tensors]] defines the smooth curvature and Ricci fields of the metric-selected connection, with the conventions in [F1]. These are mathematical interfaces for arbitrary smooth Lorentzian metrics.

[F5] [[math:cor-two-continuous-maps-into-a-hausdorff-space-agreeing-on-a-dense-set-are-equal]] states that continuous maps from a topological space to a Hausdorff space which agree on a dense subset agree everywhere.

## Proof

**Given:** The geometric data and dense-locus equation hypotheses in the Statement.

**Goal:** Show that all three electrovacuum residuals vanish throughout $U$.

1.1 The data $(U,h,N,o,H)$ satisfy the dimensional, smoothness, orientation and time-orientation hypotheses of [F2] and [F3]. By [F4], $h^{-1}$ and $\operatorname{Ric}(h)$ are smooth; finite contractions and products with $H$ make $\mathcal R$ smooth. By [F3], $\star_hH$, $P=\mathrm dH$ and $Q=\mathrm d(\star_hH)$ are smooth forms. Thus all three residuals have continuous real coordinate components in every chart. The choice convention in [A1] covers that inherited by these geometric suppliers. [given, A1, F1, F2, F3, F4]

2.1 Let $V\subset U$ be any coordinate-chart domain. The set $D\cap V$ is dense in $V$: every nonempty relatively open subset of $V$ is open in $U$, because $V$ is open, and therefore meets $D$. For each coordinate component $r:V\to\mathbb R$ of $\mathcal R$, $P$ or $Q$, step 1.1 gives continuity, and the equation hypothesis gives $r=0$ on $D\cap V$. The constant zero map is continuous and $\mathbb R$ is Hausdorff, so [F5] implies $r=0$ on $V$. Every point lies in such a chart, hence all three residuals vanish on $U$, proving the asserted equations also at zeros of $T$. This argument uses the stipulated density, not merely nonvanishing at one point. [given, F2, F5, step 1.1] ∎
