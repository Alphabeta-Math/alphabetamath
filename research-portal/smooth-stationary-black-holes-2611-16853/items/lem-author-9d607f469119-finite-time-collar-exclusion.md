---
id: lem-author-9d607f469119-finite-time-collar-exclusion
title: A finite temporal target cannot be reached from a sufficiently small collar
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - def-stationary-section-time
  - math:def-riemannian-distance-on-a-connected-manifold
  - math:thm-the-riemannian-distance-topology-is-the-manifold-topology
  - math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary
  - math:def-smooth-collar-of-a-manifold-boundary
  - math:def-riemannian-speed-and-length
  - math:def-extended-riemannian-distance-on-a-disconnected-manifold
  - math:def-distance-from-a-point-to-a-subset
  - math:prop-distance-to-a-nonempty-subset-is-one-lipschitz
  - math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric
  - math:def-absolutely-continuous-function
  - physics:lem-gr-temporal-functions-and-time-functions
  - math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions
  - math:thm-gronwall-integral-inequality
  - math:def-countable-choice
  - math:def-dependent-choice
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - physics:lem-gr-observer-projection-decomposition
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-stationary-section-time: mathematical-premise
  math:def-riemannian-distance-on-a-connected-manifold: mathematical-premise
  math:thm-the-riemannian-distance-topology-is-the-manifold-topology: mathematical-premise
  math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary: mathematical-premise
  math:def-smooth-collar-of-a-manifold-boundary: mathematical-premise
  math:def-riemannian-speed-and-length: mathematical-premise
  math:def-extended-riemannian-distance-on-a-disconnected-manifold: mathematical-premise
  math:def-distance-from-a-point-to-a-subset: mathematical-premise
  math:prop-distance-to-a-nonempty-subset-is-one-lipschitz: mathematical-premise
  math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric: mathematical-premise
  math:def-absolutely-continuous-function: mathematical-premise
  physics:lem-gr-temporal-functions-and-time-functions: mathematical-premise
  math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions: mathematical-premise
  math:thm-gronwall-integral-inequality: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-dependent-choice: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  physics:lem-gr-observer-projection-decomposition: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 5
---

## Statement

Assume the Axioms of Countable Choice and Dependent Choice. Let $(\Sigma,h)$ be a smooth Riemannian three-manifold with boundary $S$ and interior $\Sigma^\circ$. Let $E=\mathbb R_v\times\Sigma^\circ$ carry a smooth stationary time-oriented Lorentzian metric for which $v$ is temporal.

Use intrinsic length distance $d_h$ on $\Sigma$, componentwise with value $+\infty$ between distinct components, and define the boundary distance by $\rho(x)=\inf_{s\in S}d_h(x,s)$, with $\inf\varnothing=+\infty$. Extend it stationarily by $\rho(v,x)=\rho(x)$. Let $a>0$ be such that $\{\rho<a\}$ lies in a supplied smooth boundary collar. Components not meeting $S$ have $\rho=+\infty$ and contribute no points to this collar sublevel.

Suppose that, along the temporal parametrization of every future causal curve, $|d\rho/dv|\le C\rho$ almost everywhere where $0<\rho<a$, for a fixed $C\ge0$. The absolute continuity needed to interpret and integrate this inequality follows from the stated smooth geometry, as proved below. Let a nonempty compact target $Q\subset E$ project outside $\{\rho<a\}$ and satisfy $0<\min_Qv\le\max_Qv=V<\infty$. Then no point of $\{v=0,0<\rho<a e^{-CV}\}$ reaches $Q$ by a future causal curve in $E$. The boundary $S$ is excluded from $E$ and is separately regarded as inaccessible.

## Facts & Assumptions

[F1] Causal curves have locally absolutely continuous coordinates and nonzero future causal velocity almost everywhere. Temporal means that the smooth gradient of $v$ is past timelike. The stationary product and stationary extension use the section-time conventions, without requiring the additional maximal-graph hypotheses of that interface. [[def-causal-exterior-and-boundary-data]] [[def-stationary-section-time]]

