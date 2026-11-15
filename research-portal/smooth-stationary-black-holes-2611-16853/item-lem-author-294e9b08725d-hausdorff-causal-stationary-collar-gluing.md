---
title: Strongly causal complete stationary ambient gluing around the exterior
status: published
research_item: lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing
dependency_level: 14
sources:
  references: []
---

## Prerequisites

- [lem-author-294e9b08725d-abstract-complete-boost-band](item-lem-author-294e9b08725d-abstract-complete-boost-band)
- [thm-author-294e9b08725d-radu-local-bifurcate-collar-input](item-thm-author-294e9b08725d-radu-local-bifurcate-collar-input)
- [lem-author-294e9b08725d-canonical-double-stationary-realization](item-lem-author-294e9b08725d-canonical-double-stationary-realization)
- [lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar)
- [lem-author-294e9b08725d-regular-positive-stationary-mass](item-lem-author-294e9b08725d-regular-positive-stationary-mass)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity)
- [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions)
- [physics:thm-gr-smooth-cauchy-temporal-splitting](https://alphabetamath.cc/physics/item/thm-gr-smooth-cauchy-temporal-splitting)
- [physics:lem-gr-maximal-geodesics-and-extension](https://alphabetamath.cc/physics/item/lem-gr-maximal-geodesics-and-extension)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [math:thm-flowout-theorem](https://alphabetamath.cc/item/thm-flowout-theorem)
- [physics:lem-gr-finite-smooth-volume-density](https://alphabetamath.cc/physics/item/lem-gr-finite-smooth-volume-density)
- [physics:thm-gr-volume-time-function](https://alphabetamath.cc/physics/item/thm-gr-volume-time-function)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in ZFC. Let $(M,g,T,M^{\rm end},\Sigma_0,S)$ satisfy the regular non-degenerate stationary-vacuum definition, and write $E=I^-_M(M^{\rm end})\cap I^+_M(M^{\rm end})$ for its original exterior. Use the working partial-Cauchy collar and the positive-mass result for these data to meet the local boost input's GR and SBS hypotheses. Let $C_0$ be the canonical exterior Cauchy section, let $(\widehat M,\widehat g,\widehat T)$ be its compatible globally hyperbolic doubled realization, and let $\mathcal B=\{(U,V,p)\in\mathbb R^2\times S:|UV|<\delta^2\}$ be the corresponding complete abstract boost band, for sufficiently small $\delta>0$. Glue its right wedge $U,V>0$ to the proper stationary collar in $E$ by their common stationary coordinates. The resulting space $M_*$ is a smooth Hausdorff time-oriented vacuum spacetime containing $E$ and a neighborhood of $S$. Its stationary field is complete. The maps from the band and $E$ to $\widehat M$ combine to a global local isometry, and $M_*$ is stably causal and strongly causal. The section $C_0\cup S$ is connected, closed and acausal in $M_*$. Stable causality has the strictly-wider-causal-metric meaning of the causal exterior interface; strong causality and temporal functions have the causal-conditions interface's meanings. No injective embedding of all of $M_*$ into $\widehat M$ is asserted.

## Statement references

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar)

[lem-author-294e9b08725d-regular-positive-stationary-mass](item-lem-author-294e9b08725d-regular-positive-stationary-mass)

[lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice)

[lem-author-294e9b08725d-canonical-double-stationary-realization](item-lem-author-294e9b08725d-canonical-double-stationary-realization)

[lem-author-294e9b08725d-abstract-complete-boost-band](item-lem-author-294e9b08725d-abstract-complete-boost-band)

[thm-author-294e9b08725d-radu-local-bifurcate-collar-input](item-thm-author-294e9b08725d-radu-local-bifurcate-collar-input)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

**Given:** The regular stationary-vacuum data, the original exterior $E$ and bifurcation sphere $S$, and the compatible working collar, canonical section $C_0$, doubled realization and boost band specified in the Statement; the ambient set theory is ZFC.

**Goal:** Construct the asserted ambient spacetime with complete stationary flow and the stated causal and section properties.

[F1] The abstract band has complete action and a compatible local-isometry map. [lem-author-294e9b08725d-abstract-complete-boost-band](item-lem-author-294e9b08725d-abstract-complete-boost-band)

[F2] The source right stationary collar is embedded and its $r\downarrow0$ end escapes all compact subsets of the quotient. [thm-author-294e9b08725d-radu-local-bifurcate-collar-input](item-thm-author-294e9b08725d-radu-local-bifurcate-collar-input)

[F3] The exterior embeds equivariantly into the globally hyperbolic realization, with its section in the doubled Cauchy hypersurface. The canonical section is connected, has closure $C_0\cup S$, and equals $U=V>0$ near $S$. [lem-author-294e9b08725d-canonical-double-stationary-realization](item-lem-author-294e9b08725d-canonical-double-stationary-realization) [lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice)

[F4] The regular definition supplies the smooth time-oriented Ricci-flat four-dimensional geometry, future stationary end with the stated differentiated decay, globally hyperbolic exterior, complete exterior stationary orbits meeting the original section, and smooth transverse nonexpanding horizons tangent to $T$ (SBS). The working spacetime $M'$ preserves $E$, the end and horizon germs, and supplies an acausal edgeless section $\Sigma'$ with $\Sigma'\cap I^+_{M'}(M^{\rm end})=\Sigma'\cap I^-_{M'}(M^{\rm end})=\Sigma_0\cap E$. The positive-mass result supplies the additional GR condition $M_0>0$. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar) [lem-author-294e9b08725d-regular-positive-stationary-mass](item-lem-author-294e9b08725d-regular-positive-stationary-mass)

