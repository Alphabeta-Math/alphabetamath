---
id: lem-author-ce4974f559ec-killing-end-flux
title: The mass-one Killing form has electric seed flux minus four pi
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-regular-stationary-vacuum-spacetime
  - def-killing-ernst-notation
  - def-stationary-asymptotic-decay-data
  - def-source-free-geometric-electrovacuum-data
  - math:def-axiom-of-choice
  - physics:lem-emx-unit-sphere-radial-flux
  - math:thm-the-exterior-derivative-commutes-with-pullback
  - math:thm-general-stokes-theorem
dependency_roles:
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  physics:lem-emx-unit-sphere-radial-flux: mathematical-premise
  math:thm-the-exterior-derivative-commutes-with-pullback: mathematical-premise
  math:thm-general-stokes-theorem: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

In a stationary end with $T=\partial_t$, suppose $g_{00}=-1+2/r+O_1(r^{-2})$, $g_{0i}=O_1(r^{-2})$ and $g_{ij}=\delta_{ij}+O_1(r^{-1})$. Put $F=\tfrac12dT^\flat$ and use signature $(-,+,+,+)$ and the orientation for which $dt\wedge dx^1\wedge dx^2\wedge dx^3$ is positive. On the outward oriented coordinate sphere $S_R$ in $t=0$, $\int_{S_R}F=O(R^{-1})$ and $\int_{S_R}\star_gF=-4\pi+O(R^{-1})$. In fact the first integral is exactly zero, since $F$ is an exact spacetime form. No specified leading angular-momentum coefficient of $g_{0i}$ is required.

## Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The regular end, spatial derivative notation and Killing-form convention are fixed. [[def-regular-stationary-vacuum-spacetime]] [[def-killing-ernst-notation]] [[def-stationary-asymptotic-decay-data]]

[F2] The geometric charge convention uses the oriented Lorentzian Hodge star and the factor four pi. Work in ZFC; its choice axiom supplies the countable choice required by general Stokes. [[def-source-free-geometric-electrovacuum-data]] [[math:def-axiom-of-choice]]

[F3] On the standard smooth unit sphere with outward orientation, the area form $d\omega$ satisfies $\int_{\mathbb S^2}d\omega=4\pi$. [[physics:lem-emx-unit-sphere-radial-flux]]

[F4] Exterior differentiation commutes with pullback by a smooth map. General Stokes applies to an oriented smooth manifold of dimension at least one and a compactly supported smooth form of one lower degree; an empty boundary contributes zero. [[math:thm-the-exterior-derivative-commutes-with-pullback]] [[math:thm-general-stokes-theorem]]

## Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The regular end, spatial derivative notation and Killing-form convention are fixed. [[def-regular-stationary-vacuum-spacetime]] [[def-killing-ernst-notation]] [[def-stationary-asymptotic-decay-data]]

[F2] The geometric charge convention uses the oriented Lorentzian Hodge star and the factor four pi. Work in ZFC; its choice axiom supplies the countable choice required by general Stokes. [[def-source-free-geometric-electrovacuum-data]] [[math:def-axiom-of-choice]]

[F3] On the standard smooth unit sphere with outward orientation, the area form $d\omega$ satisfies $\int_{\mathbb S^2}d\omega=4\pi$. [[physics:lem-emx-unit-sphere-radial-flux]]

[F4] Exterior differentiation commutes with pullback by a smooth map. General Stokes applies to an oriented smooth manifold of dimension at least one and a compactly supported smooth form of one lower degree; an empty boundary contributes zero. [[math:thm-the-exterior-derivative-commutes-with-pullback]] [[math:thm-general-stokes-theorem]]



**Proof technique:** direct.

1.1 Stationarity gives $F_{0i}=-\tfrac12\partial_ig_{00}=x^i/r^3+O(r^{-3})$ and $F_{ij}=\tfrac12(\partial_ig_{0j}-\partial_jg_{0i})=O(r^{-3})$. Write $\eta=-dt^2+\sum_i(dx^i)^2$. The inverse-matrix identity and determinant continuity give $g^{-1}-\eta^{-1}=O(r^{-1})$ and $\sqrt{|\det g|}=1+O(r^{-1})$, so the Hodge component formula yields $(\star_gF-\star_\eta F)_{ij}=O(r^{-3})$. The time-space leading part of $F$ is $r^{-2}dt\wedge dr$, while its other coefficients and the time-space remainders are $O(r^{-3})$. [F1, F2]

2.1 On an oriented Minkowski orthonormal coframe, $\star_\eta(dt\wedge dr)=-R^2d\omega$ on $S_R$, since the two-form has norm squared minus one and its wedge with its star must be minus the oriented volume. Here $d\omega$ is the outward unit-sphere area form, and the sphere is identified with $\mathbb S^2$ by the orientation-preserving map $\omega\mapsto(0,R\omega)$. Thus the leading sphere pullback is $-d\omega$. A two-form with Cartesian coefficients $O(R^{-3})$ pulls back under this map with coefficients $O(R^{-1})$, since each of its two tangent slots contributes a factor $R$. Its integral is $O(R^{-1})$ on the fixed unit sphere. The area identity $\int_{\mathbb S^2}d\omega=4\pi$ therefore proves both estimates. [step 1.1, F2, F3]

3.1 Let $i_R:S_R\hookrightarrow M^{\mathrm{end}}$ be the smooth inclusion and let $\alpha_R=i_R^*T^\flat$. Naturality of the exterior derivative gives $i_R^*F=\tfrac12d\alpha_R$. The coordinate sphere $S_R$ is a compact oriented smooth two-manifold without boundary. The smooth one-form $\alpha_R$ has compact support because its support is closed in compact $S_R$. Applying general Stokes in dimension two, with countable choice supplied by ZFC, gives $\int_{S_R}F=\tfrac12\int_{S_R}d\alpha_R=\tfrac12\int_{\partial S_R}\alpha_R=0$. The form $T^\flat$ need only be defined on the end; no filling ball inside the coordinate domain is used. This proves the exact vanishing and completes the Statement without specifying a leading angular-momentum coefficient. [F1, F2, F4, step 2.1] ∎
