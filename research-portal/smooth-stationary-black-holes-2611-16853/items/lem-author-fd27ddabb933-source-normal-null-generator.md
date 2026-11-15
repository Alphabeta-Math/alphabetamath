---
id: lem-author-fd27ddabb933-source-normal-null-generator
title: Time reversal supplies a source-normal generator without interior source
  focal points
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-fd27ddabb933-first-contact-chronological-boundary
  - lem-compact-target-achronal-generator-input
  - def-causal-exterior-and-boundary-data
  - def-null-screen-expansion-and-focal-data
  - math:def-axiom-of-choice
dependency_roles:
  lem-author-fd27ddabb933-first-contact-chronological-boundary: mathematical-premise
  lem-compact-target-achronal-generator-input: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 7
---

## Statement

Work in ZFC. Let $(\mathcal E,g,N)$ be a smooth globally hyperbolic time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$, and let $\tau:\mathcal E\to\mathbb R$ be temporal, with past-directed timelike metric gradient. Let $A\subset\tau^{-1}(0)$ be a nonempty compact smooth embedded two-manifold without boundary with positive-definite induced metric. Use the data and hypotheses of the earliest-cylinder-contact construction on this same exterior, source and temporal function, and let $p_R$ be one of its earliest contact points. All chronological relations and boundaries below are relative to $\mathcal E$.

There is a nonconstant future affine null geodesic from $A$ to $p_R$, wholly in $\partial_{\mathcal E}I^+_{\mathcal E}(A)$, initially normal to $A$ and without a focal point to $A$ strictly before $p_R$, with focality measured from $A$ toward $p_R$. The statement supplies both the direction and the focal orientation correctly; it does not yet choose the outgoing source ray.

## Facts & Assumptions

[F1] Use the full data and hypotheses of the first-contact chronological-boundary lemma on this same $(\mathcal E,g,N)$, source $A$ and temporal function $\tau$. Its earliest contact satisfies $p_R\in\partial_{\mathcal E}I^+_{\mathcal E}(A)$ and $\tau(p_R)>0$. [[lem-author-fd27ddabb933-first-contact-chronological-boundary]]

[F2] The compact-target generator theorem supplies a null segment on a chronological boundary, normal at the compact surface and without focal points from that surface. [[lem-compact-target-achronal-generator-input]]

[F3] Use the causal-curve, chronological-relation, boundary, temporal-function and global-hyperbolicity definitions on $\mathcal E$. Reversing the time orientation replaces $N$ by $-N$ while retaining the metric and topology. [[def-causal-exterior-and-boundary-data]]

[F4] A spacelike two-surface is smooth, embedded, nonempty and without boundary, with positive-definite induced metric. Focality from such a surface is rank loss of its normal screen Jacobi map along the geodesic parametrized away from that surface. [[def-null-screen-expansion-and-focal-data]]

[A1] Work in ZFC, including the countable and dependent choice required by the invoked geodesic, compactness and causal interfaces. [[math:def-axiom-of-choice]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Obtain the source-normal future null boundary segment with the stated source-oriented focal exclusion.

1.1 Replace $N$ by $-N$ and write $I^-_{\rm rev}$ for the chronological past in that orientation. Reversing a timelike curve parameter gives $I^-_{\rm rev}(A)=I^+_{\mathcal E}(A)$, and the boundaries agree because the topology is unchanged. Strong causality is unchanged by reversing curve parameters, and each reversed causal diamond is an original diamond with its endpoints exchanged, so global hyperbolicity is preserved. The function $-\tau$ is temporal for $-N$: its gradient has the same negative squared norm as that of $\tau$, and $d(-\tau)(-N)=d\tau(N)>0$. [given, A1, F3]

2.1 By [F1] and step 1.1, $p_R\in\partial_{\mathcal E}I^-_{\rm rev}(A)$ and $-\tau(p_R)<0=\min_A(-\tau)$. The same $A$ is a compact spacelike two-surface in the reversed orientation, since its smoothness, dimension, absence of boundary and induced metric have not changed. Thus every hypothesis of [F2] holds with target $A$ and temporal function $-\tau$. It supplies a null affine segment from $p_R$ to a point $a\in A$, future-directed in the reversed orientation, contained in $\partial_{\mathcal E}I^-_{\rm rev}(A)$, orthogonal to $A$ at $a$, and without an interior focal point measured from $A$ toward $p_R$. It is nonconstant because $\tau(p_R)>0=\tau(a)$. [given, A1, F1, F2, F4, step 1.1]

3.1 Reverse the affine segment parameter. Its tangent changes sign and its covariant acceleration remains zero, so it is now a future affine null segment from $a\in A$ to $p_R$ in the original orientation. Its image lies in $\partial_{\mathcal E}I^+_{\mathcal E}(A)$ by step 1.1, and sign reversal preserves orthogonality at $a$. The focal exclusion in [F2] was already measured from $A$ toward $p_R$, which is exactly the source direction of the reparametrized segment under [F4]; no exchange of source and target focal data is made. A further positive affine scaling only reindexes this normal screen Jacobi map and preserves its rank, as well as the segment image and boundary containment. Selection of the outgoing source ray remains a separate input. [F2, F3, F4, step 1.1, step 2.1, algebra] ∎
