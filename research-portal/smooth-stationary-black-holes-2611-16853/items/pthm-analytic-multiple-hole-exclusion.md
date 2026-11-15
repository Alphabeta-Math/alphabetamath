---
id: pthm-analytic-multiple-hole-exclusion
title: Exclusion of regular analytic multiple horizons
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-author-ae62588ad46a-analytic-geometric-data
  - lem-author-ae62588ad46a-canonical-end-slice
  - lem-author-ae62588ad46a-cofinal-end-causal-sets
  - lem-author-ae62588ad46a-positive-area-nonzero-angular-momentum
  - lem-author-ae62588ad46a-horizon-case-partition
  - thm-author-ae62588ad46a-stationary-asymptotic-normal-form
  - pthm-author-ae62588ad46a-analytic-geometric-classification-input
  - math:def-axiom-of-choice
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-author-ae62588ad46a-analytic-geometric-data: mathematical-premise
  lem-author-ae62588ad46a-canonical-end-slice: mathematical-premise
  lem-author-ae62588ad46a-cofinal-end-causal-sets: mathematical-premise
  lem-author-ae62588ad46a-positive-area-nonzero-angular-momentum: mathematical-premise
  lem-author-ae62588ad46a-horizon-case-partition: mathematical-premise
  thm-author-ae62588ad46a-stationary-asymptotic-normal-form: mathematical-premise
  pthm-author-ae62588ad46a-analytic-geometric-classification-input: physical-result
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: "Original-claim attribution only: §1.3, PDF p.5, multiple-black-hole
        case split"
    - title: Huang–Li–Zhu, Nonexistence of Multiple Black Holes in Stationary Analytic
        Vacuum Spacetimes
      url: https://arxiv.org/html/2611.03766v1
      locator: §1, complete multiple-horizon classification discussion from the
        paragraph beginning “For the general case” through the Main Theorem and
        final unnumbered Corollary; (H1)–(H3) specify its geometric class.
      statement: "In four-dimensional stationary, asymptotically flat, I-plus-regular
        analytic vacuum black-hole spacetimes the future horizon is connected:
        the rotating class has connected horizon; the all-nonrotating
        nondegenerate class is Schwarzschild; the remaining all-nonrotating
        class is excluded by the Main Theorem. The classification has no initial
        horizon-connectedness assumption."
      hypotheses: Analytic Ricci-flat four-dimensional spacetime. H1 requires a
        spacelike Cartesian exterior with h_ij=(1+2M/r)delta_ij+o_2(r^-1) and
        k_ij=o_2(r^-1), where M is the ADM mass in geometric units. H2 requires
        the stationary Killing field timelike on its saturated end. H3 requires
        completeness of that field, a globally hyperbolic DOC, and a connected
        spacelike acausal section containing the end, with compact core,
        finitely many ends and a completed boundary on the future horizon
        meeting every generator once. A nonempty black-hole horizon is
        understood. No local componentwise Killing-generator or surface-gravity
        data are additional hypotheses of this full geometric conclusion.
      reading_limits: Read v1 HTML §1, including H1–H3, Definitions 1.2–1.5, both
        classes of the multiple-horizon discussion, Theorem 1.6, Lemma 1.7, the
        Main Theorem, and final Corollary. Import the connectedness conclusion
        of that complete classification discussion, rather than infer an
        extension to the horizon from a DOC isometry alone. The source uses its
        own horizon preparation and case analysis; these were not reconstructed,
        nor were §§2–4 or the cited rigidity/staticity/balance proofs audited.
        Checked application against the supplied normal-form, canonical-slice
        and cofinal-end interfaces. No source-defined labels are asserted to
        satisfy the stronger local Killing-generator interface merely by
        definition.
physical_scope: Conditional four-dimensional classical stationary vacuum general
  relativity, with zero cosmological constant. No observation,
  dynamical-settling claim or smooth nonanalytic uniqueness assertion is made.
dependency_level: 8
---

## Statement

The article concludes nonexistence of multiple black holes in stationary asymptotically flat $I^+$-regular analytic vacuum spacetimes: a rotating component gives axisymmetry; the area–angular-momentum relation [21], combined with the balance result of Han–Khuri–Weinstein–Xiong [18], yields conical singularities on every finite axis interval between horizons, contrary to regularity; [32] treats two-hole configurations. If all components are non-rotating and non-degenerate, maximal-slice staticity and Bunting–Masood-ul-Alam [9] give Schwarzschild. If all are non-rotating and some is degenerate, it cites exclusion by [22].

