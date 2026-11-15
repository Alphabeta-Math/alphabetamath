---
id: pthm-harrison-forced-normalization
title: Cartan normalization at the bifurcation pole
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-spacelike-maximal-hypersurface-data
  - pthm-local-hawking-circle-fields
  - def-stationary-lorentzian-data
  - def-killing-ernst-notation
  - math:def-interior-product-of-a-form-by-a-vector-field
  - math:thm-cartans-magic-formula
  - math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  pthm-local-hawking-circle-fields: physical-result
  def-stationary-lorentzian-data: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  math:def-interior-product-of-a-form-by-a-vector-field: mathematical-premise
  math:thm-cartans-magic-formula: mathematical-premise
  math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 8, §2.1, equations (2.1)–(2.2) and the following paragraph
      reading_limits: Read the frozen article text at the cited passage for
        attribution. The proof below is a local calculation from the stated
        definitions and Cartan identity; the article citation is not used as its
        proof.
physical_scope: Conditional deduction in the smooth four-dimensional stationary
  vacuum black-hole model; no observation or measurement is asserted.
dependency_level: 8
---

## Statement

Adopt the stationary vacuum model and regular stationary vacuum spacetime data, with bifurcation sphere $S$, $T|_S\not\equiv0$, and maximal exterior section $\Sigma_0\cap\mathcal E$. The local Hawking-field result gives a point $p\in S$ with $T_p=0$. Let $U$ be a connected open set containing $p$ on which a smooth normalized Ernst potential $\sigma=f+i\psi$ is supplied, where $f=-g(T,T)$ and $F_{ab}=\nabla_aT_b$. Fix $q\in[0,1]$ and put $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $d_q=D_q(p)$.

Suppose a smooth real one-form $W_q$ on $U$ is stationary, meaning $\mathcal L_TW_q=0$, and satisfies $dW_q=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$. Then $d(W_q(T)+D_q)=\mathcal L_TW_q-\iota_TdW_q+dD_q=0$ on $U$, and consequently $W_q(T)+D_q=d_q$ throughout $U$. In particular, smoothness at the pole forces $W_q(T)=d_q-D_q$; the conclusion is conditional on the supplied one-form and does not assert its existence.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-spacelike-maximal-hypersurface-data]]

[[pthm-local-hawking-circle-fields]]

[[def-stationary-lorentzian-data]]

[[def-killing-ernst-notation]]

[[math:def-interior-product-of-a-form-by-a-vector-field]]

[[math:thm-cartans-magic-formula]]

[[math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component]]

## Facts & Assumptions

[A1] Adopt the stationary vacuum model and the regular spacetime hypotheses, including the stated maximal exterior section and $T|_S\not\equiv0$. A maximal spacelike section has vanishing mean curvature. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-spacelike-maximal-hypersurface-data]]

[F1] Under these hypotheses the local Hawking-field result supplies a pole $p\in S$ at which $T_p=0$. [[pthm-local-hawking-circle-fields]]

[F2] The stationary data define the smooth metric, Killing field and Levi–Civita connection. The Ernst potential convention gives $df=2\iota_TF$ and $d\psi=2\iota_T\star_gF$. [[def-stationary-lorentzian-data]] [[def-killing-ernst-notation]]

[F3] By the inline definitions in the Statement, the denominator and its pole value are $D_q=|q(1+\sigma)+(1-\sigma)|^2$ and $d_q=D_q(p)$.

[F4] Cartan’s identity for a smooth one-form is $\mathcal L_TW=d(\iota_TW)+\iota_TdW$. [[math:thm-cartans-magic-formula]]

[F5] A smooth real-valued function whose differential vanishes is constant on each connected component of its manifold. [[math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component]]

[F6] For a smooth one-form $W$ and smooth two-form $B$, the interior product inserts $T$ into the first slot: $\iota_TW=W(T)$ and $(\iota_TB)(V)=B(T,V)$. [[math:def-interior-product-of-a-form-by-a-vector-field]]

## Proof

**Given:** The model and data, connected set $U$, potential, parameter and one-form in the Statement.

**Goal:** Prove the differential identity and the forced value of the contraction.

1.1 Write $a=(1-q)f-(1+q)$. The denominator is $D_q=a^2+(1-q)^2\psi^2$, so $dD_q=2(1-q)(a\,df+(1-q)\psi\,d\psi)$. Using the two Ernst identities and the assumed equation for $dW_q$ gives $\iota_TdW_q=2(1-q)(a\,df+(1-q)\psi\,d\psi)=dD_q$. [given, F2, F3, F6, algebra]

2.1 Cartan’s identity and stationarity give $d(W_q(T)+D_q)=\mathcal L_TW_q-\iota_TdW_q+dD_q=0$. By [F5], this smooth real-valued function is constant on the connected manifold $U$. At the supplied pole, smoothness makes $W_q$ an ordinary covector and $T_p=0$, so $W_q(T)(p)=0$. Its constant value is therefore $D_q(p)=d_q$, proving the stated normalization. [given, A1, F1, F3, F4, F5, F6, step 1.1] ∎

## Source notes

The article citation attributes the original normalization claim. The argument above uses the explicitly supplied potential equation, the one-form equation, Cartan’s identity and the zero-differential constancy proposition.
