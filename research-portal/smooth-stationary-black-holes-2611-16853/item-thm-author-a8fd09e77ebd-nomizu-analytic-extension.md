---
title: Nomizu extension and uniqueness in the analytic Lorentzian setting
status: published
research_item: thm-author-a8fd09e77ebd-nomizu-analytic-extension
dependency_level: 1
sources:
  references:
    - title: P. T. Chruściel, On rigidity of analytic black holes
      url: https://arxiv.org/pdf/gr-qc/9610011
      locator: Section 2, Theorem 2.1 (Nomizu) and footnote 6, printed/PDF p. 6.
      statement: A Killing field on a connected open subset of a connected simply
        connected analytic pseudo-Riemannian manifold extends to the whole
        manifold.
      hypotheses: An analytic pseudo-Riemannian metric, connected simply connected
        ambient manifold, and a smooth Killing field on a nonempty connected
        open set; no field equation or completeness assumption.
      reading_limits: Read the web-extracted PDF text of Theorem 2.1 and footnote 6,
        which explicitly covers pseudo-Riemannian metrics. Existence is imported
        at statement level; neither Nomizu’s original proof nor its
        pseudo-Riemannian adaptation was reconstructed.
    - title: Ionescu–Klainerman, On the local extension of Killing vector-fields in
        Ricci flat manifolds
      url: https://arxiv.org/pdf/1108.3575
      locator: Section 1, printed/PDF p. 2, opening extension-problem paragraph and
        footnote 1.
      statement: The preceding extension is unique for a real-analytic
        pseudo-Riemannian metric when the ambient manifold and initial open set
        are connected and the ambient manifold is simply connected.
      hypotheses: A smooth Killing field on the connected open set in the
        real-analytic pseudo-Riemannian manifold; connectedness and simple
        connectedness as stated. No field equation or boundary condition is
        assumed for this analytic theorem.
      reading_limits: Read the web-extracted PDF text of the opening Section 1
        paragraphs and footnote 1. This verifies the statement and its general
        pseudo-Riemannian setting, not Nomizu’s proof or the later Ricci-flat
        extension results.
external_input: true
---

## Prerequisites

- [lem-author-a8fd09e77ebd-isometry-analytic-pullback](item-lem-author-a8fd09e77ebd-isometry-analytic-pullback)
- [math:def-simply-connected](https://alphabetamath.cc/item/def-simply-connected)
- [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)
- [` P. T. Chruściel, On rigidity of analytic black holes · Section 2, Theorem 2.1 (Nomizu) and footnote 6, printed/PDF p. 6. `](https://arxiv.org/pdf/gr-qc/9610011)
- [` Ionescu–Klainerman, On the local extension of Killing vector-fields in Ricci flat manifolds · Section 1, printed/PDF p. 2, opening extension-problem paragraph and footnote 1. `](https://arxiv.org/pdf/1108.3575)


## Statement

Let $(U,g)$ be a connected simply connected real-analytic Lorentzian manifold. Here $U$ is a smooth $n$-manifold without boundary, $n\geq1$, with a compatible real-analytic atlas, and $g$ is a smooth symmetric nondegenerate covariant two-tensor whose components in that atlas are real analytic. Lorentzian means that at each point some tangent-space basis gives the metric matrix $\operatorname{diag}(-1,1,\ldots,1)$, with $n-1$ positive entries. A smooth vector field $Y$ on an open set is Killing when $\mathcal L_Yg=\left.\frac{d}{dt}\right|_{t=0}\Phi_t^*g=0$, where $\Phi_t$ is its local flow. No orientation or time orientation is assumed.

Every smooth Killing field on a nonempty connected open subset $O$ extends to a unique smooth Killing field on all of $U$. In particular, two global Killing fields agreeing on a nonempty open subset agree everywhere: restrict to a connected coordinate subneighborhood of that subset and use uniqueness.

## Statement references

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[lem-author-a8fd09e77ebd-isometry-analytic-pullback](item-lem-author-a8fd09e77ebd-isometry-analytic-pullback)

[math:def-simply-connected](https://alphabetamath.cc/item/def-simply-connected)

## Facts & Assumptions

[F1] Smooth manifolds, smooth structures, charts and coordinate domains have the general-dimensional convention in the smooth-manifold definition. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[F2] Compatible real-analytic atlases, analytic metric components, symmetric nondegenerate metrics and Killing fields have the dimension-independent conventions explicitly formulated in the analytic-pullback supplier. Only these formulation conventions are used here, without imposing the isometry hypotheses of its transport conclusion. The Lorentzian signature is specified inline above. [lem-author-a8fd09e77ebd-isometry-analytic-pullback](item-lem-author-a8fd09e77ebd-isometry-analytic-pullback)

[F3] Simple connectedness has the nonempty path-connected convention in the cited definition. [math:def-simply-connected](https://alphabetamath.cc/item/def-simply-connected)

[F4] The imported Nomizu existence and uniqueness inputs apply to these analytic pseudo-Riemannian data and hence to the Lorentzian subclass; they require neither a field equation nor completeness of the Killing field.

## External input

Chruściel, Section 2, Theorem 2.1 and footnote 6, supplies global existence in the analytic pseudo-Riemannian setting. Ionescu–Klainerman, Section 1, p. 2, explicitly supplies uniqueness under the same hypotheses. These established results are imported at statement level; no proof reconstruction is claimed.
