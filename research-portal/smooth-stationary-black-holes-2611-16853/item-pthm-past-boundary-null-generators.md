---
title: "Lemma 4.2: null generators of the causal past boundary"
status: published
research_item: pthm-past-boundary-null-generators
dependency_level: 25
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 24, Lemma 4.2 and proof
      attribution: A point on the causal past boundary of the comparison sphere,
        inside its cylinder and earlier in section time than the sphere, is
        joined to the sphere by a boundary null geodesic with the normalized
        outward final tangent and no interior focal point.
      hypotheses: The article's regular stationary vacuum construction and a
        sufficiently small positive parameter, with causal relations relative to
        the exterior.
      reading_limits: Historical reading note retained from the current source; this
        maintenance revision claims no fresh article or external full-text
        reading. The frozen article text at the cited lemma and proof was read
        for attribution. The article's assertion is not used as a proof premise
        below.
---

PDF p. 24: ` Lemma 4.2 and proof `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-stationary-section-time](item-def-stationary-section-time)
- [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [pthm-transformed-cauchy-sections](item-pthm-transformed-cauchy-sections)
- [pthm-adm-temporality](item-pthm-adm-temporality)
- [pthm-comparison-sphere-properties](item-pthm-comparison-sphere-properties)
- [pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates)
- [lem-compact-target-achronal-generator-input](item-lem-compact-target-achronal-generator-input)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)


## Statement

Work in ZFC with the regular mass-one stationary vacuum construction, the original maximal exterior section and $T|_S\not\equiv0$, as in [post-stationary-vacuum-model](item-post-stationary-vacuum-model) and [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime). Fix $q\in(0,1]$, a supplied complete maximal stationary graph section, and its section time $v_q$. Choose the sufficiently large comparison radius supplied by [pthm-comparison-sphere-properties](item-pthm-comparison-sphere-properties). Denote the supplied stationary end time coordinate by $t'$ and reserve $t\in\mathbb R$ for the value indexing the translated sphere. Let $C_t=\{t'=t,r=R_0q^{-2/3}\}$ and let $\mathscr C=\{r=R_0q^{-2/3}\}$ be its stationary cylinder. Inside the cylinder means the component of its complement containing the bifurcation sphere in the stationary spatial projection. All causal relations and boundaries below are relative to the exterior $\mathcal E$ with metric $g_q$.

If $p\in\partial_{\mathcal E}I^-_{g_q}(C_t)$ lies inside $\mathscr C$ and $v_q(p)<\min_{C_t}v_q$, then a future-directed null geodesic segment joins $p$ to $C_t$ and lies entirely in $\partial_{\mathcal E}I^-_{g_q}(C_t)$. Its final tangent is the future outward null normal $L_{q,t}$ after the normalization $g_q(T,L_{q,t})=-d_q/4$, where $d_q>0$ is the supplied pole denominator. There is no focal point to $C_t$ strictly between the endpoints, measured along the segment from $C_t$ toward $p$.

Here $I^-_{g_q}(C_t)$ consists of points connected to $C_t$ by future-directed timelike curves in $\mathcal E$. A focal point is defined by a nonzero Jacobi variation normal to $C_t$ that vanishes at the point, with the normal initial conditions in [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data). The outward direction is the null normal whose radial component points toward increasing $r$.

## Facts & Assumptions

[A1] The model, regular data, mass-one normalization, maximal original section and nontriviality of $T|_S$ are the hypotheses of the completed positive-parameter construction. Work in ZFC, including choice. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-harrison-normalization](item-def-harrison-normalization) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] For the chosen $q$ and section, $(\mathcal E,g_q)$ is smooth, time-oriented and globally hyperbolic, and $v_q$ is temporal. The section-time construction identifies the exterior with the stationary product. [pthm-transformed-cauchy-sections](item-pthm-transformed-cauchy-sections) [pthm-adm-temporality](item-pthm-adm-temporality) [def-stationary-section-time](item-def-stationary-section-time)

