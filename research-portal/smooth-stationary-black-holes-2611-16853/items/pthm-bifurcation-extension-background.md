---
id: pthm-bifurcation-extension-background
title: Bifurcation extension, local non-Kerr deformations and smooth local rigidity
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-horizon-rotation-surface-gravity
  - def-bifurcate-killing-horizon-data
  - thm-nondegenerate-bifurcate-extension-input
  - thm-author-a8fd09e77ebd-kerr-local-deformation
  - lem-author-a8fd09e77ebd-analytic-isometry-obstruction
  - thm-local-bifurcate-rigidity-input
  - math:def-axiom-of-choice
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-horizon-rotation-surface-gravity: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  thm-nondegenerate-bifurcate-extension-input: mathematical-premise
  thm-author-a8fd09e77ebd-kerr-local-deformation: mathematical-premise
  lem-author-a8fd09e77ebd-analytic-isometry-obstruction: mathematical-premise
  thm-local-bifurcate-rigidity-input: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 2,3; §1.1, [1,24,33,34]
      statement: The article reports existence of bifurcate extensions under the
        global assumptions of Rácz–Wald [33,34], possible non-Kerr local
        extensions near a horizon away from the bifurcation sphere [24], and
        extension of the Hawking Killing field to a full neighborhood of the
        bifurcation sphere without analyticity [1]. These are distinct
        local/global claims, not a claimed global smooth rigidity theorem.
      hypotheses: Exactly the conditions and parameter ranges recorded in this
        inventory statement; this is attribution to the article, not independent
        prerequisite evidence.
      reading_limits: Read the frozen original-article extracted text at PDF pp. 2–3,
        §1.1, and visually inspected PDF p. 2. This source attributes the three
        background claims only; independent suppliers below establish their
        precise conditional content.
physical_scope: Conditional geometric background within four-dimensional smooth
  stationary vacuum general relativity. Local vacuum deformations are not
  asserted to satisfy the global black-hole assumptions.
dependency_level: 7
---

## Statement

Within the stationary vacuum model [[post-stationary-vacuum-model]], with horizon terminology from [[def-horizon-rotation-surface-gravity]] and [[def-bifurcate-killing-horizon-data]], the three background claims reported in the article have different hypotheses and scopes.

(1) For the exact global collapse class and a future horizon generator with nonzero constant surface gravity, [[thm-nondegenerate-bifurcate-extension-input]] gives an isometric extension of the whole original spacetime whose event horizon is a proper subset of a bifurcate Killing horizon. The specified horizon-generating action extends; the statement does not automatically extend matter fields or assert global hyperbolicity of the enlarged spacetime.

(2) Near the horizon of rotating Kerr, away from the bifurcation sphere and axis, [[thm-author-a8fd09e77ebd-kerr-local-deformation]] produces smooth local stationary vacuum deformations agreeing with Kerr on the matching side and obstructing extension of its axial field. By [[lem-author-a8fd09e77ebd-analytic-isometry-obstruction]] the whole constructed neighborhood cannot be isometric to an analytic Kerr model neighborhood, even by an isometry not preserving the stationary generator. Thus the neighborhood-level non-Kerr claim follows; no failure of Kerr isometry in every smaller germ is asserted. These local deformations do not supply global black-hole counterexamples.

(3) Under the regular bifurcate non-expanding horizon hypotheses and Ricci-flatness of [[thm-local-bifurcate-rigidity-input]], the Hawking Killing field exists in a full neighborhood of the bifurcation sphere without analyticity. The extra branch-tangent stationary symmetry, not identically zero on that sphere, yields a commuting rotational field there. This is not an extension theorem over the entire exterior.

## Facts & Assumptions

[A1] Use ZFC, including the Axiom of Choice inherited through the geometric suppliers. [[math:def-axiom-of-choice]]

[A2] The stationary vacuum postulate fixes the physical model; the conclusions here are conditional geometric background, not measurements. [[post-stationary-vacuum-model]]

[F1] Horizon rotation, surface gravity and bifurcation use the supplied conventions. [[def-horizon-rotation-surface-gravity]] [[def-bifurcate-killing-horizon-data]]

[F2] The global bifurcate-extension input applies only with its precise collapse class and nonzero-constant surface gravity. [[thm-nondegenerate-bifurcate-extension-input]]

[F3] The local deformation has the prescribed axial obstruction; the analytic-isometry obstruction supplies the missing bridge. [[thm-author-a8fd09e77ebd-kerr-local-deformation]] [[lem-author-a8fd09e77ebd-analytic-isometry-obstruction]]

[F4] The local bifurcate rigidity input requires its regular non-expanding null pair and provides only full-neighborhood conclusions. [[thm-local-bifurcate-rigidity-input]]

## Proof

**Given:** The physical model and, separately for each clause, the corresponding complete mathematical hypotheses.

**Goal:** Derive the three conditional background statements while keeping their scopes distinct.

1.1 With the collapse-class and surface-gravity assumptions of clause (1), apply [F2]. Its isometric embedding and horizon-action conclusion give exactly that clause; matter extension is explicitly separate in that supplier. The physical vacuum model does not replace any global hypothesis. [A1, A2, F1, F2]

1.2 Apply the local deformation theorem [F3] with $0<a<m$. Its connected simply connected collar and matching axial data satisfy the obstruction lemma, which imports Nomizu analyticity extension to rule out any isometry of the whole $U$ onto an analytic Kerr neighborhood. It does not assume the hypothetical isometry preserves $T$. This proves the non-Kerr local-neighborhood assertion, while preserving possible smaller Kerr regions and the lack of global-black-hole hypotheses. [F3]

1.3 Under the hypotheses of clause (3), apply [F4] for the Hawking field, then its additional branch-tangent-symmetry conclusion for the commuting rotational field when that extra hypothesis holds. Its domain is a neighborhood of the bifurcation sphere, so it yields no unasserted global extension of that field. [A1, A2, F1, F4]

2.1 The local construction of step 1.2 omits the bifurcation sphere and global assumptions used in the other clauses. Consequently these conditional background statements are compatible and make no assertion resolving global smooth black-hole uniqueness by themselves. This completes the preserved three-part claim. [step 1.1, step 1.2, step 1.3] ∎

## External input

The original article, PDF pp. 2–3 §1.1, is retained solely as attribution for these three background claims. The proofs above use the independent global-extension, local-deformation, analytic-extension and local-rigidity suppliers; the article is not used to establish its own prerequisite.
