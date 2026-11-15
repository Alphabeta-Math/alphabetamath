---
id: lem-author-840894718169-boundary-one-sheet-normal-graph
title: A one-sheet boundary germ propagates across the common normal collar
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-840894718169-uniform-gaussian-flow-cone
  - lem-author-840894718169-normal-projection-local-and-boundary-jets
  - lem-author-840894718169-fixed-target-collar-properness
  - math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets
  - def-normal-graph-and-mean-curvature-data
dependency_roles:
  lem-author-840894718169-uniform-gaussian-flow-cone: mathematical-premise
  lem-author-840894718169-normal-projection-local-and-boundary-jets: mathematical-premise
  lem-author-840894718169-fixed-target-collar-properness: mathematical-premise
  math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets: mathematical-premise
  def-normal-graph-and-mean-curvature-data: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 6
---

## Statement

Under the previous hypotheses the proper normal projection onto the fixed target collar has one sheet. Consequently every candidate is represented there as a unique smooth normal graph $\tau=w_q(R,y)$, smooth down to $S$ for each fixed candidate. If $|\tau|\le\theta R$ on its $K$-flow image, the same cone bound holds for $w_q$, on that fixed collar. This does not supply a uniform bound for interior derivatives of $w_q$.

## Statement references

[[lem-author-840894718169-uniform-gaussian-flow-cone]]

[[lem-author-840894718169-normal-projection-local-and-boundary-jets]]

[[lem-author-840894718169-fixed-target-collar-properness]]

[[math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets]]

[[def-normal-graph-and-mean-curvature-data]]

## Facts & Assumptions

[F1] The radial comparison forces preimages of sufficiently small target radii into arbitrarily small source boundary collars. [[lem-author-840894718169-uniform-gaussian-flow-cone]]

[F2] Each individual boundary germ is one-to-one and covers an individual target boundary collar. [[lem-author-840894718169-normal-projection-local-and-boundary-jets]]

[F3] The common target has a proper finite covering by the projection; its fibre number is locally constant. [[lem-author-840894718169-fixed-target-collar-properness]] [[math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets]]

[F4] A unique normal-projection inverse defines a normal graph in the stated sense. [[def-normal-graph-and-mean-curvature-data]]

## Proof

**Given:**The stated data and complete hypotheses.

**Goal:** Establish the conclusions with the asserted parameter uniformity and domains.

1.1 Fix a candidate. Choose its individual injective source boundary collar from [F2]. By [F1], sufficiently small target radius has all preimages inside that collar. A point there has a preimage by [F2] and only one by its injectivity. Thus the covering has a fibre of size one. Local constancy of the finite fibre number and connectedness of the common target give one sheet everywhere, even though the initially chosen germ width depended on the candidate. [F1, F2, F3]

2.1 The projection is now a global diffeomorphism onto the fixed punctured target collar. Its smooth inverse agrees near $S$ with the individual half-collar inverse in [F2], so extends smoothly to the boundary. The Gaussian time coordinate of that inverse is $w_q$; the geometric cone inequality is unchanged by reparametrization. This proves the graph and cone claims on the common domain, without asserting an interior gradient bound before it is proved elsewhere. [F2, F4, step 1.1] ∎
