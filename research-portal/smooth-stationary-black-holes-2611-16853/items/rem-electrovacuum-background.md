---
id: rem-electrovacuum-background
title: Reported analytic and smooth electrovacuum uniqueness literature
kind: remark
status: published
origin: pipeline
domain: physics
deps:
  - def-source-free-geometric-electrovacuum-data
  - def-black-hole-comparison-hypothesis-data
  - physics:def-gr-killing-field
  - math:def-axiom-of-choice
dependency_roles:
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  def-black-hole-comparison-hypothesis-data: mathematical-premise
  physics:def-gr-killing-field: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 3, §1.1, final paragraph; bibliography entries 8, 13, 28, 30 and
        42
      statement: The article mentions stationary electrovacuum black-hole uniqueness
        results in the analytic case, citing references 8, 13 and 30, and in the
        smooth case, citing references 28 and 42.
      hypotheses: The passage does not state a complete theorem or a common list of
        hypotheses for the cited works.
      reading_limits: Read the frozen article text at the indicated passage and
        bibliography entries. The cited works were not independently read for
        this item; their results and proofs are not imported here.
physical_scope: Literature context for stationary black holes in
  four-dimensional source-free Einstein–Maxwell theory; the remark reports the
  article's attribution and states no observation or unconditional uniqueness
  theorem.
dependency_level: 5
---

## Statement

The article mentions uniqueness results for stationary electrovacuum black holes in the analytic case, citing its references [8, 13, 30], and in the smooth case, citing [28, 42]. The passage does not give a complete common theorem or hypothesis list for those works. In particular, this report does not assert that every smooth stationary electrovacuum black hole is uniquely determined without further hypotheses.

For the terminology used here, source-free geometric electrovacuum data comprise a smooth time-oriented and oriented Lorentzian four-manifold with a smooth real two-form $F$ satisfying $dF=0$, $d(\star_g F)=0$, and $\operatorname{Ric}_{ab}=2(F_{ac}F_b{}^c-\tfrac14 g_{ab}F_{cd}F^{cd})$, in the stated geometric normalization. In the asymptotically flat black-hole setting used here, stationarity relative to a selected asymptotically flat spacelike end means that a specified Killing field is future timelike on a sufficiently distant tail of that end. The local flow of a Killing field preserves the metric wherever defined. Analytic means that the metric is represented locally by convergent real power series in a compatible real-analytic atlas; smooth means $C^\infty$. A uniqueness result identifies solutions within the class and under the hypotheses specified by that result. The precise horizon, regularity, field and asymptotic hypotheses must therefore be read separately for each cited result. The geometric suppliers use the Axiom of Choice.

## Statement references

[[def-source-free-geometric-electrovacuum-data]]

[[def-black-hole-comparison-hypothesis-data]]

[[physics:def-gr-killing-field]]

[[math:def-axiom-of-choice]]

## Source notes

References [8] and [30] in the article are works by Bunting and Mazur; [13] is the review by Chruściel, Costa and Heusler. References [28] and [42] are works by Lai, Li and Yu, and by Yu, respectively. These are bibliographic identifications from the article, not independent verification of their theorem statements or proofs. The citation to the article supplies attribution for the report above; it is not a proof of electrovacuum uniqueness.
