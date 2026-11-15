---
id: lem-author-9d607f469119-graph-section-compact-inside-core
title: A smooth graph section with a genuine end has a compact inside core
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-9d607f469119-bounded-radius-on-boundary-collar
  - math:thm-continuous-image-of-a-compact-space-is-compact
  - math:lem-closed-subset-of-a-compact-space-is-compact
  - math:thm-the-riemannian-distance-topology-is-the-manifold-topology
  - math:def-riemannian-distance-on-a-connected-manifold
  - math:thm-collar-neighborhood-theorem
  - math:def-smooth-collar-of-a-manifold-boundary
  - math:def-axiom-of-choice
  - math:def-countable-choice
  - math:thm-heine-borel-rn
  - math:cor-bolzano-weierstrass-in-rn
  - math:thm-extreme-value-metric
  - math:thm-compact-subset-is-closed-and-bounded
  - math:def-distance-from-a-point-to-a-subset
  - math:prop-distance-to-a-nonempty-subset-is-one-lipschitz
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:def-differential-of-a-smooth-real-valued-function
  - math:def-connected-space
  - math:def-path-connected
  - math:cor-euclidean-spheres-are-path-connected
  - math:thm-path-connected-implies-connected
  - math:def-connected-component-and-quasicomponent
  - math:def-metric-compactness
  - math:lem-compactness-is-intrinsic
  - math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold
  - math:def-metric-interior-closure-boundary
dependency_roles:
  lem-author-9d607f469119-bounded-radius-on-boundary-collar: mathematical-premise
  math:thm-continuous-image-of-a-compact-space-is-compact: mathematical-premise
  math:lem-closed-subset-of-a-compact-space-is-compact: mathematical-premise
  math:thm-the-riemannian-distance-topology-is-the-manifold-topology: mathematical-premise
  math:def-riemannian-distance-on-a-connected-manifold: mathematical-premise
  math:thm-collar-neighborhood-theorem: mathematical-premise
  math:def-smooth-collar-of-a-manifold-boundary: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:thm-heine-borel-rn: mathematical-premise
  math:cor-bolzano-weierstrass-in-rn: mathematical-premise
  math:thm-extreme-value-metric: mathematical-premise
  math:thm-compact-subset-is-closed-and-bounded: mathematical-premise
  math:def-distance-from-a-point-to-a-subset: mathematical-premise
  math:prop-distance-to-a-nonempty-subset-is-one-lipschitz: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:def-differential-of-a-smooth-real-valued-function: mathematical-premise
  math:def-connected-space: mathematical-premise
  math:def-path-connected: mathematical-premise
  math:cor-euclidean-spheres-are-path-connected: mathematical-premise
  math:thm-path-connected-implies-connected: mathematical-premise
  math:def-connected-component-and-quasicomponent: mathematical-premise
  math:def-metric-compactness: mathematical-premise
  math:lem-compactness-is-intrinsic: mathematical-premise
  math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold: mathematical-premise
  math:def-metric-interior-closure-boundary: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Assume the preceding radius and collar data, with $S$ a connected two-sphere. For each $R>1$, let $B_R= S\cup G(\{1<|x|\le R\})$. Then $B_R$ is compact in $\Sigma$ and contains a neighborhood of $S$. Its boundary away from $S$ is exactly the compact sphere $G(\{|x|=R\})$. For sufficiently small $\eta>0$, $B_R\cap\{\rho\ge\eta\}$ is compact in $\Sigma^\circ$, where $\rho$ is distance to $S$.

## Facts & Assumptions

[F1] Use the preceding connected smooth Riemannian manifold with compact boundary, interior graph diffeomorphism $G$, radius $r(G(x))=|x|$, and bounded far-end $|dr|_h$. Its radius is bounded on every fixed compact smooth collar without any boundary extension of the graph map. [[lem-author-9d607f469119-bounded-radius-on-boundary-collar]]

[F2] Continuous images of compact sets and closed subsets of compact spaces are compact. Compact subsets of metric spaces are closed. [[math:thm-continuous-image-of-a-compact-space-is-compact]] [[math:lem-closed-subset-of-a-compact-space-is-compact]] [[math:thm-compact-subset-is-closed-and-bounded]]

