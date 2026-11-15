---
title: Comparison spheres and their stationary cylinders
status: published
research_item: def-coordinate-comparison-spheres
dependency_level: 3
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 21–23, Proposition 4.1 and notation after (4.2)
      statement: For sufficiently large fixed R_0 and 0 < q ≤ 1, the comparison sphere
        is t = 0, r = R_0 q^(-2/3); at fixed q its stationary translates are
        denoted C_t and their union is denoted by a calligraphic C. The chosen
        radius tends to infinity more slowly than the scale q^(-1).
      hypotheses: The article's original stationary end coordinates and the parameter
        range stated in Proposition 4.1.
      reading_limits: Read the frozen article text at Proposition 4.1 and the
        subsequent notation. This citation attributes the construction; the
        justification below is local and does not invoke the article's geometric
        conclusions.
---

PDF p. 21: ` Proposition 4.1 definition `; PDF p. 22: ` Proposition 4.1 and notation after (4.2) `; PDF p. 23: ` notation after (4.2) `

## Prerequisites

- [def-harrison-normalization](item-def-harrison-normalization)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)
- [math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)


## Definition

Let stationary Lorentzian data and an original Cartesian exterior end be supplied as in [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) and [def-harrison-normalization](item-def-harrison-normalization). More specifically, suppose the spacetime end is supplied with a diffeomorphism from $\mathbb R\times E$ onto its image, where $E=\{x\in\mathbb R^3:|x|>a\}$ for some $a>0$, the corresponding coordinates are $(t,x^1,x^2,x^3)$, and the stationary field is $T=\partial_t$ there. Set $r=|x|$, using the Cartesian-radius convention of [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data). The flow of $T$ on this end is consequently $\phi_s^T(t,x)=(t+s,x)$.

Fix $R_0>a$, to be chosen sufficiently large when further geometric estimates require it. For every $0<q\leq1$, define the **comparison sphere**
$$C_q=\{(t,x):t=0,\ r=R_0q^{-2/3}\}.$$
At a fixed $q$, write $C=C_q$, $C_s=\phi_s^T(C)$, and $\mathscr C=\bigcup_{s\in\mathbb R}C_s$. Here $\mathscr C$ is called the **stationary cylinder** of $C$; this name alone does not assert that it is timelike. The phrase that the spheres move to infinity more slowly than the scale $q^{-1}$ means precisely that their radii $R(q)=R_0q^{-2/3}$ satisfy $R(q)\to\infty$ and $R(q)/q^{-1}\to0$ as $q\downarrow0$.

## Facts & Assumptions

[F1] Stationary Lorentzian data include the smooth vector field $T$; the product end and the equation $T=\partial_t$ are additional supplied coordinate data. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] The original end has a Cartesian radius $r=|x|$; the mass-one convention and the existence of its mass limit, when used, are separate assumptions. [def-harrison-normalization](item-def-harrison-normalization) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F3] A smooth embedded two-dimensional submanifold is characterized by local smooth slice charts in which it is a coordinate two-plane. [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

[F4] A smooth vector field on a smooth manifold has a unique maximal integral curve through each specified initial point. [math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)

## Justification

**Given:**The product end, $R_0>a$, and $0<q\leq1$ in the Definition.

**Goal:** Justify the coordinate sets, their translated union, and the stated scale comparison.

1.1 Since $q^{-2/3}\geq1$, the radius $R(q)$ exceeds $a$. The set $|x|=R(q)$ is a smooth embedded two-sphere: near each point one nonzero coordinate can be solved as $x^i=\pm\sqrt{R(q)^2-\sum_{j\ne i}(x^j)^2}$, giving smooth local graphs, and radial scaling identifies it with the unit sphere. The supplied product diffeomorphism carries this sphere at $t=0$ into the spacetime end. [given, F2, F3]

2.1 The curve $s\mapsto(t+s,x)$ has velocity $\partial_t=T$ and is defined for every real $s$ in the supplied product end. By uniqueness of the maximal integral curve through $(t,x)$, these globally defined curves are the stationary flow trajectories. Thus $C_s=\{t=s,r=R(q)\}$ and $\mathscr C=\{r=R(q)\}$ there. Finally $R(q)=R_0q^{-2/3}\to\infty$ while $R(q)/q^{-1}=R_0q^{1/3}\to0$ as $q\downarrow0$. [given, F1, F4, step 1.1, algebra] ∎



The article supplies attribution for the definition and the scale choice. Spacelikeness, timelikeness, expansion, and transformed area require additional metric hypotheses and estimates; they are not consequences of this coordinate definition alone.

## Source notes

The article supplies attribution for the definition and the scale choice. Spacelikeness, timelikeness, expansion, and transformed area require additional metric hypotheses and estimates; they are not consequences of this coordinate definition alone.
