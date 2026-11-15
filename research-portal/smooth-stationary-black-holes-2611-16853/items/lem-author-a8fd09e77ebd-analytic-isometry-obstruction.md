---
id: lem-author-a8fd09e77ebd-analytic-isometry-obstruction
title: A commuting-extension obstruction excludes arbitrary analytic-model isometries
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-author-a8fd09e77ebd-relative-stationary-deformation
  - thm-author-a8fd09e77ebd-nomizu-analytic-extension
  - lem-author-a8fd09e77ebd-commutation-from-uniqueness
  - lem-author-a8fd09e77ebd-isometry-analytic-pullback
dependency_roles:
  def-author-a8fd09e77ebd-relative-stationary-deformation: mathematical-premise
  thm-author-a8fd09e77ebd-nomizu-analytic-extension: mathematical-premise
  lem-author-a8fd09e77ebd-commutation-from-uniqueness: mathematical-premise
  lem-author-a8fd09e77ebd-isometry-analytic-pullback: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

A relative stationary deformation datum with a commuting-extension obstruction as in [[def-author-a8fd09e77ebd-relative-stationary-deformation]] admits no compatible real-analytic structure making its deformed metric analytic. Consequently it cannot be isometric, by any smooth diffeomorphism, to an analytic model neighborhood. The isometry need not preserve $T$, $Z$ or the matching coordinates. This statement concerns an isometry defined on the entire specified $U$; it does not exclude Kerr germs at particular points in a part where the deformation vanishes.

## Facts & Assumptions

[F1] The relative datum has connected simply connected $U$, connected nonempty $O$, and prohibits a commuting extension. [[def-author-a8fd09e77ebd-relative-stationary-deformation]]

[F2] For an analytic metric Nomizu supplies a global Killing extension and uniqueness on nonempty open sets. [[thm-author-a8fd09e77ebd-nomizu-analytic-extension]]

[F3] Under this uniqueness property every extension commutes with $T$. [[lem-author-a8fd09e77ebd-commutation-from-uniqueness]]

[F4] An isometry to an analytic metric supplies an analytic pullback structure. [[lem-author-a8fd09e77ebd-isometry-analytic-pullback]]

## Proof

**Given:** An obstructed relative datum.

**Goal:** Exclude an analytic presentation and an arbitrary isometry onto an analytic model.

1.1 Suppose a compatible real-analytic structure makes $\widetilde g$ analytic. The field $Z$ is a smooth Killing field on the connected open set $O$, since the metrics agree there. Apply Nomizu with the connected simply connected manifold $U$ to obtain a global Killing extension $Y$ and the required uniqueness property. The commutation lemma yields $[T,Y]=0$, contradicting the obstruction. [F1, F2, F3]

2.1 If an isometry $F$ onto an analytic model existed, its pulled-back atlas would supply exactly the analytic structure excluded in step 1.1. Hence no such isometry exists, independently of the images of the original symmetry fields. Neither step asserts that every smaller neighborhood carries an obstruction. [F4, step 1.1] ∎
