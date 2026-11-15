---
title: Stationary ADM speed bounds and Cauchy sections
status: draft
research_item: lem-stationary-adm-causal-completeness-input
dependency_level: 5
sources:
  references: []
---

## Prerequisites

- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)
- [lem-author-eb8e266b8b92-interior-compact-confinement](item-lem-author-eb8e266b8b92-interior-compact-confinement)
- [lem-author-eb8e266b8b92-compact-causal-endpoint](item-lem-author-eb8e266b8b92-compact-causal-endpoint)
- [physics:thm-gr-cauchy-surface-implies-globally-hyperbolic](https://alphabetamath.cc/physics/item/thm-gr-cauchy-surface-implies-globally-hyperbolic)
- [lem-author-eb8e266b8b92-proper-radius-control](item-lem-author-eb8e266b8b92-proper-radius-control)


## Statement

Assume the Axiom of Choice. Let $\overline\Sigma$ be a connected smooth three-manifold with compact boundary $B$ and interior $\Sigma^\circ$. Let $h$ extend to a smooth positive-definite metric on $\overline\Sigma$, complete up to its compact boundary, meaning that its intrinsic metric with the boundary included is complete. Let $N:\overline\Sigma\to\mathbb R$ be a smooth real-valued function and $X$ a smooth tangent vector field on $\overline\Sigma$, with $N>0$ in the interior. On $E=\mathbb R_v\times\Sigma^\circ$ put $g=-N^2dv^2+h_{ij}(dx^i+X^idv)(dx^j+X^jdv)$, oriented by $n=N^{-1}(\partial_v-X)$; all coefficients are independent of $v$.

Supply a collar $[0,\epsilon)\times B$ with coordinate $\rho$, and constants with $N\le A\rho$, $|X(\rho)|\le A\rho$, and $|d\rho|_h\le A$ there. Supply a smooth nonnegative proper exhaustion $R$ of $\overline\Sigma$: each $\{R\le m\}$ is compact. Outside a compact core require $|dR|_h(N+|X|_h)\le C$. A sufficient end-coordinate realization is to provide a compact core with finitely many ends $[r_0,\infty)\times F_j$, compact $F_j$, let $R$ equal their unbounded radial coordinates sufficiently far out, and impose this estimate there. A bounded function of radius is insufficient. If $B$ is empty, omit the collar conditions.

Then each inextendible causal curve, with locally absolutely continuous nonzero causal velocity almost everywhere, has $v$-image all of $\mathbb R$. Consequently every $v$-level is a spacelike Cauchy hypersurface, and $(E,g,n)$ is globally hyperbolic. This is completeness of causal section time, not completeness of geodesic affine parameters. The smoothness and proper-exhaustion conditions explicitly specify all escape mechanisms; spatial metric completeness alone does not replace the proper-radius estimate.

## Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)

[lem-author-eb8e266b8b92-interior-compact-confinement](item-lem-author-eb8e266b8b92-interior-compact-confinement)

[lem-author-eb8e266b8b92-compact-causal-endpoint](item-lem-author-eb8e266b8b92-compact-causal-endpoint)

[physics:thm-gr-cauchy-surface-implies-globally-hyperbolic](https://alphabetamath.cc/physics/item/thm-gr-cauchy-surface-implies-globally-hyperbolic)

[lem-author-eb8e266b8b92-proper-radius-control](item-lem-author-eb8e266b8b92-proper-radius-control)

## Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice implies Dependent Choice and Countable Choice, supplying the inherited choice assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F2] Causal curves, absence of endpoints, Cauchy hypersurfaces and global hyperbolicity are interpreted relative to $E$. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F3] Lapse and shift use the unit-normal decomposition; completeness up to compact boundary concerns the intrinsic spatial distance with that boundary included. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F4] The ADM section-time lemma gives strict monotonicity, a causal locally Lipschitz reparametrization and spatial speed $|x\prime|_h\le N+|X|_h$. [lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)

[F5] Under the stated collar and proper-radius assumptions, both barriers put a bounded section-time spatial trajectory in a compact subset of the interior. [lem-author-eb8e266b8b92-interior-compact-confinement](item-lem-author-eb8e266b8b92-interior-compact-confinement)

[F6] A causal section-time trajectory in an interior compact set has a limit in $E$ at each finite section-time endpoint. [lem-author-eb8e266b8b92-compact-causal-endpoint](item-lem-author-eb8e266b8b92-compact-causal-endpoint)

[F7] On a time-oriented smooth Lorentzian four-manifold, existence of a Cauchy set implies strong causality and compact causal diamonds, assuming countable and dependent choice. [physics:thm-gr-cauchy-surface-implies-globally-hyperbolic](https://alphabetamath.cc/physics/item/thm-gr-cauchy-surface-implies-globally-hyperbolic)

[F8] When the boundary is empty, the proper-radius control alone confines bounded section-time trajectories to compact interior sets. [lem-author-eb8e266b8b92-proper-radius-control](item-lem-author-eb8e266b8b92-proper-radius-control)

## Proof

**Given:**The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

1.1 The displayed ADM metric has Lorentzian signature, and its unit future normal is $n$ as specified. Each $v$-level is an embedded copy of $\Sigma^\circ$ with induced positive metric $h$. For an inextendible future causal curve, the section-time lemma makes $v$ strictly increasing and gives its locally Lipschitz section-time representation on an interval $I$. This change of parameter preserves the absence of endpoints. [F2, F3, F4, algebra]

2.1 If $\sup I=v_*<\infty$, fix $v_0\in I$. The barrier hypotheses give interior compact confinement of the spatial trajectory for $v_0\le v<v_*$. The compact endpoint lemma then gives a limit $(v_*,p)\in E$, contradicting inextendibility. When $B$ is empty, the proper-radius estimate alone gives the required interior compact set, since all spatial points are interior. The identical argument at $\inf I$ excludes a finite lower endpoint. Therefore $I=\mathbb R$. [F5, F6, F8, step 1.1, algebra]

3.1 For every real $a$, the continuous strictly increasing section time on each inextendible causal curve takes the value $a$ exactly once. Thus $\{v=a\}$ is a Cauchy set in $E$ and, by its already established positive induced metric, a Cauchy hypersurface. The Cauchy-set implication applies to the smooth Lorentzian four-manifold $(E,g,n)$; its Countable Choice and Dependent Choice hypotheses follow from the assumed Axiom of Choice by F1. Hence $E$ is strongly causal with compact causal diamonds, which is global hyperbolicity. [F1, F2, F7, step 1.1, step 2.1] ∎

## Remarks

The proper-exhaustion version is the general contract; the finite product-end version is a sufficient way to supply it, rather than a consequence of an arbitrary radial notation. The theorem does not construct a stationary product from a stationary flow, and does not assert existence of a maximal section. Applications to a transformed geometry must separately supply the global product, the smooth boundary/collar data and the actual proper end radius for each fixed parameter. No uniform estimate as a deformation parameter tends to zero is asserted. The spatial completeness hypothesis is retained from the scaffold, although the compact-exhaustion proof does not need it once the explicit escape controls are supplied.