[F3] Work in ZFC, as in the preceding collar data; in particular $\mathrm{AC}_\omega$ holds by applying choice to a countable family. A smooth collar is an embedding $c:S\times[0,b)\to\Sigma$ with $c(s,0)=s$ and open image. Under countable choice the collar theorem supplies such a collar. [[math:def-axiom-of-choice]] [[math:def-countable-choice]] [[math:def-smooth-collar-of-a-manifold-boundary]] [[math:thm-collar-neighborhood-theorem]]

[F4] Closed bounded subsets of Euclidean space are compact; bounded Euclidean sequences have convergent subsequences; continuous real functions on nonempty compact metric spaces attain their minimum and maximum. [[math:thm-heine-borel-rn]] [[math:cor-bolzano-weierstrass-in-rn]] [[math:thm-extreme-value-metric]]

[F5] The length-defined Riemannian distance $d_h$ induces the manifold topology, also at the boundary. Set $\rho(p)=d_h(p,S)=\inf_{s\in S}d_h(p,s)$. Since $\Sigma$ is connected and $S$ is nonempty, this function is finite and $1$-Lipschitz, hence continuous, and it vanishes on $S$. [[math:def-riemannian-distance-on-a-connected-manifold]] [[math:thm-the-riemannian-distance-topology-is-the-manifold-topology]] [[math:def-distance-from-a-point-to-a-subset]] [[math:prop-distance-to-a-nonempty-subset-is-one-lipschitz]]

[F6] A Riemannian metric is a smooth positive-definite tensor, with smoothness up to the boundary here. A diffeomorphism and its inverse are smooth and continuous. For a smooth real-valued function, $dr_p(v)=v([r])$; the inherited bound on $|dr|_h$ uses this differential and the metric. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]] [[math:def-differential-of-a-smooth-real-valued-function]]

[F7] Connected means admitting no separation into two nonempty relatively open pieces. A path is a continuous map from $[0,1]$ with the specified endpoints; path-connected spaces are connected. The unit two-sphere is path connected. A component through a point is the largest connected subset containing that point. [[math:def-connected-space]] [[math:def-path-connected]] [[math:cor-euclidean-spheres-are-path-connected]] [[math:thm-path-connected-implies-connected]] [[math:def-connected-component-and-quasicomponent]]

[F8] A compact subset of a metric space is compact with its subspace metric: every open cover in that subspace has a finite subcover. Equivalently, every family of ambient open sets covering the subset has a finite subfamily covering it. [[math:def-metric-compactness]] [[math:lem-compactness-is-intrinsic]]

[F9] The manifold boundary is $S=\partial\Sigma$, defined by zero last coordinate in boundary charts; $\Sigma^\circ=\Sigma\setminus S$ is the manifold interior. These are distinct from the boundary of a subset $A$ in an ambient metric space $X$, which is $\partial_X A=\overline{A}^{\,X}\setminus\operatorname{int}_X A$: every neighborhood of a boundary point meets both $A$ and $X\setminus A$. For subset boundaries in the proof use the indicated ambient space with its restricted Riemannian metric; [F5] identifies that metric topology with the manifold subspace topology. [[math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold]] [[math:def-metric-interior-closure-boundary]]

## Proof

**Given:** The hypotheses in the Statement, with the inherited ZFC convention in [F3].

**Goal:** Establish the stated conclusion.

1.1 By [F3], take a smooth collar $c:S\times[0,b)\to\Sigma$ and restrict to $0<a<b$. Identify $W=c(S\times[0,a])$, $U=c(S\times(0,a))$, and $\Gamma=c(S\times\{a\})$ with their collar coordinates. The model $\mathbb S^2\times[0,a]\subset\mathbb R^4$ is closed and bounded, so [F4] and the smooth two-sphere parameterization of $S$ make $W$ and $\Gamma$ compact by [F2]. In particular $W$ is closed in $\Sigma$. By [F1] and [F6], the continuous map $G^{-1}$ sends $\Gamma$ to a nonempty compact set; its radius has minimum $m>1$ and finite maximum by [F4]. Inside $\Sigma^\circ\setminus\Gamma$, $U$ is open and closed, since its only boundary in $\Sigma^\circ$ is $\Gamma$. For any $s_0,s_1\in S$, transfer a sphere path from [F7] through a smooth identification $\mathbb S^2\cong S$, obtaining a path $\alpha$ from $s_0$ to $s_1$. For $u_0,u_1\in(0,a)$, the continuous path $t\mapsto c(\alpha(t),(1-t)u_0+tu_1)$ stays in $U$ and joins the corresponding collar points. Composing with $G^{-1}$ proves that $H=G^{-1}(U)$ is path connected and hence connected by [F7]; it is nonempty and clopen in $X=\{r>1\}\setminus G^{-1}(\Gamma)$. Any connected subset of $X$ meeting $H$ cannot also meet $X\setminus H$, since its intersections with these two open sets would be a separation. Consequently the component of any point of $H$ contains $H$ by maximality and cannot leave $H$, so equals $H$. Thus $G^{-1}(U)$ is a component of $X$. [given, F1, F2, F3, F4, F5, F6, F7, F9]

