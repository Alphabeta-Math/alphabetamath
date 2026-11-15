---
title: Spacetime stably outermost condition and the slice bridge
status: published
research_item: def-author-97780c2fed82-spacetime-stably-outermost-data
dependency_level: 6
---

## Prerequisites

- [def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data)
- [lem-author-97780c2fed82-mots-variation-second-jet](item-lem-author-97780c2fed82-mots-variation-second-jet)
- [lem-author-97780c2fed82-mots-boost-variation](item-lem-author-97780c2fed82-mots-boost-variation)
- [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)


## Definition

Assume Countable Choice $\mathrm{AC}_\omega$ for the supplied general-surface and spacetime-deformation constructions and, in the slice setting below, the normal-graph construction.

For a closed MOTS with supplied global future null pair $g(\ell,k)=-1$, say that it is spacetime stably outermost when there are smooth functions $\bar\gamma\ge0$ and $\psi>0$ such that, with $x=\bar\gamma\ell-k$ and $X=\psi x=\gamma\ell-\psi k$ where $\gamma=\psi\bar\gamma$, one has $\delta_X\theta_{(\ell)}\ge0$ pointwise. The derivative is the general spacetime deformation derivative, not a derivative restricted by definition to a spacelike slice. Stability with respect to a specified normal direction $v$ means the same condition with $X=\psi v$ for some positive $\psi$.

When $S$ is also in a spacelike hypersurface with future unit normal $n$ and outward unit normal $\nu$ within it, use $\ell=n+\nu$, $k=(n-\nu)/2$. Its normal-graph operator $\mathcal L$ is the derivative defined in the slice supplier. If a smooth positive function $f$ satisfies $\mathcal Lf\ge0$, then this supplies the spacetime-stability witness $X=f\nu=(f/2)\ell-fk$, namely $\psi=f$ and $\bar\gamma=1/2$. A principal-eigenvalue argument can supply such an $f$ only after its own positive-eigenfunction theorem and hypotheses have been supplied.

## Definition references

[def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data)

[lem-author-97780c2fed82-mots-variation-second-jet](item-lem-author-97780c2fed82-mots-variation-second-jet)

[lem-author-97780c2fed82-mots-boost-variation](item-lem-author-97780c2fed82-mots-boost-variation)

[def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

## Facts & Assumptions

[A1] Countable Choice is assumed as required by the general-surface, spacetime-deformation and slice normal-graph suppliers. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F1] Under [A1], general spacelike MOTS data and well-defined spacetime expansion variation are available. [def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data) [lem-author-97780c2fed82-mots-variation-second-jet](item-lem-author-97780c2fed82-mots-variation-second-jet)

[F2] Positivity of the variation condition is independent of boosts of the base null pair. [lem-author-97780c2fed82-mots-boost-variation](item-lem-author-97780c2fed82-mots-boost-variation)

[F3] Under [A1], in the slice setting, the graph gauge and its derivative $\mathcal Lf$ have the stated fixed base normal and actual admissible deformations. [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)

## Justification

**Given:** The objects and hypotheses in the Definition, including Countable Choice.

**Goal:** Establish the assertions and well-definedness stated there.

1.1 Under [A1], the quantified functions and the well-defined derivative of [F1] give an unambiguous predicate. The equivalence of the two displayed coefficient descriptions follows from $\gamma=\psi\bar\gamma$ and $\psi>0$. The normal velocity is spacelike or null by the calculation in [F2], while [F2] also makes the predicate independent of a positive rescaling of the chosen pair. [A1, F1, F2]

2.1 Under [A1], the slice supplier gives actual admissible normal-graph deformations. In the slice gauge, direct substitution gives $\ell/2-k=\nu$. The graph with initial velocity $f\nu$ is one of the spacetime deformation families in [F1], and its outgoing normal has precisely the same base $\ell=n+\nu$. Independence of the family and of its extension gauge at a MOTS in [F1] identifies its derivative with $\delta_{f\nu}\theta_{(\ell)}$. Thus $\mathcal Lf\ge0$ supplies exactly the stated witness. This proves the bridge from an actual positive supersolution; it makes no unsupported spectral-existence assertion. [A1, F1, F3, step 1.1] ∎
