---
id: pthm-adm-temporality
title: ADM form and stable causality of positive-q metrics
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
proof_strategy: direct
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - def-harrison-one-form
  - def-stationary-maximal-graph
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-section-time
  - def-causal-exterior-and-boundary-data
  - pthm-harrison-electrovacuum
  - pthm-ernst-potential-existence
  - pthm-complete-maximal-slices
  - pthm-positive-transformed-lapse
  - physics:lem-gr-temporal-functions-and-time-functions
  - math:def-axiom-of-choice
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-harrison-one-form: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-section-time: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  pthm-harrison-electrovacuum: physical-result
  pthm-ernst-potential-existence: physical-result
  pthm-complete-maximal-slices: physical-result
  pthm-positive-transformed-lapse: physical-result
  physics:lem-gr-temporal-functions-and-time-functions: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 23, Section 4, ADM display and following sentence
      attribution: For positive q the article writes the transformed metric in
        stationary lapse–shift form, obtains the negative squared norm of the
        section-time differential, and states temporality and stable causality.
      hypotheses: The article's regular stationary vacuum construction and complete
        maximal stationary section for the positive parameter.
      reading_limits: The frozen extracted article text at this passage was read for
        attribution. The article is not used as a proof of the claim.
physical_scope: Conditional geometric consequences of the regular stationary
  vacuum model and its source-free Einstein–Maxwell Harrison family; no
  measurement is asserted.
dependency_level: 22
---

## Statement

Adopt the regular mass-one stationary vacuum construction, with maximal original exterior section and $T|_S\not\equiv0$, and assume the Axiom of Choice. For each $q\in(0,1]$, choose a complete maximal stationary graph section $\Sigma_q$ with boundary $S$ as supplied by the maximal-slice theorem, and let $v_q$ be its stationary section time. In local spatial coordinates $x^i$ transported along the stationary field, let $h_q$ be the induced metric, $N_q$ the positive lapse, and $X_q=X_q^i\partial_i$ the shift, all transported from the section. Then on the exterior $\mathcal E$,

$$g_q=-N_q^2dv_q^2+h_{q,ij}(dx^i+X_q^i dv_q)(dx^j+X_q^j dv_q),\qquad g_q^{-1}(dv_q,dv_q)=-N_q^{-2}<0.$$

Thus $v_q$ is temporal and $(\mathcal E,g_q)$ is stably causal. The displayed coordinate expression is local in the spatial variables; the conclusions hold on the entire exterior.

## Facts & Assumptions

**Given:** The model, regular data, choice convention and positive parameter in the Statement.

**Goal:** Derive the ADM expression, temporality and stable causality for the transformed exterior.

[A1] The regular construction supplies the stationary exterior and original section, and the normalization supplies the positive-q Harrison data. The chosen original section is maximal and $T|_S\not\equiv0$. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-harrison-normalization]]

[A2] Work in ZFC, including the choice assumptions inherited by the causal-curve result. [[math:def-axiom-of-choice]]

[F1] For every fixed $q\in(0,1]$, the maximal-slice theorem supplies a smooth spacelike maximal global stationary graph with boundary $S$, complete up to that boundary, and normalized end derivatives tending to zero. The graph and regular-data interfaces give the connected one-ended section and the specified end coordinates. [[pthm-complete-maximal-slices]] [[def-stationary-maximal-graph]] [[def-regular-stationary-vacuum-spacetime]]

[F2] The transformed metric is smooth. On the section, the lapse theorem applies with the future normal agreeing with $T$ at infinity and gives $N_q>0$ in the interior. [[pthm-harrison-electrovacuum]] [[pthm-positive-transformed-lapse]]

[F3] A spacelike section has positive-definite induced metric and a future unit normal $n_q$; its lapse and tangent shift satisfy $T=N_qn_q+X_q$. The section time has $Tv_q=1$, vanishes on the graph, and its level sets are the flow translates of the graph. [[def-spacelike-maximal-hypersurface-data]] [[def-stationary-section-time]]

[F4] A temporal function has past-directed timelike gradient. Stable causality means that a smooth wider Lorentzian metric with the same time orientation has no closed future causal curve. A temporal function has no closed future causal curve, under the stated choice assumptions. [[def-causal-exterior-and-boundary-data]] [[physics:lem-gr-temporal-functions-and-time-functions]]

[F5] The adopted electrovacuum construction uses a single smooth stationary primitive $W_0$ and $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. Its normalized Ernst potential obeys $d\sigma=2\iota_T\mathcal F$, where $\mathcal F$ is a complex two-form, and $D_q=|q(1+\sigma)+(1-\sigma)|^2$. The defining Harrison tensor is $g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q)$, with $f=-g(T,T)$; it is defined on the whole exterior by the adopted construction. The one-form's existence is supplied by that construction, not by its conditional definition. [[pthm-harrison-electrovacuum]] [[def-harrison-normalization]] [[def-harrison-one-form]] [[pthm-ernst-potential-existence]]

## Proof

**Given:**The model, regular data, choice convention and positive parameter in the Statement.

**Goal:** Derive the ADM expression, temporality and stable causality for the transformed exterior.

[A1] The regular construction supplies the stationary exterior and original section, and the normalization supplies the positive-q Harrison data. The chosen original section is maximal and $T|_S\not\equiv0$. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-harrison-normalization]]

[A2] Work in ZFC, including the choice assumptions inherited by the causal-curve result. [[math:def-axiom-of-choice]]

[F1] For every fixed $q\in(0,1]$, the maximal-slice theorem supplies a smooth spacelike maximal global stationary graph with boundary $S$, complete up to that boundary, and normalized end derivatives tending to zero. The graph and regular-data interfaces give the connected one-ended section and the specified end coordinates. [[pthm-complete-maximal-slices]] [[def-stationary-maximal-graph]] [[def-regular-stationary-vacuum-spacetime]]

