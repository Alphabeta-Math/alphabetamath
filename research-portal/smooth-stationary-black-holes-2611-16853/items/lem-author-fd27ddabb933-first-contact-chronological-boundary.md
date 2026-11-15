---
id: lem-author-fd27ddabb933-first-contact-chronological-boundary
title: First contact lies on the chronological and causal future boundary
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-fd27ddabb933-compact-first-cylinder-contact
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-push-up-rule
  - physics:lem-gr-globally-hyperbolic-causal-structure
  - def-causal-exterior-and-boundary-data
  - physics:thm-gr-local-geodesics-and-exponential-map
  - physics:lem-gr-parallel-transport-and-geodesic-speed
  - math:def-axiom-of-choice
dependency_roles:
  lem-author-fd27ddabb933-compact-first-cylinder-contact: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-push-up-rule: mathematical-premise
  physics:lem-gr-globally-hyperbolic-causal-structure: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  physics:lem-gr-parallel-transport-and-geodesic-speed: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

Work in ZFC. At the earliest cylinder time, every contact point $p_R$ lies in $\partial I^+(A)=\partial J^+(A)$ and satisfies $\tau(p_R)>0$ for the supplied temporal function $\tau$. No point of the whole cut $C_{t_R}$ belongs to $I^+$(A). These statements concern causal relations in the open exterior and do not assume a global event-horizon identity for the transformed metric.

## Facts & Assumptions

[F1] Use the full data and hypotheses of the compact-contact lemma in the same exterior $\mathcal E$: its compact source $A\subset\tau^{-1}(0)$, cuts $C_t=\Phi(\{t\}\times C_0)$, continuous parameter map $\Phi$, and finite earliest causal-contact time $t_R$. Its conclusion supplies $C_{t_R}\cap J^+(A)\ne\varnothing$ and $\tau(p)>0$ for every causal contact point $p$ with the cylinder. This positivity concerns the temporal-function value; no sign for the cut parameter $t_R$ is supplied. [[lem-author-fd27ddabb933-compact-first-cylinder-contact]]

[F2] Chronological futures are open. [[physics:lem-gr-chronology-openness]]

[F3] A causal segment followed or preceded by a timelike segment gives a timelike relation. [[physics:lem-gr-push-up-rule|Push-up rule]]

[F4] The causal future of the compact source is closed in the globally hyperbolic exterior. [[physics:lem-gr-globally-hyperbolic-causal-structure]]

[F5] Use the causal-curve, chronological-future and temporal-function conventions of the causal-data definition. All relations, closures, interiors and boundaries in this argument are relative to $\mathcal E$; boundary means closure minus interior. [[def-causal-exterior-and-boundary-data]]

[F6] On a time-oriented smooth Lorentzian four-manifold, the geodesic with any initial point and tangent exists on an open parameter interval containing zero and is smooth. Use clauses (a) and (b) on $\mathcal E$ with initial tangent $N_p$, the future timelike orientation vector at $p$. [[physics:thm-gr-local-geodesics-and-exponential-map]]

[F7] Along a nonconstant geodesic its tangent is nowhere zero, its squared norm is constant, and a causal tangent retains its time orientation. Use clause 3 and Proof 3.2 for the geodesic in [F6]; no geodesic completeness is required. [[physics:lem-gr-parallel-transport-and-geodesic-speed]]

[A1] Work in ZFC, including the countable and dependent choice required by the invoked geodesic, compactness and causal interfaces. [[math:def-axiom-of-choice]]

## Proof

**Given:** The assumptions in the Statement, with the data and hypotheses specified in [F1].

**Goal:** Establish the stated conditional claim.

1.1 Suppose $p\in C_{t_R}\cap I^+(A)$ and write $p=\Phi(t_R,x)$ for some $x\in C_0$. By [F2], $I^+(A)$ is open (it is the union of the open chronological futures of points of $A$). Continuity of $\Phi$ from [F1] then puts $\Phi(t_R-\varepsilon,x)$ in $I^+(A)\subset J^+(A)$ for all sufficiently small $\varepsilon>0$. This is a causal contact on $C_{t_R-\varepsilon}$, contradicting the minimum property of $t_R$. Hence the whole first cut misses $I^+(A)$. Every causal contact point $p$ on it satisfies $\tau(p)>0$ by the temporal-value conclusion already proved in [F1]. [given, A1, F1, F2, F5, contradiction]

1.2 For any $p\in\mathcal E$, take the geodesic $\gamma$ of [F6] with $\gamma(0)=p$ and $\gamma'(0)=N_p$. By [F7] it is future timelike on a sufficiently small interval about zero. For small $s>0$, its restrictions give $\gamma(-s)\ll p\ll\gamma(s)$, and smoothness gives $\gamma(\pm s)\to p$ as $s\downarrow0$. These segments and their endpoints lie in $\mathcal E$, since the geodesic was constructed on that manifold. Thus every neighborhood of $p$ contains points strictly to its timelike past and future. [A1, F5, F6, F7, construct]

2.1 If $p\in J^+(A)$, the future points from step 1.2 lie in $I^+(A)$ by [F3], so $p\in\overline{I^+(A)}$. Conversely $I^+(A)\subset J^+(A)$ and [F4] give $\overline{I^+(A)}\subset J^+(A)$. Thus $J^+(A)=\overline{I^+(A)}$. If $p\in\operatorname{int}J^+(A)$, an open neighborhood of $p$ contained in $J^+(A)$ contains a point $z\ll p$ by step 1.2; some $a\in A$ satisfies $a\le z$, and [F3] gives $a\ll p$. The reverse inclusion $I^+(A)\subset\operatorname{int}J^+(A)$ follows from [F2]. Hence $\operatorname{int}J^+(A)=I^+(A)$. Using the boundary convention of [F5], $\partial I^+(A)=J^+(A)\setminus I^+(A)=\partial J^+(A)$. The contact points supplied by [F1] belong to that difference by step 1.1, which also proves the whole-cut exclusion and positivity of $\tau$. [A1, F1, F2, F3, F4, F5, step 1.1, step 1.2, algebra] ∎
