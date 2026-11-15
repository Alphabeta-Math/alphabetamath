---
title: Divergence comparison between S and the translated causal cut
status: published
research_item: pthm-distance-divergence-area-comparison
dependency_level: 32
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 26, proof of Theorem 4.1, divergence display and the limits
        epsilon down to zero, then eta down to zero
      attribution: The passage integrates $\nabla\rho$ over $\Omega^\epsilon$ and
        displays
        $|S|=\int_{D^\epsilon}h(\nabla\rho,\nu)\,d\mu-\int_{\Omega^\epsilon}\Delta\rho\,dV\le|D^\epsilon|+O(\eta)\le|C|+\epsilon+O(\eta)$.
        It then sends $\epsilon\downarrow0$ followed by $\eta\downarrow0$ to
        obtain $|S|_{g_q}\le|C_q|_{g_q}$.
      hypotheses: Standing regular stationary vacuum construction, original maximal
        section, mass one, rotating bifurcation sphere, fixed sufficiently small
        positive q and supplied smooth maximal section and smooth cuts.
      reading_limits: "Historical reading note retained from the current source; this
        maintenance revision claims no fresh article or external full-text
        reading. Consulted the frozen PDF image of p. 26 and the extracted text
        of Lemma 4.4 and the proof of Theorem 4.1 on pp. 25–26. Attribution
        only: this passage supplies the displayed divergence comparison and
        order of limits. It does not state the explicit uniform fixed-collar
        error contract or construct the normal-distance collar. Those parts of
        the present local proof use the declared mathematical collar and flux
        suppliers. No independent verification of other article results is
        claimed."
---

PDF p. 26: ` Proof of Theorem 4.1 `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets)
- [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)
- [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)
- [pthm-complete-maximal-slices](item-pthm-complete-maximal-slices)
- [pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation)
- [pthm-past-boundary-localization](item-pthm-past-boundary-localization)
- [pthm-smooth-area-controlled-cut](item-pthm-smooth-area-controlled-cut)
- [pthm-harrison-lorentzian-algebra](item-pthm-harrison-lorentzian-algebra)
- [lem-thin-collar-divergence-area-input](item-lem-thin-collar-divergence-area-input)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-60420990c802-uniform-inward-normal-exponential-collar](item-lem-author-60420990c802-uniform-inward-normal-exponential-collar)
- [lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance](item-lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance)
- [lem-author-60420990c802-bounded-distance-laplacian-and-collar-density](item-lem-author-60420990c802-bounded-distance-laplacian-and-collar-density)
- [lem-author-60420990c802-uniform-thin-collar-flux-comparison](item-lem-author-60420990c802-uniform-thin-collar-flux-comparison)
- [lem-author-60420990c802-isometric-target-area-and-vanishing-errors](item-lem-author-60420990c802-isometric-target-area-and-vanishing-errors)
- [pthm-coarea-sard-smoothing](item-pthm-coarea-sard-smoothing)
- [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)


## Statement

In the standing regular mass-one stationary vacuum Harrison construction, with original maximal outer section, $T|_S\not\equiv0$ and fixed sufficiently small positive $q$, let $\Sigma=\Sigma_{q,0}$ be the supplied complete smooth maximal section, with induced metric $h$, compact boundary $S$ and intrinsic boundary distance $\rho$. On a fixed sufficiently small smooth distance collar, the smooth comparison regions $\Omega_\epsilon\subset\{0\le\rho\le\eta\}$ supplied by the cut construction have boundary $S\sqcup D_\epsilon$ and satisfy
$$|S|=\int_{D_\epsilon}h(\nabla\rho,\nu)\,dA-\int_{\Omega_\epsilon}\Delta_h\rho\,dV\le|D_\epsilon|+O_q(\eta)\le|C_t|_{g_q}+\epsilon+O_q(\eta).$$
The fixed-collar error is uniform in the region, smoothing parameter and chosen late target. Sending $\epsilon\downarrow0$ and then $\eta\downarrow0$, with $q$ fixed, gives $|S|_{g_q}\le|C_q|_{g_q}$, since every stationary translate $C_t$ has the same area as $C_q$.

## Facts & Assumptions

[F1] Use the exact hypotheses and interface of [post-stationary-vacuum-model](item-post-stationary-vacuum-model).

[F2] Use the exact hypotheses and interface of [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime).

[F3] Use the exact hypotheses and interface of [def-harrison-normalization](item-def-harrison-normalization).

[F4] Use the exact hypotheses and interface of [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data).

[F5] Use the exact hypotheses and interface of [def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets).

[F6] Use the exact hypotheses and interface of [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres).

[F7] Use the exact hypotheses and interface of [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data).

[F8] Use the exact hypotheses and interface of [pthm-complete-maximal-slices](item-pthm-complete-maximal-slices).

[F9] Use the exact hypotheses and interface of [pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation).

[F10] Use the exact hypotheses and interface of [pthm-past-boundary-localization](item-pthm-past-boundary-localization).

[F11] Use the exact hypotheses and interface of [pthm-smooth-area-controlled-cut](item-pthm-smooth-area-controlled-cut).

[F12] Use the exact hypotheses and interface of [pthm-harrison-lorentzian-algebra](item-pthm-harrison-lorentzian-algebra).

[F13] Use the exact hypotheses and interface of [lem-thin-collar-divergence-area-input](item-lem-thin-collar-divergence-area-input).

[F14] Use the exact hypotheses and interface of [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice).