[F2] The coordinate $t'$ is the stationary end coordinate called $t$ in the comparison-sphere definition. The comparison sphere is a compact smooth spacelike two-sphere; its stationary translates form $\mathscr C$, and its spatial projection surrounds $S$. On and outside the cylinder, the coordinate $t'$ is temporal. The stationary field $T=\partial_{t'}$ is future timelike there for the chosen sufficiently large radius. [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres) [pthm-comparison-sphere-properties](item-pthm-comparison-sphere-properties) [pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates)

[F3] On each comparison sphere the future outward null normal is normalized by $g_q(T,L_{q,t})=-d_q/4$, with $d_q>0$. The two future null normal directions are distinct and the outward one has positive radial component. [pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data) [def-harrison-normalization](item-def-harrison-normalization)

[F4] In a smooth globally hyperbolic time-oriented Lorentzian four-manifold, a point on the chronological past boundary of a compact spacelike two-surface, strictly earlier than the surface under a temporal function, is joined to it by a boundary null geodesic orthogonal at the target and without an interior focal point to the target. [lem-compact-target-achronal-generator-input](item-lem-compact-target-achronal-generator-input) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F5] In a smooth time-oriented Lorentzian four-manifold, each chronological past of a point is open. Apply this within $(\mathcal E,g_q)$; the countable and dependent choice hypotheses of the supplier follow from ZFC in [A1]. [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[F6] In a topological space, an arbitrary union of open sets is open. Apply this to the relative manifold topology of $\mathcal E$. [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)

## Proof

**Given:** The construction, $q$, $t$, comparison sphere and point $p$ in the Statement.

**Goal:** Obtain the stated boundary generator, focal exclusion and normalized outward final tangent.

1.1 By [F1], the exterior with $g_q$ is globally hyperbolic and $v_q$ is temporal. By [F2], $C_t$ is a compact smooth spacelike two-sphere. The given strict inequality supplies the temporal separation required by [F4]. Applying [F4] in $\mathcal E$ gives a future null geodesic segment from $p$ to some $c\in C_t$, entirely in $\partial_{\mathcal E}I^-_{g_q}(C_t)$, orthogonal to $C_t$ at $c$, and without a focal point to $C_t$ strictly between its endpoints. [given, F1, F2, F4]

2.1 Suppose its final tangent is the other future null normal direction. By [F3], this direction has negative radial component: the tangent plane to the sphere is spacelike, and its two future null normal rays have opposite nonzero radial components because the cylinder is timelike. Thus, immediately before reaching $c$, the segment lies outside the cylinder. Since $p$ is inside, continuity and the product separation of [F1]–[F2] give a last cylinder intersection $z$ before that final exterior segment. The coordinate $t'$ is a future-increasing temporal coordinate there: its differential is timelike, and $dt'(T)=1$ with $T$ future timelike. Hence $t'(z)<t'(c)=t$. The future timelike stationary orbit in the cylinder joins $z$ to the point with the same spatial coordinate on $C_t$. Therefore $z\in I^-_{g_q}(C_t)$. By [F5], $I^-_{g_q}(C_t)=\bigcup_{c'\in C_t}I^-_{g_q}(c')$ is a union of open subsets of $\mathcal E$, hence is open. This contradicts containment of the whole segment, including $z$, in its boundary. [given, F1, F2, F3, F5, F6, step 1.1]

3.1 The final tangent is consequently on the outward future null ray. Because $T$ is future timelike and $d_q>0$, there is a unique positive scaling of that tangent for which its inner product with $T$ is $-d_q/4$. By [F3] this normalized vector is $L_{q,t}$. Positive affine reparametrization effects that scaling without changing the segment or its focal-point conclusion. This proves all assertions. [F2, F3, step 1.1, step 2.1] ∎

## Source notes

The article reference attributes the lemma and its cylinder argument. The proof uses the declared completed compact-target and geometric suppliers; the article's claim is not a premise.
