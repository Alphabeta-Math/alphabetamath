---
id: lem-author-cea8e61dc3c6-divergence-hodge-closure
title: Vanishing divergence implies closed Hodge dual
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-complex-self-dual-two-form-data
  - physics:lem-emg-lorentz-hodge-calculus
  - physics:thm-gr-point-normal-and-exponential-coordinate-charts
  - physics:def-gr-metric-volume-form-and-current-flux
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  physics:lem-emg-lorentz-hodge-calculus: mathematical-premise
  physics:thm-gr-point-normal-and-exponential-coordinate-charts: mathematical-premise
  physics:def-gr-metric-volume-form-and-current-flux: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references: []
dependency_level: 1
---

## Statement

For the stationary Lorentzian data and a smooth real two-form $U$, $\nabla^aU_{ab}=0$ implies $d(\star_gU)=0$. Thus the word co-closed here means precisely the vanishing-divergence condition, equivalently the displayed Hodge-closure equation.

## Facts & Assumptions

[F1] Use the metric connection and index conventions of [[def-stationary-lorentzian-data]].

[F2] The real Hodge star and its complex extension are those of [[def-complex-self-dual-two-form-data]].

[F3] The Hodge formula is $(\star_gU)_{ab}=\tfrac12\epsilon_{abcd}U^{cd}$, and exterior differentiation is alternating differentiation. [[physics:lem-emg-lorentz-hodge-calculus]]

[F4] At each point one may choose coordinates with $g_{ab}=\operatorname{diag}(-1,1,1,1)$ and first metric derivatives zero. [[physics:thm-gr-point-normal-and-exponential-coordinate-charts]]

[F5] In a positively oriented chart the metric volume form is $\epsilon=\sqrt{|\det(g_{ab})|}\,dx^0\wedge dx^1\wedge dx^2\wedge dx^3$; its component array is the positive density times the alternating symbol. [[physics:def-gr-metric-volume-form-and-current-flux]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove all asserted identities under these hypotheses.

1.1 Fix a point $p$ and use [F4], making the chart positively oriented by reversing one spatial coordinate if necessary. The Christoffel symbols and first metric derivatives vanish at $p$. Write $\epsilon$ for the metric volume form of [F5]. Its components are $\sqrt{|\det g|}$ times the alternating symbol. Since the determinant is a polynomial in the metric entries and the square-root function is smooth at $|\det g(p)|=1$, the vanishing of their first derivatives gives $\partial\epsilon(p)=0$. For distinct indices $a,b,c$ let $j$ be the missing fourth index. The Hodge formula gives $(\star_gU)_{bc}=\epsilon_{bcaj}U^{aj}$, with no sum over $a,j$, since the two complementary terms in the half-sum agree. [F1, F2, F3, F4, F5, algebra]

2.1 At $p$, cyclically adding derivatives and using $\partial\epsilon(p)=0$ gives $(d\star_gU)_{abc}=\epsilon_{abcj}(\partial_aU^{aj}+\partial_bU^{bj}+\partial_cU^{cj})=\epsilon_{abcj}\nabla_kU^{kj}$ for distinct $a,b,c$, with only $k$ summed in the last expression; the missing $k=j$ term is zero by antisymmetry. Put $V^j=\nabla_kU^{kj}$. Metric compatibility gives $V^j=g^{jb}\nabla^aU_{ab}$, with $a,b$ summed. Thus vanishing divergence implies $V=0$, and the displayed identity makes every distinct-index component of $d\star_gU$ zero. Repeated-index components vanish by alternation. Since $p$ was arbitrary, $d\star_gU=0$ globally. [step 1.1, F1, F3, F4, algebra]

3.1 Conversely, suppose $d\star_gU=0$. For each $j$ at $p$, choose the other three indices as $a,b,c$. The identity in step 2.1 gives $0=\epsilon_{abcj}V^j$, with no summation here. By [F5] and the normal metric at $p$, $\epsilon_{abcj}=\pm1$, so $V^j=0$ for each $j$. Lowering the free index in $V^j=g^{jb}\nabla^aU_{ab}$ using the nondegenerate metric yields $\nabla^aU_{ab}=g_{bj}V^j=0$, with the contracted indices summed. The point was arbitrary, proving the converse globally and hence the asserted equivalence. [step 1.1, step 2.1, F1, F5, algebra] ∎
