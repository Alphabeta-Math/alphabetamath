---
id: lem-author-cea8e61dc3c6-killing-exact-two-form
title: The Killing derivative is an exact closed two-form
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - physics:lem-emg-lorentz-hodge-calculus
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  physics:lem-emg-lorentz-hodge-calculus: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Lecture Notes on General Relativity
      url: https://arxiv.org/pdf/gr-qc/9712019
      locator: §5, equations (5.41)–(5.42), PDF p. 147
      statement: The vanishing Lie derivative of the metric is equivalent to the
        Killing equation.
      hypotheses: A smooth metric and its Levi–Civita connection.
      reading_limits: Read the cited Killing equations. The exactness and closure
        consequences are proved locally in this item.
dependency_level: 1
---

## Statement

For the stationary Lorentzian data, put $\alpha=T^\flat$ and $F_{ab}=\nabla_aT_b$. Then $F_{ab}=-F_{ba}$, $F=\tfrac12d\alpha$ and $dF=0$. Here a two-form has coordinate expansion $F=\tfrac12F_{ab}dx^a\wedge dx^b$.

## Facts & Assumptions

[F1] The metric, Killing field, local flow and torsion-free metric connection are those of [[def-stationary-lorentzian-data]].

[F2] Exterior differentiation has its coordinate formula and satisfies $d^2=0$. [[physics:lem-emg-lorentz-hodge-calculus]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove all asserted identities under these hypotheses.

1.1 In a coordinate chart, the derivative of the flow pullback is $(\mathcal L_Tg)_{ab}=T^c\partial_cg_{ab}+g_{cb}\partial_aT^c+g_{ac}\partial_bT^c$. Metric compatibility and symmetry of the Christoffel symbols rewrite this as $\nabla_aT_b+\nabla_bT_a$. The Killing condition makes this sum zero, so $F$ is alternating. [F1, algebra]

2.1 Torsion freedom gives $(d\alpha)_{ab}=\partial_aT_b-\partial_bT_a=\nabla_aT_b-\nabla_bT_a=2F_{ab}$. Applying $d$ once more gives $dF=\tfrac12d^2\alpha=0$. [step 1.1, F1, F2, algebra] ∎

## External input

The cited Killing equation supplies background for the local exactness calculation.