[F15] Use the exact hypotheses and interface of [lem-author-60420990c802-uniform-inward-normal-exponential-collar](item-lem-author-60420990c802-uniform-inward-normal-exponential-collar).

[F16] Use the exact hypotheses and interface of [lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance](item-lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance).

[F17] Use the exact hypotheses and interface of [lem-author-60420990c802-bounded-distance-laplacian-and-collar-density](item-lem-author-60420990c802-bounded-distance-laplacian-and-collar-density).

[F18] Use the exact hypotheses and interface of [lem-author-60420990c802-uniform-thin-collar-flux-comparison](item-lem-author-60420990c802-uniform-thin-collar-flux-comparison).

[F19] Use the exact hypotheses and interface of [lem-author-60420990c802-isometric-target-area-and-vanishing-errors](item-lem-author-60420990c802-isometric-target-area-and-vanishing-errors).

[F20] On the same localized collar and late target, coarea smoothing supplies $\Omega_\epsilon=\{u_i\le b\}$, preserving $u_i=-2\delta$ near $S$, with $b\in(-\delta,-\delta/2)$ and the stated boundary and area bound. [pthm-coarea-sard-smoothing](item-pthm-coarea-sard-smoothing)

[F21] For a smooth tensor field $B$ and the local flow $\Phi_t$ of a smooth vector field $X$, $\mathcal L_XB=0$ implies $\Phi_t^*B=B$ on every common local flow domain. [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)

## Proof

**Given:**The hypotheses in the Statement.

**Goal:** Establish the stated conclusions.

1.1 The maximal-section supplier gives the smooth spacelike section with included compact boundary $S$. Its induced metric is smooth and positive definite up to that boundary; the transformed horizon/metric supplier ensures the ambient smooth geometry there. Apply the first two new lemmas to this fixed $h$: the inward unit-normal exponential produces a compact Gaussian collar on which its coordinate equals intrinsic distance from $S$, even among paths allowed to leave the collar. Thus $\rho$ is smooth there and $|\nabla_h\rho|=1$. No global regularity of boundary distance or extension of stationary graph height is assumed. [given, F2, F4, F5, F8, F9, F15, F16]

2.1 The third new lemma gives fixed constants $C_q,K_q$ on that collar with $|\Delta_h\rho|\le C_q$ and product-volume density at most $K_q$. They depend on the fixed section and parameter, and remain valid when $\eta$ shrinks. Choose $\eta$ below this collar width. Use the localization and smooth-cut construction to fix a sufficiently late target $C_t$ and its localized data, independently of $\epsilon$. For each $\epsilon>0$, choose directly from the coarea-smoothing supplier a smooth compact sublevel region $\Omega_\epsilon=\{u_i\le b\}$ inside that collar, with boundary $S\sqcup D_\epsilon$ and $|D_\epsilon|\le|C_t|+\epsilon$. The same supplier preserves $u_i=-2\delta$ on a neighborhood of $S$ and gives $b\in(-\delta,-\delta/2)$. Since $-2\delta<b$, that neighborhood lies in $\Omega_\epsilon$, so the region contains the inward side of $S$, as required by the divergence input. [F10, F11, F13, F17, F20, step 1.1]

3.1 Apply the fourth new lemma, which matches all the divergence and density hypotheses established in steps 1.1 and 2.1. The outward unit normal at $S$ is $-\nabla\rho$, so the exact flux identity has the displayed minus sign on its volume integral. The outer flux is at most $|D_\epsilon|$, and its volume error is bounded by $C_qK_q\eta|S|$. Substituting the selected coarea-smoothing area bound proves $|S|\le|C_t|+\epsilon+C_qK_q\eta|S|$. This bound is uniform in $\epsilon$, the possible disconnectedness of $D_\epsilon$, and the late target. [F7, F13, F18, step 1.1, step 2.1]

4.1 The Harrison algebra supplier gives $\mathcal L_Tg_q=0$. Apply [F21] to the smooth tensor $g_q$ and vector field $T$ on the stationary end: on each common flow domain containing $C_q$, $(\phi_t^T)^*g_q=g_q$. The coordinate-sphere convention supplies the product-end flow $\phi_t^T(s,x)=(s+t,x)$ for every real $t$, so the comparison sphere is in such a domain for every selected $t$ and $C_t=\phi_t^T(C_q)$. Thus these translations satisfy the ambient isometry condition of the fifth new lemma. The fifth new lemma therefore gives $|C_t|_{g_q}=|C_q|_{g_q}$ exactly, for every selected $t$, including targets that move as $\eta$ shrinks. The collar and $C_q$ remain fixed at the chosen $q$. Let $\epsilon\downarrow0$ at each admissible $\eta$, then $\eta\downarrow0$ with the fixed constant $C_qK_q|S|$. The same lemma gives $|S|_{g_q}\le|C_q|_{g_q}$ as asserted. No uniform estimate as $q\downarrow0$ is needed for this fixed-$q$ conclusion. [F6, F12, F19, F21, step 3.1] ∎

## Source notes

The proof of Theorem4.1, original PDF p.26, attributes the flux identity and order of limits. The five local prerequisites supply a genuine intrinsic normal-distance collar, its unit gradient, bounded Laplacian and density, uniform thin-collar flux control, and stationary-isometry area invariance. The existing smooth-cut theorem supplies its coarea/Sard construction; coarea is not invoked afresh in the divergence step. No new external theorem is needed after the exact existing exponential, inverse-function, density and divergence suppliers and this five-item chain. This is proposed Step5 authoring, not independent proof review, mathematical acceptance or a claim about the separate $q=0$ limit.
