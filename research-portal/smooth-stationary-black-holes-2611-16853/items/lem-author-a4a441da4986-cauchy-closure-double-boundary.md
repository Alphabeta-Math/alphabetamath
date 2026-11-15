---
id: lem-author-a4a441da4986-cauchy-closure-double-boundary
title: Closure of the exterior Cauchy section meets only the double horizon
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-push-up-rule
  - physics:lem-gr-maximal-geodesics-and-extension
  - physics:lem-gr-causal-curve-calculus
  - math:def-countable-choice
  - math:def-dependent-choice
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-push-up-rule: mathematical-premise
  physics:lem-gr-maximal-geodesics-and-extension: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-dependent-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

Assume Countable Choice and Dependent Choice. Let $(M,g,N)$ be a time-oriented smooth Lorentzian four-manifold of signature $(-,+,+,+)$, let $U\subset M$ be open, and set $E=I^-_M(U)\cap I^+_M(U)$, using ambient chronology in $M$. Suppose $E$ is globally hyperbolic with the restricted metric and time orientation, and let $C$ be a smooth spacelike Cauchy hypersurface of $E$. Then $C$ is closed in $E$, and every point of $\overline C^{\,M}\setminus C$ belongs to $\partial_M I^-_M(U)\cap\partial_M I^+_M(U)$. No acausality of a larger hypersurface outside $E$ is assumed.

## Statement references

[[def-causal-exterior-and-boundary-data]]

[[physics:lem-gr-chronology-openness]]

[[physics:lem-gr-push-up-rule|Push-up rule]]

[[physics:lem-gr-maximal-geodesics-and-extension]]

[[physics:lem-gr-causal-curve-calculus]]

[[math:def-countable-choice]]

[[math:def-dependent-choice]]

## Facts & Assumptions

[A1] Assume Countable Choice and Dependent Choice as in [[math:def-countable-choice]] and [[math:def-dependent-choice]]. These assumptions discharge the choice hypotheses of the chronology, push-up and causal-curve calculus suppliers; no necessity claim for the conclusion is made.

[F1] Use [[def-causal-exterior-and-boundary-data]] with its ambient domain $D$ denoted here by $M$. Only its constructions for an arbitrary open $U$ are used. Chronological sets and ambient closures and boundaries are computed in $M$; Cauchy sets, inextendibility and global hyperbolicity on $E$ use the restricted geometry and curves in $E$. Inextendibility means having no limit in the specified domain at either parameter end.

[F2] Under [A1], [[physics:lem-gr-chronology-openness]], clauses (a) and (b), gives openness of chronological futures, pasts and the chronological relation. It applies both in $M$ and in every open Lorentzian domain with the restricted geometry, in particular $E$ once its openness is established.

[F3] Under [A1], [[physics:lem-gr-push-up-rule|Push-up rule]], clauses (a) and (b), gives $a\ll b\le c\Rightarrow a\ll c$ and $a\le b\ll c\Rightarrow a\ll c$; clause (c) makes a causal segment containing a nondegenerate timelike subsegment chronological between its endpoints. These statements apply in $M$ or in the open restricted spacetime $E$.

[F4] For any open restricted Lorentzian spacetime, [[physics:lem-gr-maximal-geodesics-and-extension]], clause (c), places a compact causal segment on an inextendible causal curve with an increasing affine identification of that segment; clause (d) makes every Cauchy set acausal. Both apply to the Cauchy and inextendibility conventions in [F1], so they can be used in $E$, without ambient completeness.

[F5] Restrictions to nondegenerate subintervals preserve the curve class by its defining local absolute continuity and almost-everywhere velocity condition in [[def-causal-exterior-and-boundary-data]]. Under [A1], [[physics:lem-gr-causal-curve-calculus]], clauses (c), (d), (e) and (f), supplies smooth timelike segments, finite causal or timelike concatenations, positive affine reparametrizations, and transitivity. For a concatenation on open intervals, apply the finite closed-interval assertion on each compact subinterval.

## Proof

**Given:** The geometry, open set $U$, globally hyperbolic exterior $E$, Cauchy hypersurface $C$ and choice assumptions of the Statement, with [A1] and [F1]--[F5].

**Goal:** Prove relative closedness in $E$ and locate every additional ambient closure point in the double chronological boundary.