Under these stationary asymptotically flat $I^+$-regular analytic vacuum hypotheses, a nonempty future horizon is therefore connected; no extra common nondegeneracy, nonzero total angular momentum, global maximal slice or a priori mixed-rod-map assumption is added. The asymptotic and causal terminology is made explicit in [[def-author-ae62588ad46a-analytic-geometric-data]]. This does not assert the corresponding smooth nonanalytic statement.

## Facts & Assumptions

[A1] Adopt [[post-stationary-vacuum-model]] and the exact analytic comparison hypotheses [[def-author-ae62588ad46a-analytic-geometric-data]]. Work in ZFC, [[math:def-axiom-of-choice]]. Multiple black holes means more than one connected horizon component.

[F1] The external stationary normal form is [[thm-author-ae62588ad46a-stationary-asymptotic-normal-form]]. Its local slice calculation and invariance of cofinal end causal sets are [[lem-author-ae62588ad46a-canonical-end-slice]] and [[lem-author-ae62588ad46a-cofinal-end-causal-sets]]. The local ADM calculation in [[pthm-author-ae62588ad46a-analytic-geometric-classification-input]], Proof 1.1–2.1, identifies the leading coefficient as $M_{\rm ADM}=m$ on this same canonical end. It uses the differentiated spatial expansion and the stronger $k=o_2(r^{-2})$ estimate proved in the canonical-slice supplier’s Proof 2.1, under the ADM surface-definition falloffs recorded in that calculation. Together these inputs match the exact source (H1)–(H3) convention without imposing a global maximal slice or changing the DOC.

[F2] For comparison with the article’s case split, [[lem-author-ae62588ad46a-horizon-case-partition]] partitions a horizon only when its componentwise labels and their defining data have been supplied. Likewise [[lem-author-ae62588ad46a-positive-area-nonzero-angular-momentum]] uses a supplied smooth compact spacelike section and the stated area equality. The separate rotating connectedness, non-rotating degenerate exclusion and all-nonrotating/nondegenerate Schwarzschild statements are imported in [[pthm-author-ae62588ad46a-analytic-geometric-classification-input]], using its [F7] source terminology and horizon preparation. The auxiliary comparisons in steps 2.1–2.3 additionally require a componentwise label correspondence on the same future horizon: with the same stationary field $T$ and null-generator lines, the local rotation predicate agrees with Huang–Li–Zhu Definition 1.3; on each component the supplied local Killing generator has vanishing surface gravity if and only if the source-defined surface gravity in Definition 1.4 vanishes. Local nondegeneracy and source nondegeneracy then also agree. This correspondence is an explicit premise of these auxiliary comparisons only. Neither the existence of local component data nor their correspondence with the source labels is inferred from the base geometric hypotheses. The general connectedness application in step 3.1 requires neither premise.

[F3] Independently of the local component-label interface, the full geometric connectedness conclusion of Huang–Li–Zhu’s §1 classification discussion is imported in External input below. Its hypotheses are (H1)–(H3), analyticity and vacuum; it has no extra component-label assumption. The general Corollary is already recorded in [[pthm-author-ae62588ad46a-analytic-geometric-classification-input]]; the precise connectedness conclusion used here is the whole preceding classification discussion, not a boundary-extension deduction from DOC isometry alone.

## Proof

**Given:**The original analytic stationary vacuum comparison geometry, a nonempty horizon and [A1]–[F3].

**Goal:** Exclude more than one horizon component without assuming all components have the same rotation or degeneracy type.

1.1 Apply the stationary normal-form input on a sufficiently far-out end. The canonical-slice calculation gives $h=(1+2m/r)\delta+o_2(r^{-1})$ and $k=o_2(r^{-1})$. Apply the ADM calculation in [F1] to this same Cartesian end: its spatial remainder is $o_2(r^{-1})$ and its stronger $k=o_2(r^{-2})$ estimate verifies the stated ADM falloffs. That calculation yields $M_{\rm ADM}=m$, so the spatial expansion has exactly the ADM-mass coefficient required in (H1), as well as its differentiated decay. Cofinal end invariance keeps the same chronological sets, DOC and horizon. The section-deformation conclusion supplied in [F1] supplies an acausal section containing the canonical end and retaining its compact horizon cross-section; equality of chronological sets alone is not used to supply that section. Completeness and timelikeness are the supplied stationary hypotheses, while analyticity and vacuum are unchanged. Thus the exact geometric source hypotheses (H1)–(H3) hold in an allowed end representation. [given, A1, F1]

