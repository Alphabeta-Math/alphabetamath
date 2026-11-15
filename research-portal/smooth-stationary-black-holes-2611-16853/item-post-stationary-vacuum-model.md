---
title: Stationary vacuum model and asymptotic normalization
status: draft
research_item: post-stationary-vacuum-model
dependency_level: 1
sources:
  references:
    - title: Alexandru D. Ionescu and Sergiu Klainerman, On the uniqueness of smooth,
        stationary black holes in vacuum (arXiv:0711.0040v2)
      url: https://arxiv.org/pdf/0711.0040v2
      locator: Section 1.1, printed/PDF p. 5, equation (1.1) and adjoining Ricci-flat
        condition; Section 1.2, printed/PDF p. 6, opening assumptions, AF,
        equation (1.4), T = partial_t, and footnote 4.
      statement: The source assumes a smooth time-oriented four-dimensional vacuum
        spacetime with a smooth Killing field. AF specifies a Cartesian product
        end, T = partial_t and g00 = -1 + 2M/r + O(r^-2); thus g(T,T) tends to
        -1 and is negative sufficiently far out.
      hypotheses: These are adopted model and AF assumptions, with positive mass M in
        the source; they are not conclusions of its uniqueness theorem.
      reading_limits: Consulted the extracted PDF passages at the cited locators. Only
        formulation is used; no uniqueness proof, existence theorem or
        measurement was checked. The source imposes stronger conditions than
        this postulate.
---

PDF p. 1: ` §1.1, vacuum and stationarity equations `

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [` Alexandru D. Ionescu and Sergiu Klainerman, On the uniqueness of smooth, stationary black holes in vacuum (arXiv:0711.0040v2) · Section 1.1, printed/PDF p. 5, equation (1.1) and adjoining Ricci-flat condition; Section 1.2, printed/PDF p. 6, opening assumptions, AF, equation (1.4), T = partial_t, and footnote 4. `](https://arxiv.org/pdf/0711.0040v2)


## Postulate

Work in ZFC. Adopt stationary Lorentzian data $(M,g,N,T)$ as in [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data): in particular, $M$ is a connected smooth oriented four-manifold without boundary, $g$ has signature $(-,+,+,+)$, $N$ is a time orientation, and $T$ is a smooth Killing field, so $\mathcal L_Tg=0$. Adopt the vacuum equation $\operatorname{Ric}(g)=0$ on $M$.

Assume a designated spatial end with an exterior Cartesian radial coordinate $r=|x|$, as in the fixed-chart convention of [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data), and an end region of the form $\mathbb R\times\{x\in\mathbb R^3:|x|>R_0\}$. On a sufficiently far-out part of this end, assume $T$ is future timelike: $g(T,T)<0$ and $g(T,N)<0$. Normalize it by $g(T,T)\to-1$ as $r\to\infty$ on the end.

These equations and end conditions are assumptions of the model. They do not assert that a solution exists, that the field is timelike everywhere, or that a measurement has established the model. The displayed normalization alone does not impose differentiated decay bounds.

## Facts & Assumptions

[A1] The set-theoretic convention is ZFC, including the axiom of choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The stationary Lorentzian-data definition supplies the metric signature, time orientation, future direction, Killing condition and Ricci-tensor convention used in the postulate. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] The asymptotic-data definition supplies the fixed Cartesian exterior and radial-coordinate convention; its differentiated bounds are additional conditions and are not assumed merely by using the chart. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

## Source notes

Ionescu–Klainerman provide an independent formulation of the vacuum/Killing model and product end at the cited locators. Their AF expansion fixes the asymptotic norm; its positive-mass coefficient and other AF requirements are not imported here. The future-direction choice relative to $N$ remains an explicit adopted convention. This citation supplies formulation, not proof, existence or observation.
