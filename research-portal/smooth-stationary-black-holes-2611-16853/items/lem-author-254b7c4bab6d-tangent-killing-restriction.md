---
id: lem-author-254b7c4bab6d-tangent-killing-restriction
title: A branch-tangent Killing field restricts to the bifurcation sphere
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-author-254b7c4bab6d-regular-null-horizon-pair
  - def-stationary-lorentzian-data
  - math:cor-transverse-intersection-theorem
  - math:prop-a-vector-field-tangent-to-an-embedded-submanifold-restricts-to-a-vector-field
  - math:def-embedded-submanifold-and-slice-chart
  - math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor
dependency_roles:
  def-author-254b7c4bab6d-regular-null-horizon-pair: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  math:cor-transverse-intersection-theorem: mathematical-premise
  math:prop-a-vector-field-tangent-to-an-embedded-submanifold-restricts-to-a-vector-field: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

For the transverse branch pair in [[def-author-254b7c4bab6d-regular-null-horizon-pair]], let $T$ be a smooth ambient Killing field tangent to each branch. Then $T|_S$ is tangent to $S$ and is Killing for the Riemannian induced metric $\gamma=g|_{TS}$. Nontriviality on $S$ means $T|_S\not\equiv0$ and allows isolated zeroes. Use the Killing and metric conventions in [[def-stationary-lorentzian-data]].

## Facts & Assumptions

[F1] The horizon pair supplies smooth embedded transverse branches $H_1,H_2$ with intersection the embedded spacelike sphere $S$ and induced positive metric $\gamma=g|_{TS}$. The stationary-data conventions define the ambient Killing equation $\mathcal L_Tg=0$ using the local-flow Lie derivative. [[def-author-254b7c4bab6d-regular-null-horizon-pair]] [[def-stationary-lorentzian-data]]

[F2] For transverse embedded submanifolds, the tangent space of their intersection is the intersection of their tangent spaces. Applied to these branches, $T_pS=T_pH_1\cap T_pH_2$. [[math:cor-transverse-intersection-theorem]]

[F3] A smooth ambient vector field tangent to an embedded submanifold restricts to a smooth vector field on it. [[math:prop-a-vector-field-tangent-to-an-embedded-submanifold-restricts-to-a-vector-field]]

[F4] An embedded submanifold admits slice charts in which it is the coordinate slice with all normal coordinates zero. [[math:def-embedded-submanifold-and-slice-chart]]

[F5] For a smooth covariant two-tensor $h$ and vector field $V$, the local-flow Lie derivative has components $(\mathcal L_Vh)_{ij}=V^k\partial_kh_{ij}+h_{kj}\partial_iV^k+h_{ik}\partial_jV^k$. This formula applies to both $g$ on the ambient manifold and $\gamma$ on $S$; it imposes no signature restriction. [[math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor]]

## Proof

**Given:** The transverse pair and branch-tangent Killing field.

**Goal:** Establish tangency and the intrinsic Killing equation.

1.1 For $p\in S$, branch tangency gives $T_p\in T_pH_1\cap T_pH_2=T_pS$ by the transverse-intersection theorem. Since $S$ is embedded and $T$ is smooth, the restriction theorem gives a smooth field $A=T|_S$ on $S$. [given, F1, F2, F3]

2.1 Fix $p\in S$ and take a slice chart $(x^1,x^2,x^3,x^4)$ around $p$ with $S$ given by $x^3=x^4=0$. Tangential indices $a,b,c$ range over $1,2$ and normal indices $\mu$ over $3,4$. On the slice, $A^a=T^a|_S$ and $\gamma_{ab}=g_{ab}|_S$. Tangency gives $T^\mu|_S=0$, so differentiating this identically zero function in each tangential coordinate gives $(\partial_aT^\mu)|_S=0$. [F1, F4, step 1.1]

3.1 Apply the covariant two-tensor coordinate formula first on $S$ and then in the ambient chart. With $c$ summed over $1,2$, it gives $(\mathcal L_A\gamma)_{ab}=\left.(T^c\partial_cg_{ab}+g_{cb}\partial_aT^c+g_{ac}\partial_bT^c)\right|_S=\left.(\mathcal L_Tg)_{ab}\right|_S=0$. Indeed, the additional normal-index terms in the ambient formula vanish by $T^\mu|_S=0$ and $(\partial_aT^\mu)|_S=(\partial_bT^\mu)|_S=0$. Thus $\mathcal L_A\gamma=0$ in every such chart, and $A$ is Killing for the induced Riemannian metric. Nontriviality means $A\not\equiv0$ and does not require $A$ to be nowhere zero. [F1, F5, step 1.1, step 2.1] ∎
