---
title: Past access to the far tail by exact time reversal
status: draft
research_item: lem-author-d20d145f998f-maximal-stationary-past-tail-access
dependency_level: 4
---

## Prerequisites

- [lem-author-12a8dba09036-maximal-stationary-far-tail-access](item-lem-author-12a8dba09036-maximal-stationary-far-tail-access)
- [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)


## Statement

Under all the hypotheses of the maximal stationary far-tail-access lemma, every point of $E$ belongs also to $I^+_E(U_f)$ for every sufficiently far stationary tail $U_f=\mathbb R\times\{r>R_f\}$. Here the metric, domain, slice and end are unchanged. Thus the original-metric chronological access is two-sided. This is not a statement about the Harrison metric with a fixed parameter or about its transferred future paths.

## Statement references

[lem-author-12a8dba09036-maximal-stationary-far-tail-access](item-lem-author-12a8dba09036-maximal-stationary-far-tail-access)

[physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

## Facts & Assumptions

[F1] The authored future-access lemma applies to any smooth maximal stationary Lorentz product with the exact geometric, positivity, tangency and asymptotic hypotheses stated there. [lem-author-12a8dba09036-maximal-stationary-far-tail-access](item-lem-author-12a8dba09036-maximal-stationary-far-tail-access)

[F2] Chronological past/future and time orientation are those of the causal-curve interface, and the hypersurface conventions define $k=-g(\nabla n,\cdot)$. [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

## Proof

**Given:**The explicit hypotheses of the Statement.

**Goal:** Establish its exact chronological-access conclusion.

1.1 Reverse the spacetime time orientation and replace $T$ by $T'=-T$ and its stationary coordinate $t$ by $t'=-t$. The future unit normal is $n'=-n$. Hence $T'=Nn'+X'$ with $X'=-X$ and unchanged positive $N$. The induced metric is unchanged; $k'=-k$ is still trace-free. Boundary tangency and smooth extension are unchanged, as are the complete stationary flow and product topology. The end components satisfy $g'_{00}=g_{00}$, $g'_{0i}=-g_{0i}$, $g'_{ij}=g_{ij}$, so all end bounds and future timelikeness of $T'$ in the reversed orientation hold. The set $U_f$ is the same subset because its time factor is all of $\mathbb R$. Thus every hypothesis of [F1] is preserved, not merely the maximal-slice condition. [F1, F2]

2.1 Apply [F1] in this reversed setting. It gives $E\subset I^-_{E,\mathrm{rev}}(U_f)$. Reversing a future timelike curve in the reversed orientation gives a future timelike curve in the original orientation from $U_f$ to its original starting point. Therefore this is precisely $E\subset I^+_E(U_f)$. Combining it with the original [F1] gives both chronological accesses. No assertion about a deformed metric is used. [F1, F2, step 1.1] ∎
