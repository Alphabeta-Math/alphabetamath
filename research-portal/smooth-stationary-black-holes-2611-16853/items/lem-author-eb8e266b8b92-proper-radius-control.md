---
id: lem-author-eb8e266b8b92-proper-radius-control
title: Proper end radius and exclusion of finite-time spatial infinity
kind: lemma
status: draft
origin: pipeline
domain: mathematics
proof_strategy: direct
deps:
  - math:def-axiom-of-choice
  - lem-author-eb8e266b8b92-adm-time-speed
  - physics:lem-gr-causal-curve-calculus
  - math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions
  - math:thm-choice-implies-dependent-implies-countable-choice
  - math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary
  - math:def-smooth-map-between-manifolds-with-boundary
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces
  - math:thm-compactness-under-continuous-maps
  - math:thm-heine-borel-r
  - math:thm-finite-products-of-compact-spaces
  - math:thm-closed-subspace-of-a-compact-space-is-compact
dependency_roles:
  math:def-axiom-of-choice: mathematical-premise
  lem-author-eb8e266b8b92-adm-time-speed: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions: mathematical-premise
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
  math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary: mathematical-premise
  math:def-smooth-map-between-manifolds-with-boundary: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:thm-heine-borel-r: mathematical-premise
  math:thm-finite-products-of-compact-spaces: mathematical-premise
  math:thm-closed-subspace-of-a-compact-space-is-compact: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
dependency_level: 3
---

## Statement

Assume the Axiom of Choice and the stationary ADM setting of the section-time speed lemma. Let $\overline S$ be a connected smooth three-manifold with compact boundary, with $S=\operatorname{int}\overline S$, and a smooth positive-definite extension of $h$. Smoothness on $\overline S$ is understood in boundary charts by local smooth extension; the metric and differential norms use the section-time speed lemma's conventions, extended to the boundary using the inverse metric. Suppose $N$ and $X$ extend smoothly to $\overline S$, and supply a smooth function $R:\overline S\to[0,\infty)$ such that every sublevel $\{R\le m\}$ is compact. This is the proper-radius hypothesis. Suppose outside a compact set $K_0\subset\overline S$ one has $|dR|_h(N+|X|_h)\le C_0$. Then there is a finite constant $C_R$ such that every causal section-time curve satisfies $|R(x(v))-R(x(v_0))|\le C_R|v-v_0|$. In particular its spatial image for bounded section time stays in a compact subset of $\overline S$, although that subset can meet the boundary. One sufficient end realization of this hypothesis is a compact core with finitely many product ends $[r_0,\infty)\times F_j$, each $F_j$ compact, and a smooth $R$ equal to their unbounded first coordinate outside a larger compact core, with the displayed estimate for that coordinate.

## Statement references

[[math:def-axiom-of-choice]]

[[lem-author-eb8e266b8b92-adm-time-speed]]

[[physics:lem-gr-causal-curve-calculus]]

[[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions]]

[[math:thm-choice-implies-dependent-implies-countable-choice]]

[[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary]]

[[math:def-smooth-map-between-manifolds-with-boundary]]

[[math:def-riemannian-metric-and-riemannian-manifold]]

[[math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces]]

[[math:thm-compactness-under-continuous-maps]]

[[math:thm-heine-borel-r]]

[[math:thm-finite-products-of-compact-spaces]]

[[math:thm-closed-subspace-of-a-compact-space-is-compact]]

## Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice implies Dependent Choice and Countable Choice, which discharge the choice hypotheses of the causal-curve calculus and the absolutely-continuous fundamental theorem. [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]]

[F2] The section-time speed lemma makes $\gamma(v)=(v,x(v))$ a causal, locally Lipschitz curve on the smooth time-oriented Lorentzian four-manifold $E=\mathbb R_v\times S$ and gives $|(R\circ x)\prime|\le N|dR|_h+|X(R)|$ almost everywhere. Apply clause (b) of the causal-curve calculus to the smooth scalar $F:E\to\mathbb R$, $F(v,p)=R(p)$: its composite $F\circ\gamma=R\circ x$ is locally absolutely continuous. The required Countable Choice and Dependent Choice follow from F1. [[lem-author-eb8e266b8b92-adm-time-speed]] [[physics:lem-gr-causal-curve-calculus]]

