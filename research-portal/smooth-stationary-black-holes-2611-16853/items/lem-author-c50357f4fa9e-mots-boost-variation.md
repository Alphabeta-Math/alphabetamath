---
id: lem-author-c50357f4fa9e-mots-boost-variation
title: Boost dependence of expansion variation and the MOTS gauge
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-c50357f4fa9e-outward-graph-null-gauge
  - lem-author-c50357f4fa9e-linear-expansion-variation
  - physics:def-gr-fx-null-screen-geometry
  - math:thm-chain-rule-for-differentials-of-smooth-maps
  - math:def-affine-connection-on-a-smooth-manifold
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:def-countable-choice
dependency_roles:
  lem-author-c50357f4fa9e-outward-graph-null-gauge: mathematical-premise
  lem-author-c50357f4fa9e-linear-expansion-variation: mathematical-premise
  physics:def-gr-fx-null-screen-geometry: mathematical-premise
  math:thm-chain-rule-for-differentials-of-smooth-maps: mathematical-premise
  math:def-affine-connection-on-a-smooth-manifold: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:def-countable-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 4
---

## Statement

Assume countable choice $\mathrm{AC}_\omega$. Let $S$ and its canonical graph gauge be as in the linear-expansion variation lemma. Let $u(t,p)$ be a jointly smooth admissible graph path on a common open parameter interval containing $0$, with $u(0,p)=0$. A **marginally outer trapped surface** (MOTS) here means $\theta_{L_0}=0$ identically on $S$ for the chosen outward future null ray. For any jointly smooth real $f(t,p)$ with $f(0,p)=0$, replace the normals along $F_{u(t)}$ by $\widehat L_t=e^{f(t,p)}L_{u(t)}$ and $\widehat{\underline L}_t=e^{-f(t,p)}\underline L_{u(t)}$. If $\dot u(0)=\phi$, their pulled-back expansion obeys
$$\left.\partial_t\widehat\Theta_t\right|_0=\mathcal L\phi+\dot f(0,\cdot)\theta_{L_0}.$$
Hence at a MOTS this variation is unchanged by every such smooth boost fixing the base normal. If the base scale changes by a smooth $f_0(p)$, the variation at a MOTS is instead multiplied by $e^{f_0}$; absolute equality is not asserted for different base scales. A smooth reparametrization of the graph by diffeomorphisms $\eta_t:S\to S$ with $\eta_0=\mathrm{id}$ adds $d\theta_{L_0}(\dot\eta_0)$, which is also zero at a MOTS.

## Facts & Assumptions

[F1] [[lem-author-c50357f4fa9e-outward-graph-null-gauge]] fixes the base normal $L_0=n+\nu$ and the graph gauge.

[F2] Under the geometric and graph-domain hypotheses inherited in the Statement and countable choice in [F6], [[lem-author-c50357f4fa9e-linear-expansion-variation]] supplies the canonical variation $\mathcal L\phi$ for the stated jointly smooth admissible graph path with $u(0,p)=0$.

[F3] [[physics:def-gr-fx-null-screen-geometry]] supplies the expansion trace and its boost scaling; [[math:thm-chain-rule-for-differentials-of-smooth-maps]] supplies differentiation of smooth composites.

[F4] [[math:def-affine-connection-on-a-smooth-manifold]] supplies the connection product rule $\nabla_X(aY)=X(a)Y+a\nabla_XY$. The along-surface derivative convention in [F3] permits applying this rule to local ambient extensions.

[F5] [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]] defines the diffeomorphisms $\eta_t:S\to S$ used for reparametrization. The assumed smooth family means $(t,p)\mapsto\eta_t(p)$ is jointly smooth.

[F6] Adopt countable choice $\mathrm{AC}_\omega$ in the sense of [[math:def-countable-choice]]. It meets the inherited graph-construction requirements of [F2] and the smooth tangent-bundle and time-orientation conventions of [F3]. No stronger choice principle is assumed.

## Proof

**Given:** The geometric and graph-domain data of the Statement, countable choice in [F6], the jointly smooth admissible graph path with $u(0,p)=0$, and the smooth boost with specified base scale.

**Goal:** Establish the precise extent of gauge independence.

1.1 The path hypotheses and [F6] meet the requirements of [F2] and [F3]. For any graph-tangent $X,Y$, the product rule in [F4], applied through the along-surface convention in [F3], yields $g(\nabla_X(e^fL),Y)=e^fg(\nabla_XL,Y)+e^fX(f)g(L,Y)$. The last term is zero because $L$ is normal. Taking the surface trace gives $\widehat\Theta=e^f\Theta$; reciprocal scaling of the other normal preserves the pairing $-1$. Differentiating and using [F2] gives $\partial_t\widehat\Theta|_0=e^{f_0}(\mathcal L\phi+\dot f_0\theta_{L_0})$. Setting $f_0=0$ gives the displayed formula; setting $\theta_{L_0}=0$ gives both base-scale assertions. Without the MOTS condition, the additional term generally remains. [F1, F2, F3, F4, F6, given, algebra]

2.1 Pullback by the smooth diffeomorphism family in [F5] replaces the scalar by $\Theta_t(\eta_t(p))$. The chain rule differentiates this to $\partial_t\Theta_t|_0+d\theta_{L_0}(\dot\eta_0)$. A function identically zero has zero differential, so the second term vanishes at a MOTS. These computations establish gauge and parameterization independence only with the stated base-scale and smoothness hypotheses. [F2, F3, F5, step 1.1, algebra] ∎
