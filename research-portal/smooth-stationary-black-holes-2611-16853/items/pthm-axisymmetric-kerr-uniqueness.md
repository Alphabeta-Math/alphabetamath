---
id: pthm-axisymmetric-kerr-uniqueness
title: Axisymmetric vacuum uniqueness with complete global hypotheses
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-kerr-metric
  - def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data
  - def-black-hole-comparison-hypothesis-data
  - lem-author-69e1abcd87be-stationary-causal-exterior-invariance
  - lem-author-69e1abcd87be-axial-stationary-field-invariance
  - lem-author-69e1abcd87be-regular-axis-elementary-flatness
  - lem-author-69e1abcd87be-exact-global-regularity-assembly
  - lem-author-69e1abcd87be-vacuum-zero-maxwell-embedding
  - math:def-axiom-of-choice
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-kerr-metric: mathematical-premise
  def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data: mathematical-premise
  def-black-hole-comparison-hypothesis-data: mathematical-premise
  lem-author-69e1abcd87be-stationary-causal-exterior-invariance: mathematical-premise
  lem-author-69e1abcd87be-axial-stationary-field-invariance: mathematical-premise
  lem-author-69e1abcd87be-regular-axis-elementary-flatness: mathematical-premise
  lem-author-69e1abcd87be-exact-global-regularity-assembly: mathematical-premise
  lem-author-69e1abcd87be-vacuum-zero-maxwell-embedding: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
physical_scope: Conditional classical four-dimensional smooth vacuum Einstein
  model with zero cosmological constant; classification concerns its entire
  domain of outer communications, not arbitrary extensions.
sources:
  references:
    - title: "P. T. Chruściel, J. L. Costa and M. Heusler, Stationary Black Holes:
        Uniqueness and Beyond"
      url: https://arxiv.org/pdf/1205.6112
      locator: §3.2.7 Theorem 3.2, p.15; vacuum Kerr specialization in §3.2.4, p.15;
        no-analyticity distinction in §3.3.1, p.16; definitions §2.1 and §2.3,
        p.5 and Definition2.1, pp.10–11; global axisymmetric framework §3.2.1,
        p.13
      statement: "Theorem3.2: a stationary, axisymmetric, asymptotically flat,
        $I^+$-regular electrovacuum four-dimensional spacetime has domain of
        outer communications isometric to a Weinstein solution; if the event
        horizon is connected, it is the domain of outer communications of
        Kerr–Newman. The vacuum case is the Kerr uniqueness conclusion in
        §3.2.4. Section3.3.1 states explicitly that this axisymmetric theorem
        requires no analyticity."
      hypotheses: Four-dimensional smooth spacetime; complete stationary Killing flow
        timelike at the selected asymptotically flat end; global
        stationary-axisymmetric structure, not a merely local Killing field;
        full I-plus-regularity of Definition2.1; vacuum specialization and
        connected event horizon. The local item assumes an effective commuting
        axial circle action with regular axis explicitly. Nondegeneracy is not a
        hypothesis of Theorem3.2. There is no additional unspecified orbit-space
        assumption in its stated theorem; the global reduction and
        reconstruction are part of the imported classification.
      reading_limits: Read the specified definitions, theorem statement and adjacent
        discussions from the downloaded full PDF, visually inspected p.15. Did
        not read or reconstruct the cited primary Robinson, Carter, Bunting,
        Weinstein or global orbit-space proofs. The full exterior classification
        is accepted as an external established input; the five local helpers
        prove only elementary prerequisite bridges. The source itself is a
        review theorem, not a newly reconstructed proof.
dependency_level: 7
---

## Statement

Adopt the smooth four-dimensional classical stationary vacuum model $\operatorname{Ric}(g)=0$ with zero cosmological constant. Assume the exact smooth global axisymmetric comparison data relative to the selected asymptotically flat end: the stationary Killing flow is complete on $M$ and timelike near that end; there is a global effective isometric axial circle action of period $2\pi$ commuting with that flow and with the specified regular axis; the entire exterior $D=I_M^+(M_{\rm ext})\cap I_M^-(M_{\rm ext})$ is $I^+$-regular in the full stated sense; and its event horizon is connected. Then $D$, with its metric, is isometric to the domain of outer communications of a Kerr spacetime in the convention of the Kerr definition.

No analyticity is required for this already axisymmetric classification. It concerns the entire exterior, not merely a neighborhood of the horizon or a reduced potential, and asserts no classification of arbitrary extensions beyond the exterior. A global axial action is a hypothesis: existence of a local horizon Killing field alone does not satisfy it. If mean-nondegeneracy or nondegeneracy is also imposed in an application, retain that separate hypothesis; the imported axisymmetric theorem does not need it, and no mean-to-pointwise nondegeneracy inference is made. The complete source theorem imposes no additional unspecified orbit-space hypotheses beyond its stated global assumptions.

## Facts & Assumptions

[F1] Adopt the classical stationary vacuum equation and asymptotic normalization as model assumptions, not as observations or existence conclusions. [[post-stationary-vacuum-model]]

