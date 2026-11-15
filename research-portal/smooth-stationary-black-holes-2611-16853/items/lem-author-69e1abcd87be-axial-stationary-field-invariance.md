---
id: lem-author-69e1abcd87be-axial-stationary-field-invariance
title: A commuting axial action preserves the stationary field and its causal
  character
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data
  - def-stationary-lorentzian-data
  - def-black-hole-comparison-hypothesis-data
  - math:thm-chain-rule-for-differentials-of-smooth-maps
dependency_roles:
  def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-black-hole-comparison-hypothesis-data: mathematical-premise
  math:thm-chain-rule-for-differentials-of-smooth-maps: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 6
---

## Statement

For the complete stationary flow $\phi_t$ and commuting global axial isometries $\psi_s$ in the comparison data, $(\psi_s)_*T=T$ for every $s$ and $g(T,T)\circ\psi_s=g(T,T)$. Here vector-field pushforward is defined by $((\psi_s)_*T)_{\psi_s(p)}=d\psi_s|_p(T_p)$ for $p\in M$; the action map $\psi_s$ is a diffeomorphism with inverse $\psi_{-s}$. In particular the timelike set, null set and ergoregion of the specified stationary field are preserved by this circle action. These identities use a supplied global action and assert no extension of a locally constructed axial field.

## Facts & Assumptions

[F1] The stationary and axial actions are globally defined commuting isometries. [[def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data]]

[F2] The stationary generator is $T=\left.\partial_t\right|_{t=0}\phi_t$, and its metric norm determines its pointwise causal character. [[def-stationary-lorentzian-data]]

[F3] The ergoregion of the specified stationary field is $\{p:g_p(T,T)>0\}$; points with $g(T,T)=0$ are excluded. [[def-black-hole-comparison-hypothesis-data]]

[F4] For smooth maps $F:M\to N$ and $G:N\to P$, the chain rule gives $d(G\circ F)_p=dG_{F(p)}\circ dF_p$ for every $p\in M$. [[math:thm-chain-rule-for-differentials-of-smooth-maps]]

## Proof

**Given:** The data and assumptions in the Statement.

**Goal:** Establish the claimed conditional conclusion.

1.1 By the chain rule [F4] applied to the smooth orbit curve $t\mapsto\phi_t(p)$ and the smooth map $\psi_s$, differentiate $\psi_s(\phi_t(p))=\phi_t(\psi_s(p))$ at $t=0$. This yields $d\psi_s|_p(T_p)=T_{\psi_s(p)}$ at every point and every circle parameter. By the inline definition, this is $(\psi_s)_*T=T$. The differentiation is legitimate globally because both compositions are defined globally by hypothesis. [F1, F2, F4, given]

2.1 Since $\psi_s^*g=g$, substitute the identity from step 1.1 into the metric pairing to obtain $g(T,T)(\psi_s(p))=g(T,T)(p)$. Each of the strict positive, strict negative and zero level sets is therefore invariant. Thus the axial action preserves the stationary field, the metric and the stated causal subsets, with the strict positive set being the ergoregion by [F3]. No extension of a local horizon symmetry is asserted. [F1, step 1.1, F2, F3, algebra] ∎
