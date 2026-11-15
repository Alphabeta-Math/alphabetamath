---
id: lem-author-c92bdd91a36e-compatible-jet-limit
title: Passing a local Harrison identity through compatible stationary jets
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-complex-self-dual-two-form-data
  - def-source-free-geometric-electrovacuum-data
  - lem-author-c92bdd91a36e-residual-jet-continuity
  - lem-author-c92bdd91a36e-stationary-local-jets
  - math:thm-metric-continuity-characterisations
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  lem-author-c92bdd91a36e-residual-jet-continuity: mathematical-premise
  lem-author-c92bdd91a36e-stationary-local-jets: mathematical-premise
  math:thm-metric-continuity-characterisations: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references: []
dependency_level: 5
---

## Statement

Fix a parameter $q\in[0,1]$ and one oriented stationary coordinate representation $(t,x^1,x^2,x^3)$ with $T=\partial_t$. Let $J$ and $J_n$ be stationary two-jets of $(g,\psi,W_0)$, where $g$ is Lorentzian, $\psi$ is a real scalar and $W_0$ is a real one-form. Their component values and coordinate derivatives through order two, with all time-containing derivatives zero, are compared in the same finite-dimensional real coordinate space with its Euclidean metric. Suppose $J_n\to J$ in this space.

Use the algebraic Harrison residuals $(E,M,P)$ and the quantities $D_q,W_q$ of the residual-continuity interface, with this same fixed $q$ throughout. Assume $D_q>0$ and $D_q+W_q(T)>0$ at $J$ and every $J_n$, that each $J_n$ has $f_n=-g_n(T,T)>0$, that $J$ and all $J_n$ carry the same normalization label $d_0$, and that all three transformed Einstein–Maxwell residuals vanish at every $J_n$. Then the transformed residuals also vanish at $J$. These two-jets need not be realized by vacuum solutions on any common open set.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-complex-self-dual-two-form-data]]

[[def-source-free-geometric-electrovacuum-data]]

[[lem-author-c92bdd91a36e-stationary-local-jets]]

[[lem-author-c92bdd91a36e-residual-jet-continuity]]

## Facts & Assumptions

[F1] Metric, form and electrovacuum conventions use [[def-stationary-lorentzian-data]], [[def-complex-self-dual-two-form-data]] and [[def-source-free-geometric-electrovacuum-data]].

[F2] For each fixed $q\in[0,1]$, the three algebraically extended residuals are continuous finite-dimensional functions of the stationary two-jet on the domain $D_q>0$, $D_q+W_q(T)>0$ by [[lem-author-c92bdd91a36e-residual-jet-continuity]]. That supplier also specifies the normalization label $d_0$; restricting to compatible jets with a fixed label preserves this continuity.

[F3] Stationary two-jets are the component lists described in [[lem-author-c92bdd91a36e-stationary-local-jets]], including the stationary scalar and one-form and all derivatives through order two. Here the same oriented coordinate representation is fixed for every list, so convergence means convergence in that finite-dimensional Euclidean space.

[F4] A continuous map between metric spaces sends a convergent sequence to a sequence converging to the image of its limit. Use only the choice-free implication (a) to (d) of [[math:thm-metric-continuity-characterisations]], applied to the positive-domain jet space with the restricted Euclidean metric and to the real line.

## Proof

**Given:** The fixed parameter, common stationary coordinate representation, convergent jets, positivity, normalization and vanishing hypotheses in the Statement.

**Goal:** Show that all three transformed residuals vanish at the limit jet without requiring realizations by vacuum solutions on a common open set.

1.1 Fix one coordinate component of any of the three residual tensors, using the fixed representation of [F3] and the conventions of [F1]. On the positive-domain jet space this component is a continuous real-valued function $R$ by [F2]. The hypotheses place $J$ and all $J_n$ in that domain, with the same $q\in[0,1]$, and give $J_n\to J$ in its restricted Euclidean metric. Thus [F4] applies and gives $R(J_n)\to R(J)$. [given, F1, F2, F3, F4]

2.1 The assumed vanishing gives $R(J_n)=0$ for every $n$. Consequently $R(J)=0$: if $R(J)\ne0$, convergence from step 1.1 with $\varepsilon=|R(J)|/2>0$ would give $|R(J_n)-R(J)|<|R(J)|/2$ eventually, whereas the left side equals $|R(J)|$. Since the component was arbitrary, every component of all three residual tensors vanishes at $J$. [given, step 1.1]

3.1 The argument uses evaluations of the residual functions on lists of values and derivatives at a single point, rather than convergence of spacetime solutions. Consequently no realization by local vacuum metrics, convergence on an open region or density of timelike points in the original metric is needed. Existence of the compatible sequence and the identity on its jets remain separate explicit hypotheses; this lemma does not establish either. [given, F2, F3, step 1.1, step 2.1] ∎
