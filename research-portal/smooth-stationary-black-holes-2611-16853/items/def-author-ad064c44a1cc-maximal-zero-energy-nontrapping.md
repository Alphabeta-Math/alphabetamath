---
id: def-author-ad064c44a1cc-maximal-zero-energy-nontrapping
title: The precise maximal zero-energy nontrapping predicate
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-ad064c44a1cc-nontrapping-gr
  - def-author-ad064c44a1cc-nontrapping-sbs
  - def-author-ad064c44a1cc-stationary-orbit-topology
  - lem-author-ad064c44a1cc-zero-stationary-energy
  - math:def-geodesic-of-an-affine-connection
dependency_roles:
  def-author-ad064c44a1cc-nontrapping-gr: mathematical-premise
  def-author-ad064c44a1cc-nontrapping-sbs: mathematical-premise
  def-author-ad064c44a1cc-stationary-orbit-topology: mathematical-premise
  lem-author-ad064c44a1cc-zero-stationary-energy: mathematical-premise
  math:def-geodesic-of-an-affine-connection: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Alexandru F. Radu, On rigidity of stationary black holes under a
        nontrapping assumption
      url: https://arxiv.org/html/2609.23872v1
      locator: "Version 1, section 1.1: quotient definition after SBS; NT and its
        following maximality/compactness paragraph; energy discussion
        immediately after Theorem 1.1."
      statement: NT forbids a maximal unparametrized null geodesic in E orthogonal to
        T whose entire stationary projection lies in a compact subset of Q=E/R.
        Maximality is within E and includes finite affine parameter intervals.
        Compact sets belong to the quotient of the open exterior, away from
        horizon and asymptotic ends. The energy discussion restricts NT to zero
        stationary energy and allows usual Kerr photon trapping.
      hypotheses: "The source GR/SBS setting: a smooth connected oriented
        time-oriented stationary Ricci-flat four-spacetime, the specified
        asymptotically flat end and partial Cauchy slice, globally hyperbolic
        exterior with complete stationary orbits, and smooth transverse
        nonexpanding bifurcate event horizons. This imports a predicate, not a
        rigidity conclusion."
      reading_limits: Read the version-1 HTML section 1.1 setup, GR, SBS, quotient
        definition, NT, its maximality/compactness clarification and
        post-Theorem-1.1 energy discussion. Used only for formulation and
        attribution; no rigidity proof or quotient-regularity proof was
        reviewed.
dependency_level: 4
---

## Definition

In the Radu NT source setting, a **maximal unparametrized null geodesic in $E$** is a nonconstant smooth null geodesic image with its local geodesic parameterizations, taken up to regular reparametrization, which has no proper continuation as an unparametrized geodesic within $E$. Maximality is relative to this open exterior; its maximal affine parameter interval is allowed to have finite endpoints. Affine completeness is not an added hypothesis.

The source **NT condition** is that no such maximal null geodesic $\gamma$ with zero stationary energy has $\pi(\gamma)$ contained in any compact subset $K\subset Q=E/\mathbb R$. In quantified form: for every maximal zero-energy null geodesic $\gamma$ and every compact $K\subset Q$, some point of $\pi(\gamma)$ lies outside $K$. It excludes whole-geodesic containment, not every geodesic segment in a compact set. It neither excludes ordinary photon trapping at nonzero stationary energy nor requires a particular spacetime coordinate radius to be unbounded. The compact subsets are in the quotient of the open exterior; approaching the horizon or infinity is not trapped compact containment there.

## Facts & Assumptions

[F1] [[def-author-ad064c44a1cc-nontrapping-gr]] and [[def-author-ad064c44a1cc-nontrapping-sbs]] fix the source exterior and horizon hypotheses. [[def-author-ad064c44a1cc-stationary-orbit-topology]] supplies $Q,\pi$ and its compactness convention.

[F2] [[math:def-geodesic-of-an-affine-connection]] supplies affine geodesics, and [[lem-author-ad064c44a1cc-zero-stationary-energy]] proves that zero energy is independent of the permitted parameterization.

## Justification

The source geodesic image and continuation relation specify the maximality predicate within $E$. The quotient topology supplies a definite class of compact sets, and the energy lemma makes the orthogonality test independent of a chosen parameter. Negating existence of a containing compact set is exactly the displayed universal condition. This equivalence uses only the negation of set containment, and makes no assertion that every such geodesic has infinite affine length or that every compact segment must leave its initial compact set in a prescribed direction or time. The definition is therefore the precise source condition rather than a stronger two-sided or affine-completeness substitute.
