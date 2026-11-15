---
title: "Lemma 4.4: smooth compact comparison region"
status: draft
research_item: pthm-smooth-area-controlled-cut
dependency_level: 31
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 25–26, Lemma 4.4 and proof
      attribution: For every positive error there is a smooth compact region bounded
        by S and a smooth closed, possibly disconnected surface between S and
        the comparison collar, whose area is at most the comparison sphere area
        plus that error.
      hypotheses: The fixed sufficiently small positive parameter and stationary
        vacuum construction, maximal section, collar and sufficiently late
        comparison sphere chosen in Section 4.
      reading_limits: Historical reading note retained from the current source; this
        maintenance revision claims no fresh article or external full-text
        reading. Read the frozen extracted article text at the cited passage.
        This reference attributes the article claim and is not a proof premise.
---

PDF p. 25: ` Lemma 4.4 and proof `; PDF p. 26: ` Lemma 4.4 and proof `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-harrison-one-form](item-def-harrison-one-form)
- [def-stationary-section-time](item-def-stationary-section-time)
- [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)
- [def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets)
- [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)
- [pthm-past-boundary-localization](item-pthm-past-boundary-localization)
- [pthm-coarea-sard-smoothing](item-pthm-coarea-sard-smoothing)
- [def-truncated-null-boundary-height](item-def-truncated-null-boundary-height)
- [pthm-null-endpoint-map-properties](item-pthm-null-endpoint-map-properties)
- [pthm-null-boundary-lipschitz-levels](item-pthm-null-boundary-lipschitz-levels)
- [pthm-complete-maximal-slices](item-pthm-complete-maximal-slices)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)
- [pthm-harrison-lorentzian-algebra](item-pthm-harrison-lorentzian-algebra)
- [pthm-adm-temporality](item-pthm-adm-temporality)
- [lem-author-594d78e425ed-compact-normal-flow-and-area-distortion](item-lem-author-594d78e425ed-compact-normal-flow-and-area-distortion)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in ZFC in the regular mass-one stationary vacuum Harrison construction, with original maximal exterior section and $T|_S\not\equiv0$. Fix a sufficiently small positive $q$, a supplied complete smooth maximal section $\Sigma=\Sigma_{q,0}$ with compact boundary $S$, a sufficiently small smooth distance collar $\mathcal R=\{0\le\rho\le\eta\}$, and a sufficiently late comparison sphere $C=C_t$ as in the localized construction. Here $\rho$ is intrinsic distance from $S$ in the induced Riemannian metric $h_0$ on $\Sigma$, and $S_\eta=\{\rho=\eta\}$.

For every $\epsilon>0$ there is a smooth compact region $\Omega_\epsilon\subset\Sigma$ with $\partial\Omega_\epsilon=S\sqcup D_\epsilon$, where $D_\epsilon$ is smooth, closed, possibly disconnected, lies between $S$ and $S_\eta$, and satisfies $|D_\epsilon|\le|C|+\epsilon$. Areas use the fixed-$q$ metric $g_q$ induced on the respective spacelike surfaces.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-harrison-normalization](item-def-harrison-normalization)

[def-harrison-one-form](item-def-harrison-one-form)

[def-stationary-section-time](item-def-stationary-section-time)

[def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)

[def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets)

[def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[pthm-past-boundary-localization](item-pthm-past-boundary-localization)

[pthm-coarea-sard-smoothing](item-pthm-coarea-sard-smoothing)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[A1] Use the stated stationary vacuum model, regular construction, mass-one normalization and supplied maximal section, in ZFC. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-harrison-normalization](item-def-harrison-normalization) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The stationary section-time interface defines $\Sigma_{q,0}$ as the supplied zero-time section. The comparison-sphere interface defines $C_t$ as the stationary translate of $C_q=\{t=0,r=R_0q^{-2/3}\}$. The near-horizon data define $\rho$ as intrinsic distance from $S$ and $S_\eta$ as its level set. The localized construction supplies a sufficiently small collar and a sufficiently late target. [def-stationary-section-time](item-def-stationary-section-time) [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres) [def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets) [pthm-past-boundary-localization](item-pthm-past-boundary-localization)

