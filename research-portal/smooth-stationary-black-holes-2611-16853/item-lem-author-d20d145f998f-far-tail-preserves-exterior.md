---
title: Two-sided far-tail access preserves the ambient causal exterior
status: published
research_item: lem-author-d20d145f998f-far-tail-preserves-exterior
dependency_level: 5
---

## Prerequisites

- [lem-author-12a8dba09036-maximal-stationary-far-tail-access](item-lem-author-12a8dba09036-maximal-stationary-far-tail-access)
- [lem-author-d20d145f998f-maximal-stationary-past-tail-access](item-lem-author-d20d145f998f-maximal-stationary-past-tail-access)
- [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Assume the Axiom of Choice. For a specified end region $U\subset M$, define its domain of outer communications (DOC) in the fixed ambient spacetime $M$ by $D_M(U):=I^-_M(U)\cap I^+_M(U)$. Let the original ambient chronological exterior be $E=D_M(U_0)=I^-_M(U_0)\cap I^+_M(U_0)$ and suppose that, with the metric and time orientation induced from $M$, $E$ satisfies all the hypotheses of the maximal stationary future-access lemma. For a sufficiently far stationary tail $U_f\subset U_0\cap E$, assume this is the tail identified with $\mathbb R\times\{r>R_f\}$ in that product. Then $I^-_M(U_f)\cap I^+_M(U_f)=E$. In particular $D_M(U_f)=D_M(U_0)$: the original DOC is preserved when its designated end is truncated to any such sufficiently far stationary tail. No assertion about equality of each individual past or future set on the whole ambient manifold is included.

## Statement references

[lem-author-12a8dba09036-maximal-stationary-far-tail-access](item-lem-author-12a8dba09036-maximal-stationary-far-tail-access)

[lem-author-d20d145f998f-maximal-stationary-past-tail-access](item-lem-author-d20d145f998f-maximal-stationary-past-tail-access)

[physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[A1] The Axiom of Choice is assumed to meet the foundational hypothesis of both far-tail access suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Under [A1] and all the future-access hypotheses in the Statement, every $E$ point reaches $U_f$ along a future timelike curve contained in $E$, and is reached from $U_f$ along one. [lem-author-12a8dba09036-maximal-stationary-far-tail-access](item-lem-author-12a8dba09036-maximal-stationary-far-tail-access) [lem-author-d20d145f998f-maximal-stationary-past-tail-access](item-lem-author-d20d145f998f-maximal-stationary-past-tail-access)

[F2] Chronological reachability is existential over timelike curves, so inclusion of domains or endpoint sets gives the corresponding inclusion of chronological sets. [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

## Proof

**Given:**The explicit hypotheses of the Statement.

**Goal:** Establish its exact chronological-access conclusion.

1.1 The Axiom of Choice in [A1] and the full future-access hypotheses in the Statement meet the hypotheses of both access lemmas in [F1]. For $p\in E$, the two curves of [F1] are also timelike curves in $M$. Consequently $p\in I^-_M(U_f)\cap I^+_M(U_f)$, proving inclusion of the original exterior in the new one. The fact that the paths remain in $E$ is part of [F1], not an inference from the old definition alone. [given, A1, F1, F2]

2.1 Conversely $U_f\subset U_0$ implies $I^-_M(U_f)\subset I^-_M(U_0)$ and $I^+_M(U_f)\subset I^+_M(U_0)$. Intersecting and using the definition of $E$ gives the reverse inclusion. By the definition of $D_M$, this also gives $D_M(U_f)=E=D_M(U_0)$, proving preservation of the DOC. Separate one-sided ambient identities remain unasserted. [given, F2, step 1.1] ∎
