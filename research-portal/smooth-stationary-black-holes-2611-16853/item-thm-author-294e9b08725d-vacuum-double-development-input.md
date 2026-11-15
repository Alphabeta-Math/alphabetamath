---
title: External vacuum KID development and complete stationary flow
status: published
research_item: thm-author-294e9b08725d-vacuum-double-development-input
dependency_level: 11
sources:
  references:
    - title: Robert Beig and Piotr T. Chruściel, Killing Initial Data
      url: https://arxiv.org/pdf/gr-qc/9604040v1
      locator: §2, vacuum Case2, pp4–5, equations(2.6) and(2.13)
      statement: Smooth vacuum constraint initial data admit a vacuum Cauchy
        development, and a vacuum KID extends to a Killing field in that
        development. No nonvanishing lapse hypothesis is used in vacuum Case2.
      hypotheses: Three-dimensional initial-data manifold; vacuum constraints rho=J=0,
        sufficiently regular data (here smooth), and vacuum KID stress tau_ij=0,
        meaning the stationary vacuum KID equations. The transversal lapse
        condition N nonzero belongs to separate Case1, not Case2.
      reading_limits: Read actual §2 vacuum Case2 and the KID equations and
        conventions; no independent reconstruction of hyperbolic propagation or
        the cited Cauchy-existence proofs.
    - title: Piotr T. Chruściel, On completeness of orbits of Killing vector fields
      url: https://arxiv.org/pdf/gr-qc/9304029v1
      locator: MGHD existence/uniqueness discussion p2; Theorem1.1 p2; Corollary1.2(2)
        p3; Definition3.1 and sufficient falloff p12; Proposition2.4 pp9–10
      statement: Smooth three-dimensional vacuum initial data have a unique maximal
        globally hyperbolic vacuum development. On such a development a Killing
        field has complete orbits if its Cauchy data are complete asymptotically
        flat without boundary as in Definition3.1; sufficient bounds are h−delta
        O4(r^-alpha), K O3(r^-1-alpha), alpha>0. Any globally hyperbolic vacuum
        development of an open initial submanifold embeds into its MGHD, which
        in the full MGHD is D of that initial submanifold (Proposition2.4).
      hypotheses: Four-dimensional smooth vacuum maximal globally hyperbolic
        spacetime; complete boundaryless three-dimensional AF Cauchy
        hypersurface, compact core and finitely many Euclidean ends with the
        indicated falloff; smooth Killing field. There is no common future
        orientation requirement at all ends in Corollary1.2(2).
      reading_limits: Read actual introduction, theorem/corollary, complete AF
        definition and Proposition2.4 statement/proof for its exact scope. The
        Cauchy development and completeness theorems are imported, not
        reconstructed or reviewed.
external_input: true
---

## Prerequisites

- [lem-author-294e9b08725d-smooth-vacuum-data-double](item-lem-author-294e9b08725d-smooth-vacuum-data-double)
- [lem-author-294e9b08725d-stationary-vacuum-kid-double](item-lem-author-294e9b08725d-stationary-vacuum-kid-double)
- [lem-author-294e9b08725d-complete-asymptotically-flat-double](item-lem-author-294e9b08725d-complete-asymptotically-flat-double)
- [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)
- [` Robert Beig and Piotr T. Chruściel, Killing Initial Data · §2, vacuum Case2, pp4–5, equations(2.6) and(2.13) `](https://arxiv.org/pdf/gr-qc/9604040v1)
- [` Piotr T. Chruściel, On completeness of orbits of Killing vector fields · MGHD existence/uniqueness discussion p2; Theorem1.1 p2; Corollary1.2(2) p3; Definition3.1 and sufficient falloff p12; Proposition2.4 pp9–10 `](https://arxiv.org/pdf/gr-qc/9304029v1)


## Statement

Let smooth vacuum initial data on a complete boundaryless three-dimensional manifold have finitely many Euclidean ends, compact intervening region and $h-\delta=O_4(r^{-\alpha})$, $K=O_3(r^{-1-\alpha})$, $\alpha>0$. A smooth vacuum KID extends to a Killing field on the maximal globally hyperbolic vacuum development of these data, and that field has complete orbits. The lapse may have opposite signs on different ends. A globally hyperbolic vacuum development of an open part of the data embeds isometrically in the corresponding domain of dependence in this development. These are external Cauchy/KID/completeness inputs.

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[F1] Conditional reflection application: assume all hypotheses of the smooth vacuum data-double and stationary vacuum KID suppliers, including the specified canonical collar and signed double, data induced throughout the positive section by the same smooth Ricci-flat ambient metric, and an ambient Killing field commuting with the exact boost on that collar. Then the reflected canonical data and KID are smooth and satisfy the vacuum constraint and KID equations on the full double. These additional reflection hypotheses are not assumed for the general data of the Statement. [lem-author-294e9b08725d-smooth-vacuum-data-double](item-lem-author-294e9b08725d-smooth-vacuum-data-double) [lem-author-294e9b08725d-stationary-vacuum-kid-double](item-lem-author-294e9b08725d-stationary-vacuum-kid-double)

[F2] Conditional geometric application: assume all hypotheses of the complete asymptotically flat double supplier, including the connected positive half with nonempty compact boundary, its specified canonical collar, compact smooth radial truncations exhausting that half, and $h-\delta=O_6(r^{-1})$, $K=O_5(r^{-3})$ on its specified Euclidean end. Then the doubled initial geometry is complete, has two Euclidean ends and a compact intervening region, and retains these stronger differentiated end estimates. These additional hypotheses are required for this application. [lem-author-294e9b08725d-complete-asymptotically-flat-double](item-lem-author-294e9b08725d-complete-asymptotically-flat-double)

## External input

Import the cited external results only under the exact hypotheses in the Statement and source records. Their proofs are not reconstructed or independently reviewed here.