[F2] The Kerr definition fixes the exterior metric, parameter and horizon conventions, including both subextremal and extremal possibilities. [[def-kerr-metric]]

[F3] Assume the complete global axisymmetric comparison data, with connected event horizon and any separately retained optional mean condition. [[def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data]]

[F4] The full global end, regular axis, I-plus-regularity and separate nondegeneracy predicates are explicit. [[def-black-hole-comparison-hypothesis-data]]

[F5] The complete stationary flow acts on the whole selected causal exterior. [[lem-author-69e1abcd87be-stationary-causal-exterior-invariance]]

[F6] Commutation makes the axial action preserve the selected stationary field and its causal character. [[lem-author-69e1abcd87be-axial-stationary-field-invariance]]

[F7] The assumed smooth weight-one regular axis has the elementary-flatness normalization. [[lem-author-69e1abcd87be-regular-axis-elementary-flatness]]

[F8] The global I-plus-regularity hypothesis expands to the exact full source predicate, with no quotient-coordinate placeholder. [[lem-author-69e1abcd87be-exact-global-regularity-assembly]]

[F9] The adopted vacuum model is the zero-Maxwell-field specialization of the stationary electrovacuum equations and asymptotic field conditions. [[lem-author-69e1abcd87be-vacuum-zero-maxwell-embedding]]

[F10] Work in ZFC, retaining the mathematical suppliers' choice assumptions. [[math:def-axiom-of-choice]]

[F20] Use the imported connected-horizon vacuum axisymmetric classification with its complete stated hypotheses, as recorded in External input.

## Proof

**Given:** The data and assumptions in the Statement.

**Goal:** Establish the claimed conditional conclusion.

1.1 The model assumption [F1] and bridge [F9] place the given metric in the vacuum specialization of the source framework. The complete end, time orientation, stationary flow, global axial action and connected horizon are supplied by [F3] and [F4]. The stationary and axial actions have the global identities in [F5] and [F6]; the regular axis uses the normalization in [F7]. The expanded $I^+$-regularity predicate in [F8] agrees clause for clause with source Definition2.1, including the finite-end completion and once-only generator condition. [given, F1, F3, F4, F5, F6, F7, F8, F9, F10]

2.1 Apply the imported connected-horizon axisymmetric classification [F20], using its vacuum Kerr case from §3.2.4. It supplies an isometry of the entire domain of outer communications to a Kerr exterior, with the metric convention identified by [F2]. The source's §3.3.1 explicitly separates the analytic rigidity/globalization argument from this already axisymmetric theorem, which needs no analyticity. Hence this application neither proves nor assumes an extension of an arbitrary local field. [F20, F2, step 1.1]

3.1 The conclusion in step 2.1 is for the exact exterior $D$ appearing in [F8]. It supplies no claim about extensions beyond that domain. Adding an independently imposed mean-nondegeneracy or nondegeneracy hypothesis does not obstruct the implication, because the classification just applied already holds without it; this observation does not identify the two predicates. All stated global and local distinctions are therefore preserved. [step 2.1, F3, F4, F8, given] ∎

## External input

Imported established classification: Theorem3.2: a stationary, axisymmetric, asymptotically flat, $I^+$-regular electrovacuum four-dimensional spacetime has domain of outer communications isometric to a Weinstein solution; if the event horizon is connected, it is the domain of outer communications of Kerr–Newman. The vacuum case is the Kerr uniqueness conclusion in §3.2.4. Section3.3.1 states explicitly that this axisymmetric theorem requires no analyticity. Hypotheses: Four-dimensional smooth spacetime; complete stationary Killing flow timelike at the selected asymptotically flat end; global stationary-axisymmetric structure, not a merely local Killing field; full I-plus-regularity of Definition2.1; vacuum specialization and connected event horizon. The local item assumes an effective commuting axial circle action with regular axis explicitly. Nondegeneracy is not a hypothesis of Theorem3.2. There is no additional unspecified orbit-space assumption in its stated theorem; the global reduction and reconstruction are part of the imported classification. Reading limits: Read the specified definitions, theorem statement and adjacent discussions from the downloaded full PDF, visually inspected p.15. Did not read or reconstruct the cited primary Robinson, Carter, Bunting, Weinstein or global orbit-space proofs. The full exterior classification is accepted as an external established input; the five local helpers prove only elementary prerequisite bridges. The source itself is a review theorem, not a newly reconstructed proof.

## Source notes

Original article attribution: The uniqueness of smooth stationary black holes, arXiv:2611.16853v1, §1.1, PDF p.2, Carter–Bunting/Robinson discussion. That paragraph reports the stationary-axisymmetric Kerr conclusion and says its final uniqueness step does not require analyticity. It is retained as attribution only; the independent CCH theorem supplies the classification. The ambiguous generated supplier phrase about additional unspecified orbit-space hypotheses is not used as a premise. Its original item and authentic history remain untouched. The five local prerequisite lemmas establish only the stated elementary bridges; no orbit-space topology, harmonic-map uniqueness or global reconstruction is claimed locally.
