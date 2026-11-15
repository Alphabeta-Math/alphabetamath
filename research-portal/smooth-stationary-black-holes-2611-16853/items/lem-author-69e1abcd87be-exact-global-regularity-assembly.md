---
id: lem-author-69e1abcd87be-exact-global-regularity-assembly
title: Exact assembly of the global I-plus regularity assumptions
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data
  - def-black-hole-comparison-hypothesis-data
  - def-causal-exterior-and-boundary-data
dependency_roles:
  def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data: mathematical-premise
  def-black-hole-comparison-hypothesis-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 6
---

## Statement

The smooth global comparison data imply the following complete $I^+$-regularity package relative to the selected end: the stationary field is complete on $M$; $D=I_M^+(M_{\rm ext})\cap I_M^-(M_{\rm ext})$ is globally hyperbolic; and there is a spacelike connected hypersurface $S\subset D$, acausal in $M$ and containing the end, whose ambient closure is a topological manifold with boundary, consisting of a compact core and finitely many asymptotic ends. Its boundary lies in $\mathcal E^+=\partial_M D\cap I_M^+(M_{\rm ext})$ and meets every generator of $\mathcal E^+$ exactly once. These are all the clauses of the declared $I^+$-regularity predicate. No orbit-space coordinate system, analyticity or local Killing-field extension is part of this definition.

## Facts & Assumptions

[F1] The supplied global comparison data impose the full end, complete-flow and I-plus-regularity predicates, together with a global axial action and connected event horizon. [[def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data]]

[F2] The comparison definition specifies the compact-core-plus-finite-ends closure, ambient boundary, once-only generator cross-section and end decay explicitly. [[def-black-hole-comparison-hypothesis-data]]

[F3] Chronological reachability and global hyperbolicity refer to the stated domains, and the distinction between ambient and restricted causal curves is retained. [[def-causal-exterior-and-boundary-data]]

## Proof

**Given:** The data and assumptions in the Statement.

**Goal:** Establish the claimed conditional conclusion.

1.1 Expand the $I^+$-regularity requirement in [F1] using [F2]. It gives completeness of the stationary field on all of $M$, global hyperbolicity of the specific $D$, and the spacelike connected ambient-acausal $S$ containing the specified end. In particular, compactness applies to the core of the completion and does not remove the stated asymptotic ends. [F1, F2, F3, given]

2.1 The remaining clauses in [F2] identify the boundary in the ambient topology, retain the factor $I_M^+(M_{\rm ext})$ in $\mathcal E^+$, and require exactly one intersection with every generator. Together these are precisely the displayed full predicate, with no hypothesis about a quotient coordinate chart. A global uniqueness theorem using this predicate must supply its own global reduction; expanding the definition neither proves nor assumes that reduction. [F2, F3, step 1.1] ∎
