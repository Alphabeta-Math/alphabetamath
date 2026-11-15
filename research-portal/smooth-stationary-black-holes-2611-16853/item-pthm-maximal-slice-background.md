---
title: "Remark 1.1: maximal slice and decay"
status: draft
research_item: pthm-maximal-slice-background
dependency_level: 17
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p4, Remark1.1; MainTheorem1.1 maximality assumption immediately above
      statement: The article states that a maximal slice in its regular non-degenerate
        stationary vacuum setting can be obtained from [15], and that the
        required decay can then be obtained by elliptic estimates. This records
        the existence/decay claim as stated, not an independent verification of
        [15].
      hypotheses: Attribution of the preserved original claim only. The regular
        stationary-vacuum hypotheses are supplied independently by the declared
        definition/model premises.
      reading_limits: Read actual original Remark1.1 and the separate explicit
        maximality hypothesis in MainTheorem1.1. The article citation is
        attribution only, not prerequisite proof. The mathematical construction
        and imported existence/elliptic sources are recorded in the declared
        suppliers.
---

PDF p. 4: ` Remark 1.1 `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [thm-stationary-maximal-slice-existence-input](item-thm-stationary-maximal-slice-existence-input)
- [lem-author-294e9b08725d-regular-cw-maximal-section](item-lem-author-294e9b08725d-regular-cw-maximal-section)
- [lem-author-294e9b08725d-maximal-end-differentiated-end-reconstruction](item-lem-author-294e9b08725d-maximal-end-differentiated-end-reconstruction)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

The article states that a maximal slice in its regular non-degenerate stationary vacuum setting can be obtained from [15], and that the required decay can then be obtained by elliptic estimates. This records the existence/decay claim as stated, not an independent verification of [15].

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

## Facts & Assumptions

**Given:** The stationary-vacuum model and exactly the article regular-spacetime hypotheses.

**Goal:** Supply the maximal section and its required differentiated end decay while preserving the original attribution.

[F1] The authoring convention is ZFC, including the Axiom of Choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F2] The physical model assumes smooth four-dimensional general relativity with a stationary Ricci-flat geometry and the specified end normalization. [post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[F3] The regular-spacetime hypotheses supply the exterior Cauchy section, complete stationary exterior flow and smooth transverse nonexpanding bifurcate boundary; maximality is not part of this definition. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F4] The authored completion chain matches all class-(b) and exclusion hypotheses of the precise CW external input and supplies a maximal bifurcation-boundary section with Cauchy interior in exactly the original exterior. [lem-author-294e9b08725d-regular-cw-maximal-section](item-lem-author-294e9b08725d-regular-cw-maximal-section) [thm-stationary-maximal-slice-existence-input](item-thm-stationary-maximal-slice-existence-input)

[F5] The independent end-gauge chain supplies the required stationary chart adapted to that same maximal section, with differentiated metric decay through order six. [lem-author-294e9b08725d-maximal-end-differentiated-end-reconstruction](item-lem-author-294e9b08725d-maximal-end-differentiated-end-reconstruction) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

## Proof

1.1 Apply the completion-chain conclusion to the regular vacuum geometry. Its positive-mass, full-jet reflection, vacuum development and abstract collar construction supply a strongly causal stationary ambient spacetime with complete stationary field, closed acausal section with boundary $S$, and interior domain of dependence exactly $E$. The precise CW input therefore gives a smooth maximal section whose boundary is $S$ and whose interior is Cauchy in $E$. This uses neither a maximality hypothesis from MainTheorem1.1 nor global axisymmetry. [F1, F2, F3, F4]

2.1 Apply the end-gauge conclusion to this same maximal section and stationary vacuum end. It gives a stationary chart with $T=\partial_t$ and the section at $t=0$, satisfying $g_{00}=-1+2M/r+O_6(r^{-2})$, $g_{0i}=O_6(r^{-2})$, and $g_{ij}=\delta_{ij}+O_6(r^{-1})$, with the stated stationary mass normalization. These are the required differentiated bounds. Thus the maximal-slice existence and elliptic-decay claims have their separate matched inputs; the article citation only identifies the original remark. [F2, F4, F5, step 1.1] ∎

## Source notes

The maximality explicitly assumed in MainTheorem1.1 is not a premise of this proof. The existence theorem and the stronger end normalization are separate imported/local chains, with their actual source hypotheses and reading limits retained in those suppliers. No independent reconstruction of the cited nonlinear existence theorem, no separate proof review and no article-defect judgment is claimed.
