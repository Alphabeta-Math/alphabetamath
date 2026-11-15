---
id: def-truncated-null-boundary-height
title: Truncated causal-boundary height for smooth approximation
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-near-horizon-past-boundary-sets
  - def-stationary-section-time
  - def-causal-exterior-and-boundary-data
  - def-spacelike-maximal-hypersurface-data
  - math:lem-extended-reals-complete
  - math:def-local-and-global-flow
dependency_roles:
  def-near-horizon-past-boundary-sets: mathematical-premise
  def-stationary-section-time: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:lem-extended-reals-complete: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 25, proof of Lemma 4.4, definitions of Ψ and u
      reading_limits: The frozen article text at the cited passage was read for
        attribution; this reference is not used as proof of well-definedness.
dependency_level: 6
---

## Definition

Use the supplied near-horizon data with $C=C_t$ for a fixed $t$, the section $\Sigma=\Sigma_{q,0}$, boundary $S$, distance function $\rho$, and section time $v$. All causal relations and boundaries below are relative to the exterior $\mathcal E$ with metric $g_q$. Thus $I^-(C)$ is the set of points joined to $C$ by a future-directed timelike curve in $\mathcal E$, and $\partial I^-(C)$ is its boundary in $\mathcal E$. Let $W\subset\mathcal E$ be the specified portion inside the stationary cylinder $\mathscr C$.

Let $\eta>0$ and $\mathcal R=\{x\in\Sigma:0\le\rho(x)\le\eta\}$. On the relevant translated section interiors use the future unit normal $n$, lapse $N>0$, and tangent shift $X$ of the stationary field $T$, so $T=Nn+X$. Put $V=Nn=T-X$. Assume a local flow $\Psi_z$ of $V$ is supplied on $\mathcal R$ for every $|z|\le2\delta$, for a chosen $\delta>0$, with $\Psi_z(x)\in\mathcal E$ for $x\in\mathcal R\setminus S$. If $S$ is outside $\mathcal E$, this includes a separately supplied extension of the flow to $S$; membership in $I^-(C)$ is false for points outside $\mathcal E$. The parameter $\delta$ is the local smoothing parameter, distinct from any fixed lower bound on $q$. Define

$$u(x)=\sup\bigl(\{-2\delta\}\cup\{z\in[-2\delta,2\delta]:\Psi_z(x)\in I^-(C)\}\bigr).$$

For $|z|\le2\delta$, let $\Sigma_z^\circ=\{p\in\mathcal E:v(p)=z\}$ and define the cut $D_z=\Sigma_z^\circ\cap\partial I^-(C)\cap W$. Assume $v$ is temporal: $dv$ is positive on every nonzero future-directed causal vector. Use the supplied family of past-directed affinely parametrized null geodesics $\gamma_c$ from $c\in C$, with the specified outward null-normal direction and with affine parameter increasing toward the past. Define $A_z=\{c\in C:\gamma_c\text{ meets }D_z\}$, and for $c\in A_z$ let $F_z(c)$ be that intersection point.

## Definition references

[[def-near-horizon-past-boundary-sets]]

[[def-stationary-section-time]]

[[def-causal-exterior-and-boundary-data]]

[[def-spacelike-maximal-hypersurface-data]]

[[math:lem-extended-reals-complete]]

[[math:def-local-and-global-flow]]

## Facts & Assumptions

[F1] The near-horizon interface supplies $\Sigma$, $S$, $\rho$, $C$, the cylinder, and the specified family of past null geodesics; it treats the choice of inside and the geodesic family as data. [[def-near-horizon-past-boundary-sets]]

[F2] The section-time interface gives $T(v)=1$ and identifies each translated section interior with a level of $v$. [[def-stationary-section-time]]

[F3] The lapse–shift interface gives $T=Nn+X$, with $X$ tangent to each section and $n$ future timelike. [[def-spacelike-maximal-hypersurface-data]]

[F4] Chronological reachability and relative boundary are defined in the specified Lorentzian domain. [[def-causal-exterior-and-boundary-data]]

[F5] Every nonempty real set bounded above has a real least upper bound. [[math:lem-extended-reals-complete]]

[F6] A local flow of a smooth vector field has an open time–point domain, interval time fibres, identity at time zero, integral-curve trajectories and the flow composition law wherever defined. [[math:def-local-and-global-flow]]

## Justification

**Given:** The section, cut data, temporal function, geodesic family, positive lapse and common flow domain specified in the Definition.

**Goal:** Check the flow normalization and the well-definedness of $u$, $D_z$, $A_z$ and $F_z$.

1.1 Since $X$ is tangent to a level of $v$, $X(v)=0$; hence $V(v)=T(v)-X(v)=1$. The positive multiple $Nn$ is future timelike on the relevant section interiors. The existence and common domain of its flow, including any extension to $S$, are hypotheses. [F2, F3, F6]

2.1 For each $x$, the set inside the supremum contains $-2\delta$ and is bounded above by $2\delta$. It therefore has a unique real supremum, lying in $[-2\delta,2\delta]$. The specified level set, relative boundary, and inside set determine $D_z$, and the intersection condition determines $A_z$. [F4, F5, step 1.1]

3.1 Along a past-directed null geodesic, the temporal function $v$ strictly decreases as its affine parameter increases. Thus each such geodesic meets the level $v=z$ at most once; every $c\in A_z$ consequently has exactly one intersection with $D_z$, which defines $F_z:A_z\to D_z$. No claim is made here that $F_z$ is onto, that the cuts are regular, or that $u$ is Lipschitz. [F1, F2, step 2.1] ∎

## Source notes

The article citation attributes the construction. The justification uses the stated supplier interfaces and supplied data, rather than the article's claim as a proof of itself.
