---
title: Combining the collar and end barriers into interior compact confinement
status: published
research_item: lem-author-eb8e266b8b92-interior-compact-confinement
dependency_level: 4
sources:
  references: []
---

## Prerequisites

- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-eb8e266b8b92-collar-nonarrival](item-lem-author-eb8e266b8b92-collar-nonarrival)
- [lem-author-eb8e266b8b92-proper-radius-control](item-lem-author-eb8e266b8b92-proper-radius-control)
- [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)
- [math:thm-the-interior-is-an-open-smooth-n-manifold](https://alphabetamath.cc/item/thm-the-interior-is-an-open-smooth-n-manifold)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)


## Statement

Assume the Axiom of Choice. Let $\overline S$ have the stationary ADM, smooth-boundary and compact-boundary collar data of the collar-barrier lemma, and the proper radius and smooth extensions of the proper-radius lemma. Assume both lemmas' stated estimates. Every causal curve on a bounded section-time interval containing $v_0$ has its spatial image in a compact subset of the interior $S$. More precisely, if $|v-v_0|\le T$, choose $\eta=\tfrac12 b(x(v_0))e^{-CT}>0$ and $m=R(x(v_0))+C_RT$ with the constants and the truncated collar coordinate $b$ of those lemmas. The set $K=\{R\le m\}\setminus\{\rho<\eta\}$ contains the image and is compact in $S$; the removed set denotes the collar neighborhood including the boundary.

## Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[lem-author-eb8e266b8b92-collar-nonarrival](item-lem-author-eb8e266b8b92-collar-nonarrival)

[lem-author-eb8e266b8b92-proper-radius-control](item-lem-author-eb8e266b8b92-proper-radius-control)

[math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

[math:thm-the-interior-is-an-open-smooth-n-manifold](https://alphabetamath.cc/item/thm-the-interior-is-an-open-smooth-n-manifold)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

## Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice is assumed for the inherited interfaces. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F2] The collar barrier gives $b(x(v))\ge b(x(v_0))e^{-C|v-v_0|}$, with $b=\rho$ close to the boundary and constant farther away. [lem-author-eb8e266b8b92-collar-nonarrival](item-lem-author-eb8e266b8b92-collar-nonarrival)

[F3] Proper-radius control gives $R(x(v))\le R(x(v_0))+C_R|v-v_0|$, and every sublevel of $R$ is compact in the manifold with boundary. [lem-author-eb8e266b8b92-proper-radius-control](item-lem-author-eb8e266b8b92-proper-radius-control)

[F4] A closed subspace of a compact topological space is compact; no metric hypothesis is required. [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

[F5] The interior $S=\operatorname{Int}\overline S$ is open in $\overline S$ and carries the smooth structure of restricted charts. Its topology is the subspace topology: open sets are traces of ambient open sets, and because $S$ is open these traces are also open in $\overline S$. [math:thm-the-interior-is-an-open-smooth-n-manifold](https://alphabetamath.cc/item/thm-the-interior-is-an-open-smooth-n-manifold) [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[F6] For a subset of any topological space with the subspace topology, compactness is equivalent to the finite-subcover property for families of ambient open sets covering that subset, including the empty-subset case. [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

## Proof

1.1 The radius estimate places the entire image in $\{R\le m\}$. The collar estimate places it outside $\{\rho<\eta\}$, since within that neighborhood $b=\rho<\eta$ contradicts $b(x(v))\ge2\eta$. The chosen $\eta$ is less than the truncation threshold, so the removed collar neighborhood is unambiguously defined. [F2, F3, algebra]

2.1 Let $C_m=\{R\le m\}$ and let $U_\eta=\{\rho<\eta\}$ denote the stated collar neighborhood. Under the supplied collar diffeomorphism, $U_\eta$ is the image of $[0,\eta)\times B$, open relative to $[0,\epsilon)\times B$; hence it is open in $\overline S$ and contains the entire boundary $B$. Thus $K=C_m\setminus U_\eta$ is closed in the compact space $C_m$ and lies in $S$. The closed-subspace theorem makes $K$ compact with the topology induced from $C_m$. [given, F2, F3, F4, step 1.1]

3.1 The restricted charts identify the topology of $S$ with its open subspace topology in $\overline S$. Consequently, if $V$ is open in $S$, it is open in $\overline S$, and $V\cap C_m$ is open in $C_m$. For any family of open subsets of $S$ covering $K$, their traces on $C_m$ cover $K$. Compactness from step 2.1 and the ambient-cover criterion in $C_m$ give finitely many of those traces covering $K$, so the corresponding original sets also cover $K$. The same ambient-cover criterion in $S$ now proves that $K$ is compact in $S$. Together with step 1.1 this proves interior compact confinement. [F5, F6, step 1.1, step 2.1] ∎