[F2] Boundary charts and the supplied smooth collar have their usual half-space and embedding meanings. A smooth Riemannian metric up to $S$ is a positive-definite smooth tensor in those charts; no collar-existence theorem is invoked. [[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary]] [[math:def-smooth-collar-of-a-manifold-boundary]]

[F3] Intrinsic lengths, componentwise distance and distance to a subset have the supplied definitions. On each component meeting $S$, distance to $S$ is finite and $1$-Lipschitz for $d_h$. The distance topology is the manifold topology, including at the boundary; the metric and topology suppliers explicitly treat half-balls in their proofs. [[math:def-riemannian-speed-and-length]] [[math:def-riemannian-distance-on-a-connected-manifold]] [[math:def-extended-riemannian-distance-on-a-disconnected-manifold]] [[math:def-distance-from-a-point-to-a-subset]] [[math:prop-distance-to-a-nonempty-subset-is-one-lipschitz]] [[math:thm-the-riemannian-distance-topology-is-the-manifold-topology]]

[F4] On compact coordinate neighborhoods, a smooth positive-definite metric is bounded above and below by positive Euclidean multiples. Absolute continuity is the small-total-interval-length condition for sums of endpoint increments. [[math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric]] [[math:def-absolutely-continuous-function]]

[F5] Under the stated choice assumptions, $v\circ\gamma$ is locally absolutely continuous and strictly increasing on every future causal curve, and $dv(\gamma')>0$ almost everywhere. For an absolutely continuous scalar function $f$ on a compact interval, $f'\in L^1$ and $f(t)-f(0)=\int_0^t f'(s)\,ds$ after translating the interval if necessary. [[physics:lem-gr-temporal-functions-and-time-functions]] [[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions]] [[math:def-countable-choice]] [[math:def-dependent-choice]]

[F6] If a continuous nonnegative $r$ obeys $r(t)\le A+C\int_0^t r(s)\,ds$ on a compact interval, where $A,C\ge0$, the constant-coefficient case of the supplied integral Gronwall theorem gives $r(t)\le A e^{Ct}$. [[math:thm-gronwall-integral-inequality]]

[F7] The inverse metric and musical isomorphisms satisfy $\nabla v=(dv)^\sharp$, $g(\nabla v,Z)=dv(Z)$ and $g^{-1}(dv,dv)=g(\nabla v,\nabla v)$; the inverse metric is smooth. For a future unit timelike vector $n$, its orthogonal complement $n^\perp$ is three-dimensional and positive definite, every vector $Z$ decomposes as $Z=-g(Z,n)n+\pi_n Z$, and $g(\pi_n Z,\pi_n Z)=g(Z,Z)+g(Z,n)^2$, where $\pi_n Z=Z+g(n,Z)n$. [[physics:def-gr-inverse-metric-and-musical-isomorphisms]] [[physics:lem-gr-observer-projection-decomposition]]

## Proof

**Given:** The smooth product, boundary metric, collar, choice assumptions, causal differential inequality and compact target in the Statement.

**Goal:** Prove the finite-time collar exclusion with the stated radius.

1.1 Work in a connected component $H$ of $\Sigma$ meeting $S$. By [F3], $\rho$ is finite and continuous there, and $\rho=0$ on $S\cap H$. At an interior point $x$, the interior is open, so the distance-topology assertion supplies $\varepsilon>0$ with $B_{d_h}(x,\varepsilon)\subset\Sigma^\circ\cap H$. Thus $d_h(x,s)\ge\varepsilon$ for every $s\in S\cap H$, and $\rho(x)\ge\varepsilon>0$. Every continuous curve starting in $H$ stays in $H$, since components are open and a parameter interval is connected. Components missing $S$ have $\rho=+\infty$ and cannot contain an allowed starting point. [given, F2, F3]

1.2 Let $\gamma(s)=(v(s),y(s))$ be a future causal curve on a compact parameter interval. By [F5], $v(s)$ is absolutely continuous and strictly increasing, so it is a homeomorphism onto its time interval. Using the inverse metric of [F7], put $N=(-g^{-1}(dv,dv))^{-1/2}$, $n=-N\nabla v$ and $X=\partial_v-Nn$. Temporality gives $N>0$, $g(n,n)=-1$, future-directed $n$ and $dv(n)=1/N$. Since $g(n,Z)=-N\,dv(Z)$, the tangent space of a $v$-slice is $\ker dv=n^\perp$; [F7] therefore makes its induced metric $k$ positive definite. Also $dv(X)=0$, so $X$ is slice-tangent and $\gamma'=Nv'n+(y'+Xv')$ is its orthogonal normal–tangent decomposition. The projection identity in [F7] now gives $k(y'+Xv',y'+Xv')=g(\gamma',\gamma')+N^2(v')^2\le N^2(v')^2$ almost everywhere. On a compact product-coordinate neighborhood inside $E$, smoothness, $N>0$ and the lower metric bound of [F4] therefore give $|y'(s)|\le L v'(s)$ for a finite $L$; enlarge $L$ to bound all coordinate components. Coordinatewise application of the absolutely continuous fundamental theorem in [F5] yields $|y(s_2)-y(s_1)|\le L\bigl(v(s_2)-v(s_1)\bigr)$, after enlarging $L$ once more for the Euclidean norm. Thus the spatial time graph $y(v)$ is locally Lipschitz. This uses only the temporal condition and the mathematical decomposition in [F7], with no maximality or field-equation assumption. [given, F1, F4, F5, F7]

2.1 In a sufficiently small convex coordinate ball, or half-ball at the boundary, the coordinate segment from $x$ to $y$ has $h$-length at most $K|x-y|$ by the upper metric bound in [F4] and the length definition in [F3]. Hence $d_h(x,y)\le K|x-y|$. Combining this with the distance-to-set bound gives $|\rho(x)-\rho(y)|\le K|x-y|$ on every such neighborhood in a component meeting $S$. In particular $\rho$ is locally Lipschitz in spatial coordinates, without an assumption that distance is smooth. [F2, F3, F4, step 1.1]

3.1 If the connected component of $\Sigma$ containing the spatial image of $\gamma$ meets $S$, steps 2.1 and 1.2 show that $r(v)=\rho(y(v))$ is locally Lipschitz. On any compact time interval, choose a finite subdivision subordinate to these local neighborhoods. Taking the maximum of the finitely many Lipschitz constants and splitting endpoint increments at subdivision points makes $r$ Lipschitz on that whole interval. For any disjoint finite family of subintervals, the sum of its absolute $r$-increments is then bounded by this constant times their total length; this is absolute continuity by [F4]. Thus [F5] applies to $r$, rather than absolute continuity being an extra assumption on causal curves. [F3, F4, F5, step 1.1, step 2.1, step 1.2]

4.1 Suppose a curve from $(0,x_0)$ with $0<\rho_0=\rho(x_0)<a$ reaches a point of $Q$ at time $v_Q\le V$. Its spatial component remains in a component meeting $S$, and $r$ is positive and continuous throughout $[0,v_Q]$ by steps 1.1 and 3.1. Since $r(0)=\rho_0<a$ and $r(v_Q)\ge a$, the nonempty closed set $\{v\in[0,v_Q]:r(v)\ge a\}$ has a least element $v_*>0$. Continuity gives $r(v_*)=a$ and $0<r(v)<a$ for $0\le v<v_*$. The assumed derivative inequality therefore holds almost everywhere before $v_*$; absolute continuity and [F5] give $r(t)\le\rho_0+C\int_0^t r(s)\,ds$ for every $0\le t\le v_*$. All hypotheses of [F6] hold with $A=\rho_0$, so $a=r(v_*)\le\rho_0 e^{Cv_*}\le\rho_0 e^{CV}$. [given, F5, F6, step 1.1, step 3.1]

5.1 Every reachable starting point with $0<\rho_0<a$ consequently satisfies $\rho_0\ge a e^{-CV}$. This excludes the asserted strict sublevel at $v=0$. Since $\rho=0$ on $S$ and is continuous in each boundary-meeting component, $S\cup\{0<\rho<a e^{-CV}\}$ is a neighborhood of $S$ in the section. Its interior part has just been excluded from causal access; $S$ itself remains outside $E$ by the separate domain convention. [given, F3, step 1.1, step 4.1] ∎
