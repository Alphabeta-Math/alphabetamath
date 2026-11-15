---
id: lem-author-ae62588ad46a-horizon-case-partition
title: The exhaustive analytic horizon-component case split
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-horizon-rotation-surface-gravity
  - def-black-hole-comparison-hypothesis-data
dependency_roles:
  def-horizon-rotation-surface-gravity: mathematical-premise
  def-black-hole-comparison-hypothesis-data: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 5
---

## Statement

For a nonempty horizon with its componentwise rotation and degeneracy labels, exactly one of the following cases holds: (R) some component rotates; (N) every component is non-rotating and none is degenerate; (D) every component is non-rotating and at least one is degenerate. Case (D) includes mixed degenerate and nondegenerate components. Multiplying a specified horizon generator by any fixed nonzero constant preserves whether its surface gravity vanishes.

## Facts & Assumptions

[F1] Rotation and normalized surface gravity are [[def-horizon-rotation-surface-gravity]], and component/regularity conventions are [[def-black-hole-comparison-hypothesis-data]]. Non-rotation is tangency of $T$ to the generator line everywhere on the specified component. Degeneracy is the zero surface-gravity condition for the supplied Killing generator.

## Proof

**Given:** The componentwise predicates and specified generators.

**Goal:** Establish exhaustive disjoint cases and normalization invariance.

1.1 Either some component rotates or none does. In the second alternative all components are non-rotating; either at least one is degenerate or none is. These are mutually exclusive alternatives and yield precisely (R), (D) and (N). No assumption that every component has the same degeneracy type is introduced. [given, F1]

2.1 For $K'=aK$ with constant $a\ne0$, the Killing-horizon equation gives $\nabla_{K'}K'=a^2\nabla_KK=a\kappa K'$. Thus the new coefficient is $a\kappa$, which vanishes exactly when $\kappa$ does. Also scaling the stationary field by a positive constant does not change its tangency to the same generator lines. The case partition is consequently independent of those constant normalizations. [given, F1, step 1.1, algebra] ∎
