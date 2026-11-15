---
title: Ionescu–Klainerman local Kerr criterion with full interface
status: draft
research_item: pthm-ik-local-kerr-criterion-input
dependency_level: 4
sources:
  references:
    - title: Ionescu–Klainerman, On the uniqueness of smooth, stationary black holes
        in vacuum
      url: https://arxiv.org/pdf/0711.0040
      locator: §1.2 AF, SBS, T, equations (1.4)–(1.7), printed pp. 6–7; Main Theorem,
        printed p. 8
      statement: Under AF, SBS and T the domain of outer communication E is locally
        isometric to the domain of outer communication of a Kerr spacetime with
        mass M and 0<a<M.
      hypotheses: Smooth time-oriented vacuum Einstein spacetime of dimension 3+1;
        connected orientable paracompact C∞ manifold without boundary, smooth
        Killing T; exact AF and SBS packages and technical identities
        (1.6)–(1.7), using the same supplied Ernst potential normalized to 1 at
        infinity along the t=0 spatial end of the AF section.
      reading_limits: Consulted the PDF text of §1.2 AF, SBS and T, equations
        (1.4)–(1.7), footnotes 4–6 and the Main Theorem on printed pp. 6–8,
        specifically rechecking the normalization paragraph before (1.6). This
        imports the theorem under its full hypotheses; no page-image inspection,
        reconstruction of its analytic proof, or independent proof review is
        claimed.
    - title: Ionescu–Klainerman, On the uniqueness of smooth, stationary black holes
        in vacuum
      url: https://arxiv.org/pdf/0711.0040
      locator: §8, Lemma 8.1 and (8.2), printed p. 41; sublevel definition and
        Propositions 8.2–8.3, printed p. 42; §8.2, printed pp. 48–49; completion
        (8.1)
      statement: Under the full setting of the Main Theorem, y has a constant value
        yS0 on S0, and UR is the unique sublevel component anchored at S0 for
        R>yS0. Proposition 8.2 supplies R1>yS0, and Proposition 8.3 gives S=0 on
        every UR for R≥R1. The completion proves 1−σ≠0 and S=0 on Σ0∩E.
      hypotheses: All AF, SBS and T assumptions, including normalization of the same
        supplied Ernst potential to 1 along the AF section, and all
        constructions and estimates of preceding sections, including the initial
        neighborhood of Proposition 6.1/8.2 and conditional continuation
        Proposition 8.5. This is not a statement for arbitrary smooth reciprocal
        potentials or stationary tensors.
      reading_limits: Consulted the PDF text of Lemma 8.1 and (8.2), the sublevel
        definition, Propositions 8.2–8.3 and the §8.2 completion at the listed
        locators, specifically checking the parameter ranges and
        denominator-zero exclusion. The analytic continuation result is
        imported; no page-image inspection, Carleman proof reconstruction, or
        independent proof review is claimed.
