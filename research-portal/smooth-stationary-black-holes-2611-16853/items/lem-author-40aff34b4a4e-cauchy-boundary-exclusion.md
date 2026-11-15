---
id: lem-author-40aff34b4a4e-cauchy-boundary-exclusion
title: A Cauchy section cannot end on only one chronological horizon
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - physics:def-gr-causal-curves-and-reachability
  - physics:lem-gr-causal-curve-conventions
  - lem-author-40aff34b4a4e-chronological-exterior-connectivity
  - math:def-axiom-of-choice
  - physics:lem-gr-push-up-rule
  - physics:lem-gr-chronology-openness
  - math:thm-choice-implies-dependent-implies-countable-choice
  - physics:thm-gr-local-geodesics-and-exponential-map
  - physics:lem-gr-parallel-transport-and-geodesic-speed
  - physics:lem-gr-maximal-geodesics-and-extension
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  physics:lem-gr-causal-curve-conventions: mathematical-premise
  lem-author-40aff34b4a4e-chronological-exterior-connectivity: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  physics:lem-gr-push-up-rule: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  physics:lem-gr-parallel-transport-and-geodesic-speed: mathematical-premise
  physics:lem-gr-maximal-geodesics-and-extension: mathematical-premise
proof_strategy: direct
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 3
---

## Statement

In the setting of [[lem-author-40aff34b4a4e-chronological-exterior-connectivity]], let $\Sigma$ be a smooth spacelike hypersurface and $C=\Sigma\cap E$ a Cauchy hypersurface of $E$. Then every point of the boundary of $C$ in $\Sigma$ lies in $\partial A\cap\partial B$. The Cauchy and inextendibility conventions are those of [[def-causal-exterior-and-boundary-data]].

## Facts & Assumptions

[F1] Work in ZFC, including the Axiom of Choice. AC implies Dependent Choice and Countable Choice, meeting the inherited choice hypotheses of the causal suppliers used below. [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]]

[F2] Use the stated locally absolutely continuous causal and timelike curves, endpoint definition of inextendibility, and parameter-counting Cauchy condition, recomputed in the open spacetime $E$. The chronological exterior supplier makes $A$, $B$ and $E$ open and $E$ causally convex in $D$. Chronological openness and push-up give transitivity, so $A=I_D^-(U)$ is a past set and $B=I_D^+(U)$ is a future set. [[def-causal-exterior-and-boundary-data]] [[physics:def-gr-causal-curves-and-reachability]] [[lem-author-40aff34b4a4e-chronological-exterior-connectivity]] [[physics:lem-gr-chronology-openness]] [[physics:lem-gr-push-up-rule|Push-up rule]]

[F3] The geodesic initial-value theorem, clause (a), supplies a smooth geodesic through any specified point and tangent on an open interval about zero. The geodesic-speed lemma, clause 3 and its time-orientation argument in Proof 3.2, preserves the timelike character and future direction of a geodesic initially tangent to the specified future timelike orientation field $N$. Thus these suppliers apply at $p$ with initial tangent $N_p$. [[physics:thm-gr-local-geodesics-and-exponential-map]] [[physics:lem-gr-parallel-transport-and-geodesic-speed]]

[F4] The maximal-geodesic extension lemma, clause (c), places every causal segment on an inextendible causal curve through a strictly increasing affine identification of the segment parameters. Its clause (d) gives acausality of Cauchy sets. Apply these mathematical conclusions to the time-oriented smooth Lorentzian four-manifold $(E,g|_E,N|_E)$, with inextendibility relative to $E$. [[physics:lem-gr-maximal-geodesics-and-extension]]

[F5] The causal-convention lemma, clause (d), extends a future-inextendible future causal curve on $[0,\infty)$ to a curve inextendible in both directions while preserving that entire half-line parametrization. It applies in $E$; it does not assert extension of an arbitrary finite segment. [[physics:lem-gr-causal-curve-conventions]]

## Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Its asserted conclusions.

