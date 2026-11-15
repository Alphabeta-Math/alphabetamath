---
title: Precise Rácz–Wald global collapse class
status: published
research_item: def-author-4cb89398a4ab-racz-wald-collapse-class
dependency_level: 5
sources:
  references:
    - title: Rácz–Wald, Global Extensions of Spacetimes Describing Asymptotic Final
        States of Black Holes
      url: https://arxiv.org/pdf/gr-qc/9507055
      locator: End of §2, printed/PDF pp. 8–9; Theorem 4.2, pp. 15–16; §5 opening
        paragraph, p. 17
      statement: For the exact end-of-§2 class stated here and nonzero constant
        surface gravity on N, the whole original spacetime admits an isometric
        extension in which N is a proper subset of a bifurcate Killing horizon;
        the original horizon-generating action extends and the extension can
        have a wedge-reflection isometry about the bifurcation surface.
      hypotheses: Smooth globally hyperbolic spacetime; smooth spacelike Cauchy
        surface with the single asymptotically stationary end of Chruściel–Wald
        Definition 2.1; nonempty black-hole region and empty white-hole region
        relative to its complete stationary action; connected Killing event
        horizon with compact intersection with the Cauchy surface; a globally
        defined one-parameter isometry group with horizon-normal generator,
        future directed there; nonzero constant surface gravity. No field
        equation is assumed.
      reading_limits: Read the independent PDF end-of-§2 class, Theorem 4.2 and its
        displayed construction, and §5 opening scope restriction; visually
        checked PDF pp. 8 and 15. The orbit-space lemmas and complete extension
        proof were not independently reconstructed or reviewed. The extension of
        additional tensor fields, vacuum equations, global hyperbolicity of the
        extension, and extension of the distinct stationary action are not
        claimed by this import.
---

## Prerequisites

- [def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end)
- [lem-author-4cb89398a4ab-end-coordinate-cones](item-lem-author-4cb89398a4ab-end-coordinate-cones)
- [lem-author-4cb89398a4ab-complete-end-saturation](item-lem-author-4cb89398a4ab-complete-end-saturation)
- [lem-author-4cb89398a4ab-chronological-equivariance](item-lem-author-4cb89398a4ab-chronological-equivariance)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [` Rácz–Wald, Global Extensions of Spacetimes Describing Asymptotic Final States of Black Holes · End of §2, printed/PDF pp. 8–9; Theorem 4.2, pp. 15–16; §5 opening paragraph, p. 17 `](https://arxiv.org/pdf/gr-qc/9507055)


## Definition

A **Rácz–Wald collapse-class datum** is a smooth globally hyperbolic spacetime $(M,g)$ with a smooth spacelike Cauchy surface $\Sigma=\Sigma_{\mathrm{end}}\cup\Sigma'$, satisfying the full end contract [def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end) for this single asymptotically flat end. Global hyperbolicity, spacelike and Cauchy are used as in [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data). In particular the coordinate-cone conclusions [lem-author-4cb89398a4ab-end-coordinate-cones](item-lem-author-4cb89398a4ab-end-coordinate-cones) hold, while the stationary generator $T$ has the complete action $\phi_u$ of [lem-author-4cb89398a4ab-complete-end-saturation](item-lem-author-4cb89398a4ab-complete-end-saturation). The remainder $\Sigma'$ is not assumed compact by this definition.

Using that stationary saturation, set $B=M\setminus I^-(M_{\mathrm{end}})$, $W=M\setminus I^+(M_{\mathrm{end}})$ and $N=\partial I^-(M_{\mathrm{end}})$ as in [lem-author-4cb89398a4ab-chronological-equivariance](item-lem-author-4cb89398a4ab-chronological-equivariance). Require $B\ne\varnothing$ and $W=\varnothing$ (equivalently $M=I^+(M_{\mathrm{end}})$).

Require $N$ to be a connected Killing horizon, with $N\cap\Sigma$ compact. More explicitly a second one-parameter group of isometries $\chi_u$ is defined on all of $M$ for every $u\in\mathbb R$, with Killing generator $\xi$ normal to $N$ and chosen future directed on its nonzero-generator part; use the horizon and signed-surface-gravity conventions of [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data). The groups $\chi$ and $\phi$ may differ. Completeness of $T$ never substitutes for the asserted completeness of $\xi$. No numerical normalization of $\xi$ and no nonzero or constant value of its surface gravity are imposed until a theorem requires them.

## Facts & Assumptions

[F1] The exact end contract and its cone and saturation consequences apply. [def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end) [lem-author-4cb89398a4ab-end-coordinate-cones](item-lem-author-4cb89398a4ab-end-coordinate-cones) [lem-author-4cb89398a4ab-complete-end-saturation](item-lem-author-4cb89398a4ab-complete-end-saturation)

[F2] The causal definitions and the chronological equivariance result give the stated meanings and the no-white-hole equivalence. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [lem-author-4cb89398a4ab-chronological-equivariance](item-lem-author-4cb89398a4ab-chronological-equivariance)

[F3] The horizon supplier defines normal Killing generators and their signed surface gravity. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[F4] The independent source specifies this conjunction at the end of §2; the distinct global group $\chi_u$ is expressly part of that contract.

## Justification

**Given:** The displayed metric, surface, end and actions satisfying the listed conditions.

**Goal:** Specify the complete input class used in the global extension theorem.

1.1 The end contract supplies coordinate and complete stationary-action data; its two local consequences distinguish the coordinate time direction from $T$ and define the invariant saturated end. The causal definitions then define $B,W,N$, and the no-white-hole identity is the set equality proved in the chronological lemma. [F1, F2]

2.1 The horizon supplier gives the meaning of the separate normal generator and scalar. Connectedness, compactness and existence of the second complete group are further hypotheses on the data; none is inferred from local stationarity. The conjunction therefore gives a precise, well-defined input class matching the source, without asserting that an arbitrary stationary horizon belongs to it. [F3, F4, step 1.1] ∎

## External input

The collapse-class restrictions are transcribed from Rácz–Wald, end of §2, pp. 8–9. Its observation that the asymptotic conditions could be weakened is not used to remove any of the stated hypotheses.
