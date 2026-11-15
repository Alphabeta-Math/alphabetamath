---
id: lem-author-12a8dba09036-complete-volume-preserving-shift-flow
title: Complete volume preserving shift flow on a spherical exterior
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary
  - math:def-smooth-map-between-manifolds-with-boundary
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-smooth-vector-field-as-a-tangent-bundle-section
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves
  - math:thm-unique-maximal-integral-curve-through-each-point
  - math:def-local-and-global-flow
  - math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density
  - math:prop-coordinate-formula-for-riemannian-divergence
  - math:thm-determinant-differential-and-jacobis-formula
  - math:thm-c-one-change-of-variables-for-nonnegative-lebesgue-measurable-functions
  - math:def-axiom-of-choice
dependency_roles:
  math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary: mathematical-premise
  math:def-smooth-map-between-manifolds-with-boundary: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-smooth-vector-field-as-a-tangent-bundle-section: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves: mathematical-premise
  math:thm-unique-maximal-integral-curve-through-each-point: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density: mathematical-premise
  math:prop-coordinate-formula-for-riemannian-divergence: mathematical-premise
  math:thm-determinant-differential-and-jacobis-formula: mathematical-premise
  math:thm-c-one-change-of-variables-for-nonnegative-lebesgue-measurable-functions: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Work in ZFC. Let $\overline C$ be a smooth manifold with compact boundary $S$, diffeomorphic to $\{|x|\ge1\}\subset\mathbb R^3$, and $C=\overline C\setminus S$. Fix a diffeomorphism $F:\overline C\to\{|y|\ge1\}$. Let $h$ be a smooth positive definite metric up to $S$.

Specify an end chart: an open set $E\subset C$ and a diffeomorphism $x:E\to\{x\in\mathbb R^3:|x|>R_0\}$ for some $R_0>0$, such that $K_R=\overline C\setminus x^{-1}(\{|x|>R\})$ is compact for every $R>R_0$. Put $r(p)=|x(p)|$ on $E$. Assume $h$ is asymptotically Euclidean in this chart: its coordinate coefficients satisfy $\sup_{|x|\ge R}\max_{i,j}|h_{ij}(x)-\delta_{ij}|\to0$ as $R\to\infty$. This is the metric convergence convention used here; no rate or derivative decay of $h$ is required.

Let $X$ be smooth up to $S$, tangent to $S$, divergence free for $h$, and with $X^i=O(r^{-2})$ on this end. Here $X^i=dx^i(X)$, and the decay means that there are $A>0$ and $R_1>R_0$ with $|X^i(p)|\le A r(p)^{-2}$ for all $i=1,2,3$ and all $p\in E$ with $r(p)\ge R_1$. The global exterior map $F$ supplies the boundary coordinates; $x$ supplies the asymptotic coordinates, with their relation specified by the compact sets $K_R$.

Then $Z=-X$ has a complete smooth flow $\psi_s:C\to C$, $s\in\mathbb R$, by diffeomorphisms preserving the Riemannian Borel measure $\mu_h$. This measure is positive on nonempty open sets and finite on Borel subsets contained in a bounded exterior annulus, including sets accumulating at $S$. Here a bounded exterior annulus is $\{p\in C:1<|F(p)|\le L\}$ for some finite $L>1$.

## Facts & Assumptions

