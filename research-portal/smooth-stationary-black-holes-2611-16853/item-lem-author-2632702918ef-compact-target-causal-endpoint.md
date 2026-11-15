---
title: A compact chronological target supplies a causal endpoint
status: published
research_item: lem-author-2632702918ef-compact-target-causal-endpoint
dependency_level: 2
sources:
  references: []
---

## Prerequisites

- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [physics:lem-gr-globally-hyperbolic-causal-structure](https://alphabetamath.cc/physics/item/lem-gr-globally-hyperbolic-causal-structure)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)
- [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)


## Statement

Let $(E,g,N)$ be globally hyperbolic in the causal-exterior interface, and let $C\subset E$ be a compact spacelike two-surface in the null-screen interface. Let $\tau$ be a temporal function and suppose $p\in\partial_E I_E^-(C)$ with $\tau(p)<\min_C\tau$. Then some $c\in C$ satisfies $p\le_Ec$ and $p\ne c$, whereas $p\notin I_E^-(C)$. No acausality of $C$ is assumed.

## Facts & Assumptions

[A1] Work in ZFC; the axiom of choice includes the countable and dependent choice assumptions of the causal suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] All chronological and causal relations, boundaries, temporal functions and global hyperbolicity are relative to $E$. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F2] A spacelike two-surface is a nonempty smooth embedded two-manifold without boundary with positive-definite induced metric. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F3] In a globally hyperbolic spacetime, $J^-(C)$ is closed for compact $C$. [physics:lem-gr-globally-hyperbolic-causal-structure](https://alphabetamath.cc/physics/item/lem-gr-globally-hyperbolic-causal-structure)

[F4] The chronological past of each point is open. [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[F5] Arbitrary unions of open sets are open, by topology axiom (T2). [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)

[F6] A continuous real-valued function on a nonempty compact space attains its minimum, by the extreme-value clause (2). The restriction of a continuous function to a subspace is continuous. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the asserted conclusion.

1.1 The set $I_E^-(C)=\bigcup_{c\in C}I_E^-(c)$ is open by [F4] and [F5], so its boundary is disjoint from it. Every point of that set lies in $J_E^-(C)$; its closure also lies there by [F3]. Thus $p\in J_E^-(C)\setminus I_E^-(C)$. [A1, F1, F2, F3, F4, F5, given]

2.1 The temporal function $\tau$ is continuous by [F1], so $\tau|_C$ is continuous by [F6]. The space $C$ is nonempty by [F2] and compact by hypothesis; clause (2) of [F6] therefore makes $\min_C\tau$ well defined. By the definition of $J_E^-(C)$ there is a $c\in C$ with $p\le_Ec$. If $p\in C$, minimality would give $\min_C\tau\le\tau(p)$, contrary to the strict temporal inequality. Thus $p\notin C$ and $p\ne c$. Together with step 1.1 this proves the assertion without any condition on causal relations among different points of $C$. [step 1.1, F1, F2, F6, given] ∎
