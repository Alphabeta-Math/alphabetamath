---
title: An exact local Killing field is Killing to every order on a horizon
status: draft
research_item: lem-author-9a15bef58785-exact-killing-horizon-jets
dependency_level: 0
---

## Prerequisites

- [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)
- [physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-codimension-and-hypersurface](https://alphabetamath.cc/item/def-codimension-and-hypersurface)
- [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)
- [math:prop-the-inclusion-of-an-embedded-submanifold-is-a-smooth-embedding](https://alphabetamath.cc/item/prop-the-inclusion-of-an-embedded-submanifold-is-a-smooth-embedding)
- [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)
- [math:def-immersion-submersion-and-constant-rank-map](https://alphabetamath.cc/item/def-immersion-submersion-and-constant-rank-map)
- [math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map)
- [math:lem-the-differential-sends-derivations-to-derivations-and-is-linear](https://alphabetamath.cc/item/lem-the-differential-sends-derivations-to-derivations-and-is-linear)


## Statement

Assume the axiom of countable choice $\mathrm{AC}_\omega$. Let $(M,g,N)$ be a time-oriented smooth Lorentzian four-manifold without boundary, with metric $g$ of signature $(-,+,+,+)$. Let $H\subset M$ be a smooth embedded hypersurface, let $O\subset M$ be an open set containing $H$, and let $K$ be a smooth Killing field of $g|_O$. Write $\nabla$ for the metric-selected connection of $g$, restricted to $O$, and $\pi=\mathcal L_K(g|_O)$ for the deformation tensor. Set $\nabla^0\pi=\pi$ and $\nabla^{m+1}\pi=\nabla(\nabla^m\pi)$. Every covariant derivative $\nabla^m\pi$ vanishes on $O$, for every integer $m\ge0$, and hence on $H$. Here restriction to $H$ retains the ambient tensor at each $p\in H$, with all its ambient tangent arguments. Let $i:H\hookrightarrow M$ denote the inclusion, with $H$ carrying the smooth structure from its restricted slice charts. We identify $T_pH$ with the subspace $di_p(T_pH)\subseteq T_pM$ using the injective linear differential $di_p:T_pH\to T_pM$. A direction transverse to $H$ at $p$ means a vector $v\in T_pM$ with $v\notin T_pH$. Thus an actual smooth Killing field near a smooth horizon is Killing to all orders there, including transverse derivatives; merely specifying a field on $H$ would not by itself define those transverse derivatives.

## Statement references

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:def-codimension-and-hypersurface](https://alphabetamath.cc/item/def-codimension-and-hypersurface)

[math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

[math:prop-the-inclusion-of-an-embedded-submanifold-is-a-smooth-embedding](https://alphabetamath.cc/item/prop-the-inclusion-of-an-embedded-submanifold-is-a-smooth-embedding)

[math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

[math:def-immersion-submersion-and-constant-rank-map](https://alphabetamath.cc/item/def-immersion-submersion-and-constant-rank-map)

[math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map)

[math:lem-the-differential-sends-derivations-to-derivations-and-is-linear](https://alphabetamath.cc/item/lem-the-differential-sends-derivations-to-derivations-and-is-linear)

## Facts & Assumptions

[F1] A Killing field of $g|_O$ is defined by $\mathcal L_K(g|_O)=0$ on its open domain. [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[F2] On a smooth four-manifold without boundary, a smooth nondegenerate symmetric metric has a unique metric-selected connection, whose induced tensor derivatives are linear and extend to every finite tensor rank. The cited construction assumes $\mathrm{AC}_\omega$ for the canonical tangent-bundle smooth structure. [physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[F3] The ambient time-oriented Lorentzian data include a smooth symmetric nondegenerate metric and a smooth timelike field $N$ on a Hausdorff second-countable smooth four-manifold without boundary. Countable choice is assumed for the canonical smooth bundle structures used by this definition and [F2]; the vanishing induction makes no further choices. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F4] A smooth embedded hypersurface is an embedded submanifold of codimension one, with its smooth structure supplied by restricted slice charts. Transverse directions are understood in the explicit sense given in the Statement, with no spacelike or null requirement on $H$. [math:def-codimension-and-hypersurface](https://alphabetamath.cc/item/def-codimension-and-hypersurface) [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

[F5] For the restricted-slice-chart smooth structure, the inclusion $i:H\hookrightarrow M$ is a smooth embedding. An embedding is an immersion, and an immersion has injective differential at every point. The differential $di_p:T_pH\to T_pM$ is well defined and linear, so its image is a vector subspace and it identifies $T_pH$ with that image. This is the ambient tangent-subspace identification used here. [math:prop-the-inclusion-of-an-embedded-submanifold-is-a-smooth-embedding](https://alphabetamath.cc/item/prop-the-inclusion-of-an-embedded-submanifold-is-a-smooth-embedding) [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding) [math:def-immersion-submersion-and-constant-rank-map](https://alphabetamath.cc/item/def-immersion-submersion-and-constant-rank-map) [math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map) [math:lem-the-differential-sends-derivations-to-derivations-and-is-linear](https://alphabetamath.cc/item/lem-the-differential-sends-derivations-to-derivations-and-is-linear)

## Proof

**Given:** The hypotheses and data in the Statement.

**Goal:** Prove vanishing of all ambient covariant derivatives on $O$ and on $H$.

1.1 The ambient data and countable-choice assumption in [F3] meet the hypotheses of [F2], so the metric-selected connection and its induced derivatives are available on $O$. By [F1], $\pi$ is the identically zero tensor field on $O$. Linearity gives $\nabla\pi=\nabla0=0$ on the same open set. [F1, F2, F3]

2.1 The case $m=0$ holds by step 1.1. If $\nabla^m\pi=0$ on $O$, then [F2] gives $\nabla^{m+1}\pi=\nabla0=0$ there. Induction proves the assertion for every $m\ge0$. At each $p\in H\subset O$, evaluating this zero ambient tensor on any ambient tangent arguments still gives zero, including arguments transverse to $T_pH$ under the identification in [F5] and the convention in [F4]. These derivatives are defined using the field on $O$; data given only on $H$ do not specify its variation off $H$. [F2, F4, F5, step 1.1] ∎
