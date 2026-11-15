---
title: The exterior Cauchy component has a complete asymptotically Euclidean closure
status: draft
research_item: lem-author-a4a441da4986-exact-outer-cauchy-section
dependency_level: 3
---

## Prerequisites

- [lem-author-a4a441da4986-doc-connected-and-causally-convex](item-lem-author-a4a441da4986-doc-connected-and-causally-convex)
- [lem-author-a4a441da4986-cauchy-closure-double-boundary](item-lem-author-a4a441da4986-cauchy-closure-double-boundary)
- [lem-author-e7cde3233cd7-cauchy-section-product](item-lem-author-e7cde3233cd7-cauchy-section-product)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:thm-connectedness-characterisations](https://alphabetamath.cc/item/thm-connectedness-characterisations)
- [math:thm-the-riemannian-distance-topology-is-the-manifold-topology](https://alphabetamath.cc/item/thm-the-riemannian-distance-topology-is-the-manifold-topology)
- [math:thm-compact-implies-complete-and-totally-bounded](https://alphabetamath.cc/item/thm-compact-implies-complete-and-totally-bounded)
- [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)
- [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)
- [math:thm-path-connected-implies-connected](https://alphabetamath.cc/item/thm-path-connected-implies-connected)
- [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)
- [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)


## Statement

Under the regular-spacetime hypotheses, put $C=\Sigma_0\cap E$ and $B=C\cup S$. Then $C$ is exactly the connected component of $\Sigma_0\setminus S$ containing the original stationary $t=0$ end. Its ambient closure is $B$, a smooth embedded manifold with compact boundary $S$, diffeomorphic to $\{y\in\mathbb R^3:|y|\ge1\}$. Its induced intrinsic length metric, allowing boundary points and piecewise $C^1$ curves, is complete.

The specified global identification $j:\Sigma_0\to\{|y|>1/2\}$ need not put $C$ on its outer side and need not agree with the physical end chart. There exists an adapted topological radial identification $\widetilde j$, equal either to $j$ or to its radial inversion fixing $|y|=1$ pointwise, with $\widetilde j(C)=\{|y|>1\}$. This is an existential coordinate choice, not a property of every specified chart.

Independently, on the original stationary end chart $(t,x)$ the section is $t=0$, and its induced metric satisfies $h_{ij}-\delta_{ij}=O_6(r^{-1})$, $r=|x|$, hence $O_2(r^{-1})$. For every sufficiently large physical end radius $R$, the truncation $B_R=B\setminus\{t=0,r>R\}$ is a compact smooth region with boundary $S\sqcup\{t=0,r=R\}$. These truncations exhaust $B$, and their exterior tails are connected; thus $B$ has exactly one asymptotically Euclidean end. The end estimates use these physical coordinates only; no agreement with $j$ or $\widetilde j$ is asserted. Neither a stationary product nor maximality is assumed.

Here an asymptotically Euclidean end means a metric-only condition in the original stationary end spatial chart: outside a compact subset of $C\cup S$ the chart is $\{x\in\mathbb R^3:r=|x|>R\}$, and its induced metric $h$ satisfies $h_{ij}-\delta_{ij}=O_2(r^{-1})$. Explicitly, for $1\le i,j\le3$ and each spatial multi-index $\alpha$ with $|\alpha|\le2$, there are constants $C_{ij\alpha}$ and a common sufficiently large radius such that $|\partial_x^\alpha(h_{ij}-\delta_{ij})|\le C_{ij\alpha}r^{-1-|\alpha|}$. Completeness means completeness of the intrinsic length metric on $C\cup S$, allowing piecewise $C^1$ curves through its boundary. This end convention makes no additional assertion about extrinsic curvature or a fixed leading asymptotic coefficient.

## Statement references

[lem-author-a4a441da4986-doc-connected-and-causally-convex](item-lem-author-a4a441da4986-doc-connected-and-causally-convex)

[lem-author-a4a441da4986-cauchy-closure-double-boundary](item-lem-author-a4a441da4986-cauchy-closure-double-boundary)

[lem-author-e7cde3233cd7-cauchy-section-product](item-lem-author-e7cde3233cd7-cauchy-section-product)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[math:thm-connectedness-characterisations](https://alphabetamath.cc/item/thm-connectedness-characterisations)

[math:thm-the-riemannian-distance-topology-is-the-manifold-topology](https://alphabetamath.cc/item/thm-the-riemannian-distance-topology-is-the-manifold-topology)

[math:thm-compact-implies-complete-and-totally-bounded](https://alphabetamath.cc/item/thm-compact-implies-complete-and-totally-bounded)

[math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)

[math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

[math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

[math:thm-path-connected-implies-connected](https://alphabetamath.cc/item/thm-path-connected-implies-connected)

[math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)

[math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

## Facts & Assumptions

[F1] The regular-spacetime data supply a smooth spacelike embedded $\Sigma_0$, a global diffeomorphism $j$ taking the double chronological boundary $S$ to the unit sphere, and a separate open stationary end on which $\Sigma_0$ agrees with $t=0$ and $g_{ij}=\delta_{ij}+O_6(r^{-1})$. The set $C=\Sigma_0\cap E$ is Cauchy in the globally hyperbolic exterior $E$. The two coordinate systems are not assumed to agree. Work in the inherited ZFC convention, including the axiom of choice. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F2] For the connected open end, the DOC lemma (Proof 1.1 and 2.1) gives openness of the chronological sets, openness and connectedness of $E$, and inclusion of the end in $E$. The generic Cauchy-section product supplies connectedness of $C$. The Cauchy-closure lemma puts every point of $\overline C^{\,M}\setminus C$ in the double chronological boundary $S$. Their choice hypotheses hold in the ZFC convention of [F1]. [lem-author-a4a441da4986-doc-connected-and-causally-convex](item-lem-author-a4a441da4986-doc-connected-and-causally-convex) [lem-author-e7cde3233cd7-cauchy-section-product](item-lem-author-e7cde3233cd7-cauchy-section-product) [lem-author-a4a441da4986-cauchy-closure-double-boundary](item-lem-author-a4a441da4986-cauchy-closure-double-boundary)

[F3] A path-connected set is connected; a nonempty relatively clopen subset of a connected space is the whole space. [math:thm-path-connected-implies-connected](https://alphabetamath.cc/item/thm-path-connected-implies-connected) [math:thm-connectedness-characterisations](https://alphabetamath.cc/item/thm-connectedness-characterisations)

[F4] A Euclidean subset is compact exactly when it is closed and bounded; continuous images of compact spaces are compact. A closed subspace of a compact topological space is compact (claim 1). A smooth positive Riemannian metric has finite positive coordinate-comparison bounds on compact chart subsets. [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn) [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps) [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric) [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

[F5] The intrinsic Riemannian distance gives the manifold topology, including boundary half-charts, and compact metric spaces are complete. [math:thm-the-riemannian-distance-topology-is-the-manifold-topology](https://alphabetamath.cc/item/thm-the-riemannian-distance-topology-is-the-manifold-topology) [math:thm-compact-implies-complete-and-totally-bounded](https://alphabetamath.cc/item/thm-compact-implies-complete-and-totally-bounded) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F6] An embedded smooth submanifold with boundary is a subset supplied with a manifold-with-boundary smooth structure for which its inclusion into the ambient manifold is a smooth embedding. [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)

## Proof

**Given:** The regular-spacetime data and exact declared interfaces.

**Goal:** Identify the intrinsic exterior component, its complete closure and its physical asymptotic end.

1.1 The physical end $U=M^{\mathrm{end}}$ is connected: its product coordinate domain is joined by time, radial and spherical paths. Apply [F2] to $U$ and its supplied smooth Cauchy portion. Thus $C$ is connected, is open in $\Sigma_0$, contains the whole stationary $t=0$ end, and is disjoint from $S$, since the double chronological boundary is disjoint from $E$. Any relative closure point in $\Sigma_0\setminus S$ is an ambient closure point, so [F2] puts it in $C$. Hence $C$ is relatively clopen in $\Sigma_0\setminus S$. [given, F1, F2, F3]

2.1 The two components in the specified $j$ coordinates are $1/2<|y|<1$ and $|y|>1$, each path connected by radial segments and spherical arcs. Connectedness and the clopen property identify $C$ with one of them, specifically the one containing the physical end. The radial map $I(y)=(f(|y|)/|y|)y$, $f(u)=1/2+1/(4(u-1/2))$, is a smooth involution on $|y|>1/2$, fixes the unit sphere pointwise and exchanges the two sides. Choose $\widetilde j=j$ or $I\circ j$ accordingly. This gives $\widetilde j(C)=\{|y|>1\}$ without asserting that the originally specified chart had that property. [F1, F3, step 1.1, algebra]

3.1 In the adapted coordinates of step 2.1, the region $B$ is the closed radial side $|y|\ge1$. Its usual boundary half-charts restrict the smooth structure of $\Sigma_0$, and its inclusion is the restriction of the original smooth embedding through $S$; hence it is an embedded manifold with boundary in the sense of [F6]. The sphere $S$ is compact, and $h$ is smooth and positive definite up to $S$ because $\Sigma_0$ is spacelike there. Radial segments and spherical arcs join points of $B$, so it is connected by [F3]; let $d_B$ be its intrinsic length metric from [F5]. Every point of $S$ is approached from $C$ along an adapted radial ray. Conversely [F2] excludes any additional ambient closure point, so $\overline C^{\,M}=B$. Adapted radial truncations $\{1\le|y|\le A\}$ are compact by [F4]. These topological coordinates are used only for compactness and topology, not for metric decay. [F1, F2, F3, F4, F5, F6, step 2.1]

4.1 Choose a sufficiently large physical radius $R$ within the stationary end so that $h=g_{ij}dx^idx^j\ge\tfrac12\delta_{ij}dx^idx^j$ on its $t=0$ tail $V_R=\{t=0,r>R\}$. Its sphere $\Gamma_R=\{t=0,r=R\}$ is compact in $C$, and $|dr|_h\le\sqrt2$ on the tail. We claim $V_R$ has no boundary in $B$ other than $\Gamma_R$. Otherwise take a putative boundary point $b\notin V_R\cup\Gamma_R$ and a small relatively compact boundary half-ball or interior coordinate ball neighborhood of $b$ disjoint from $\Gamma_R$. Join a point of $V_R$ there to $b$ by the coordinate straight segment, whose $h$-length is finite by the compact upper comparison in [F4] applied in a chart of the boundaryless $\Sigma_0$, and stop at its first exit from $V_R$. Before exit, the radial bound gives $r\le r(0)+\sqrt2\operatorname{length}_h(\gamma)$. The path's tail is therefore confined to the image of a closed physical coordinate annulus $R\le r\le A$, compact by [F4]. The image of that annulus is also closed in $B$: its image under the global adapted chart is compact by [F4], hence closed in Euclidean space by [F4]. Continuity of the path puts its first exit in the annulus, hence either in $V_R$ or on $\Gamma_R$, contradicting first exit and the neighborhood choice. Thus $V_R\cup\Gamma_R$ is closed in $B$ and is disjoint from $S$. [F1, F4, step 3.1]

5.1 In the adapted topological chart, compactness of $\Gamma_R$ and its disjointness from $S$ put it between $1+\epsilon<|y|<A$ for some $\epsilon>0,A<\infty$. The closed set $V_R\cup\Gamma_R$ avoids compact $S$, so an adapted boundary collar is disjoint from it. If its topological radii were bounded above, it would be a closed subset of a compact adapted annulus, hence compact. But the continuous physical radius on $V_R\cup\Gamma_R$ is unbounded, a contradiction. Thus $V_R$ meets $|y|>A$. It is clopen in $B\setminus\Gamma_R$ by step 4.1, and the connected adapted tail $|y|>A$ avoids $\Gamma_R$, so the entire tail lies in $V_R$. Consequently $B_R=B\setminus V_R$ is a closed subset of the compact topological truncation $|y|\le A$, hence compact. Its boundary is precisely $S\sqcup\Gamma_R$, with smoothness inherited from the section and the physical end chart. This holds for every sufficiently large physical $R$. [F3, F4, step 3.1, step 4.1]

6.1 The physical equality $\Sigma_0\cap M^{\mathrm{end}}=\{t=0\}$ makes $h_{ij}=g_{ij}=\delta_{ij}+O_6(r^{-1})$ in the actual end chart, independently of the adapted topological chart. This gives all stated derivative bounds through order two. The compact physical truncations from step 5.1 exhaust $B$ and are cofinal among compact subsets: if a compact subset had points of unbounded physical radius, the tail closedness in step 4.1 would make its intersection with $V_R\cup\Gamma_R$ compact, contradicting boundedness of the continuous radius on that intersection. Their connected tails have the ordinary spherical end structure. Together with the topological exterior description this establishes exactly one asymptotically Euclidean end, not a claim about arbitrary global coordinates. [F1, F3, F4, step 5.1]

6.2 Define $F=0$ on $B_R$ and $F=s^2/(1+s)$ on $V_R$, where $s=r-R>0$. In the physical collar of $\Gamma_R$, the value and first derivative of this expression tend to zero as $s\downarrow0$, so the two formulas define a nonnegative $C^1$ function on $B$. It vanishes near $S$ by step 4.1. On the tail its radial derivative is $1-(1+s)^{-2}\in[0,1]$, so step 4.1 gives $|dF(v)|\le\sqrt2\sqrt{h(v,v)}$ everywhere, including the core where $dF=0$. Its sublevels are compact: $s^2/(1+s)\to\infty$, so a sublevel is a closed subset of some compact physical truncation from step 5.1. Integrating along the piecewise $C^1$ curves defining $d_B$ gives $|F(p)-F(q)|\le\sqrt2d_B(p,q)$. Hence a $d_B$-Cauchy sequence has bounded $F$ and lies in a compact sublevel. [F4, F5, step 3.1, step 4.1, step 5.1, algebra]

7.1 By [F5], the restriction of $d_B$ to that compact sublevel induces its subspace manifold topology. It is thus a compact metric space, complete by [F5], so the Cauchy sequence converges in the same intrinsic distance $d_B$. This proves completeness including $S$. The argument used the auxiliary Cauchy product only for connectedness and neither assumed a stationary product nor imposed maximality. [F2, F4, F5, step 3.1, step 6.2] ∎
