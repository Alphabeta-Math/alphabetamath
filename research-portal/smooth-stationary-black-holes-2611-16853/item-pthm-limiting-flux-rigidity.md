---
title: "Corollary 4.1: area and pointwise limiting flux rigidity"
status: draft
research_item: pthm-limiting-flux-rigidity
dependency_level: 34
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 1, 7, 27; Abstract, §1.4, Corollary 4.1 and proof
      attribution: In the mass-one limit the bifurcation-sphere area is 4π, the
        electric density is 1 and the magnetic density is 0 pointwise; the proof
        combines area bounds, limiting stability energy and electric flux.
      hypotheses: The article's regular stationary vacuum construction, original
        maximal exterior section, mass-one normalization and nontrivial
        stationary field on the bifurcation sphere.
      reading_limits: Historical reading note retained from the current source; this
        maintenance revision claims no fresh article or external full-text
        reading. The frozen article extraction and supplied claim were read for
        attribution. This citation is not used as a proof premise.
---

PDF p. 1: ` Abstract `; PDF p. 7: ` §1.4 `; PDF p. 27: ` Corollary 4.1 and proof `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-horizon-flux-and-stability-notation](item-def-horizon-flux-and-stability-notation)
- [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)
- [pthm-bifurcation-area-upper-bound](item-pthm-bifurcation-area-upper-bound)
- [pthm-bifurcation-area-lower-bound](item-pthm-bifurcation-area-lower-bound)
- [pthm-stable-bifurcation-mots](item-pthm-stable-bifurcation-mots)
- [pthm-stable-horizon-area-charge](item-pthm-stable-horizon-area-charge)
- [pthm-harrison-flux](item-pthm-harrison-flux)
- [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum)
- [lem-compact-flux-equality-input](item-lem-compact-flux-equality-input)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)


## Statement

Adopt the regular non-degenerate stationary vacuum construction, with its original exterior section spacelike and maximal, ADM mass one and stationary Killing field $T$ not identically zero on the bifurcation sphere $S$. Use the single primitive and regular Harrison family $g_q,F_q$, $0\le q\le1$, supplied in this construction, with the mass-one end normalization required by the Harrison flux theorem. Work in ZFC. Orient $S$ by the outward end-sphere convention and set $\gamma_q=g_q|_{TS}$ and $d\mu_q=d\mu_{\gamma_q}$. Define $e_q,b_q$ by $(\star_{g_q}F_q)|_{TS}=e_q\,d\mu_q$ and $F_q|_{TS}=b_q\,d\mu_q$. Then

$$|S|_{g_0}=4\pi,\qquad e_0=1,\qquad b_0=0$$

pointwise on $S$. The area radius, defined as $\sqrt{|S|_{g_0}/(4\pi)}$, is therefore one. Moreover $\int_S(e_0^2+b_0^2)\,d\mu_0\le4\pi$ and $\int_Se_0\,d\mu_0=4\pi$.

## Facts & Assumptions

[A1] The stationary vacuum model, regular spacetime, maximal section and mass-one convention are specified by [post-stationary-vacuum-model](item-post-stationary-vacuum-model), [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime), [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) and [def-harrison-normalization](item-def-harrison-normalization). ZFC includes [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice).

[F1] The upper area theorem gives $|S|_{g_0}\le4\pi$; the lower area theorem gives $|S|_{g_q}\ge4\pi(1-q^2)$ for sufficiently small $q>0$. [pthm-bifurcation-area-upper-bound](item-pthm-bifurcation-area-upper-bound) [pthm-bifurcation-area-lower-bound](item-pthm-bifurcation-area-lower-bound)

[F2] The regular Harrison result gives a jointly smooth metric family on a neighborhood of the fixed sphere and a two-form family continuous in $q$ and smooth in spacetime. [pthm-harrison-electrovacuum](item-pthm-harrison-electrovacuum) For $q\in(0,1]$, the spacelike section supplied by the stable-bifurcation result makes $\gamma_q$ Riemannian; at $q=0$, the upper-area interface treats $S$ as spacelike, so $\gamma_0$ is Riemannian as well. [pthm-stable-bifurcation-mots](item-pthm-stable-bifurcation-mots) [pthm-bifurcation-area-upper-bound](item-pthm-bifurcation-area-upper-bound) The horizon and surface conventions define the positive area form and the two density ratios in the Statement. [def-horizon-flux-and-stability-notation](item-def-horizon-flux-and-stability-notation) [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)

