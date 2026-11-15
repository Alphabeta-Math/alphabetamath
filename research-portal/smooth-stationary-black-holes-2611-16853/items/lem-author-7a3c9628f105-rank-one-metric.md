---
id: lem-author-7a3c9628f105-rank-one-metric
title: Regular Lorentzian metric from the normalized rank-one map
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-complex-self-dual-two-form-data
  - lem-author-7a3c9628f105-primitive-parameter-lift
  - lem-author-7a3c9628f105-denominator-positivity
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  lem-author-7a3c9628f105-primitive-parameter-lift: mathematical-premise
  lem-author-7a3c9628f105-denominator-positivity: mathematical-premise
provenance:
  statement: ai-altered
  proof: literature-derived
proof_strategy: direct
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: Section 3.2, equations (3.11), (3.12), (3.20)–(3.23) and the paragraph
        immediately following (3.23).
      statement: The normalized rank-one factorization has determinant D_q(p)/D_q, the
        stated inverse and Lorentz signature; its tensor expansion is regular at
        f=0, its stationary-field contraction preserves sign, and W_1=0 with
        D_1=4 recovers the original metric.
      hypotheses: The source uses its smooth stationary vacuum data and normalized
        parameter one-form with W_q(T)=D_q(p)-D_q and positive D_q and D_q(p).
        Here only the smooth conditional algebraic data supplied by the declared
        local dependencies are used.
      reading_limits: Consulted the cited HTML equations and adjacent explanations
        only. This reference attributes the existing rank-one calculation; no
        field equations, primitive existence or global extension result is
        imported. The inverse, determinant, expansion and contractions are
        explicitly calculated in the local proof.
dependency_level: 3
---

## Statement

Assume the normalized family in [[lem-author-7a3c9628f105-primitive-parameter-lift]], with $D_q>0$ and $D_q(p)>0$. Define $A_qv=v+D_q^{-1}W_q(v)T$ and $g_q=(D_q/4)A_q^*g$. Then $A_q$ is orientation preserving and invertible, $g_q$ is Lorentzian and smooth through $f=0$, and $g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-(f/D_q)W_q\otimes W_q)$. Also $g_1=g$ and $g_q(T,T)=D_q(p)^2g(T,T)/(4D_q)$; in particular its sign is unchanged.

## Facts & Assumptions

[F1] Metric duals and $f$ use [[def-stationary-lorentzian-data]], and fiberwise algebraic pullbacks use [[def-complex-self-dual-two-form-data]].

[F2] The one-forms and their contraction normalization are supplied by [[lem-author-7a3c9628f105-primitive-parameter-lift]].

[F3] The smooth denominator is $D_q=|1+q-(1-q)\sigma|^2$ for the smooth scalar $\sigma=f+i\psi$ and $q\in[0,1]$, as in [[lem-author-7a3c9628f105-denominator-positivity]]. In particular, evaluating its defining formula at $q=1$ gives $D_1=|2|^2=4$.

## Proof

**Given:**The hypotheses in the Statement and the Facts below.

**Goal:** Establish the stated conclusions.

1.1 Write $D=D_q$, $C=D_q(p)$ and $W=W_q$. Since $D+W(T)=C$, direct multiplication gives $(I+T\otimes W/D)^{-1}=I-T\otimes W/C$. If $T\ne0$, a basis starting with $T$ makes this rank-one map triangular with diagonal $(C/D,1,1,1)$; if $T=0$, it is the identity and $C=D$. Thus its determinant is $C/D>0$. Invertible algebraic pullback and positive rescaling preserve Lorentz signature. [given, F1, F2]

2.1 Expanding $g(A_qu,A_qv)$ gives the stated tensor formula because $g(T,T)=-f$. Its only denominator is the positive $D_q$, so it is smooth through $f=0$. The identity $W_1=0$ from [F2] and the evaluation $D_1=4$ in [F3] give $g_1=g$. Finally $A_qT=(C/D)T$, hence the asserted contraction and sign identity. All coefficients are smooth in $q$ and spacetime wherever $D_q>0$. [given, F1, F2, F3, algebra, step 1.1] ∎

## Source notes

This conditional calculation follows §3.2 (3.11), (3.20)–(3.23) of the cited independent source. No existence of the stationary primitive or Einstein–Maxwell solution is inferred from this calculation alone.
