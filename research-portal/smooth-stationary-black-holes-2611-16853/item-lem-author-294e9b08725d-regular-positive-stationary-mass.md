---
title: Positive stationary mass from the bifurcate vacuum boundary
status: published
research_item: lem-author-294e9b08725d-regular-positive-stationary-mass
dependency_level: 7
sources:
  references: []
---

## Prerequisites

- [lem-author-294e9b08725d-complete-boundary-initial-data-interface](item-lem-author-294e9b08725d-complete-boundary-initial-data-interface)
- [lem-author-294e9b08725d-vacuum-section-dominant-energy](item-lem-author-294e9b08725d-vacuum-section-dominant-energy)
- [lem-author-294e9b08725d-stationary-end-extrinsic-decay](item-lem-author-294e9b08725d-stationary-end-extrinsic-decay)
- [lem-author-294e9b08725d-bifurcation-boundary-zero-expansions](item-lem-author-294e9b08725d-bifurcation-boundary-zero-expansions)
- [thm-author-294e9b08725d-boundary-positive-energy-input](item-thm-author-294e9b08725d-boundary-positive-energy-input)
- [thm-author-294e9b08725d-stationary-vacuum-adm-komar-input](item-thm-author-294e9b08725d-stationary-vacuum-adm-komar-input)
- [lem-author-294e9b08725d-stationary-end-komar-coefficient](item-lem-author-294e9b08725d-stationary-end-komar-coefficient)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)


## Statement

Under exactly the article regular stationary-vacuum hypotheses, the original stationary end coefficient $M_0$ is strictly positive. More precisely the complete exterior section has ADM energy $E>0$, zero linear momentum, and $M_0=m_K=E$. This conclusion assumes neither maximality nor axisymmetry.

## Statement references

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions](item-def-author-cea8e61dc3c6-kerr-asymptotic-charge-conventions)

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[F1] The section satisfies complete AF initial-data assumptions, vacuum DEC, and trace decay of order three. [lem-author-294e9b08725d-complete-boundary-initial-data-interface](item-lem-author-294e9b08725d-complete-boundary-initial-data-interface) [lem-author-294e9b08725d-vacuum-section-dominant-energy](item-lem-author-294e9b08725d-vacuum-section-dominant-energy) [lem-author-294e9b08725d-stationary-end-extrinsic-decay](item-lem-author-294e9b08725d-stationary-end-extrinsic-decay)

[F2] The into-exterior boundary expansions both vanish. [lem-author-294e9b08725d-bifurcation-boundary-zero-expansions](item-lem-author-294e9b08725d-bifurcation-boundary-zero-expansions)

[F3] The exact boundary positive-energy input applies with $n=3$ and $\gamma=3$. [thm-author-294e9b08725d-boundary-positive-energy-input](item-thm-author-294e9b08725d-boundary-positive-energy-input)

[F4] Ordinary stationary vacuum ADM and Komar masses agree and the latter is the original coefficient. [thm-author-294e9b08725d-stationary-vacuum-adm-komar-input](item-thm-author-294e9b08725d-stationary-vacuum-adm-komar-input) [lem-author-294e9b08725d-stationary-end-komar-coefficient](item-lem-author-294e9b08725d-stationary-end-komar-coefficient)

## Proof

1.1 Apply the boundary positive-energy input to $\overline C$ using completeness and smooth nonempty compact boundary, the decay with $q=1$, zero constraint densities, zero boundary expansions, and trace decay with $\gamma=3>2$. Every condition is supplied without a maximality assumption, hence $E>0$. The same initial-data interface gives $P=0$. [F1, F2, F3, algebra]

2.1 The end is ordinary four-dimensional stationary vacuum, so ADM–Komar equality applies with the normalization fixed in the explicit end flux. Therefore $M_0=m_K=E>0$. [F4, algebra] ∎
