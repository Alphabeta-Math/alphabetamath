---
title: The maximal equation upgrades pointwise order-four graph decay to
  weighted order five
status: draft
research_item: lem-author-45355d85383b-weighted-fifth-graph-derivative
dependency_level: 3
---

## Prerequisites

- [lem-author-45355d85383b-stationary-maximal-flux-formula](item-lem-author-45355d85383b-stationary-maximal-flux-formula)
- [lem-author-db87cb8e0bab-coefficient-regularity](item-lem-author-db87cb8e0bab-coefficient-regularity)
- [lem-author-db87cb8e0bab-linear-fourth-derivative-estimate](item-lem-author-db87cb8e0bab-linear-fourth-derivative-estimate)
- [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations)
- [def-weighted-holder-spaces](item-def-weighted-holder-spaces)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in ZFC. Let a smooth stationary maximal graph have $|D^ju|\le Cr^{-3/4-j}$ for $0\le j\le4$, in a background satisfying the preceding flux lemma. Then $u\in C^{5,\alpha}_{-3/4}$ on the end for every fixed $0<\alpha<1$. The realized linear graph equation may be normalized as $a^{ij}u_{ij}+b^ju_j=f$ with $a-\delta\in C^{2,\alpha}_{-1}$, $b\in C^{2,\alpha}_{-2}$, and $f\in C^{2,\alpha}_{-3}$. In particular $\Delta_0u\in C^{2,\alpha}_{-3}$, where $\Delta_0$ is the Euclidean Laplacian.

## Facts & Assumptions

[F1] The stationary graph equation has a uniformly elliptic flux on fixed rescaled annuli. [lem-author-45355d85383b-stationary-maximal-flux-formula](item-lem-author-45355d85383b-stationary-maximal-flux-formula)

[F2] The preliminary differentiated-flux bootstrap gives realized coefficient $C^{2,\alpha}$ bounds. [lem-author-db87cb8e0bab-coefficient-regularity](item-lem-author-db87cb8e0bab-coefficient-regularity)

[F3] The controlled realized linear equation has the interior $C^{4,\alpha}$ estimate linear in height and forcing. [lem-author-db87cb8e0bab-linear-fourth-derivative-estimate](item-lem-author-db87cb8e0bab-linear-fourth-derivative-estimate)

[F4] The linear interior Schauder estimate applies to derivatives once their coefficient Hölder bounds are established. [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations)

[F5] The end-weight convention measures derivatives and Hölder seminorms on fixed rescaled annuli. [def-weighted-holder-spaces](item-def-weighted-holder-spaces)

[A1] Work in ZFC, including the Axiom of Choice required by [F2] and [F3]. It also supplies the Countable Choice required by [F4]: for a sequence of nonempty sets, apply Choice to its family of values and compose the choice function with the sequence. This assumption is used when invoking [F2] and [F3] in step 1.1 and [F4] in step 2.1. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The assumptions in the Statement.

**Goal:** Establish the stated conditional construction or estimate.

1.1 Under [A1], put $v(y)=u(Ry)$ and $w=v/R$. The height and slope assumptions bound $w$ and keep $Dw$ in a fixed spacelike ball. [F1] and [F2] first give the realized coefficient bounds, before applying [F3]. The forcing for $v$ is $-R s(y,0)=O(R^{-1})$ in $C^{2,\alpha}$. Thus $\|v\|_{C^{4,\alpha}}\le C(R^{-3/4}+R^{-1})\le CR^{-3/4}$ on a smaller fixed annulus. The conclusion includes Hölder control of fourth derivatives, not just their pointwise bounds. [F1, F2, F3, F5, A1, given]

2.1 One further differentiation is legitimate because the original solution is smooth. The realized coefficients now have uniform $C^{3,\alpha}$ bounds: differentiating $P_p(y,Dw)$ three times uses at most fourth derivatives of $w$, and differentiating $\int_0^1s_p(y,tDw)dt$ three times uses background spatial derivatives through order four. All finite slope derivatives are controlled by [F1]. The rescaled forcing has $C^{3,\alpha}$ norm $O(R^{-1})$. Differentiate the realized equation three times and, using the Countable Choice supplied by [A1], apply [F4] to each $D^3v$; every commutator contains coefficient derivatives through order three and solution derivatives through order four, already bounded by step 1.1. This bounds $v$ in $C^{5,\alpha}$ by $CR^{-3/4}$ on a further smaller annulus. [step 1.1, F1, F4, A1, algebra]

3.1 The pointwise small slope and step 2.1 give, in the original coordinates, $a-\delta=O_{C^{2,\alpha}}(r^{-1})$, $b=O_{C^{2,\alpha}}(r^{-2})$ and $f=O_{C^{2,\alpha}}(r^{-3})$ by the explicit flux and zero-slope formulas. Here the quadratic slope correction is $O(r^{-7/2})$ and does not weaken the metric error. Hence $\Delta_0u=f-(a-\delta):D^2u-b\cdot Du$ has weighted order $-3$ through two Hölder derivatives. Rescale back and use the fixed finite annular covers for the global end assertion. [F1, F5, step 2.1, algebra] ∎
