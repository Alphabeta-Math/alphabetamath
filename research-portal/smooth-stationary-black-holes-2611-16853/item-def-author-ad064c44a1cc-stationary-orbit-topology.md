---
title: Stationary orbit space with its quotient topology
status: published
research_item: def-author-ad064c44a1cc-stationary-orbit-topology
dependency_level: 3
sources:
  references:
    - title: Alexandru F. Radu, On rigidity of stationary black holes under a
        nontrapping assumption
      url: https://arxiv.org/html/2609.23872v1
      locator: "Version 1, §1.1, printed pp. 4–5: quotient-space definition after SBS
        and the compact-set clarification immediately after NT."
      statement: Identify points of the open exterior E on the same stationary orbit
        to form Q=E/R, with orbit projection pi. A subset of Q is open exactly
        when its inverse image in E is open. The compact sets used in NT belong
        to this open-exterior quotient, excluding a compactification by the
        horizon or asymptotic ends.
      hypotheses: The passage is in Radu's GR/SBS setting. This construction uses the
        GR exterior E and its complete stationary flow. The NT predicate and the
        later smooth-quotient theorem are not assumptions needed to define this
        topology.
      reading_limits: Read the version-1 HTML §1.1 GR complete-orbit clause, SBS
        context, quotient definition and NT compact-set clarification;
        cross-checked the corresponding PDF passage on printed pp. 4–5. Only the
        definition and compact-set interpretation are imported; Proposition 2.1
        and the rigidity proof were not reviewed.
---

## Prerequisites

- [def-author-ad064c44a1cc-nontrapping-gr](item-def-author-ad064c44a1cc-nontrapping-gr)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:def-equivalence-relation](https://alphabetamath.cc/item/def-equivalence-relation)
- [math:def-quotient-topology](https://alphabetamath.cc/item/def-quotient-topology)
- [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)
- [` Alexandru F. Radu, On rigidity of stationary black holes under a nontrapping assumption · Version 1, §1.1, printed pp. 4–5: quotient-space definition after SBS and the compact-set clarification immediately after NT. `](https://arxiv.org/html/2609.23872v1)


## Definition

For the complete stationary flow $\Phi_t$ on the exterior in the NT package, define $p\sim q$ when $q=\Phi_t(p)$ for some $t\in\mathbb R$. Let $Q=E/\mathbb R$ be its set of orbits and let $\pi:E\to Q$ send each point to its orbit. Give $Q$ the quotient topology: $U\subset Q$ is open precisely when $\pi^{-1}(U)$ is open in $E$. A subset $K\subset Q$ is compact when every cover of it by open subsets of $Q$ has a finite subcover.

For a curve $\gamma:I\to E$, its stationary projection means $\pi\circ\gamma$, or its image $\pi(\gamma(I))$ when discussing containment. A compact set for the source NT condition is a compact subset of this open-exterior quotient, not a subset of a compactification containing the horizon or infinity. No choice of global time coordinate, smooth quotient structure, free action or proper action is required to state this topological condition; those additional source results are not assumed here.

## Facts & Assumptions

[F1] [def-author-ad064c44a1cc-nontrapping-gr](item-def-author-ad064c44a1cc-nontrapping-gr) supplies complete exterior orbits. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) defines the local flow; completeness in [F1] makes it the indicated real-parameter flow on $E$.

## Justification

The flow identities give reflexivity, symmetry and transitivity of $\sim$, so its equivalence classes define $Q$ and the surjection $\pi$. Preimages preserve arbitrary unions and finite intersections and take the empty set and whole space to their counterparts; hence the specified collection of subsets is a topology. The projection is continuous by this definition. The compactness predicate and curve-image containment therefore make sense without identifying $Q$ with a section or assuming a smooth-manifold theorem about it. In particular time drift along an orbit is removed by $\pi$, so boundedness in an arbitrary spacetime coordinate chart cannot replace this definition.
