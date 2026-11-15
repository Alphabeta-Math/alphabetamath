---
id: lem-author-89004136b63c-compact-temporal-persistence
title: A compact temporal covector persists under metric perturbation
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - lem-author-89004136b63c-compact-neighborhood-localization
  - lem-author-89004136b63c-temporal-compact-margins
  - lem-author-89004136b63c-uniform-inverse-metric-continuity
  - math:def-smooth-manifold
  - math:def-topological-manifold-without-boundary
  - math:thm-compact-subset-of-a-hausdorff-space-is-closed
  - math:def-subspace-topology-top
  - math:thm-closed-subspace-of-a-compact-space-is-compact
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  lem-author-89004136b63c-compact-neighborhood-localization: mathematical-premise
  lem-author-89004136b63c-temporal-compact-margins: mathematical-premise
  lem-author-89004136b63c-uniform-inverse-metric-continuity: mathematical-premise
  math:def-smooth-manifold: mathematical-premise
  math:def-topological-manifold-without-boundary: mathematical-premise
  math:thm-compact-subset-of-a-hausdorff-space-is-closed: mathematical-premise
  math:def-subspace-topology-top: mathematical-premise
  math:thm-closed-subspace-of-a-compact-space-is-compact: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

Let $g$ be a $C^2$ Lorentz metric on an open subset of a smooth four-manifold, $N$ a continuous timelike orientation field, $K$ compact, and $\alpha$ a continuous covector field near $K$ with $g^{-1}(\alpha,\alpha)<0$ and $\alpha(N)>0$ on $K$. There is $\delta>0$ such that every Lorentz metric $\widetilde g$ whose coefficients differ from those of $g$ by less than $\delta$ on a fixed finite compact chart cover of $K$ satisfies $\widetilde g(N,N)<0$, $\widetilde g^{-1}(\alpha,\alpha)<0$ and $\alpha(N)>0$ on $K$. Orient $\widetilde g$ by $N$ on $K$. Thus if $\alpha=d\tau$ for a smooth real function $\tau$, the $\widetilde g$-gradient of $\tau$ is past timelike on $K$. This asserts persistence on the compact set; it asserts no causal property away from that set.

## Statement references

[[def-causal-exterior-and-boundary-data]]

[[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

[[lem-author-89004136b63c-compact-neighborhood-localization]]

[[lem-author-89004136b63c-temporal-compact-margins]]

[[lem-author-89004136b63c-uniform-inverse-metric-continuity]]

[[math:def-smooth-manifold]]

[[math:def-topological-manifold-without-boundary]]

[[math:thm-compact-subset-of-a-hausdorff-space-is-closed]]

[[math:def-subspace-topology-top]]

[[math:thm-closed-subspace-of-a-compact-space-is-compact]]

## Facts & Assumptions

[F1] Use a finite compact chart cover and the compact margins and component bounds for $\alpha,N$. [[lem-author-89004136b63c-compact-neighborhood-localization]] [[lem-author-89004136b63c-temporal-compact-margins]]

[F2] Uniformly small matrix perturbations make inverse coefficients uniformly close. [[lem-author-89004136b63c-uniform-inverse-metric-continuity]]

[F3] The inverse metric raises covectors, and the past-timelike convention is fixed by pairing positively with $N$. [[physics:def-gr-inverse-metric-and-musical-isomorphisms]] [[def-causal-exterior-and-boundary-data]]

[F4] A smooth manifold has an underlying topological manifold, which is Hausdorff. Every compact subset of a Hausdorff space is closed. Closed sets in a subspace are traces of ambient closed sets, and a closed subspace of a compact space is compact. [[math:def-smooth-manifold]] [[math:def-topological-manifold-without-boundary]] [[math:thm-compact-subset-of-a-hausdorff-space-is-closed]] [[math:def-subspace-topology-top]] [[math:thm-closed-subspace-of-a-compact-space-is-compact]]

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the conclusions in the Statement.

1.1 If $K$ is empty the conclusion is vacuous. Otherwise write $C_j$ for the pieces of the fixed finite compact chart cover and set $K_j=C_j\cap K$. The ambient smooth manifold is Hausdorff by [F4]. Each compact $C_j$ is therefore closed in it, so $K_j=C_j\cap K$ is closed in the compact subspace $K$ and hence compact by [F4]. These compact pieces still cover $K$ and lie where $\alpha,N$ are defined. Choose $m,a,b>0$ from [F1], and a common bound $R\ge1$ for all components of $\alpha$ and $N$ on the restricted pieces $K_j$. For a coefficient perturbation less than $\delta$, the change in $g(N,N)$ has absolute value at most $16\delta R^2$. Choose $\delta<b/(32R^2)$ to retain $\widetilde g(N,N)<0$. [F1, F3, F4]

2.1 Apply [F2] on the restricted pieces $K_j$ with $\eta=m/(32R^2)$ and reduce $\delta$ to its resulting threshold. The change in $g^{-1}(\alpha,\alpha)$ then has absolute value at most $16\eta R^2=m/2$, so it remains negative. The pairing $\alpha(N)\ge a$ does not change with the metric. For $\alpha=d\tau$, [F3] identifies these inequalities with a past-timelike $\widetilde g$-gradient. [F1, F2, F3, step 1.1] ∎
