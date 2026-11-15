---
title: Smooth rotating degenerate-horizon uniqueness
status: published
research_item: op-smooth-degenerate-uniqueness
dependency_level: 6
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 5, §1.3, first paragraph
      statement: The article asks about uniqueness of rotating degenerate black holes
        without analyticity and discusses analytic rigidity and axisymmetric
        extremal uniqueness as partial results.
      hypotheses: The discussion concerns stationary, asymptotically flat, regular
        vacuum black holes with a connected horizon; the paragraph invokes
        I-plus-regularity for its analytic comparison.
      reading_limits: Read the frozen article text at the cited paragraph. This
        reference attributes the question and the article's description of
        partial results; it is not a proof of a prerequisite or of uniqueness.
    - title: A uniqueness theorem for degenerate Kerr-Newman black holes
      url: https://arxiv.org/abs/1002.1737v1
      locator: Abstract
      statement: The abstract states a Kerr–Newman uniqueness result for domains of
        dependence of stationary, I-plus-regular, analytic electrovacuum
        spacetimes with a connected, nonempty, rotating, degenerate event
        horizon.
      hypotheses: Stationarity, I-plus-regularity, analyticity, electrovacuum
        equations and a connected, nonempty, rotating, degenerate event horizon,
        as stated in the abstract.
      reading_limits: Read the arXiv abstract only; the theorem's full technical
        formulation and proof were not checked. This is contextual status
        information, not a premise for a deduction here.
---

PDF p. 5: ` §1.3, end of first paragraph `

## Prerequisites

- [def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity)
- [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data)
- [def-kerr-metric](item-def-kerr-metric)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)
- [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)
- [` A uniqueness theorem for degenerate Kerr-Newman black holes · Abstract `](https://arxiv.org/abs/1002.1737v1)


## Open problem

The article asks whether uniqueness holds for a smooth, stationary, asymptotically flat vacuum black hole with a connected rotating degenerate horizon without assuming analyticity. The intended uniqueness conclusion is that its domain of outer communications is isometric to an extremal Kerr exterior, under suitable regularity hypotheses.

One precise subcase is the following. Let $(M,g,T)$ be a smooth, time-oriented Lorentzian four-manifold with $\operatorname{Ric}(g)=0$ and a stationary Killing field $T$, and assume it is $I^+$-regular relative to a specified asymptotically flat spacelike end in the sense of [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data). In particular, $T$ is complete, the domain of outer communications $D$ is globally hyperbolic, and the specified spacelike section has the end, boundary and horizon-generator properties stated in that definition. Suppose the nonempty future event horizon $H$ is connected and is a smooth Killing horizon for a specified generating Killing field $K$. Require the nonzero-generator part $H_*=\{p\in H:K_p\ne0\}$ to be nonempty and dense in $H$, with $K$ tangent and normal to $H$ on $H_*$. It is rotating relative to $T$ when $T$ fails somewhere to lie in the horizon's null normal line; it is degenerate when the surface-gravity function of $K$ vanishes on its nonzero-generator part, as in [def-horizon-rotation-surface-gravity](item-def-horizon-rotation-surface-gravity). Must $(D,g|_D)$ be isometric to an extremal Kerr exterior from [def-kerr-metric](item-def-kerr-metric), with $M>0$ and $|a|=M$?

This subcase explicitly assumes a smooth horizon-generating Killing field. The broader article question also asks for a treatment without assuming such a field merely as a consequence of smooth stationarity; neither its existence nor global axisymmetry is asserted here.

## Status

The article dated 12 November 2026 presents the smooth, non-analytic rotating degenerate case as a question. Its §1.3 describes analytic rigidity and axisymmetric extremal uniqueness as partial results, with their own hypotheses. In particular, Chruściel–Nguyen's abstract states an analytic electrovacuum result for a connected rotating degenerate horizon; analyticity is an explicit hypothesis of that result. These comparisons do not answer the question above. The status recorded here is the article-date status, not a claim that a complete later literature search has ruled out a resolution.