[F5] Stable causality means existence of a smooth Lorentzian metric with strictly wider cones, the same time orientation, and no closed causal curve. Strong causality means existence of arbitrarily small open causally convex neighborhoods. Temporal functions have past timelike gradient. A temporal function strictly increases along every future causal curve and forbids closed causal curves. All these are mathematical conditions on the metric. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity) [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions)

[F6] On a nonempty time-oriented smooth Lorentzian four-manifold, the finite-density lemma supplies a positive smooth density with total measure one, positive measure on nonempty open sets and zero measure on chart-Lebesgue-null Borel sets. Under global hyperbolicity the volume-time theorem applies to that measure, and the smooth Cauchy temporal splitting theorem applies to the resulting volume time. This gives a global Cauchy temporal function and a complete future timelike field $X$ whose temporal derivative is one. Transverse flowouts of an embedded hypersurface give local smooth product charts. Cauchy sets are acausal. Smooth maps preserve local absolute continuity of curves and obey the almost-everywhere velocity chain rule. [physics:lem-gr-finite-smooth-volume-density](https://alphabetamath.cc/physics/item/lem-gr-finite-smooth-volume-density) [physics:thm-gr-volume-time-function](https://alphabetamath.cc/physics/item/thm-gr-volume-time-function) [physics:thm-gr-smooth-cauchy-temporal-splitting](https://alphabetamath.cc/physics/item/thm-gr-smooth-cauchy-temporal-splitting) [math:thm-flowout-theorem](https://alphabetamath.cc/item/thm-flowout-theorem) [physics:lem-gr-maximal-geodesics-and-extension](https://alphabetamath.cc/physics/item/lem-gr-maximal-geodesics-and-extension) [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[F7] The working-collar supplier's Proof 1.1 and 2.1 construct a thin timelike flowout $O_0$ of an annular collar in the original radial section and set $M'_0=E\cup O_0$. Its Proof 2.1 excludes causal relations in either direction between $E$ and the inner section collar or $S$. Its Proof 5.1 gives both chronological section equalities, the unchanged exterior, and the horizon germs by local one-sided timelike access through $E$. The transverse flowout theorem permits an embedded flowout with time fibers that are intervals containing zero, inside any prescribed open neighborhood of the section. [lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar) [math:thm-flowout-theorem](https://alphabetamath.cc/item/thm-flowout-theorem)

[A1] Work in ZFC, including the Axiom of Choice. In particular Countable Choice and Dependent Choice hold for the finite-density, volume-time, smooth-temporal, flowout and causal-curve suppliers. Retain the same choice convention for the canonical doubled realization and abstract band. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

## Proof

1.1 First orient $E$, without using the boost collar or doubled realization. Apply the finite-density, volume-time and smooth-temporal inputs successively to $E$: it is a nonempty smooth time-oriented globally hyperbolic four-manifold, [A1] supplies their choice hypotheses, and the density satisfies the three measure conditions required by the volume-time theorem. The resulting complete future timelike field $X$ has temporal derivative one. Its flow lines have no endpoint in $E$, since the temporal function tends to the two infinities on them, so each meets the original Cauchy section $C=\Sigma_0\cap E$ exactly once. Transversality, flow uniqueness and completeness make the flowout map $\mathbb R\times C\to E$ a bijective local diffeomorphism, hence a diffeomorphism. Orient $C$ by the original radial chart of $\Sigma_0$ and give $E$ the transported product orientation, with the future time direction first. Along $C$ this is precisely its future-normal orientation: any future timelike transverse vector differs from a positive multiple of the future normal by a tangent vector. [F4, F6, A1]

2.1 Use the concrete working construction in [F7]. Choose a smaller open annular collar $A\subset\Sigma_0$ of $S$, with compact closure inside the original annular collar, and its future timelike flowout $H(s,a)$ with $|s|<\epsilon(a)$ and image $O\subset O_0$, where $\epsilon$ is positive and smooth. This is the transverse flowout theorem applied to the same future timelike field, restricted inside $M'_0$. Orient $O$ by the radial orientation on $A$ and the increasing future time coordinate. For $H(s,a)\in O\cap E$, [F7] forces $a$ to be on the outer part $A\cap C$: an inner or $S$ base point would be causally related to $E$. The whole flow segment between $a$ and $H(s,a)$ lies in $E$. Indeed both endpoints have timelike connections to and from the end, so concatenating those connections with subsegments of this timelike flow gives both end connections at each intermediate point. At $s=0$ the two orientations agree by step 1.1; the sign comparing two smooth orientations is constant along this connected segment in $O\cap E$. They therefore agree on every component of the overlap, and define an orientation on $M'=E\cup O$. [F4, F7, F6, A1, step 1.1]

3.1 Verify that this restriction still supplies the working data. Its section is $\Sigma'=C\cup A=\Sigma'_0\cap M'$, so smoothness, spacelikeness, closedness and acausality are inherited from the original working section, and edgelessness is local and persists on this open restriction. The inner annulus has the same open radial topology after reparametrization. No new chronological connections can appear because $M'\subset M'_0$. Every point of $E$ retains both end connections inside $E$: given end paths to and from that point, each intermediate point on either path has both end connections by timelike concatenation. Thus $E$ is still the exterior in $M'$ and $\Sigma'\cap I^+_{M'}(M^{\rm end})=\Sigma'\cap I^-_{M'}(M^{\rm end})=C$. The open set $O$ contains a neighborhood of all of $S$. The local one-sided timelike access through $E$ used in [F7] remains available after this restriction, by taking its short local segments inside $O$ and its end paths inside $E$. Hence the original two horizon germs and their transverse nonexpanding intersection are retained. The restricted metric and field retain the vacuum equation, end decay and completeness of stationary orbits in the whole $E$. Together with the orientation in step 2.1 and the positive mass $M_0>0$ from [F4], these are the required GR and SBS data. Only now invoke the local boost input and the compatible canonical splice, doubled realization and band for these same data. [F1, F2, F3, F4, F7, F6, A1, step 1.1, step 2.1]

