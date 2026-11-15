---
id: lem-author-84ac8de0c2f0-positive-parameter-end-normalization
title: Positive-parameter normalized time and spatial ends
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-asymptotic-decay-data
  - lem-author-84ac8de0c2f0-end-denominator-bounds
  - lem-author-84ac8de0c2f0-weighted-one-form-decay
  - lem-author-84ac8de0c2f0-spatial-harrison-end
  - def-harrison-one-form
  - def-harrison-normalization
dependency_roles:
  def-stationary-asymptotic-decay-data: mathematical-premise
  lem-author-84ac8de0c2f0-end-denominator-bounds: mathematical-premise
  lem-author-84ac8de0c2f0-weighted-one-form-decay: mathematical-premise
  lem-author-84ac8de0c2f0-spatial-harrison-end: mathematical-premise
  def-harrison-one-form: mathematical-premise
  def-harrison-normalization: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 8
---

## Statement

Use the same family, including the contraction $W_q(T)=d_q-D_q$, and let $q>0$. The exact coordinate change
$$t_q=\frac{d_q}{4q}t,\qquad x_q=qx,\qquad r_q=qr$$
gives
$$(g_q)_{t_qt_q}=-1+O_5(r_q^{-1}),\quad (g_q)_{t_qx_q^i}=O_5(r_q^{-2}),\quad (g_q)_{x_q^ix_q^j}=\delta_{ij}+O_5(r_q^{-1}).$$
The constants and a common end radius may be chosen uniformly on $q\in[\delta,1]$ for any fixed $\delta>0$. No uniform normalized end at $q=0$ is asserted. Since $d_q$ is bounded above and away from zero, $t_q$ has the scale $t/q$ (meaning that its coefficient relative to $t/q$ is bounded above and below by positive constants). A fixed normalized radius $r_q=R$ corresponds to original radius $r=R/q$, which tends to infinity as $q\downarrow0$.

## Facts & Assumptions

[F1] [[def-stationary-asymptotic-decay-data]] defines fixed-chart differentiated bounds and parameter uniformity. [[lem-author-84ac8de0c2f0-end-denominator-bounds]] gives the denominator expansion, the pole constant bounds and the mass-one potential and metric estimates.

[F2] [[lem-author-84ac8de0c2f0-weighted-one-form-decay]] and [[lem-author-84ac8de0c2f0-spatial-harrison-end]] give the spatial one-form and metric estimates.

[F3] [[def-harrison-one-form]] gives the tensor and the contraction condition; [[def-harrison-normalization]] fixes the pole-evaluation normalization. The time coordinate is normalized using that same $d_q$, not an independently chosen constant.

## Proof

**Given:**The fixed-parameter family with the normalized contraction.

**Goal:** Establish the exact time scaling and differentiated normalized end estimates.

1.1 In the original chart put $a_i=g_{0i}$ and $W_t=d_q-D_q$. Expanding the Harrison tensor gives $g_q(T,T)=d_q^2g_{00}/(4D_q)$ and $(g_q)_{0i}=\tfrac{d_q}{4D_q}(D_qa_i-f(W_q)_i)$. This is also obtained from the pullback formula and $A_qT=(d_q/D_q)T$. For $q\in[\delta,1]$, [F1] yields $D_q=4q^2+O_5(r^{-1})$ and $D_q^{-1}=(4q^2)^{-1}+O_5(r^{-1})$, with constants depending on $\delta$. Hence $(g_q)_{00}=-(d_q/(4q))^2+O_5(r^{-1})$ and $(g_q)_{0i}=O_5(r^{-2})$. The spatial block is $q^2\delta_{ij}+O_5(r^{-1})$ by [F2]. [F1, F2, F3, given, algebra]

2.1 The coordinate vector factors are $\partial_{t_q}=(4q/d_q)\partial_t$ and $\partial_{x_q^i}=q^{-1}\partial_{x^i}$. Insert these into the three blocks from step 1.1. The leading temporal and spatial coefficients become $-1$ and $\delta_{ij}$. A derivative of order $k$ in $x_q$ gives $q^{-k}$ times the original spatial derivative, and $r=r_q/q$; thus a remainder of order $r^{-b-k}$ becomes $q^b r_q^{-b-k}$ before the block's constant coordinate factors. All these factors are controlled on $[\delta,1]$. This proves the stated $O_5$ estimates. The scale statement follows from the $d_q$ bounds in [F1], and the radius identity follows directly from $r_q=qr$. Neither computation permits putting $q=0$ into these coordinates. [F1, step 1.1, algebra] ∎