external_input: true
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)
- [physics:def-gr-fx-kerr-exterior](https://alphabetamath.cc/physics/item/def-gr-fx-kerr-exterior)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af)
- [def-author-9f9c6144aed8-ik-sbs](item-def-author-9f9c6144aed8-ik-sbs)
- [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)
- [lem-author-9f9c6144aed8-sublevel-path-exhaustion](item-lem-author-9f9c6144aed8-sublevel-path-exhaustion)
- [lem-author-9f9c6144aed8-stationary-zero-transport](item-lem-author-9f9c6144aed8-stationary-zero-transport)
- [` Ionescu–Klainerman, On the uniqueness of smooth, stationary black holes in vacuum · §1.2 AF, SBS, T, equations (1.4)–(1.7), printed pp. 6–7; Main Theorem, printed p. 8 `](https://arxiv.org/pdf/0711.0040)
- [` Ionescu–Klainerman, On the uniqueness of smooth, stationary black holes in vacuum · §8, Lemma 8.1 and (8.2), printed p. 41; sublevel definition and Propositions 8.2–8.3, printed p. 42; §8.2, printed pp. 48–49; completion (8.1) `](https://arxiv.org/pdf/0711.0040)


## Statement

Work in a smooth time-oriented vacuum Einstein spacetime $(M,g)$ of dimension $3+1$, with $M$ connected, orientable, paracompact and without boundary, and a smooth Killing field $T$. Impose the exact IK AF package [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af) and exact IK SBS package [def-author-9f9c6144aed8-ik-sbs](item-def-author-9f9c6144aed8-ik-sbs). Use the forms, contraction and supplied normalized Ernst potential of [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon). Require this same supplied potential to satisfy $\sigma(0,x)\to1$ as $|x|\to\infty$ on the $t=0$ spatial end of the IK AF chart, in the angularly uniform sense of that interface. Let $M>0$ be the AF mass. Assume $-4M^2\mathcal F^2=(1-\sigma)^4$ on all of $S_0$ and $\operatorname{Re}(1/(1-\sigma))>1/2$ at some point of $S_0$. Then $E$ is locally isometric to the domain of outer communication of a Kerr spacetime of mass $M$ with $0<a<M$, in the Kerr exterior convention [physics:def-gr-fx-kerr-exterior](https://alphabetamath.cc/physics/item/def-gr-fx-kerr-exterior). Here locally isometric means every point has a neighborhood with a metric-preserving diffeomorphism onto an open subset of that Kerr exterior. A single global isometry, injective global matching, or a matching of the whole extensions is not supplied by this conclusion.

## Facts & Assumptions

[F1] The formulation uses [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) under its stated hypotheses.

[F2] The formulation uses [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) under its stated hypotheses.

[F3] The formulation uses [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data) under its stated hypotheses.

[F4] The formulation uses [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data) under its stated hypotheses.

[F5] The formulation uses [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) under its stated hypotheses.

[F6] The formulation uses [physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law) under its stated hypotheses.

[F7] The formulation uses [physics:def-gr-fx-kerr-exterior](https://alphabetamath.cc/physics/item/def-gr-fx-kerr-exterior) under its stated hypotheses.

[F8] The formulation uses [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) under its stated hypotheses.

[F9] The formulation uses [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af) under its stated hypotheses.

[F10] The formulation uses [def-author-9f9c6144aed8-ik-sbs](item-def-author-9f9c6144aed8-ik-sbs) under its stated hypotheses.

[F11] The formulation uses [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon) under its stated hypotheses.

## External input

Imported input 1 is the Main Theorem of Ionescu–Klainerman at the exact locator in source 0, with all AF, SBS and T hypotheses above, including $\sigma\to1$ along the specified AF section. Both imported inputs use this same supplied potential; no additive renormalization is made between the horizon hypotheses and either invocation. It supplies the local Kerr conclusion directly; this item claims no local proof of that theorem.

Imported input 2 is Proposition 8.3 and its §8.2 completion at source 1. Put $\Sigma'_0=\{p\in\Sigma_0\cap E:\sigma(p)\ne1\}$ and $y=\operatorname{Re}(1-\sigma)^{-1}$ there. Let $y_{S_0}$ denote the constant value of $y$ on $S_0$ supplied by Lemma 8.1. For $R>y_{S_0}$ the source defines $U_R$ as the unique component of $\{p\in\Sigma'_0:y(p)<R\}$ whose closure in $\Sigma_0$ contains $S_0$. Proposition 8.2 supplies $R_1>y_{S_0}$, and under the full theorem setting Proposition 8.3 proves $\mathcal S=0$ on every $U_R$ with $R\ge R_1$. The completion then excludes the missing denominator-zero points and obtains (8.1). This analytic input, including the conditional Carleman estimate and bootstrap, is imported rather than reconstructed. The elementary path-exhaustion lemma [lem-author-9f9c6144aed8-sublevel-path-exhaustion](item-lem-author-9f9c6144aed8-sublevel-path-exhaustion) explains the exhaustion step only where its path hypotheses hold; it does not replace the source's boundary continuation, quantitative bounds, or exclusion of $\sigma=1$. The transport lemma [lem-author-9f9c6144aed8-stationary-zero-transport](item-lem-author-9f9c6144aed8-stationary-zero-transport) explains how invariant tensor vanishing extends from a section when its explicit invariance hypothesis is met; it supplies no analytic continuation estimate.
