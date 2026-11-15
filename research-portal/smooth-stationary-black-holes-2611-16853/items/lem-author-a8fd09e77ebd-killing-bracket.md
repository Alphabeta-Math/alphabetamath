---
id: lem-author-a8fd09e77ebd-killing-bracket
title: The bracket of two Killing fields is Killing
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - math:def-lie-bracket-of-smooth-vector-fields
  - math:prop-coordinate-formula-for-the-lie-bracket
  - math:def-lie-derivative-of-a-tensor-field
  - math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor
  - math:thm-clairaut-schwarz-mixed-partials
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  math:def-lie-bracket-of-smooth-vector-fields: mathematical-premise
  math:prop-coordinate-formula-for-the-lie-bracket: mathematical-premise
  math:def-lie-derivative-of-a-tensor-field: mathematical-premise
  math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor: mathematical-premise
  math:thm-clairaut-schwarz-mixed-partials: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

On a smooth Lorentzian manifold in the conventions of [[def-stationary-lorentzian-data]], the bracket $[X,Y]$ of two smooth Killing fields is a Killing field. The bracket is the commutator defined in [[math:def-lie-bracket-of-smooth-vector-fields]].

## Facts & Assumptions

[F1] A Killing field has zero metric Lie derivative, defined through its local flow. [[def-stationary-lorentzian-data]]

[F2] The bracket acts by $[X,Y]u=X(Yu)-Y(Xu)$ on smooth scalar functions. [[math:def-lie-bracket-of-smooth-vector-fields]]

[F3] The commutator is a globally defined smooth vector field, with coordinate components $[X,Y]^a=X^b\partial_bY^a-Y^b\partial_bX^a$. [[math:prop-coordinate-formula-for-the-lie-bracket]]

[F4] For any smooth tensor field $S$, the Lie derivative $\mathcal L_VS$ is defined by differentiating its pullback under the local flow of the smooth field $V$. [[math:def-lie-derivative-of-a-tensor-field]]

[F5] For every smooth covariant two-tensor $S$, the coordinate formula is $(\mathcal L_VS)_{ij}=V^a\partial_aS_{ij}+S_{aj}\partial_iV^a+S_{ia}\partial_jV^a$. [[math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor]]

[F6] For a $C^2$ scalar function on an open subset of $\mathbb R^m$, mixed second partial derivatives commute. [[math:thm-clairaut-schwarz-mixed-partials]]

## Proof

**Given:**Smooth fields $X,Y$ with $\mathcal L_Xg=\mathcal L_Yg=0$.

**Goal:** Prove $\mathcal L_{[X,Y]}g=0$.

1.1 By the smooth bracket construction, $B=[X,Y]$ is a smooth vector field. The tensor Lie derivative applies to $g$ and to the smooth covariant two-tensors $\mathcal L_Xg$ and $\mathcal L_Yg$; its flow definition agrees with the metric Lie derivative in the Killing condition. Thus both iterated derivatives and $\mathcal L_Bg$ are defined. [F1, F3, F4, F5]

2.1 Substitute the formula $(\mathcal L_VS)_{ij}=V^a\partial_aS_{ij}+S_{aj}\partial_iV^a+S_{ia}\partial_jV^a$ twice into $\mathcal L_X\mathcal L_Yg-\mathcal L_Y\mathcal L_Xg$. The smooth metric and vector-field coordinate components are $C^2$ on each chart, so their mixed second partial derivatives commute. The mixed second metric derivatives cancel. The coefficients of $\partial_ag_{ij}$ become $B^a=X^b\partial_bY^a-Y^b\partial_bX^a$, and the coefficients multiplying $g_{aj}$ and $g_{ia}$ are $\partial_iB^a$ and $\partial_jB^a$, respectively. The remaining terms cancel in pairs. By the same formula applied to $B$, this is exactly $\mathcal L_Bg$. [F3, F5, F6, step 1.1, algebra]

3.1 Both iterated Lie derivatives vanish because each inner derivative of $g$ vanishes and the coordinate formula sends the zero tensor to zero. The identity in step 2.1 therefore gives $\mathcal L_{[X,Y]}g=0$, so the smooth bracket field is Killing. [F1, F5, step 1.1, step 2.1] ∎