[F3] Absolutely continuous scalar functions are recovered by integrating their almost-everywhere derivatives. [[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions]]

[F4] Boundary charts use the local-extension notion of smoothness, smooth maps are continuous, and a Riemannian metric is a smooth positive-definite symmetric tensor, with smoothness up to the boundary where stated. [[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary]] [[math:def-smooth-map-between-manifolds-with-boundary]] [[math:def-riemannian-metric-and-riemannian-manifold]]

[F5] Cauchy–Schwarz holds in each real inner product space. [[math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces]]

[F6] A continuous real-valued function on a nonempty compact space attains its maximum; continuous images of compact spaces are compact. [[math:thm-compactness-under-continuous-maps]]

[F7] Every closed bounded real interval is compact, and a finite product of compact spaces is compact in the product topology. [[math:thm-heine-borel-r]] [[math:thm-finite-products-of-compact-spaces]]

[F8] A closed subspace of a compact space is compact, and a finite union of compact subspaces is compact, including the empty union. [[math:thm-closed-subspace-of-a-compact-space-is-compact]]

## Proof

1.1 In a boundary chart write $h=(h_{ij})$. Positive definiteness makes $\det(h_{ij})$ nonzero, so the cofactor formula shows that the inverse matrix $(h^{ij})$ is smooth up to the boundary. The identities $|dR|_h^2=\sum_{i,j}h^{ij}(\partial_iR)(\partial_jR)$ and $|X|_h^2=\sum_{i,j}h_{ij}X^iX^j$ therefore give continuous nonnegative norms, including at boundary points. The vector with components $Y^i=\sum_j h^{ij}\partial_jR$ satisfies $h(Y,X)=dR(X)$ and $|Y|_h=|dR|_h$, so Cauchy–Schwarz gives $|X(R)|\le|dR|_h|X|_h$. Thus $q=N|dR|_h+|X(R)|$ is continuous on $\overline S$. [given, F2, F4, F5, algebra]

2.1 If $K_0$ is nonempty, let $M_0$ be the maximum of $q$ on $K_0$; if $K_0$ is empty, set $M_0=0$, with no extreme-value assertion needed there. On $S\setminus K_0$, step 1.1 and the given estimate imply $q\le|dR|_h(N+|X|_h)\le C_0$. Hence $C_R=\max\{0,C_0,M_0\}$ bounds $q$ along every spatial curve in $S$. The section-time speed lemma gives $|(R\circ x)\prime|\le C_R$ almost everywhere. On the compact interval between any two section times $v,v_0$ in the domain of the curve, F2 makes the scalar composition absolutely continuous; the fundamental theorem, with its choice hypotheses supplied by F1, gives $|R(x(v))-R(x(v_0))|\le C_R|v-v_0|$. [given, F1, F2, F3, F6, step 1.1, algebra]

3.1 If $|v-v_0|\le T$, step 2.1 places the image in $\{R\le R(x(v_0))+C_RT\}$, which is compact in $\overline S$ by the supplied proper-radius hypothesis. This proves confinement in the manifold with boundary; it does not exclude boundary accumulation. [given, step 2.1, algebra]

4.1 For the sufficient end realization, let $C$ be the larger compact core containing the transition region so that every point outside $C$ lies in a stated product end where $R=r$. For any real $m$, put $L=\max\{r_0,m\}$. The interval $[r_0,L]$ is compact, so each $[r_0,L]\times F_j$ is compact; its image under the end identification is compact by continuity. The union $P$ of those finitely many images with $C$ is compact. If $R(p)\le m$, either $p\in C$ or its end coordinate satisfies $r=R(p)\le m\le L$, so $p\in P$. Continuity of $R$ makes $\{R\le m\}$ closed in $\overline S$, hence closed in $P$ and compact. This includes the case $m<r_0$, where any points of the sublevel already lie in $C$. A bounded or nonproper reparameterization of an end coordinate alone supplies no such conclusion. [given, F4, F6, F7, F8] ∎