2.1 Fix $s\in S$ and let $u_j\downarrow0$. The points $c(s,u_j)$ converge to $s$ in $\Sigma$. Their inverse graph coordinates cannot have a subsequence confined to a closed annulus $1+\epsilon\le r\le M$: this annulus is closed bounded and hence compact by [F4], and the bounded-sequence assertion in [F4] gives a further convergent subsequence with limit in that annulus. By [F6], continuity of $G$ would give its image a limit in $\Sigma^\circ$, contradicting uniqueness of limits in the Riemannian metric topology and the boundary limit $s$. The radii are bounded above by [F1], so they tend to one: otherwise a subsequence would lie in such an annulus. The inner tail $\{1<r<m\}$ is path connected: write two points as $r_0\omega_0$ and $r_1\omega_1$, choose a unit-sphere path $\beta$ between $\omega_0$ and $\omega_1$ by [F7], and use the continuous path $t\mapsto((1-t)r_0+tr_1)\beta(t)$, whose radius remains in $(1,m)$. It is connected by [F7], is disjoint from $G^{-1}(\Gamma)$, and intersects $G^{-1}(U)$ because the preceding collar sequence has radii tending to one. The clopen separation argument of step 1.1 forces the entire tail to lie in $G^{-1}(U)$. [F1, F3, F4, F5, F6, F7, F9, step 1.1]

3.1 Choose $0<\epsilon<\min(m-1,R-1)$. Step 2.1 gives $G(\{1<r<1+\epsilon\})\subset U$. Hence $B_R$ is contained in $W\cup G(\{1+\epsilon\le r\le R\})$, a compact set: the annulus is closed bounded in $\mathbb R^3$ by [F4], its image is compact by [F2], and [F8] gives a finite subfamily of any ambient open cover covering each compact piece. Combining these two finite subfamilies covers their union, which is compact by the converse in [F8]. The complement of $B_R$ is $G(\{r>R\})$, an open subset of the open interior, so $B_R$ is closed in $\Sigma$ and is compact by [F2]. It contains a neighborhood of $S$. Indeed, otherwise choose collar points $c(s_j,u_j)$ outside $B_R$ with $0<u_j\le a/(j+1)$. Their inverse radii exceed $R$ and are uniformly bounded by [F1]. By [F4], the inverse points have a subsequence converging in a closed annulus $R\le r\le M$. Also, using the smooth identification $S\cong\mathbb S^2$ and [F4], pass to a further subsequence with $s_j\to s\in S$. Collar continuity gives $c(s_j,u_j)\to s$, whereas graph continuity by [F6] gives an interior limit, the same contradiction as in step 2.1. The countable selections here are permitted by [F3]. [F1, F2, F3, F4, F5, F6, F8, F9, step 1.1, step 2.1]

4.1 Away from $S$, the diffeomorphism $G$ from [F6] identifies the relative boundary of $B_R$ with $r=R$, whose sphere is closed bounded in $\mathbb R^3$ and therefore has compact image by [F4] and [F2]. By [F5], $\rho$ is continuous, so $B_R\cap\{\rho\ge\eta\}$ is closed in compact $B_R$. For every $\eta>0$ it avoids $S$, because $\rho=0$ on $S$. By [F8], its compactness therefore also holds in the interior subspace topology, which agrees with the Riemannian distance topology. In particular the stated conclusion holds for sufficiently small positive $\eta$. [F1, F2, F4, F5, F6, F8, F9, step 3.1] ∎
