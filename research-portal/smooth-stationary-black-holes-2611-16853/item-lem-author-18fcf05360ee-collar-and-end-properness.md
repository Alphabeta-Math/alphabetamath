---
title: Collar comparison and an exact end projection imply properness
status: draft
research_item: lem-author-18fcf05360ee-collar-and-end-properness
dependency_level: 6
---

## Prerequisites

- [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)
- [lem-author-18fcf05360ee-existing-graph-stationary-projection](item-lem-author-18fcf05360ee-existing-graph-stationary-projection)
- [lem-author-18fcf05360ee-uniform-stationary-return-with-tangential-motion](item-lem-author-18fcf05360ee-uniform-stationary-return-with-tangential-motion)
- [math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary)
- [math:prop-smooth-maps-are-continuous](https://alphabetamath.cc/item/prop-smooth-maps-are-continuous)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:thm-compact-subset-of-a-hausdorff-space-is-closed](https://alphabetamath.cc/item/thm-compact-subset-of-a-hausdorff-space-is-closed)
- [math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top)
- [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)


## Statement

Let $F_w:\Sigma_*\to\Sigma_w$ be an admissible fixed-boundary flow graph with small $w$ and let $P=\Pi_*\circ F_w$ on the interiors, with $\Pi_*$ the existing global stationary projection. Suppose near $S$ the return construction applies with $|w|\le\epsilon\rho_*$, so that return points stay in a fixed boundary collar and their boundary distances are comparable to those of the base points. Suppose on the exterior end $Y=T$, so $P(x)=x$ there. With the compact annular truncations of the existing section, $P$ is proper: the preimage of every compact interior target set is compact. In particular neither boundary escape nor escape to infinity can occur in a sequence whose projections stay compact.

## Statement references

[def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[lem-author-18fcf05360ee-existing-graph-stationary-projection](item-lem-author-18fcf05360ee-existing-graph-stationary-projection)

[lem-author-18fcf05360ee-uniform-stationary-return-with-tangential-motion](item-lem-author-18fcf05360ee-uniform-stationary-return-with-tangential-motion)

[math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary)

[math:prop-smooth-maps-are-continuous](https://alphabetamath.cc/item/prop-smooth-maps-are-continuous)

[math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[math:thm-compact-subset-of-a-hausdorff-space-is-closed](https://alphabetamath.cc/item/thm-compact-subset-of-a-hausdorff-space-is-closed)

[math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top)

[math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

[math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

## Facts & Assumptions

[F1] The existing projection is smooth and globally defined, and each stationary orbit meets the reference section exactly once. The reference interior has compact annular truncations between its full boundary collar and its stationary graph end. Their nested open interiors exhaust the reference interior, and each avoids a sufficiently small boundary collar and a sufficiently far end. [lem-author-18fcf05360ee-existing-graph-stationary-projection](item-lem-author-18fcf05360ee-existing-graph-stationary-projection)

[F2] Under the stated return-construction applicability hypothesis, the orbit through a collar graph point has a local return to the reference section in a fixed collar, with uniformly comparable positive boundary distances. [lem-author-18fcf05360ee-uniform-stationary-return-with-tangential-motion](item-lem-author-18fcf05360ee-uniform-stationary-return-with-tangential-motion)

[F3] The admissible flow graph map is smooth, is an embedding, and maps onto the supplied graph; its restriction maps the reference interior onto the graph interior. [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[F4] The reference and graph interiors are manifolds without boundary, hence Hausdorff. Smooth maps between smooth manifolds are continuous. [math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary) [math:prop-smooth-maps-are-continuous](https://alphabetamath.cc/item/prop-smooth-maps-are-continuous)

[F5] A compact subset is compact in its subspace topology, so every open cover of that subspace has a finite subcover. Open and closed subsets of a subspace are traces of ambient open and closed sets. Restrictions of continuous maps are continuous, and subspace topologies are transitive. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[F6] A compact subset of a Hausdorff space is closed. For a continuous map, inverse images of closed sets are closed. A closed subspace of a compact space is compact. [math:thm-compact-subset-of-a-hausdorff-space-is-closed](https://alphabetamath.cc/item/thm-compact-subset-of-a-hausdorff-space-is-closed) [math:thm-continuity-characterisations-top](https://alphabetamath.cc/item/thm-continuity-characterisations-top) [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

[F7] The image of a compact subset under a continuous map is compact. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

## Proof

**Given:** The stated admissible fixed-boundary graph, applicable return comparison, global stationary projection and compact annular truncations.

**Goal:** Prove properness of $P$ and of the stationary projection from the graph interior.

1.1 For $x$ in a sufficiently small source boundary collar, the stated applicability hypothesis and [F2] give a local stationary intersection $z(x)$ on the reference section, remaining in a fixed target collar and satisfying $C^{-1}\rho_*(x)\le\rho_*(z(x))\le C\rho_*(x)$ for a common $C\ge1$. Uniqueness of the global stationary intersection in [F1] identifies $z(x)$ with $P(x)$. Hence the image of a sufficiently small source collar lies in any prescribed sufficiently small target collar. In particular a base sequence approaching $S$ has projected boundary distance tending to zero. This uses the assumed return comparison directly. [given, F1, F2, F3]

2.1 Let $K\subset\Sigma_*^\circ$ be compact; if $K$ is empty its inverse image is empty and compact. Otherwise, intersect the nested open annular interiors from [F1] with $K$. These intersections cover the compact subspace $K$, so [F5] gives a finite subcover. By nesting, $K$ lies in one annulus and avoids a sufficiently small target boundary collar and a sufficiently far end. Step 1.1 therefore excludes a sufficiently small source collar from $P^{-1}(K)$. On the source end, the assumed identity $P(x)=x$ excludes all sufficiently far source points. The remaining source portion lies in a compact annular truncation $A$ by [F1]. Both $F_w$ and $\Pi_*$ are smooth by [F1] and [F3], hence continuous by [F4]; their composite $P$ is continuous, since an open inverse image under $P$ is an iterated open inverse image. The target is Hausdorff by [F4], so [F6] makes $K$ closed and $P^{-1}(K)$ closed in the source. It is closed in $A$ by [F5], hence compact by [F6], with its original source subspace topology by [F5]. This proves properness of $P$ and excludes both boundary and end escape with compact projections. [F1, F3, F4, F5, F6, step 1.1]

3.1 Write $\pi=\Pi_*|_{\Sigma_w^\circ}$. Since $F_w$ maps the reference interior onto the graph interior and $P=\pi\circ F_w$, one has $\pi^{-1}(K)=F_w(P^{-1}(K))$. The restriction of $F_w$ to $P^{-1}(K)$ is continuous by [F3], [F4] and [F5]. Its domain is compact by step 2.1, so [F7] makes its image compact in the graph interior. Thus projection from $\Sigma_w^\circ$ is proper as well. [F3, F4, F5, F7, step 2.1] ∎
