---
title: General stationary vacuum black-hole uniqueness conjecture
status: draft
research_item: op-black-hole-uniqueness-conjecture
dependency_level: 6
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 1, §1.1; p. 4, Theorem 1.1; p. 5, §1.3
      statement: The article states the general stationary vacuum black-hole
        uniqueness conjecture, claims a conditional smooth non-degenerate single
        rotating-horizon result, and identifies smooth degenerate rotating and
        multiple-horizon questions.
      hypotheses: The general opening uses the informal word regular; Theorem 1.1 uses
        Definition 1.1, nonzero restriction of the stationary field to the
        bifurcation sphere, and the stated maximal-slice condition. Section 1.3
        discusses I+-regular smooth vacuum spacetimes.
      reading_limits: The frozen article text at the cited pages was read for
        formulation, attribution and reported status. The article's proofs and
        cited literature were not independently checked; its claimed result is
        not used as a premise.
---

PDF p. 1: ` §1.1, opening conjecture `; PDF p. 4: ` Theorem 1.1 `; PDF p. 5: ` §1.3, degenerate horizons and multiple black holes `

## Prerequisites

- [def-kerr-metric](item-def-kerr-metric)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Open problem

The article asks whether the domain of outer communications of every regular, four-dimensional, asymptotically flat stationary vacuum black hole is isometric to a Kerr exterior. Its opening does not give a single precise definition of regularity for this general question. In particular, the non-degenerate Definition 1.1 below is not imposed on the whole conjecture.

A precise version of the question is: for smooth, time-oriented four-dimensional vacuum data $(M,g,T)$ that are $I^+$-regular relative to a specified asymptotically flat end and satisfy the black-hole hypothesis specified below, must the corresponding domain of outer communications be isometric to one of the Kerr exteriors with $M_{\rm Kerr}>0$ and $|a|\leq M_{\rm Kerr}$? Here $\operatorname{Ric}(g)=0$ is the vacuum equation and $T$ is a stationary Killing field, meaning $\mathcal L_Tg=0$ and $T$ is future timelike on the specified stationary end. The $I^+$-regularity conditions, including complete $T$, global hyperbolicity of the exterior and the specified horizon cross-section conditions, are exactly those of [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data). For this precise question, define the black-hole region relative to the selected end by $\mathcal B:=M\setminus I_M^-(M_{\rm ext})$ and require $\mathcal B\ne\varnothing$, with $M_{\rm ext}$ and chronology as specified below. This is an end-relative convention using chronology in $M$; a conformal completion is not part of these data. The question makes no separate connectedness, analyticity or horizon non-degeneracy assumption.

For the end-generated spacetime region $M_{\rm ext}$ specified in that definition, the exterior is $I_M^+(M_{\rm ext})\cap I_M^-(M_{\rm ext})$: $I_M^+(U)$ consists of points reached from $U$ by future-directed timelike curves and $I_M^-(U)$ consists of points from which such a curve reaches $U$. An isometry is a diffeomorphism pulling the Kerr metric back to $g$ on the exterior. The Kerr metric and its exterior are those of [def-kerr-metric](item-def-kerr-metric). The causal-set conventions are those of [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data). Work in ZFC, including choice, as in the cited geometric interfaces. This precise version is a formulation of the broad question, not a claim that the article equates its informal regularity with $I^+$-regularity.

## Status

As of the article dated 12 November 2026, the general question is presented as a conjecture. The article claims that, for the regular non-degenerate stationary vacuum data of its Definition 1.1, if $T$ is not identically zero on the bifurcation sphere and the specified portion of $\Sigma_0$ is maximal, the exterior is isometric to a subextremal Kerr exterior with $0<|J|<M^2$. The precise definition is recorded in [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime); maximal means that the mean curvature of the spacelike hypersurface vanishes, as in [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data). This is a reported conditional claim, not a proof or an assumption in the question above.

The article separately identifies uniqueness for a smooth rotating degenerate horizon without analyticity, and the existence or exclusion of multiple horizons in the smooth $I^+$-regular vacuum setting, as questions of interest. A degenerate Killing horizon has vanishing surface gravity in the stated horizon convention; multiple horizons mean multiple horizon components. The comparison interface specifies surface gravity and the distinction between connected and disconnected horizons. No resolution or independent acceptance of the article's claimed partial result is asserted here.

## Source notes

The cited article supplies attribution and its stated 2026 status only. The open question is not a logical supplier for any theorem.