[F1] A smooth manifold with boundary uses smooth boundary charts, and smoothness up to the boundary is understood in the local-extension sense. A Riemannian metric is a smooth positive definite symmetric two-tensor, allowing boundaries with smoothness up to them. On $C$, a smooth vector field is a smooth tangent-bundle section; up to $S$ its boundary-chart components admit smooth local extensions. A diffeomorphism is a bijection smooth in both directions, using the boundary smoothness convention on $\overline C$. [[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary]] [[math:def-smooth-map-between-manifolds-with-boundary]] [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:def-smooth-vector-field-as-a-tangent-bundle-section]] [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

[F2] Smooth vector fields on the boundaryless interior $C$ have unique local smoothly dependent integral curves and unique maximal integral curves. A flow is global when its domain is $\mathbb R\times C$. [[math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves]] [[math:thm-unique-maximal-integral-curve-through-each-point]] [[math:def-local-and-global-flow]]

[F3] Under countable choice, Riemannian volume is the locally finite Radon Borel measure with chart density $m=\sqrt{\det(h_{ij})}$. Its divergence formula is $\operatorname{div}_hZ=m^{-1}\partial_i(mZ^i)$. [[math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density]] [[math:prop-coordinate-formula-for-riemannian-divergence]]

[F4] The determinant differential gives Jacobi's formula; under countable choice, nonnegative measurable functions satisfy change of variables under a $C^1$ diffeomorphism between open subsets of Euclidean space. Work in ZFC, so countable choice is available for the vector-field formulation in [F1] and the measure and change-of-variables inputs in [F3] and this fact. [[math:thm-determinant-differential-and-jacobis-formula]] [[math:thm-c-one-change-of-variables-for-nonnegative-lebesgue-measurable-functions]] [[math:def-axiom-of-choice]]

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the stated conclusion.

1.1 Use the fixed global exterior diffeomorphism $F$ from the Statement. For $u\in\mathbb S^2$ and $0\le\rho\le\varepsilon$, the map $\kappa(u,\rho)=F^{-1}((1+\rho)u)$ is a smooth product parametrization of a compact collar of $S$; its inverse is $p\mapsto(F(p)/|F(p)|,|F(p)|-1)$. This constructs the collar directly from the given diffeomorphism. Tangency gives $Z\rho(u,0)=0$, and smoothness and compactness bound $|\partial_\rho(Z\rho)|\le K$ on a smaller compact collar. Hence $|Z\rho(u,\rho)|\le K\rho$ by integrating in $\rho$. Along a maximal interior integral curve, $|d(\log\rho)/ds|\le K$ whenever it lies in that collar. On a time interval of finite length $T$, each visit begins either at the initial point or at the collar edge $\rho=\varepsilon$, so this inequality gives a common positive lower bound for $\rho$ throughout all such visits, in either time direction. In the specified end chart, $Zr=-\sum_{i=1}^3X^ix^i/r$, so $|Zr|\le3Ar^{-2}$ for $r\ge R_1$. Choose $R>R_1$; this gives a bound $M$ on $|Zr|$ for $r\ge R$. Integrating from the initial time or the last crossing of $r=R$ bounds $r$ on every finite time interval, in either time direction. Thus the segment lies in some compact $K_{R_*}$. Removing the open boundary collar below the positive lower bound for $\rho$ leaves a compact subset of $C$ containing that segment. The collar estimate uses $F$, and the end estimate uses $x$; compactness of $K_{R_*}$ combines their bounds without requiring the two charts to agree. [given, F1, F2]

2.1 If a maximal orbit had a finite time endpoint, step 1.1 would confine its finite-time terminal portion to a compact subset of $C$. Cover this compact set by finitely many local-flow neighborhoods, and take the minimum of their positive existence times after shrinking the neighborhoods. At a time sufficiently near the purported endpoint the orbit therefore extends beyond it, contradicting maximality and uniqueness. This applies forward and backward, proving completeness. Local smooth dependence, composed over finitely many local-flow intervals around any fixed finite time, makes $(s,p)\mapsto\psi_s(p)$ smooth. Uniqueness gives $\psi_{s+t}=\psi_s\circ\psi_t$ and inverse $\psi_{-s}$, so every $\psi_s$ is a smooth diffeomorphism. [F2, step 1.1]

3.1 In the global exterior coordinates $y=F(p)$ let $m$ be the Riemannian density coefficient and put $J_s(y)=\det D\psi_s(y)>0$, the sign being positive by continuity from the identity and invertibility from step 2.1. Differentiating the flow equation gives $\partial_sD\psi_s=DZ(\psi_s)D\psi_s$. Jacobi's formula and the chain rule therefore give $\partial_s[m(\psi_s(y))J_s(y)]=(\partial_i(mZ^i))(\psi_s(y))J_s(y)=0$, since $\operatorname{div}_hZ=-\operatorname{div}_hX=0$. Hence $m(\psi_s(y))J_s(y)=m(y)$. For any Borel $A\subset C$, the set $\psi_s(A)$ is Borel because $\psi_s$ is a homeomorphism. Apply the nonnegative measurable change-of-variables theorem to $\mathbf1_{\psi_s(A)}m$. It gives $\mu_h(\psi_s(A))=\mu_h(A)$, allowing infinite values. Countable choice required by the measure and change-of-variables suppliers is supplied by the ambient ZFC assumption in [F4]. [given, F3, F4, step 2.1]

4.1 In any small coordinate ball the positive continuous density has a positive lower bound on a smaller ball; thus every nonempty open set has positive measure. Smoothness and positive definiteness up to compact $S$, together with compactness of the closed bounded annulus in $\overline C$, give a bounded smooth density in finitely many bounded charts there. Integrating these bounded densities over their bounded coordinate domains bounds the volume of the interior annulus by a finite sum of finite numbers. Every Borel subset of that interior annulus has no larger measure, even when its closure meets $S$. [given, F1, F3] ∎