2.1 For this conditional comparison, suppose both the local component data and the componentwise label correspondence required in [F2] are supplied, and consider local case (R). The correspondence gives a rotating component in the source terminology, so use the explicitly stated rotating geometric consequence in [F2]. It supplies global axisymmetry and connectedness for the regular analytic geometry, without an a priori connectedness assumption. On each component degenerate under the matched labels, apply the source’s area equality to its own angular-momentum scalar and supplied smooth compact spacelike cross-section. The arbitrary-scalar implication in the positive-area supplier then shows that this source angular momentum is nonzero. This use does not identify it with a separately normalized local Komar functional and does not require nonzero total angular momentum. The quantitative negative rod defects remain the narrow balance theorem’s stated mechanism in its own map class; here the global geometric consequence is imported directly, rather than treating a bare regular axisymmetric geometry as an already verified map-class input. Hence more than one horizon component is impossible in case (R). [given, F2, step 1.1]

2.2 Under the same local-component-data and label-correspondence premises in [F2], local case (N) says every component is non-rotating and nondegenerate. The correspondence makes every component non-rotating and nondegenerate in the source terminology as well. Apply the exact multi-component staticity/Schwarzschild consequence in [F2]. Its geometric source statement already includes the required maximal-slice and static-classification preparation; that substantial input is imported, not replaced by the local single-bifurcation-sphere statement. Its connected Schwarzschild horizon excludes more than one horizon component. [given, F2, step 1.1]

2.3 Under the same local-component-data and label-correspondence premises in [F2], local case (D) says all components are non-rotating and some is degenerate. The correspondence supplies a component that is both non-rotating and degenerate in the source terminology. The Main Theorem in [F2] excludes even one such source-labelled component, including in a possibly disconnected horizon. It therefore excludes this case entirely. [given, F2, step 1.1]

3.1 The partition lemma makes the local cases (R), (N), (D) exhaustive when the component data are supplied. Under the additional componentwise label correspondence in [F2], steps 2.1–2.3 apply the respective source conclusions, preserving the article’s case-split explanation, including mixed degeneracy. These auxiliary calculations establish neither the existence of local component data nor their correspondence with the source labels. For the unconditional conclusion under the Statement’s hypotheses, apply instead the full geometric connectedness input [F3]: step 1.1 supplies its exact source hypotheses on the same geometry and preserves its horizon. That imported conclusion directly excludes more than one component. No premise about a locally specified Killing generator or surface-gravity normalization, and no smooth nonanalytic result, is used in this application. [given, A1, F2, F3, step 1.1, step 2.1, step 2.2, step 2.3] ∎



The first Statement paragraph preserves the original article §1.3, PDF p.5, as attribution. The proof uses independent sources. The former escalation asked for a reconstruction of the geometric-to-HKWX map-class bridge. The rotating connectedness conclusion is explicitly stated immediately after HKWX Theorem 1.1 and in Huang–Li–Zhu’s §1 classification discussion. The latter discussion also supplies the all-nonrotating branches used here. Huang–Li–Zhu’s final Corollary states that the DOC is isometric to Kerr without assuming horizon connectedness; connectedness here is imported from the preceding classification discussion, not inferred from extending that DOC isometry. Those geometric classification statements are used at their stated hypotheses. The narrower completed rod-data supplier remains valid in its own class; it is not silently upgraded into a proof that a generic geometry satisfies every (A1)–(A3) condition. This deliberate source-level departure avoids claiming an unperformed global reduction. The source's exact end convention is separately matched rather than silently imposing a stronger original asymptotic hypothesis. No mathematical review, source-proof reconstruction or defect in the original article is claimed.

## Source notes

The first Statement paragraph preserves the original article §1.3, PDF p.5, as attribution. The proof uses independent sources. The former escalation asked for a reconstruction of the geometric-to-HKWX map-class bridge. The rotating connectedness conclusion is explicitly stated immediately after HKWX Theorem 1.1 and in Huang–Li–Zhu’s §1 classification discussion. The latter discussion also supplies the all-nonrotating branches used here. Huang–Li–Zhu’s final Corollary states that the DOC is isometric to Kerr without assuming horizon connectedness; connectedness here is imported from the preceding classification discussion, not inferred from extending that DOC isometry. Those geometric classification statements are used at their stated hypotheses. The narrower completed rod-data supplier remains valid in its own class; it is not silently upgraded into a proof that a generic geometry satisfies every (A1)–(A3) condition. This deliberate source-level departure avoids claiming an unperformed global reduction. The source's exact end convention is separately matched rather than silently imposing a stronger original asymptotic hypothesis. No mathematical review, source-proof reconstruction or defect in the original article is claimed.

## External input

Under (H1)–(H3), analyticity and vacuum, the full multiple-horizon classification in Huang–Li–Zhu §1 excludes disconnected nonempty future horizons. This is the imported geometric conclusion used in [F3]; its exact scope and reading limits are recorded in sources.references. The local proof matches the source hypotheses and applies this conclusion. It does not reconstruct the source’s horizon preparation or claim that the local definition alone supplies component data.
