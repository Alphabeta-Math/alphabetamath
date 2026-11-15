---
title: Cauchy sections do not end at a one-sided chronological horizon
status: published
research_item: lem-author-e7cde3233cd7-one-sided-boundary-exclusion
dependency_level: 2
sources:
  references: []
---

## Prerequisites

- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [physics:lem-gr-causal-curve-conventions](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-conventions)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [physics:lem-gr-maximal-geodesics-and-extension](https://alphabetamath.cc/physics/item/lem-gr-maximal-geodesics-and-extension)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [physics:lem-gr-parallel-transport-and-geodesic-speed](https://alphabetamath.cc/physics/item/lem-gr-parallel-transport-and-geodesic-speed)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [math:lem-ac-supplies-countable-and-dependent-choice-for-banach-integration](https://alphabetamath.cc/item/lem-ac-supplies-countable-and-dependent-choice-for-banach-integration)


## Statement

Let $U$ be an open region of a time-oriented spacetime, put $P=I^-(U)$, $Q=I^+(U)$ and $E=P\cap Q$, and suppose $C\subset E$ is a Cauchy hypersurface of $E$. Then $\overline C$ cannot meet $Q\cap\partial P$ or $P\cap\partial Q$. Consequently $\overline C\setminus E\subset\partial P\cap\partial Q$. Closures and boundaries here are taken in the ambient spacetime.

## Facts & Assumptions

[F1] Work in ZF with the Axiom of Choice. Chronology, ambient boundaries, the time orientation and the relative Cauchy condition use [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) and [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice).

[F2] Chronological futures and pasts are open. If $P$ is a past set and $p\in\overline P$, then $I^-(p)\subseteq P$; the dual statement holds for future sets. [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness) clauses (a) and (c).

[F3] A future-inextendible future causal curve on $[0,\infty)$ extends to a future causal curve inextendible in both directions; the dual assertion holds in the past direction. This applies in any open Lorentzian submanifold, with inextendibility recomputed there. [physics:lem-gr-causal-curve-conventions](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-conventions) clause (d).

[F4] A timelike relation followed or preceded by a causal relation remains timelike. [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule) clauses (a) and (b).

[F5] A Cauchy set is acausal in its own spacetime. [physics:lem-gr-maximal-geodesics-and-extension](https://alphabetamath.cc/physics/item/lem-gr-maximal-geodesics-and-extension) clause (d).

[F6] Through a point $p$ with future timelike initial vector $N_p$ there is a smooth geodesic on an open interval about $0$. Its tangent remains nonzero future timelike. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map) clause (a), and [physics:lem-gr-parallel-transport-and-geodesic-speed](https://alphabetamath.cc/physics/item/lem-gr-parallel-transport-and-geodesic-speed) clause 3 and its time-orientation argument.

[F7] Smooth future timelike curves belong to the locally absolutely continuous timelike class. Increasing $C^1$ diffeomorphisms of intervals with positive derivative preserve that class and future-inextendibility. Causal reachability is transitive and includes timelike reachability. [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus) clauses (c), (e) and (f).

[F8] In ZF, AC implies Countable Choice and prescribed-initial-point Dependent Choice. These are the choice hypotheses of the causal-curve, chronology and push-up suppliers used here, and AC supplies their inherited choice assumptions. The implication is not restricted to Banach spaces. [math:lem-ac-supplies-countable-and-dependent-choice-for-banach-integration](https://alphabetamath.cc/item/lem-ac-supplies-countable-and-dependent-choice-for-banach-integration).

## Proof

**Given:** The hypotheses in the Statement, the AC assumption in [F1], and the declared supplier interfaces.

**Goal:** Prove the stated conclusions.

1.1 Under the AC assumption in [F1], [F8] supplies Countable Choice and Dependent Choice for all the causal suppliers below. By [F2], $P$ and $Q$ are open, hence $E$ is an open time-oriented Lorentzian submanifold. By [F4] and the inclusion of timelike reachability in causal reachability from [F7], $I^-(P)\subseteq P$ and $I^+(Q)\subseteq Q$: for example $x\ll y\ll u$ with $y\in P$ and $u\in U$ gives $x\ll u$. Thus $P$ is a past set and $Q$ a future set. Every causal segment from $a\in E$ to $b\in E$ stays in $E$: choose $u,v\in U$ with $u\ll a$ and $b\ll v$; every point $x$ of the segment satisfies $a\le x\le b$, so [F4] gives $u\ll x\ll v$. Finally apply [F5] in $E$ to the given Cauchy hypersurface $C$, obtaining acausality relative to $E$. This invokes the Cauchy-set theorem directly, rather than applying one-sided extension to a finite segment. [given, F1, F2, F4, F5, F7, F8]

2.1 Suppose $p\in\overline C\cap Q\cap\partial P$. Use [F6] at $p$ with initial vector $N_p$ to obtain a future timelike geodesic $\beta$ with $\beta(0)=p$. Since $Q$ is open, choose $\varepsilon>0$ so that $\beta([ -\varepsilon,0])\subset Q$. For $-\varepsilon\le t<0$, its smooth timelike segment from $\beta(t)$ to $p$ is an admissible timelike curve by [F7], so $\beta(t)\ll_M p$. Since $p\in\partial P\subseteq\overline P$ and $P$ is a past set, [F2] puts this entire preceding tail in $P$, hence in $E$. Reparametrize it by $t=-\varepsilon/(1+s)$, $s\in[0,\infty)$; this is an increasing smooth diffeomorphism onto $[-\varepsilon,0)$ with positive derivative. By [F7] the resulting curve $\gamma$ is future timelike. It has ambient limit $p$ as $s\to\infty$, and $p\notin P$ since $P$ is open. It therefore has no future endpoint in $E$, so is future-inextendible relative to $E$. [given, F1, F2, F6, F7, step 1.1]

3.1 Apply [F3] in $E$ to $\gamma:[0,\infty)\to E$, obtaining an inextendible future causal curve $\gamma^*:I^*\to E$ that agrees with $\gamma$ for $s\ge0$. The Cauchy condition gives $s_c\in I^*$ with $c=\gamma^*(s_c)\in C$. Choose $s>\max\{s_c,0\}$. The segment of $\gamma^*$ gives $c\le_M\gamma(s)$, while the remaining timelike geodesic segment to $p$ gives $\gamma(s)\ll_M p$. Hence [F4] gives $c\ll_M p$. By [F2], $I_M^+(c)$ is an open neighborhood of $p$; since $p\ne c$, shrink it to a neighborhood $V$ of $p$ avoiding $c$. From $p\in\overline C$ choose $c'\in C\cap V$. Then $c'\ne c$ and $c\ll_M c'$. Step 1.1 puts a joining timelike segment entirely in $E$, contradicting acausality of $C$ there. Reversing the time orientation interchanges $P$ and $Q$ and gives the same contradiction for $p\in\overline C\cap P\cap\partial Q$. [given, F1, F2, F3, F4, F7, step 1.1, step 2.1]

4.1 Since $C\subset P\cap Q$, its closure lies in $\overline P\cap\overline Q$. At any point of that closure outside $E$, at least one of the two open-set memberships fails and hence the corresponding boundary occurs. If the point lies in exactly one of $P,Q$, step 3.1 excludes it. If it lies in neither, it belongs to $\partial P\cap\partial Q$. Thus $\overline C\setminus E\subset\partial P\cap\partial Q$, as claimed. [F1, step 1.1, step 3.1] ∎
