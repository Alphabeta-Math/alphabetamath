---
title: Eventual access is uniform on the trimmed compact inside core
status: draft
research_item: lem-author-9d607f469119-uniform-access-on-trimmed-core
dependency_level: 0
---

## Prerequisites

- [math:def-topological-manifold-with-boundary](https://alphabetamath.cc/item/def-topological-manifold-with-boundary)
- [math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)
- [math:def-metric-space](https://alphabetamath.cc/item/def-metric-space)
- [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)
- [math:def-metric-interior-closure-boundary](https://alphabetamath.cc/item/def-metric-interior-closure-boundary)
- [math:def-metric-bounded-diameter](https://alphabetamath.cc/item/def-metric-bounded-diameter)
- [math:lem-distance-to-set-is-lipschitz](https://alphabetamath.cc/item/lem-distance-to-set-is-lipschitz)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:thm-compactness-agrees-with-metric-compactness](https://alphabetamath.cc/item/thm-compactness-agrees-with-metric-compactness)
- [math:thm-compact-subset-is-closed-and-bounded](https://alphabetamath.cc/item/thm-compact-subset-is-closed-and-bounded)
- [math:lem-closed-subset-of-a-compact-space-is-compact](https://alphabetamath.cc/item/lem-closed-subset-of-a-compact-space-is-compact)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)
- [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)
- [math:lem-finite-set-has-max](https://alphabetamath.cc/item/lem-finite-set-has-max)
- [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)


## Statement

Let $\Sigma$ be a manifold with nonempty compact boundary $S$, equipped with a metric $d$ inducing its manifold topology, and write $\Sigma^\circ=\Sigma\setminus S$. Let $B\subset\Sigma$ be a compact inside region containing an open neighborhood of $S$, and denote its outer boundary by $\Gamma=\partial_\Sigma B$, the topological boundary relative to $\Sigma$. Set $\rho(x)=d(x,S)=\inf_{s\in S}d(x,s)$. Suppose $\Sigma^\circ\subset M$, where $M$ is an ambient manifold and the inclusion $\Sigma^\circ\hookrightarrow M$ is continuous for the subspace topology inherited from $\Sigma$. Let $(P_t)_{t\in\mathbb R}$ be open subsets of $M$ with $P_s\subseteq P_t$ for $s\le t$, and suppose that for every $x\in\Sigma^\circ$ there is $T_x\in\mathbb R$ such that $x\in P_t$ for all $t\ge T_x$. Then for every sufficiently small $\eta>0$ there is $t_\eta\in\mathbb R$ such that $L_\eta=B\cap\{\rho\ge\eta/2\}\subset P_t$ for all $t\ge t_\eta$. Moreover $\Gamma$ is compact and disjoint from $S$, and there is an open section neighborhood $N_\eta$ of the whole outer boundary $\Gamma$ with $N_\eta\subset P_t$ for every $t\ge t_\eta$.

## Statement references

[math:def-topological-manifold-with-boundary](https://alphabetamath.cc/item/def-topological-manifold-with-boundary)

[math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)

[math:def-metric-space](https://alphabetamath.cc/item/def-metric-space)

[math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)

[math:def-metric-interior-closure-boundary](https://alphabetamath.cc/item/def-metric-interior-closure-boundary)

[math:def-metric-bounded-diameter](https://alphabetamath.cc/item/def-metric-bounded-diameter)

[math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)

## Facts & Assumptions

[F1] The interior of a manifold with boundary $S$ is $\Sigma^\circ=\Sigma\setminus S$. A compatible metric has the manifold open sets as its metric open sets. The relative topological boundary of $B$ is $\partial_\Sigma B=\overline B\setminus\operatorname{int}_\Sigma B$, and $\operatorname{int}_\Sigma B$ is open. [math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold) [math:def-metric-space](https://alphabetamath.cc/item/def-metric-space) [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology) [math:def-metric-interior-closure-boundary](https://alphabetamath.cc/item/def-metric-interior-closure-boundary)

[F2] For a nonempty subset $S$ of a metric space, $d(x,S)=\inf_{s\in S}d(x,s)$ is a finite real number and $|d(x,S)-d(y,S)|\le d(x,y)$. [math:def-metric-bounded-diameter](https://alphabetamath.cc/item/def-metric-bounded-diameter) [math:lem-distance-to-set-is-lipschitz](https://alphabetamath.cc/item/lem-distance-to-set-is-lipschitz)

[F3] Compactness is intrinsic to the subspace topology. On a metric space, topological and metric compactness agree. Compact metric subsets are closed, and a closed subset of a compact metric space is compact. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) [math:thm-compactness-agrees-with-metric-compactness](https://alphabetamath.cc/item/thm-compactness-agrees-with-metric-compactness) [math:thm-compact-subset-is-closed-and-bounded](https://alphabetamath.cc/item/thm-compact-subset-is-closed-and-bounded) [math:lem-closed-subset-of-a-compact-space-is-compact](https://alphabetamath.cc/item/lem-closed-subset-of-a-compact-space-is-compact)

[F4] Subspace open sets are traces of ambient open sets, and subspace topologies are transitive. For a continuous inclusion, inverse images of ambient open sets are open. An indexed family of open sets of a topological space covering a compact subset has finitely many indices whose sets cover it, unless the subset is empty. [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top) [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top) [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[F5] A finite nonempty list of real numbers has a largest member. A continuous real function on a nonempty compact metric space attains a minimum. [math:lem-finite-set-has-max](https://alphabetamath.cc/item/lem-finite-set-has-max) [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the trimmed-core containment and the persistent open neighborhood of the outer boundary.

1.1 By compatibility of $d$ and [F3], $B$ and $S$ are compact metric subsets of $\Sigma$, hence closed. Since $B$ contains an open neighborhood of $S$, we have $S\subset\operatorname{int}_\Sigma B$. Closedness of $B$ implies $\overline B=B$: a point outside $B$ has a metric ball in its open complement and so is not adherent to $B$. Thus $\Gamma=B\setminus\operatorname{int}_\Sigma B$ is closed in $B$, compact by [F3], and contained in $B\setminus S\subset\Sigma^\circ$. Also $\Sigma^\circ$ is open in $\Sigma$ because $S$ is closed. [given, F1, F3]

2.1 By [F2] and $S\ne\varnothing$, $\rho$ is finite and $1$-Lipschitz, hence continuous: $d(x,y)<\epsilon$ gives $|\rho(x)-\rho(y)|<\epsilon$. It vanishes on $S$. If $x\notin S$, closedness of $S$ gives a ball of radius $r>0$ about $x$ disjoint from $S$, so $d(x,s)\ge r$ for every $s\in S$ and $\rho(x)\ge r>0$. For any $\eta>0$, $L_\eta$ is closed in $B$: at a point with $\rho(x)<\eta/2$, the Lipschitz bound keeps $\rho<\eta/2$ throughout a sufficiently small ball. By [F3], $L_\eta$ is compact, and it avoids $S$. Its topology inherited from $\Sigma^\circ$ equals that inherited from $\Sigma$, by transitivity of subspace topologies in [F4]; hence it remains intrinsically compact as a subset of $\Sigma^\circ$. [given, F1, F2, F3, F4, step 1.1]

3.1 Fix $\eta>0$ and let $U_t=\Sigma^\circ\cap P_t$. The continuity of the inclusion makes $U_t$ open in $\Sigma^\circ$. Eventual entry applies to every point of $L_\eta\subset\Sigma^\circ$, so the indexed family $(U_t)_{t\in\mathbb R}$ covers $L_\eta$. By its compactness and the indexed ambient-cover criterion in [F4], if $L_\eta\ne\varnothing$ there are finitely many indices $t_0,\ldots,t_m$ whose sets cover it. Put $t_\eta=\max\{t_0,\ldots,t_m\}$, which exists by [F5]. Increasingness gives $L_\eta\subset P_t$ for every $t\ge t_\eta$. If $L_\eta=\varnothing$, take $t_\eta=0$ and the same containment is automatic. [given, F4, F5, step 2.1]

4.1 If $\Gamma\ne\varnothing$, its compactness and the continuity of $\rho$ allow [F5] to give $\delta=\min_\Gamma\rho$ attained at a point of $\Gamma$. Step 2.1 and $\Gamma\cap S=\varnothing$ give $\delta>0$. For $0<\eta<\delta$, we have $\Gamma\subset L_\eta$. Consequently $N_\eta=\Sigma^\circ\cap P_{t_\eta}$ contains $\Gamma$, is open in $\Sigma^\circ$ by [F4], and is open in $\Sigma$ because $\Sigma^\circ$ is open. Increasingness gives $N_\eta\subset P_t$ for all $t\ge t_\eta$. If $\Gamma=\varnothing$, take $0<\eta<1$ and $N_\eta=\varnothing$; the neighborhood assertion is vacuous and the trimmed-core containment still follows from step 3.1. This proves both conclusions, with a single neighborhood valid at all later times. [given, F1, F4, F5, step 1.1, step 2.1, step 3.1] ∎
