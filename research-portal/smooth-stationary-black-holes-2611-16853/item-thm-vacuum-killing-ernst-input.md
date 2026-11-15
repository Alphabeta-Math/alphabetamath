---
title: Vacuum Killing and Ernst differential identities
status: draft
research_item: thm-vacuum-killing-ernst-input
dependency_level: 4
sources:
  references:
    - title: A. D. Ionescu and S. Klainerman, On the uniqueness of smooth, stationary
        black holes in vacuum
      url: https://arxiv.org/pdf/0711.0040
      locator: §4.1 opening; §4.2 equations (4.11)–(4.18), PDF pp. 20–23
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [lem-author-cea8e61dc3c6-killing-exact-two-form](item-lem-author-cea8e61dc3c6-killing-exact-two-form)
- [lem-author-cea8e61dc3c6-vacuum-killing-divergence](item-lem-author-cea8e61dc3c6-vacuum-killing-divergence)
- [lem-author-cea8e61dc3c6-divergence-hodge-closure](item-lem-author-cea8e61dc3c6-divergence-hodge-closure)
- [lem-author-cea8e61dc3c6-killing-flow-invariance](item-lem-author-cea8e61dc3c6-killing-flow-invariance)
- [lem-author-cea8e61dc3c6-closed-ernst-contraction](item-lem-author-cea8e61dc3c6-closed-ernst-contraction)


## Statement

For the stationary Lorentzian data with $\operatorname{Ric}(g)=0$, let $F_{ab}=\nabla_aT_b$ and $\mathcal F=F+i\star_gF$. Then $F=\tfrac12dT^\flat$, $\nabla^aF_{ab}=0$, $dF=d\star_gF=0$, and the complex one-form $\eta=2\iota_T\mathcal F$ is closed. It has smooth local potentials. On any domain where $\eta=d\sigma$, $\operatorname{Re}\sigma=-g(T,T)$ up to an additive real constant on each connected component. A single constant suffices on a connected domain. Global existence and normalization of a potential require a separate period or topology argument.

## Facts & Assumptions

[F1] The smooth oriented, time-oriented four-manifold, metric of signature $(-,+,+,+)$, Killing field, connection and curvature convention are those of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] The complex-linear Hodge star and complex self-dual form convention are those of [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data).

[F3] The Killing derivative is an exact closed two-form. [lem-author-cea8e61dc3c6-killing-exact-two-form](item-lem-author-cea8e61dc3c6-killing-exact-two-form)

[F4] Its divergence is $-\operatorname{Ric}_{bd}T^d$. [lem-author-cea8e61dc3c6-vacuum-killing-divergence](item-lem-author-cea8e61dc3c6-vacuum-killing-divergence)

[F5] A vanishing-divergence two-form has closed Hodge dual. [lem-author-cea8e61dc3c6-divergence-hodge-closure](item-lem-author-cea8e61dc3c6-divergence-hodge-closure)

[F6] The Killing flow preserves the complex two-form. [lem-author-cea8e61dc3c6-killing-flow-invariance](item-lem-author-cea8e61dc3c6-killing-flow-invariance)

[F7] In vacuum the Ernst contraction is closed, has real part $df$, and has local potentials; a primitive has real part $f$ plus componentwise constants. [lem-author-cea8e61dc3c6-closed-ernst-contraction](item-lem-author-cea8e61dc3c6-closed-ernst-contraction)

## Proof

**Given:**The data and hypotheses in the Statement.

**Goal:** Prove all asserted identities under these hypotheses.

1.1 The hypotheses give the geometric data required by [F3]–[F6]. By [F3], $F=\tfrac12dT^\flat$ and $dF=0$. Ricci flatness and [F4] give $\nabla^aF_{ab}=0$, and [F5] gives $d\star_gF=0$. The complex Hodge convention is exactly the one in [F2]. [given, F1, F2, F3, F4, F5, F6]

2.1 Apply [F7] with this same $T$, $F$ and $\star_g$: it gives all claims about $\eta$ and local or assumed global primitives. On a connected domain the componentwise constant is a single constant. None of these inputs asserts a global primitive from closedness alone, so the stated separate global obligation remains. [step 1.1, F7] ∎

## Source notes

Independently retrieved and read Ionescu–Klainerman, §4.1 opening and §4.2 (4.11)–(4.18), including the vacuum, Killing and Hodge conventions and the separate simply-connectedness sentence. The differential identities agree with the formulation here. That passage states the Ernst identities and refers elsewhere for their verification; its full cited proof was not read. The proof above instead composes the five locally authored prerequisites, whose only explicit external differential input is the convention-matched Ricci commutator from Reall. No global black-hole hypothesis or complete flow is needed for these local differential identities. No source proof review or native mathematical acceptance is claimed.
