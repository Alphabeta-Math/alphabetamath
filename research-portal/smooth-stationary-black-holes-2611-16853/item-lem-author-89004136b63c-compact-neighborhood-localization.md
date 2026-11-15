---
title: Compact sets admit relatively compact open neighborhoods and finite chart
  pieces
status: published
research_item: lem-author-89004136b63c-compact-neighborhood-localization
dependency_level: 0
---

## Prerequisites

- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)
- [math:lem-coordinate-balls-form-a-basis-of-a-topological-manifold](https://alphabetamath.cc/item/lem-coordinate-balls-form-a-basis-of-a-topological-manifold)
- [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)
- [math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary)
- [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)
- [math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)


## Statement

Let $B$ be an open subset of a smooth Hausdorff manifold without boundary, and let $Q\subset B$ be compact. There are open sets $V,W$ with $Q\subset V$, $\overline V\subset W$ and $\overline W$ compact and contained in $B$. Every compact $K\subset B$ is covered by finitely many compact sets $K_j$ each contained in one smooth coordinate chart. Here closures are in the ambient manifold; a relatively compact set has compact closure.

## Statement references

[math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[math:lem-coordinate-balls-form-a-basis-of-a-topological-manifold](https://alphabetamath.cc/item/lem-coordinate-balls-form-a-basis-of-a-topological-manifold)

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary)

[math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

[math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

## Facts & Assumptions

[F1] Compactness means finite subcovers, including the ambient-cover formulation. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[F2] In any topological manifold, every point has an open coordinate-ball neighborhood whose closure in that manifold is compact. We will apply this also with an open chart subdomain as the manifold. [math:lem-coordinate-balls-form-a-basis-of-a-topological-manifold](https://alphabetamath.cc/item/lem-coordinate-balls-form-a-basis-of-a-topological-manifold)

[F3] A smooth manifold has an underlying topological manifold and a specified maximal smooth atlas; a smooth chart is a member of that atlas. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[F4] A topological manifold without boundary is Hausdorff, second countable and locally Euclidean of fixed dimension. [math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary)

[F5] In a topological space, the closure of a set is the intersection of all closed sets containing it, hence its smallest closed superset. [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

[F6] Distinct points of a Hausdorff space have disjoint open neighborhoods. [math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space)

[F7] The open sets of a subspace are traces of ambient open sets, and its closed sets are traces of ambient closed sets. If the subspace is open, its relatively open subsets are also ambient open subsets. [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the conclusions in the Statement.

1.1 Write $M$ for the ambient Hausdorff manifold. We first record the compactness consequences used below. If $C$ is compact in an open subspace $D\subset M$, every ambient open cover restricts to an open cover in $D$, so $C$ is compact in $M$. Any compact $C\subset M$ is closed: for $x\notin C$, the open sets disjoint from some open neighborhood of $x$ cover $C$ by Hausdorff separation; take finitely many of these sets covering $C$ and intersect the corresponding finitely many neighborhoods of $x$. This gives a neighborhood of $x$ disjoint from $C$. A closed subset of a compact space is compact, since adjoining its open complement to an open cover gives a cover of the compact space and hence a finite subcover. [given, F1, F6, F7]

2.1 Let $p\in O$ with $O\subset M$ open, and choose a smooth chart $(U,\varphi)$ containing $p$. The open set $D=U\cap O$ is a topological manifold: it is Hausdorff and second countable as an open subspace, and restricting charts gives local Euclidean coordinates. Apply F2 to $D$ at $p$ to obtain an open $T\subset D$ containing $p$ with $C=\overline T^{\,D}$ compact in $D$. Since $D$ is open in $M$, $T$ is open in $M$. By step 1.1, $C$ is compact and closed in $M$, so the ambient closure $\overline T$ is contained in $C\subset D\subset O\cap U$ and is a closed subset of compact $C$, hence compact. Thus the closure lies in the prescribed open set and in the original smooth chart domain. [F1, F2, F3, F4, F5, F6, F7, step 1.1]

3.1 Apply step 2.1 with $O=B$. The family of all neighborhoods $T$ obtained there covers $Q$, so choose finitely many $T_1,\ldots,T_r$ covering $Q$ and put $W=\bigcup_{i=1}^r T_i$. It is open and contains $Q$. The closure of a finite union is the union of the closures, so $\overline W=\bigcup_{i=1}^r\overline{T_i}\subset B$. This union is compact: restrict any open cover to each compact member, take finitely many covering sets for each, and combine these finite lists. [F1, F5, step 2.1]

4.1 Repeat step 3.1 with the open set $W$ in place of $B$ to obtain an open $V$ containing $Q$ with compact $\overline V\subset W$. For a compact $K\subset B$, use step 2.1 and compactness to obtain finitely many open $T_j$ covering $K$ such that each compact $\overline{T_j}$ lies in a smooth chart domain $U_j$. Set $K_j=K\cap\overline{T_j}$. Each $K_j$ is closed in compact $K$, hence compact by step 1.1, and is contained in $U_j$; these sets cover $K$ because the $T_j$ do. If $Q$ is empty take $V=W=\varnothing$, and if $K$ is empty use the empty family of pieces. [F1, F3, F5, F7, step 1.1, step 2.1, step 3.1] ∎
