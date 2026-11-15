---
id: def-harrison-one-form
title: Stationary Harrison one-form and metric
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - def-killing-ernst-notation
  - def-complex-self-dual-two-form-data
  - def-stationary-lorentzian-data
  - math:def-smooth-differential-k-form
  - math:def-exterior-derivative-by-the-invariant-vector-field-formula
  - math:def-lie-derivative-of-a-differential-form
dependency_roles:
  def-killing-ernst-notation: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  math:def-smooth-differential-k-form: mathematical-premise
  math:def-exterior-derivative-by-the-invariant-vector-field-formula: mathematical-premise
  math:def-lie-derivative-of-a-differential-form: mathematical-premise
  math:def-complex-conjugate-real-imaginary-part-and-modulus: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pages 6 and 8, §1.4 and equations (2.2)–(2.4)
      reading_limits: Read the frozen article text at the cited passages. This
        reference attributes the formulas; it is not used to prove existence of
        the one-form or the algebraic identities below.
dependency_level: 2
---

## Definition

Let $(M,g,N,T)$ be stationary Lorentzian data, with $T^\flat=g(T,\cdot)$ and $f=-g(T,T)$. On an open set $U$ carrying the supplied normalized Ernst potential $\sigma=f+i\psi$, let $F_{ab}=\nabla_aT_b$ and let $\star_g$ be the oriented metric Hodge star. Fix $q\in[0,1]$, and put $D_q=|q(1+\sigma)+(1-\sigma)|^2$. Suppose a supplied point $p\in U$ satisfies $T_p=0$, set $d_q=D_q(p)$, and restrict to an open subset $V\subseteq U$ on which $D_q>0$.

A Harrison one-form for these data on $V$ is a supplied smooth real one-form $W_q$ satisfying $\mathcal L_TW_q=0$, $dW_q=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$, and $W_q(T)=d_q-D_q$. Here $d$ is the exterior derivative and $\mathcal L_TW_q=0$ means that the one-form is stationary under the local flow of $T$. The conditions specify a choice; they do not assert that such a one-form exists or is unique.

For such a choice define the covariant two-tensor $g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q)$ and the bundle map $A_qv=v+D_q^{-1}W_q(v)T$. Its fiberwise pullback is $(A_q^*g)(u,v)=g(A_qu,A_qv)$. Then $g_q=(D_q/4)A_q^*g$; in particular $g_q$ is a smooth Lorentzian metric on $V$.

## Definition references

[[def-stationary-lorentzian-data]]

[[def-killing-ernst-notation]]

[[def-complex-self-dual-two-form-data]]

[[math:def-complex-conjugate-real-imaginary-part-and-modulus]]

[[math:def-smooth-differential-k-form]]

[[math:def-exterior-derivative-by-the-invariant-vector-field-formula]]

[[math:def-lie-derivative-of-a-differential-form]]

## Facts & Assumptions

[F1] The stationary data supply a smooth Lorentzian metric, its metric dual $T^\flat$, and the scalar $f=-g(T,T)$. [[def-stationary-lorentzian-data]]

[F2] The Ernst notation supplies the smooth two-form $F$, the real function $\psi$, and the oriented Hodge star in the displayed potential setting. [[def-killing-ernst-notation]] [[def-complex-self-dual-two-form-data]]

[F3] For $z=a+ib$ with real $a,b$, the complex modulus is $|z|=\sqrt{a^2+b^2}$, so $|z|^2=a^2+b^2$. [[math:def-complex-conjugate-real-imaginary-part-and-modulus]] The formula for $D_q$ in the Definition and the evaluation $d_q=D_q(p)$ are local definitions; no maximal-section, mass-one or bifurcation-surface hypothesis is used.

[F4] Fiberwise pullback by an invertible bundle map preserves nondegeneracy and signature of a metric. [[def-complex-self-dual-two-form-data]]

[F5] A smooth real one-form on $V$ is a smooth section of $T^*V$. [[math:def-smooth-differential-k-form]]

[F6] The exterior derivative of a differential form is specified by the invariant vector-field formula, and its Lie derivative is the Lie derivative of the corresponding alternating covariant tensor, defined using the local flow. [[math:def-exterior-derivative-by-the-invariant-vector-field-formula]] [[math:def-lie-derivative-of-a-differential-form]]

## Justification

**Given:**The data, parameter, positivity restriction and supplied one-form in the Definition.

**Goal:** Justify the displayed tensor, pullback identity and Lorentzian signature.

1.1 Writing $q(1+\sigma)+(1-\sigma)=(1+q)-(1-q)f-i(1-q)\psi$, the modulus convention gives $D_q=((1+q)-(1-q)f)^2+(1-q)^2\psi^2$. At $p$, $T_p=0$ gives $f(p)=0$, so $d_q=(1+q)^2+(1-q)^2\psi(p)^2>0$. On $V$, the assumed $D_q>0$ makes all displayed divisions smooth. The contraction condition gives $A_qT=(d_q/D_q)T$. Direct composition shows that $v\mapsto v-d_q^{-1}W_q(v)T$ is the inverse of $A_q$: the coefficient of $T$ cancels using $W_q(T)=d_q-D_q$. Thus $A_q$ is a smooth fiberwise invertible bundle map. [given, F1, F3, F5, algebra]

2.1 Expanding $g(A_qu,A_qv)$ gives $g(u,v)+D_q^{-1}(T^\flat(u)W_q(v)+W_q(u)T^\flat(v))-fD_q^{-2}W_q(u)W_q(v)$. Multiplication by $D_q/4$ is exactly the displayed formula for $g_q$. The pullback has the signature of $g$, and multiplication by the positive scalar $D_q/4$ preserves it; hence $g_q$ is smooth and Lorentzian. The differential and stationarity equations remain conditions on the supplied one-form, not conclusions of this calculation. [given, F1, F2, F4, step 1.1, algebra] ∎



The cited article attributes the Harrison formulas. The justification uses the supplied definitions and pointwise algebra; it does not establish the existence or construction of $W_q$.

## Source notes

The cited article attributes the Harrison formulas. The justification uses the supplied definitions and pointwise algebra; it does not establish the existence or construction of $W_q$.
