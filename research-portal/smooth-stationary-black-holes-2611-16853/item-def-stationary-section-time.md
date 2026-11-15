---
title: Stationary section time and translated maximal sections
status: draft
research_item: def-stationary-section-time
dependency_level: 4
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: Section 4, immediately before Lemma 4.1, PDF page 23
---

PDF p. 23: ` §4, before Lemma 4.1 `

## Prerequisites

- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [def-lapse-shift-notation](item-def-lapse-shift-notation)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [physics:lem-tgr-isometry-natural-tensor-invariance](https://alphabetamath.cc/physics/item/lem-tgr-isometry-natural-tensor-invariance)


## Definition

Fix $q\in(0,1]$. Use the stationary maximal-graph data: the exterior is identified with $\mathcal E=\mathbb R_t\times\Sigma_1^\circ$, the stationary field is $T=\partial_t$, and the supplied section is the graph $\Sigma_q^\circ=\{(u_q(x),x):x\in\Sigma_1^\circ\}$. Assume that $g_q$ is a smooth time-oriented Lorentzian metric invariant under the $T$-flow, that this graph is spacelike and maximal for $g_q$, and that its lapse relative to the future unit normal is positive. A maximal spacelike section means a spacelike hypersurface whose mean curvature vanishes. A section $\Sigma_q$ with interior $\Sigma_q^\circ$ and boundary $S$ is supplied separately.

Define the stationary section time by $v_q(t,x)=t-u_q(x)$. For any local spatial coordinates $(x^i)$ on $\Sigma_1^\circ$, use the same coordinate functions on the product, so that they are constant along $T$-orbits. For $a\in\mathbb R$, set $\Sigma_{q,a}^\circ=\{p\in\mathcal E:v_q(p)=a\}$ and $\Sigma_{q,a}=\Sigma_{q,a}^\circ\cup S$; in particular $\Sigma_{q,0}=\Sigma_q$. The boundary notation records the supplied common set $S$ and does not by itself assert smooth boundary regularity for every translate.

On $\Sigma_q^\circ$, let $n_q$ be the future-directed unit normal, $h_q=g_q|_{T\Sigma_q^\circ}$ the induced metric, $N_q=-g_q(T,n_q)$ the lapse, and $X_q=T-N_qn_q$ the tangent shift. Thus $T=N_qn_q+X_q$ and $N_q>0$ by hypothesis. All chronological and causal relations used with these conventions are relative to the exterior $\mathcal E$ with metric $g_q$: their curves are required to remain in $\mathcal E$.

## Definition references

[def-stationary-maximal-graph](item-def-stationary-maximal-graph)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-lapse-shift-notation](item-def-lapse-shift-notation)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

## Facts & Assumptions

[F1] The stationary-graph interface supplies the product coordinates, the graph function and the meanings of spacelike and maximal; the extension with boundary $S$ is separately supplied. [def-stationary-maximal-graph](item-def-stationary-maximal-graph)

[F2] Stationary Lorentzian data define the smooth metric, time orientation, Killing field and its flow; invariance of $g_q$ under the specified flow is an explicit hypothesis here. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F3] A spacelike hypersurface has a future unit normal and an induced Riemannian metric; the lapse and shift give the stated normal–tangent decomposition. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-lapse-shift-notation](item-def-lapse-shift-notation)

[F4] Chronological and causal relations are defined relative to the specified time-oriented Lorentzian domain and its admissible curves. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F5] On common flow domains of a smooth nowhere-zero Killing field, its flow preserves the metric and the Levi–Civita connection. This is a mathematical result, applied here to $T=\partial_t$ on the product exterior. [physics:lem-tgr-isometry-natural-tensor-invariance](https://alphabetamath.cc/physics/item/lem-tgr-isometry-natural-tensor-invariance)

## Justification

**Given:**The product, graph, metric, flow, positive lapse and boundary data in the Definition.

**Goal:** Justify the section time, transported coordinates, translated sets and lapse–shift notation.

1.1 Smoothness of $u_q$ makes $v_q$ smooth. Because $T=\partial_t$, one has $Tv_q=1$, while $v_q(u_q(x),x)=0$. Conversely, each point $(t,x)$ has the unique representation as the flow by $t-u_q(x)$ of the graph point $(u_q(x),x)$. Hence $v_q$ is the unique function with these two properties, the transported $x^i$ are constant on each orbit, and $\Sigma_{q,a}^\circ$ is the flow translate of $\Sigma_q^\circ$ by parameter $a$. [given, F1, F2]

2.1 Write $\Phi_a(t,x)=(t+a,x)$ for the supplied flow. The field $T=\partial_t$ is nowhere zero on the product exterior and is Killing for $g_q$ by the assumed invariance, so [F5] gives preservation of its Levi–Civita connection $\nabla^q$ on the flow domains. The maps $\Phi_a$ are globally defined here by the product, and this connection identity is local at every point. Metric invariance makes their translated interiors spacelike. Put $n_{q,a}=\Phi_{a*}n_q$ along $\Sigma_{q,a}^\circ$. It is unit timelike and orthogonal to that interior. It is future-directed because, for each graph point $p$, the continuous path $s\mapsto\Phi_{s*}n_q(p)$ consists of timelike vectors based at $\Phi_s(p)$ and starts future-directed at $s=0$, so it cannot change time cone. Let $h_{q,a}$ and $k_{q,a}$ be the induced metric and second fundamental form with this normal, using the convention in [F3]. For graph-tangent vectors $U,V$, metric and connection preservation give $h_{q,a}(\Phi_{a*}U,\Phi_{a*}V)=h_q(U,V),\qquad k_{q,a}(\Phi_{a*}U,\Phi_{a*}V)=-g_q(\nabla^q_{\Phi_{a*}U}(\Phi_{a*}n_q),\Phi_{a*}V)=-g_q(\Phi_{a*}(\nabla^q_U n_q),\Phi_{a*}V)=k_q(U,V).$ Taking the trace with the transported induced metric yields $H_{q,a}\circ\Phi_a=-\operatorname{tr}_{h_q}k_q=H_q=0$ on $\Sigma_q^\circ$. Thus every translated interior is maximal. [given, F2, F3, F5, step 1.1]

3.1 The supplied boundary set defines the displayed unions without an additional boundary-regularity assertion. The hypersurface interface supplies the unique future unit normal and the induced metric, and the lapse–shift formulas give the tangent decomposition; positivity is the stated hypothesis. The causal convention specifies the domain in which the relevant curves are considered. [given, F3, F4, step 1.1, step 2.1] ∎
