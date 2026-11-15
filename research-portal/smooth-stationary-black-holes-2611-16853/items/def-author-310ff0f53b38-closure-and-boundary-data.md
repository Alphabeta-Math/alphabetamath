---
id: def-author-310ff0f53b38-closure-and-boundary-data
title: Ambient closure and intrinsic boundary of a hypersurface
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - math:def-topological-manifold-with-and-without-boundary
  - math:def-subspace-topology-top
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  math:def-topological-manifold-with-and-without-boundary: mathematical-premise
  math:def-subspace-topology-top: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Definition

For a subset $S\subset M$, write $\overline S^{\,M}$ for its closure in $M$: a point lies in it precisely when every open neighborhood in $M$ meets $S$. Give $\overline S^{\,M}$ its subspace topology. The ambient boundary of any subset $A\subset M$ is $\partial_M A=\overline A^{\,M}\setminus\operatorname{int}_M A$, where $\operatorname{int}_M A$ is the union of the open subsets of $M$ contained in $A$.

A topological three-manifold with boundary is a Hausdorff, second-countable space locally homeomorphic to relatively open subsets of $\{(y^1,y^2,y^3):y^3\ge0\}$. Its manifold boundary is defined by the boundary-chart convention of the supplier. For hypersurface completion data, require $\overline S^{\,M}$ to be such a manifold, $S$ to be its manifold interior, and $B:=\overline S^{\,M}\setminus S$ to be its manifold boundary and a topological two-manifold without boundary. In particular $B$ is a boundary of the completed three-manifold, whereas $\partial_M S$ is an ambient boundary; the symbols are not interchangeable. No smoothness of $B$ in $M$ is required.

## Definition references

[[physics:def-gr-smooth-lorentzian-objects]]

[[math:def-topological-manifold-with-and-without-boundary]]

[[math:def-subspace-topology-top]]

## Facts & Assumptions

[F1] The smooth manifold has its manifold topology. [[physics:def-gr-smooth-lorentzian-objects]]

[F2] Manifolds with boundary and their intrinsic boundary have the specified chart-based meaning. [[math:def-topological-manifold-with-and-without-boundary]]

[F3] For a subset $A$ of a topological space $X$, its subspace topology consists of the sets $U\cap A$ with $U$ open in $X$; this also defines relatively open subsets. [[math:def-subspace-topology-top]]

## Justification

**Given:**The objects and specified data in the Definition.

**Goal:** Verify that the displayed conditions define unambiguous objects and predicates on these data.

1.1 The neighborhood predicate determines a unique closure; the union of open subsets determines a unique interior. Their set difference therefore determines the ambient boundary, without selecting charts. [F1]

2.1 The manifold-with-boundary conditions are predicates on the specified subspace topology; requiring that its intrinsic boundary equal $B$ is an additional condition, not a consequence of the closure operation. Thus the completion data distinguish both boundary notions even when only topological boundary charts exist. [F1, F2, F3, step 1.1] ∎