[F3] For each $q\in(0,1]$, the stable-bifurcation result supplies an individually admissible maximal section and a smooth spacelike extension across $S$, in which the compact sphere has an outward normal-graph tube. These are precisely the section, extension and tube hypotheses of the stable-horizon result, which gives $\int_S(e_q^2+b_q^2)\,d\mu_q\le4\pi$ for this $q$. [pthm-stable-bifurcation-mots](item-pthm-stable-bifurcation-mots) [pthm-stable-horizon-area-charge](item-pthm-stable-horizon-area-charge)

[F4] With the stated primitive, end normalization and orientation, the Harrison flux theorem gives $\int_Se_q\,d\mu_q=4\pi\sqrt{1-q^2}$ and $\int_Sb_q\,d\mu_q=0$. [pthm-harrison-flux](item-pthm-harrison-flux) [def-horizon-flux-and-stability-notation](item-def-horizon-flux-and-stability-notation)

[F5] On a fixed compact oriented surface, the compact-flux lemma gives convergence of area and of the flux and squared-density integrals under uniform convergence of Riemannian metrics and their associated restricted two-forms. It also proves pointwise $e=1$, $b=0$ when area and electric flux are both $4\pi$ and the squared-density integral is at most $4\pi$. [lem-compact-flux-equality-input](item-lem-compact-flux-equality-input)

[F6] The Lorentzian Hodge-calculus lemma gives $(\star_gF)_{ab}=\tfrac12(\mathrm{vol}_g)_{abcd}F^{cd}$ in a positively oriented four-dimensional chart, with both indices of $F$ raised by $g^{-1}$. The volume form uses the metric and the fixed spacetime orientation. [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

## Proof

**Given:** The construction and hypotheses in the Statement.

**Goal:** Prove the limiting area, flux identities, and pointwise rigidity.

**Proof technique:** direct.

1.1 Let $q_j\in(0,1]$ decrease to zero. On the compact fixed sphere, the metric regularity in [F2] gives uniform convergence $\gamma_{q_j}\to\gamma_0$. In local positively oriented coordinates the component formula in [F6] expresses the Hodge star algebraically in the metric, its inverse and the oriented volume density. Since the limiting Lorentzian metric is nondegenerate, the same regularity and continuity give uniform convergence of the restricted forms $F_{q_j}|_{TS}$ and $(\star_{g_{q_j}}F_{q_j})|_{TS}$ to their $q=0$ counterparts. The convergence assertion of [F5] therefore applies to area, flux and squared-density integrals. [given, F2, F5, F6]

2.1 Passing to the limit in the lower area bound of [F1] gives $|S|_{g_0}\ge4\pi$; its upper bound gives the reverse inequality. Thus $|S|_{g_0}=4\pi$. For each $q_j\in(0,1]$, use its section, extension and tube from [F3] to obtain the stable-horizon estimate. Passing to the limit with step 1.1 gives $\int_S(e_0^2+b_0^2)\,d\mu_0\le4\pi$. Likewise [F4] and step 1.1 give $\int_Se_0\,d\mu_0=4\pi$ and $\int_Sb_0\,d\mu_0=0$. [F1, F3, F4, step 1.1, algebra]

3.1 The sphere is compact, connected, oriented and smooth; $d\mu_0$ is a smooth positive measure and $e_0,b_0$ are continuous. The equality assertion of [F5], with the three integral conditions from step 2.1, gives $e_0=1$ and $b_0=0$ at every point. Equivalently, expansion of the nonnegative integrand gives $0\le\int_S((e_0-1)^2+b_0^2)\,d\mu_0\le4\pi-8\pi+4\pi=0$. The area-radius definition and $|S|_{g_0}=4\pi$ give radius one. [F2, F5, step 2.1, algebra] ∎

## Source notes

The article citation attributes the preserved claim. The proof uses the listed completed suppliers and does not use the article's corollary as a premise.