[F2] For those fixed data equipped with the truncated height and maximal-family endpoint data, coarea smoothing gives, for every $\epsilon>0$, a smooth compact sublevel region in $\mathcal R$ with boundary $S\sqcup D_\epsilon$, where $D_\epsilon$ is a regular interior level, smooth, closed, possibly disconnected, and $|D_\epsilon|_{h_0}\le|C|+\epsilon$. [pthm-coarea-sard-smoothing](item-pthm-coarea-sard-smoothing)

[F3] Use the supplied Harrison metric $g_q$ on the fixed construction domain, and write $h_0=g_q|_{T\Sigma}$ for its induced Riemannian metric on the supplied spacelike section. Area on a spacelike surface uses its induced Riemannian metric and the normalized two-dimensional Hausdorff measure. [def-harrison-one-form](item-def-harrison-one-form) [def-stationary-section-time](item-def-stationary-section-time) [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[F4] For the localized compact zero-time cut $D$ and the same sufficiently late comparison sphere $C$, the endpoint theorem supplies the maximal past null-normal geodesic family in the exterior. Its unique hits define a closed, compact Borel domain $A\subset C$ and a surjective map $F:A\to D$ with local smooth extensions into the section. These are the maximal-family data of the near-horizon definition; no injectivity is needed. [pthm-null-endpoint-map-properties](item-pthm-null-endpoint-map-properties) [def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets)

[F5] With the temporal section time and common boundary-fixing normal flow supplied independently below, the height result supplies, for a sufficiently late target fixed independently of the smoothing error and a suitable sufficiently small $\delta>0$, the truncated supremum height $u$ on that collar, Lipschitz and equal to $-2\delta$ near $S$ and $2\delta$ near $S_\eta$. Its endpoint data at time zero are the same $D,A,F$ and maximal family as in [F4]. [def-truncated-null-boundary-height](item-def-truncated-null-boundary-height) [pthm-null-boundary-lipschitz-levels](item-pthm-null-boundary-lipschitz-levels)

[F6] For the fixed positive $q$, the maximal-slice theorem supplies the complete smooth spacelike maximal stationary graph section with included compact boundary $S$. Its boundary convention includes a smooth positive induced metric up to $S$. The future unit normal, lapse and shift use $N=-g_q(T,n)$ and $X=T-Nn$. [pthm-complete-maximal-slices](item-pthm-complete-maximal-slices) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F7] The supplied Harrison construction gives a smooth Lorentzian metric on the exterior and an open neighborhood of $S$. Its algebra theorem gives stationarity, $\mathcal L_Tg_q=0$. [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum) [pthm-harrison-lorentzian-algebra](item-pthm-harrison-lorentzian-algebra)

[F8] For the same complete maximal stationary graph section, the ADM theorem gives temporal section time $v=v_q$ on the exterior and the positive interior lapse in the stationary decomposition $T=Nn+X$. The section-time definition identifies the exterior with $\mathbb R_v\times\Sigma^\circ$ and its translated section interiors with $v$-levels. [pthm-adm-temporality](item-pthm-adm-temporality) [def-stationary-section-time](item-def-stationary-section-time)

[F9] On a compact smooth intrinsic boundary-distance collar in a smooth stationary geometry, if $N>0$ inside, $N=0$ on $S$, $T|_S\in TS$, and the lapse, normal and shift have their stationary extensions, the compact normal-flow lemma supplies one common smooth flow $\Psi_z$ of $V=Nn=T-X$ for all sufficiently small $|z|$, fixing $S$ and taking interior points to $v=z$. [lem-author-594d78e425ed-compact-normal-flow-and-area-distortion](item-lem-author-594d78e425ed-compact-normal-flow-and-area-distortion)

## Proof

**Given:** The construction, collar and sufficiently late target in the Statement, and $\epsilon>0$.

**Goal:** Construct the stated region and prove its boundary and area properties.