4.1 The right wedge and the source collar have the same complete stationary coordinates, so the gluing map is a diffeomorphism and the metrics and fields agree. To check Hausdorffness, only a sequence in the common wedge approaching a non-right-wedge band point could have a second limit in $E$. Such an approach has $r=\sqrt{UV}\to0$. If its exterior images converged in $E$, their quotient images would lie in a compact set, contradicting the quotient-escape assertion. The outer cutoff $|UV|=\delta^2$ is excluded from the band, so it introduces no second limit point. The graph of the identification therefore has no pair of distinct limits in the two pieces, and the gluing is Hausdorff. The images of countable bases of the two open pieces form a countable base. The ordinary gluing charts give the smooth manifold and the common vacuum metric. [F1, F2, F3, step 3.1, algebra]

5.1 The maps to $\widehat M$ agree on the overlap by equivariance and their common local germ. They define a smooth global local isometry $F_*:M_*\to\widehat M$ and the pulled-back time orientation. Completeness of the stationary field follows from the compatible complete actions on the two invariant open pieces: a point in either piece has its entire real-parameter orbit there, and the actions agree on the overlap. The band supplier already provides a smooth Cauchy temporal function $\widehat\tau$ on $\widehat M$; use that same ambient function on both pieces. Its construction is the finite-density, volume-time and smooth-temporal chain in [F6], with nonemptiness supplied by $S$ and choice supplied by [A1]. Its pullback $\tau=\widehat\tau\circ F_*$ has past timelike gradient because $F_*$ is a time-orientation-preserving local isometry. [F1, F2, F3, F5, F6, A1, step 4.1, algebra]

