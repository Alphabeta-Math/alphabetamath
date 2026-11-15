---
title: The entire target segment stays on the chronological boundary
status: published
research_item: lem-author-2632702918ef-target-segment-boundary-containment
dependency_level: 4
sources:
  references: []
---

## Prerequisites

- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)
- [lem-author-2632702918ef-compact-target-null-segment](item-lem-author-2632702918ef-compact-target-null-segment)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Under the same compact-target hypotheses, let $\gamma:[0,1]\to E$ be any future causal segment from $p$ to a point $c\in C$. Then $\gamma([0,1])\subset\partial_E I_E^-(C)$. In particular this holds for the null geodesic supplied by the compact-target null-segment lemma.

## Facts & Assumptions

[A1] Work in ZFC; the axiom of choice includes the countable and dependent choice assumptions of the causal suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The relations and metric-selected connection have the meanings in [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data).

[F2] The target is the surface defined in [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data).

[F3] The initial point does not belong to $I_E^-(C)$. [lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)

[F4] A future null geodesic segment from $p$ to some $c\in C$ exists under these hypotheses. [lem-author-2632702918ef-compact-target-null-segment](item-lem-author-2632702918ef-compact-target-null-segment)

[F5] Push-up gives $x\le y\ll z\Rightarrow x\ll z$ and $x\ll y\le z\Rightarrow x\ll z$. [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[F6] Chronological pasts are open. [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[F7] Sufficiently short geodesics with prescribed past timelike initial tangent exist smoothly. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F8] Every piecewise $C^1$ curve with future timelike tangents is a future timelike curve in the stipulated locally absolutely continuous class. [Curve calculus, clause (c)](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the asserted conclusion.

1.1 For $r=\gamma(s)$, causal restriction gives $p\le_Er\le_Ec$. If $r\in I_E^-(C)$, choose $c^{\prime}\in C$ with $r\ll_Ec^{\prime}$; push-up would imply $p\ll_Ec^{\prime}$, contradicting [F3]. Hence every such $r$ is outside $I_E^-(C)$. [F1, F2, F3, F5, given]

2.1 Fix $r=\gamma(s)$ and use [F7] in $E$ to choose a smooth geodesic $\eta$ with $\eta(0)=r$ and $\dot\eta(0)=-N_r$. At $0$ one has $g(\dot\eta,\dot\eta)<0$ and $g(\dot\eta,N)>0$. Smoothness of $g$, $N$ and $\eta$ makes these scalar functions continuous, so both strict inequalities persist on some $[0,\delta]$ within its domain. Thus $\dot\eta$ is past timelike there. For $0<\varepsilon<\delta$, put $r_\varepsilon=\eta(\varepsilon)$. The reversed segment $t\mapsto\eta(\varepsilon-t)$, $0\le t\le\varepsilon$, is smooth with future timelike tangent; [F8] makes it a future timelike curve in the stipulated class, so $r_\varepsilon\ll_Er$, and continuity gives $r_\varepsilon\to r$. Push-up and $r\le_Ec$ imply $r_\varepsilon\ll_Ec$, including when $r=c$. Thus $r$ is in the closure of $I_E^-(C)$ and outside this open set, which places it in its boundary. This argument applies to each $s$, and [F4] supplies the particular null segment. [step 1.1, F1, F4, F5, F6, F7, F8, A1] ∎