[F2] The transformed metric is smooth. On the section, the lapse theorem applies with the future normal agreeing with $T$ at infinity and gives $N_q>0$ in the interior. [[pthm-harrison-electrovacuum]] [[pthm-positive-transformed-lapse]]

[F3] A spacelike section has positive-definite induced metric and a future unit normal $n_q$; its lapse and tangent shift satisfy $T=N_qn_q+X_q$. The section time has $Tv_q=1$, vanishes on the graph, and its level sets are the flow translates of the graph. [[def-spacelike-maximal-hypersurface-data]] [[def-stationary-section-time]]

[F4] A temporal function has past-directed timelike gradient. Stable causality means that a smooth wider Lorentzian metric with the same time orientation has no closed future causal curve. A temporal function has no closed future causal curve, under the stated choice assumptions. [[def-causal-exterior-and-boundary-data]] [[physics:lem-gr-temporal-functions-and-time-functions]]

[F5] The adopted electrovacuum construction uses a single smooth stationary primitive $W_0$ and $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. Its normalized Ernst potential obeys $d\sigma=2\iota_T\mathcal F$, where $\mathcal F$ is a complex two-form, and $D_q=|q(1+\sigma)+(1-\sigma)|^2$. The defining Harrison tensor is $g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q)$, with $f=-g(T,T)$; it is defined on the whole exterior by the adopted construction. The one-form's existence is supplied by that construction, not by its conditional definition. [[pthm-harrison-electrovacuum]] [[def-harrison-normalization]] [[def-harrison-one-form]] [[pthm-ernst-potential-existence]]



1.1 Fix $q\in(0,1]$. By [A1], the original $T$-flow preserves $g$ and its own field $T$, hence also $T^\flat$ and $f=-g(T,T)$. The normalized potential equation in [F5] gives $d\sigma(T)=2\mathcal F(T,T)=0$ by alternation. Thus $\sigma$ and $D_q$ are constant along every $T$-orbit. The supplied $W_0$ is stationary, so its polynomial combination $W_q=(1-q)^2W_0-4q(1-q)T^\flat$ is stationary as well. Every factor of the defining tensor formula in [F5] is therefore invariant under the flow, and its pullback gives $\Phi_a^*g_q=g_q$ wherever $\Phi_a$ is defined. Completeness of the exterior stationary orbits in [A1] makes every $a\in\mathbb R$ available. This proves the transformed metric's stationarity directly from the adopted construction. [given, A1, F5, algebra]

2.1 Choose $\delta\in(0,\min\{q,1\})$. The section in [F1] exists at this parameter. Its graph identifies it with the connected exterior base and gives one end; its derivative decay supplies the end hypothesis of the lapse theorem. Consequently [F2] gives a positive lapse. Stationary flow transports the section, its future normal, induced metric, lapse and shift to every point of the exterior. By step 1.1 the flow preserves the metric. It preserves time orientation because the continuously transported unit timelike normal starts future-directed and cannot change time cone. Thus the transported lapse remains positive and each translated section is spacelike. [given, A1, F1, F2, F3, step 1.1]

3.1 In the coordinates $(v_q,x^i)$, the coordinate vector $\partial_{v_q}$ is $T$ and the $\partial_i$ are tangent to the translated sections. Thus $g_q(\partial_i,\partial_j)=h_{q,ij}$, $g_q(\partial_{v_q},\partial_i)=h_{q,ij}X_q^j$, and $g_q(\partial_{v_q},\partial_{v_q})=-N_q^2+h_{q,ij}X_q^iX_q^j$. These components give the displayed ADM form. Since $dv_q$ annihilates section tangents and $dv_q(T)=1$, the decomposition $T=N_qn_q+X_q$ gives $dv_q(n_q)=N_q^{-1}$. Hence $\nabla^{g_q}v_q=-N_q^{-1}n_q$ and $g_q^{-1}(dv_q,dv_q)=-N_q^{-2}<0$. The gradient is past-directed, so $v_q$ is temporal. [F3, F4, step 2.1, algebra]

4.1 Put $g=g_q$, $v=v_q$ and $a=-g^{-1}(dv,dv)>0$, and define $\widehat g=g-dv\otimes dv$. In a $g$-orthonormal frame with first vector $n=-\nabla^g v/\sqrt a$, the form $dv$ vanishes on the spatial vectors and takes value $\sqrt a$ on $n$. Therefore $\widehat g$ has diagonal entries $-(1+a),1,1,1$ and is smooth Lorentzian. Every nonzero $g$-causal vector $Y$ has $dv(Y)\ne0$, so $\widehat g(Y,Y)=g(Y,Y)-dv(Y)^2<0$. Moreover $n$ is timelike for both metrics and fixes their common time orientation. [F3, step 3.1, algebra]

5.1 Direct substitution gives $\nabla^{\widehat g}v=\nabla^g v/(1+a)$ and $\widehat g^{-1}(dv,dv)=-a/(1+a)<0$. This gradient is past-directed for the common time orientation, so $v$ is temporal for $\widehat g$. By [F4], $\widehat g$ has no closed future causal curve. Together with the strict cone widening in step 4.1, this is stable causality in the stated definition. [A2, F4, step 3.1, step 4.1, algebra] ∎



The article reference attributes the ADM and causal claims. The argument above uses the completed section and lapse suppliers and a direct construction of a wider metric; it does not use the article as a prerequisite proof.

## Source notes

The article reference attributes the ADM and causal claims. The argument above uses the completed section and lapse suppliers and a direct construction of a wider metric; it does not use the article as a prerequisite proof.