1.1 Choose the supplied section at this fixed $q>0$ from the maximal-slice family, taking any lower parameter bound strictly between zero and $q$. Thus the same section is a complete smooth spacelike maximal stationary graph, as required by the ADM theorem. The original maximal-section, mass-one, regular-vacuum and $T|_S\not\equiv0$ hypotheses are exactly the standing hypotheses, and ZFC supplies its choice convention. Apply [F8] to obtain temporal $v$ and $N>0$ in the interior. The metric and section are smooth up to $S$ by [F6] and [F7], so their normal, lapse and shift extend smoothly there. Regularity makes $T$ tangent to both transversely intersecting horizon branches, hence to their intersection $S$. Since $TS\subset T\Sigma$ is orthogonal to $n$, $N=-g_q(T,n)=0$ on $S$ and $X|_S=T|_S\in TS$. Stationarity of $g_q$ and the section-time conventions provide the stationary extensions to the translated section interiors. [given, A1, F1, F6, F7, F8]

2.1 The given sufficiently small smooth distance collar is a compact boundary-distance collar in this smooth stationary geometry, with $\rho$ equal to intrinsic distance and a slightly larger smooth collar available. Step 1.1 supplies $N>0$ inside, $N=0$ at $S$, tangency of $T$ to $S$, and stationary extensions. The section-time product and $Tv=1$ are those of [F8]. Thus every hypothesis of [F9] holds. Apply it to obtain a common smooth normal flow on $\mathcal R$, fixing $S$ and with $v(\Psi_zx)=z$ for interior $x$, for all sufficiently small $|z|$. Restrict its common interval to $|z|\le2\delta$ for all sufficiently small $\delta>0$. Its interior trajectories stay in the exterior. This supplies the flow and its boundary extension required by the truncated-height definition without assuming them from the height theorem. [given, F1, F8, F9, step 1.1]

2.2 The fixed positive $q$, original maximal exterior section, $T|_S\not\equiv0$, supplied complete smooth maximal section and sufficiently small distance collar are the standing data of localization, the endpoint theorem and the height result. The sufficiently late target is chosen to meet their late-target thresholds before it is fixed, independently of $\epsilon$. Localization supplies the compact zero-time cut $D$ in the collar. Apply the endpoint theorem to that $D$ and the same $C$ to obtain its maximal past null-normal family, compact Borel $A\subset C$ and endpoint map $F:A\to D$ with local smooth extensions. [given, A1, F1, F4, step 1.1]

3.1 For these same section, collar and target data, temporal $v$ from step 1.1 and the common boundary-fixing normal flow from step 2.1 meet the inputs of the truncated-height definition. With the sufficiently late target fixed independently of $\epsilon$, apply the height result [F5] for a suitable sufficiently small $\delta>0$ in the common flow interval. It gives the truncated supremum height $u$, Lipschitz with the two constant boundary neighborhoods, and identifies its zero-time endpoint data with those in step 2.2. This supplies the height and maximal-family endpoint construction for [F2], whose own conclusion selects a suitable height parameter for each $\epsilon$. [given, A1, F1, F4, F5, step 1.1, step 2.1, step 2.2]

4.1 Apply the coarea-smoothing result with the given $\epsilon$ to the fixed section, compact smooth collar and late target, its induced metric $h_0$, the height construction in step 3.1 and the endpoint data in step 2.2. Its own interface chooses a sufficiently small height parameter for this $\epsilon$. It gives a smooth compact sublevel region $\Omega_\epsilon\subset\mathcal R$ and regular interior level $D_\epsilon$, with boundary $S\sqcup D_\epsilon$ and $|D_\epsilon|_{h_0}\le|C|+\epsilon$. [given, F2, F3, step 2.2, step 3.1]

5.1 Since $\mathcal R\subset\Sigma$ and $D_\epsilon$ is an interior level separating its boundary components, $D_\epsilon$ lies between $S$ and $S_\eta$; the same supplier gives smoothness, closedness and possible disconnectedness. The induced $h_0$ area on $D_\epsilon$ is its fixed-$q$ spacetime-induced area, while $|C|$ uses the induced metric on $C$. Thus the inequality is exactly the asserted one. [step 4.1, F2, F3] ∎

## Source notes

The article citation is attribution only. The proof uses the completed conditional smoothing result, whose own argument supplies the Lipschitz level estimate, endpoint Jacobian bound and regular-level selection; it does not assume the article's conclusion as a premise.