1.1 Any future causal segment in $E$ with both endpoint values in $C$ would, by clause (c) in [F4], lie on an inextendible causal curve in $E$ having two distinct parameter values in $C$. This contradicts the Cauchy condition, even if the endpoint values coincide. In particular $C$ is acausal in $E$. An ambient timelike curve in $D$ whose endpoints lie in $C$ lies wholly in $E$ by causal convexity, so no such timelike curve exists either. Thus $C$ is achronal also for the ambient chronological relation. [given, F1, F2, F4]

1.2 Let $p\in\partial_\Sigma C$. Since $E$ is open and $C=\Sigma\cap E$, the set $C$ is open in $\Sigma$ and its boundary is disjoint from $C$. Hence $p\notin E$. Every neighborhood of $p$ in $D$ meets $C\subset A\cap B$, so $p\in\overline A\cap\overline B$. As $A$ and $B$ are open and $p\notin A\cap B$, at least one of $p\in\partial A$ and $p\in\partial B$ holds. [given, F2]

2.1 Suppose $p\in\partial A\setminus\partial B$. Then $p\in B$ and $p\notin A$. In $D$, take the geodesic $\rho$ with $\rho(0)=p$ and $\rho'(0)=N_p$. By [F3] it is smooth and future timelike. Since $B$ is open, continuity permits $\varepsilon>0$ such that $\rho$ is defined on $[-\varepsilon,0]$ and this segment lies in $B$. For $-\varepsilon\le t<0$, put $z=\rho(t)$; its timelike segment to $p$ gives $z\ll_D p$. Openness makes $I_D^+(z)$ a neighborhood of $p$, which therefore meets $A$ because $p\in\overline A$. Choose $w\in A\cap I_D^+(z)$; the past-set property of $A$ gives $z\in A$. Thus $\rho([-\varepsilon,0))\subset E$, and its future limit $p$ is outside $E$. [given, F1, F2, F3, step 1.2, construct]

3.1 Define $\gamma:[0,\infty)\to E$ by $\gamma(s)=\rho(-\varepsilon e^{-s})$. This is smooth with nonzero future timelike velocity, since the parameter derivative is $\varepsilon e^{-s}>0$. It tends to $p$ in $D$ as $s\to\infty$; it cannot converge to a point of $E$, by uniqueness of limits in the Hausdorff manifold $D$ and $p\notin E$. Thus it is future-inextendible in $E$. Apply [F5] to obtain an inextendible future causal $\gamma^*:I^*\to E$ agreeing with $\gamma$ on $[0,\infty)$. The Cauchy property gives $a\in I^*$ with $c=\gamma^*(a)\in C$. Choose $s>\max\{0,a\}$. The segment of $\gamma^*$ gives $c\le_E\gamma(s)$, while the remaining timelike geodesic segment gives $\gamma(s)\ll_D p$. Push-up yields $c\ll_D p$. Now $I_D^+(c)$ is an open neighborhood of $p$ and $p\in\partial_\Sigma C$, so it contains some $c'\in C$. This yields $c\ll_D c'$, contradicting step 1.1. [given, F1, F2, F5, step 1.1, step 1.2, step 2.1, construct]

4.1 If $p\in\partial B\setminus\partial A$, reverse the time orientation to $-N$. This exchanges $A$ with $B$, preserves $E$, causal convexity and the Cauchy condition, and the same geodesic and one-sided-extension suppliers apply. Steps 2.1 and 3.1 then give the time-reversed contradiction. Step 1.2 places every boundary point on at least one of the two boundaries, and both single-boundary cases have now been excluded. Therefore $\partial_\Sigma C\subset\partial A\cap\partial B$. [given, F1, F2, F3, F4, F5, step 1.1, step 1.2, step 2.1, step 3.1] ∎

## Supplier interfaces

[[math:def-axiom-of-choice]] [[physics:lem-gr-push-up-rule|Push-up rule]] [[physics:lem-gr-chronology-openness]]
