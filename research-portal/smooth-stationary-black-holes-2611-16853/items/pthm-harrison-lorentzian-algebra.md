---
id: pthm-harrison-lorentzian-algebra
title: Invertibility, Lorentz signature and stationary norm
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - def-stationary-lorentzian-data
  - def-killing-ernst-notation
  - def-harrison-one-form
  - def-harrison-one-form-family
  - lem-rank-one-lorentzian-hodge-transfer
  - math:def-lie-derivative-of-a-tensor-field
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  def-harrison-one-form: mathematical-premise
  def-harrison-one-form-family: mathematical-premise
  lem-rank-one-lorentzian-hodge-transfer: mathematical-premise
  math:def-lie-derivative-of-a-tensor-field: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pages 8–9, equations (2.4)–(2.5), following display, and equation
        (2.9)
      attribution: The Harrison tangent map has determinant d_q/D_q and the stated
        inverse; the transformed metric is Lorentzian and stationary, has the
        stated stationary norm, and equals the original metric at q=1. Equation
        (2.9) specifies the one-form family.
      hypotheses: The article's stationary vacuum construction, normalized Ernst
        potential, regular one-form family, and q in [0,1].
      reading_limits: Read the frozen article text at the cited passages. This
        reference attributes the claims and family choice; it is not used as
        their proof.
physical_scope: Conditional geometric deduction for the stationary vacuum
  Harrison construction; no observation or measurement is asserted.
dependency_level: 3
---

## Statement

Let $(M,g,N,T)$ be stationary Lorentzian data: $g$ is a smooth Lorentzian metric of signature $(-,+,+,+)$, $N$ is a smooth timelike time-orientation field, and $T$ is Killing. On an open set $U$ let a normalized Ernst potential $\sigma=f+i\psi$ be supplied, where $f=-g(T,T)$, and let a supplied pole $p\in U$ satisfy $T_p=0$. For $q\in[0,1]$ put $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $d_q=D_q(p)$. On an open subset $V\subseteq U$ where $D_q>0$, suppose the smooth stationary Harrison one-form $W_q$ is supplied, including its normalization $W_q(T)=d_q-D_q$. Define $A_qv=v+D_q^{-1}W_q(v)T$ and $g_q=(D_q/4)A_q^*g$.

Then $d_q>0$, $\det A_q=d_q/D_q>0$, $A_q^{-1}w=w-d_q^{-1}W_q(w)T$, and $g_q$ is Lorentzian. It is stationary, $\mathcal L_Tg_q=0$, and $g_q(T,T)=d_q^2g(T,T)/(4D_q)$. The smooth field $A_q^{-1}N$ defines a time orientation of $g_q$ for which $A_q$ carries future $g_q$-timelike vectors to future $g$-timelike vectors. If the supplied family is the single-potential family $W_q=(1-q)^2W_0-4q(1-q)T^\flat$, then $g_1=g$.

## Statement references

[[def-stationary-lorentzian-data]]

[[def-killing-ernst-notation]]

[[def-harrison-one-form]]

[[def-harrison-one-form-family]]

[[lem-rank-one-lorentzian-hodge-transfer]]

[[math:def-lie-derivative-of-a-tensor-field]]

## Facts & Assumptions

[F1] Stationary Lorentzian data provide the time-oriented Lorentz metric, its metric dual $T^\flat=g(T,\cdot)$, and a Killing field satisfying $\mathcal L_Tg=0$. [[def-stationary-lorentzian-data]]

[F2] The Ernst potential satisfies $d\sigma_a=2T^b\mathcal F_{ba}$, where $\mathcal F$ is an antisymmetric complex two-form. [[def-killing-ernst-notation]]

[F3] The local one-form interface uses $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $d_q=D_q(p)$ at a supplied zero $T_p=0$, on the domain $D_q>0$. These definitions require neither a maximal mass-one section nor a bifurcation surface. [[def-harrison-one-form]]

[F4] A supplied Harrison one-form is stationary and satisfies $W_q(T)=d_q-D_q$; its metric is the displayed pullback metric. [[def-harrison-one-form]]

[F5] For a Lorentz form, $D,d>0$ and $W(T)=d-D$, the rank-one map $A=I+D^{-1}T\otimes W$ has determinant $d/D$, inverse $I-d^{-1}T\otimes W$, and $(D/4)A^*g$ has the original inertia. [[lem-rank-one-lorentzian-hodge-transfer]]

[F6] The single-potential family is $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. [[def-harrison-one-form-family]]

[F7] For a smooth tensor field $B$ of any type, its Lie derivative along $T$ is $\mathcal L_TB=\left.\frac{d}{dt}\right|_{t=0}\Phi_t^*B$, where $\Phi_t$ is the local flow of $T$. Pullback acts by the inverse differential on contravariant slots and by the differential on covariant slots. This applies to the mixed tensor $A_q$ as well as to $g_q$. [[math:def-lie-derivative-of-a-tensor-field]]

## Proof

**Given:** The data, parameter, positive-denominator domain and supplied one-form in the Statement.

**Goal:** Establish the determinant, inverse, signature, stationarity, norm, time orientation and conditional endpoint identity.

1.1 At the pole, $f(p)=0$. Expanding the squared modulus gives $d_q=(1+q)^2+(1-q)^2\psi(p)^2>0$ for $q\in[0,1]$. At each point of $V$, $D_q>0$ and $W_q(T)=d_q-D_q$, so the rank-one result applies with $D=D_q$ and $d=d_q$. It gives the stated determinant and inverse and shows that $g_q$ has the Lorentzian inertia of $g$. Smoothness follows from the smooth data and positive denominators. [given, F1, F3, F4, F5, algebra]

1.2 Antisymmetry in the Ernst equation gives $T(\sigma)=2T^aT^b\mathcal F_{ba}=0$, hence $\mathcal L_TD_q=0$. Also $\mathcal L_TT=[T,T]=0$, while $\mathcal L_TW_q=0$ and $\mathcal L_Tg=0$. Therefore $\mathcal L_TA_q=0$ and differentiating the pullback expression yields $\mathcal L_Tg_q=0$. [given, F1, F2, F3, F4, F7, algebra]

2.1 The normalization gives $A_qT=(1+D_q^{-1}W_q(T))T=(d_q/D_q)T$. Substitution into the pullback metric gives $g_q(T,T)=d_q^2g(T,T)/(4D_q)$. The smooth field $A_q^{-1}N$ is $g_q$-timelike because its squared norm is $(D_q/4)g(N,N)<0$. For any $g_q$-timelike $v$, positivity of $D_q/4$ gives $g_q(v,A_q^{-1}N)=(D_q/4)g(A_qv,N)$, proving the asserted correspondence of future cones. [given, F1, F4, step 1.1, algebra]

3.1 If the supplied one-forms are the single-potential family, its formula gives $W_1=0$; the denominator definition gives $D_1=4$. Consequently $A_1=I$ and $g_1=g$. This endpoint uses the specified family choice in addition to the equations for an individual Harrison one-form. [given, F3, F6, step 1.1, algebra] ∎

## Source notes

The article passage attributes the original claims. The proof uses the stated definitions and rank-one lemma, and the endpoint identity uses the family specified in the article's equation (2.9).