6.1 Write $g_*$ for the glued metric and set $q=g_*^{-1}(d\tau,d\tau)<0$ and $g'=g_*-d\tau\otimes d\tau$. In the $g_*$-orthogonal decomposition $\mathbb R\nabla\tau\oplus\ker d\tau$, the second summand stays positive definite and the value on $\nabla\tau$ changes from $q$ to $q-q^2<0$; thus $g'$ is smooth Lorentzian. For every nonzero $g_*$-causal vector $v$, the temporal pairing result gives $d\tau(v)\ne0$, so $g'(v,v)=g_*(v,v)-d\tau(v)^2<0$. Any future $g_*$-timelike orientation field remains $g'$-timelike. Also $g'^{-1}(d\tau,d\tau)=q/(1-q)<0$, and $d\tau$ is positive on that orientation field, so $\tau$ is temporal for $g'$ as well. Apply the temporal monotonicity lemma to $g'$ to exclude all closed $g'$-causal curves. This is exactly the wider-metric certificate for stable causality. [F5, A1, step 5.1, algebra]

6.2 Check strong causality directly, including possible multiple sheets of $F_*$. Given $x\in M_*$ and an open neighborhood $O$ of $x$, choose an open $W\subset O$ on which $F_*$ is a diffeomorphism to an open neighborhood of $F_*(x)$. Global hyperbolicity of $\widehat M$ includes strong causality, so choose an open causally convex $V$ with $F_*(x)\in V\subset F_*(W)$. Put $U=(F_*|_W)^{-1}(V)$. If a future causal curve has two points in $U$, its intervening image under $F_*$ is a future causal curve by the smooth-composition chain rule and local isometry, and lies entirely in $V$. The inverse in $W$ lifts that image on the whole intervening interval. It agrees with the original curve at the initial point; their equality set is open by local injectivity of $F_*$ and closed by Hausdorffness, hence is the entire interval. The curve therefore stays in $U$. This gives arbitrarily small open causally convex neighborhoods as required. [F3, F5, F6, A1, step 4.1, step 5.1]

7.1 The restriction of $F_*$ to $C_0\cup S$ is injective and has image in the doubled Cauchy hypersurface. That hypersurface is acausal by the Cauchy-set input, so any causal curve between distinct section points would give a causal curve between distinct points of it, a contradiction. The right collar has no extra intersections with $C_0$: a nonzero stationary translate of its canonical section is a timelike pure-boost translate of a circle translate in the same canonical section, contradicting acausality of $C_0$ in $E$; omit the circle in the nonrotating case. Indeed the pure boost is timelike near the outward canonical section and remains so on its full band orbit by boost invariance. Thus in the band the section has exactly the equation $U=V\ge0$. It is closed there, while $C_0$ is closed in $E$; closedness in this open cover proves closedness in $M_*$. Finally $C_0$ is connected and $S$ is in its closure, so $C_0\cup S$ is connected. This retains the claimed section and all ambient conclusions without asserting global injectivity of $F_*$. [F1, F2, F3, F6, A1, step 5.1, step 6.2, algebra] ∎
