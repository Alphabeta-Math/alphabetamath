---
title: Exterior Schrödinger maximum principles, Hopf growth and Harnack
status: draft
research_item: lem-exterior-lapse-maximum-and-boundary-control
dependency_level: 5
---

## Prerequisites

- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [lem-author-58255dfd955f-exterior-exhaustion](item-lem-author-58255dfd955f-exterior-exhaustion)
- [lem-author-58255dfd955f-boundary-linear-growth](item-lem-author-58255dfd955f-boundary-linear-growth)
- [lem-author-58255dfd955f-local-potential-harnack](item-lem-author-58255dfd955f-local-potential-harnack)
- [lem-author-58255dfd955f-compact-harnack-chain](item-lem-author-58255dfd955f-compact-harnack-chain)
- [lem-author-58255dfd955f-anchored-uniform-positivity](item-lem-author-58255dfd955f-anchored-uniform-positivity)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

On a connected smooth Riemannian exterior $(\Sigma,h)$ with compact smooth boundary $S$, let $V\ge0$ be smooth and let $u\in C^2(\Sigma^\circ)\cap C^1_{\mathrm{loc}}(\Sigma)$ satisfy $(\Delta_h-V)u=0$, $u|_S=0$, and $u\to c>0$ uniformly at infinity. Then $0<u\le c$ in the interior; when $S\ne\varnothing$, $u<c$ there. The metric inward unit normal derivative is strictly positive at $S$. On a sufficiently small fixed compact boundary collar, $u\ge c_0\rho$ for $c_0>0$, where $\rho$ is the collar coordinate or the metric distance to $S$.

Positive solutions admit multiplicative interior Harnack comparison on fixed compact connected interior subsets. The constants are uniform for families with a common finite chart cover and uniform metric ellipticity, metric coefficient and bounded-potential controls there. A uniform absolute lower bound additionally requires a positive uniform anchor value. No uniformity is asserted when the metric degenerates, the cover loses control, or the only normalization is an individual end limit.

## Facts & Assumptions

**Given:** Work in ZFC, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) and the choice uses inherited through the declared suppliers. The exterior, end limit and Laplacian convention are those of [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data). The normal is the unit vector orthogonal to $S$ pointing into $\Sigma$; the gradient formulation fixes this notion. A collar coordinate and its distance version are specified in [lem-author-58255dfd955f-boundary-linear-growth](item-lem-author-58255dfd955f-boundary-linear-growth).

[F1] Exterior bounds and strict interior positivity are [lem-author-58255dfd955f-exterior-exhaustion](item-lem-author-58255dfd955f-exterior-exhaustion). Boundary normal positivity and fixed-collar linear growth are [lem-author-58255dfd955f-boundary-linear-growth](item-lem-author-58255dfd955f-boundary-linear-growth).

[F2] Bounded-potential multiplicative Harnack is [lem-author-58255dfd955f-local-potential-harnack](item-lem-author-58255dfd955f-local-potential-harnack), with its actual coefficient contract. Finite propagation is [lem-author-58255dfd955f-compact-harnack-chain](item-lem-author-58255dfd955f-compact-harnack-chain), and absolute uniform positivity from an anchor is [lem-author-58255dfd955f-anchored-uniform-positivity](item-lem-author-58255dfd955f-anchored-uniform-positivity).

## Proof

**Given:** The hypotheses and data in the Statement and Facts & Assumptions.

**Goal:** Establish the conclusions of the Statement.

**Proof technique:** direct.

1.1 Apply [F1] with the given boundary values and the uniform end limit. Its exhaustion argument first supplies nonnegativity and the upper bound; the strong minimum argument excludes an interior zero. Its strict upper clause applies when the boundary is nonempty. This proves all asserted interior bounds. [given, F1]

2.1 If $S$ is empty, the boundary assertions are vacuous. Otherwise apply the boundary result in [F1] to this positive solution. Smoothness of the boundary gives tangent balls in boundary charts, and the variable-coefficient barrier uses the actual nonpositive zeroth-order coefficient $-V$. It yields the strict inward normal derivative and, by compactness and $C^1$ continuity, a positive linear bound on one small collar. [step 1.1, F1]

3.1 In each of the finitely many interior chart balls use [F2]. In particular the potential belongs to the operator, not to an additive uncontrolled forcing term. The finite chain compares arbitrary values on the compact connected set. Its constants depend only on the chosen cover and the displayed coefficient controls; the anchor result identifies precisely the extra normalization needed for absolute positivity in a family. This proves the remaining statements and qualifications. [F2, given] ∎

## Source notes

The prior Laplacian-only Hopf supplier and additive-forcing Harnack supplier are not used outside their interfaces. The boundary and maximum arguments are supplied locally in the explicit helper chain. The outstanding bounded-potential Harnack theorem is an honestly labeled independent external input in the Harnack chain; its underlying iteration proof is not claimed as locally reconstructed. This resolution concerns a generated prerequisite draft, and asserts no defect in the original article or its literature.
