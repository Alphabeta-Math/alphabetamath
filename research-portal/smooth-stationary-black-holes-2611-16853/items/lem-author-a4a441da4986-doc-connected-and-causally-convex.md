---
id: lem-author-a4a441da4986-doc-connected-and-causally-convex
title: The selected exterior is connected and causally convex
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-push-up-rule
  - math:def-countable-choice
  - math:def-dependent-choice
  - physics:lem-gr-causal-curve-calculus
  - math:def-connected-space
  - math:cor-connected-subsets-of-the-line
  - math:thm-continuous-image-of-a-connected-space
  - math:thm-unions-of-connected-sets
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-push-up-rule: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-dependent-choice: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  math:def-connected-space: mathematical-premise
  math:cor-connected-subsets-of-the-line: mathematical-premise
  math:thm-continuous-image-of-a-connected-space: mathematical-premise
  math:thm-unions-of-connected-sets: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Assume Countable Choice and Dependent Choice. Let $(M,g,N)$ be a time-oriented smooth Lorentzian four-manifold of signature $(-,+,+,+)$, let $U\subset M$ be connected and open, and put $E=I^-_M(U)\cap I^+_M(U)$, with chronology and curves understood in the causal-exterior interface. Then $U\subset E$, the exterior $E$ is connected, and every causal curve in $M$ with both endpoints in $E$ stays in $E$. These claims use no stationary product, nonzero horizon field, maximal hypersurface or lapse sign.

## Statement references

[[def-causal-exterior-and-boundary-data]]

[[physics:lem-gr-chronology-openness]]

[[physics:lem-gr-push-up-rule|Push-up rule]]

[[math:def-countable-choice]]

[[math:def-dependent-choice]]

[[physics:lem-gr-causal-curve-calculus]]

[[math:def-connected-space]]

[[math:cor-connected-subsets-of-the-line]]

[[math:thm-continuous-image-of-a-connected-space]]

[[math:thm-unions-of-connected-sets]]

## Facts & Assumptions

[A1] Assume Countable Choice and Dependent Choice in the senses of [[math:def-countable-choice]] and [[math:def-dependent-choice]]. These are the hypotheses of the causal-curve calculus, chronology-openness and push-up suppliers used below; no assertion of their necessity for the conclusion is made.

[F1] The time-oriented Lorentzian geometry, locally absolutely continuous causal and timelike curves, chronological relations, and exterior $E=I^-_M(U)\cap I^+_M(U)$ have the meanings in [[def-causal-exterior-and-boundary-data]], with its ambient domain denoted by $M$. Only its construction for an arbitrary open $U$ is used; no stationary-end structure is required.

[F2] Restrictions to nondegenerate subintervals preserve local absolute continuity and the almost-everywhere future causal or timelike velocity condition, directly from the curve definitions in [[def-causal-exterior-and-boundary-data]]. Smooth future timelike segments belong to this curve class, and finite concatenation and positive affine reparametrization preserve it by [[physics:lem-gr-causal-curve-calculus]], clauses (a), (c), (d) and (e), under [A1]. In particular, chronological relations concatenate.

[F3] Under [A1], chronological futures and pasts of points are open by [[physics:lem-gr-chronology-openness]], clause (a). Also $a\ll_M p\le_M z$ implies $a\ll_M z$, and $z\le_M q\ll_M b$ implies $z\ll_M b$, by [[physics:lem-gr-push-up-rule|Push-up rule]], clauses (a) and (b), for the same smooth Lorentzian geometry and curve class.

[F4] Connected subsets have the subspace-topology meaning of [[math:def-connected-space]], including the connectedness of the empty set. Real intervals are connected by [[math:cor-connected-subsets-of-the-line]], and their continuous images are connected by [[math:thm-continuous-image-of-a-connected-space]], claim 1. A family of connected subsets each meeting a fixed connected subset has connected union together with that subset by [[math:thm-unions-of-connected-sets]], claim 2.

## Proof

**Given:** The geometry, connected open subset $U$, chronological exterior and choice assumptions in the Statement and [A1], with the interfaces [F1]–[F4].

**Goal:** Prove $U\subset E$, connectedness of $E$, and causal convexity in $M$.

1.1 For $x\in U$, take a smooth chart centered at $x$ and a future timelike vector at $x$. The coordinate straight segment in that direction is future timelike for all sufficiently small positive and negative parameter values, by continuity of the metric and the orientation field, and lies in $U$ because $U$ is open. It is an admissible timelike curve by [F2]. Its two halves give points $x_-,x_+\in U$ with $x_-\ll_M x\ll_M x_+$, hence $x\in E$. Thus $U\subset E$. The sets $I^\pm_M(U)$ are unions of the open chronological futures or pasts of their points by [F1] and [F3], so $E$ is open as well. [given, A1, F1, F2, F3]

2.1 If $U=\varnothing$, then $E=\varnothing$ and all conclusions hold, so consider nonempty $U$. Fix any $p\in E$. By [F1] there are $a,b\in U$ and future timelike curves from $a$ to $p$ and from $p$ to $b$. Reparametrize the first on $[0,1]$ using [F2]. Each interior point $z$ of that curve satisfies $a\ll_M z\ll_M p\ll_M b$ by restriction and concatenation, hence belongs to $E$; its endpoints also belong to $E$. Now take the set of all such timelike curves $\gamma:[0,1]\to M$ whose initial point lies in $U$ and whose final point lies in $E$. Their images lie in $E$ by the same argument, and every $p\in E$ is a final point of one. Each image is connected by the interval and continuous-image results in [F4], and meets the connected set $U$. The common-connected-core union result in [F4] therefore makes their union together with $U$, which equals $E$, connected. Taking all such curves selects no family of witnesses indexed by $E$. [given, A1, F1, F2, F4, step 1.1]

3.1 Let a future causal curve have endpoints $p,q\in E$, and let $z$ be any point on it. Restriction gives $p\le_M z\le_M q$, including endpoint equalities. There are $a,b\in U$ with $a\ll_M p$ and $q\ll_M b$ by [F1]. The two push-up implications of [F3], under [A1], give $a\ll_M z\ll_M b$. Thus $z\in I^+_M(U)\cap I^-_M(U)=E$, proving causal convexity. The same conclusion for a past-directed curve follows by reversing its parameter and interchanging its endpoints. [given, A1, F1, F2, F3] ∎