1.1 The sets $I^\pm_M(U)$ are unions of open chronological futures or pasts of points of $U$, so $E$ is open. It is also causally convex for this arbitrary $U$: if a future causal curve in $M$ has endpoints $a,b\in E$ and passes through $z$, choose $u,v\in U$ with $u\ll_M a$ and $b\ll_M v$. Its restrictions give $a\le_M z\le_M b$, and push-up gives $u\ll_M z\ll_M v$. Thus every point of the curve lies in $E$. Consequently any ambient causal or timelike curve between points of $E$ is also a curve in $E$. No connectedness of $U$ is used. [given, A1, F1, F2, F3, F5]

2.1 By [F4], $C$ is acausal in $E$. Suppose $p\in\overline C^{\,E}\setminus C$. A small coordinate straight segment through $p$, in a future timelike direction, is smooth timelike and lies in $E$: continuity of the metric and time orientation preserves its timelike direction after shrinking the coordinate interval. By [F4] it lies on an inextendible causal curve in $E$. That curve meets $C$ at some $x\ne p$. The subarc between $x$ and $p$ contains a nondegenerate part of the timelike segment next to $p$; [F3] therefore gives $x\ll_E p$ or $p\ll_E x$. Openness of chronology in $E$ gives a neighborhood of $p$, chosen to omit $x$, whose points have the same relation to $x$. It meets $C$ by the closure assumption, contradicting acausality. Thus $C$ is closed in $E$. Since $E$ is open, every $p\in\overline C^{\,M}\setminus C$ lies outside $E$. [given, A1, F1, F2, F3, F4, F5, step 1.1]

3.1 Fix $p\in\overline C^{\,M}\setminus C$, and suppose $p\in I^+_M(U)$. Choose a future timelike curve $\gamma:[0,1]\to M$ from some $u\in U$ to $p$. For $0<t<1$, put $z=\gamma(t)$. Then $u\ll_M z\ll_M p$. The open set $I^+_M(z)$ contains $p$ and hence meets $C$ at some $c$. Since $c\in E\subset I^-_M(U)$, there is $v\in U$ with $c\ll_M v$. Concatenation gives $z\ll_M c\ll_M v$, so $z\in I^-_M(U)$; also $u\ll_M z$ gives $z\in I^+_M(U)$. Therefore $\gamma((0,1))\subset E$. [given, A1, F1, F2, F5, step 2.1]

4.1 Choose $0<s_0<s<1$. Apply [F4] in $E$ to the compact segment $\gamma|_{[s_0,s]}$. Take the resulting inextendible causal curve's entire past portion up to its parameter corresponding to $\gamma(s)$, and then append $\gamma|_{[s,1)}$, matching the junction parameters by a positive affine change. This concatenation is a future causal curve in $E$ by [F5]. Its past end has no limit in $E$, since it is unchanged from the inextendible extension. Its future end converges in $M$ to $p\notin E$, and so cannot converge to a point of $E$, by uniqueness of limits in the Hausdorff manifold $M$. It is therefore inextendible in $E$. This construction needs only the segment-extension assertion, not an assertion that the entire extension is timelike. [given, A1, F1, F4, F5, step 2.1, step 3.1]

5.1 The Cauchy property gives a point $x\in C$ on the curve of step 4.1. Choose a point $z$ on its appended timelike tail strictly after that intersection. Then $x\le_M z\ll_M p$, so push-up gives $x\ll_M p$. The open neighborhood $I^+_M(x)$ of $p$, intersected with $M\setminus\{x\}$, meets $C$ at some $q\ne x$ because $p\in\overline C^{\,M}$ and $p\ne x$. Thus $x\ll_M q$. The connecting timelike curve stays in $E$ by step 1.1, yielding $x\ll_E q$, contrary to the acausality in step 2.1. Hence $p\notin I^+_M(U)$. [given, A1, F1, F2, F3, F5, step 1.1, step 2.1, step 4.1]

6.1 Apply steps 3.1--5.1 with time orientation reversed. The exterior $E$ and Cauchy condition are unchanged, while $I^+_M(U)$ and $I^-_M(U)$ are interchanged, so $p\notin I^-_M(U)$ as well. Finally $C\subset E\subset I^\pm_M(U)$ implies $p\in\overline{I^+_M(U)}^{\,M}\cap\overline{I^-_M(U)}^{\,M}$. Both chronological sets are open; exclusion from each therefore places $p$ in both ambient boundaries. This proves the claimed inclusion, together with the relative closedness already proved. [given, A1, F1, F2, F3, F4, F5, step 2.1, step 3.1, step 4.1, step 5.1] ∎
