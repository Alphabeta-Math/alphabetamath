---
title: Acausal hypersurface with compact core and finitely many ends
status: draft
research_item: def-author-310ff0f53b38-acausal-finite-end-section
dependency_level: 3
---

## Prerequisites

- [def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end)
- [def-author-310ff0f53b38-closure-and-boundary-data](item-def-author-310ff0f53b38-closure-and-boundary-data)
- [def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section)
- [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)


## Definition

Let $S\subset M$ be a connected spacelike embedded hypersurface containing a specified asymptotically flat end $S_{\rm ext}$ with the decay data of [def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end). Acausal means that no distinct points of $S$ are joined, in either direction, by a future causal curve in the ambient $M$. It is an additional global condition, not part of positive definiteness of the induced metric.

Use the completion data of [def-author-310ff0f53b38-closure-and-boundary-data](item-def-author-310ff0f53b38-closure-and-boundary-data): $\overline S^{\,M}$ is a topological three-manifold with manifold interior $S$ and boundary $B=\overline S^{\,M}\setminus S$, and $B$ is a topological two-manifold. A compact core with finitely many asymptotic ends means that $\overline S^{\,M}=C_0\cup S_1\cup\cdots\cup S_N$ for a compact subset $C_0$ and finitely many end regions $S_j$ with asymptotically flat end charts as above. The chosen end $S_{\rm ext}$ is one of the specified asymptotic regions, up to truncation at a larger radius. This is a finite-end condition, not compactness of $\overline S^{\,M}$.

For a specified future horizon portion $\mathcal E^+$, the boundary section condition means $B\subset\mathcal E^+$ and $|B\cap G|=1$ for every generator image $G$ of $\mathcal E^+$, in the sense of [def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section). It is a topological once-only cross-section condition; a smooth embedding or a transverse differentiable intersection is not added to it.

## Definition references

[def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end)

[def-author-310ff0f53b38-closure-and-boundary-data](item-def-author-310ff0f53b38-closure-and-boundary-data)

[def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section)

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

## Facts & Assumptions

[F1] End charts and decay, completion topology, and generator images have the stated interfaces. [def-author-310ff0f53b38-asymptotically-flat-spacelike-end](item-def-author-310ff0f53b38-asymptotically-flat-spacelike-end) [def-author-310ff0f53b38-closure-and-boundary-data](item-def-author-310ff0f53b38-closure-and-boundary-data) [def-author-310ff0f53b38-null-generator-cross-section](item-def-author-310ff0f53b38-null-generator-cross-section)

[F2] Spacelikeness and acausality have the ambient Lorentzian meanings. [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

## Justification

**Given:**The objects and specified data in the Definition.

**Goal:** Verify that the displayed conditions define unambiguous objects and predicates on these data.

1.1 The induced metric tests spacelikeness pointwise, while causal reachability tests acausality using curves in $M$. The completion and its manifold boundary are specified independently. The finite union condition then quantifies over a compact set, a finite integer and end charts of the already defined type. [F1, F2]

2.1 With those objects fixed, boundary inclusion and once-only intersection are the subset and cardinality predicates of the generator interface. Their conjunction with step 1.1 gives a definite section-data predicate. No existence, compactification by points at infinity, or smoothness theorem is inferred. [F1, F2, step 1.1] ∎
