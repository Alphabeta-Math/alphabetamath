---
id: lem-author-12a8dba09036-open-end-causal-convexity-and-geodesic-pieces
title: An open chronological exterior is causally convex without a timelike-end
  assumption
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - physics:def-gr-causal-curves-and-reachability
  - physics:lem-gr-push-up-rule
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-convex-normal-causality
  - physics:thm-gr-local-geodesics-and-exponential-map
  - math:def-axiom-of-choice
  - physics:thm-gr-convex-normal-neighborhoods
  - physics:thm-gr-normal-neighborhood-causal-cone
  - math:thm-heine-borel-rn
  - math:thm-lebesgue-number-lemma
  - physics:lem-gr-causal-curve-calculus
  - math:thm-choice-implies-dependent-implies-countable-choice
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  physics:lem-gr-push-up-rule: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-convex-normal-causality: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  physics:thm-gr-convex-normal-neighborhoods: mathematical-premise
  physics:thm-gr-normal-neighborhood-causal-cone: mathematical-premise
  math:thm-heine-borel-rn: mathematical-premise
  math:thm-lebesgue-number-lemma: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

For any open subset $U$ of a smooth time-oriented spacetime put $E=I^-(U)\cap I^+(U)$. Then $U\subset E$, and any ambient causal segment with endpoints in $E$ is contained in $E$. If $p\in E$ is chronologically before some $z$ in a specified open far tail $U_f\subset U$, a future timelike path from $p$ to $z$ can be replaced, with the same endpoints, by finitely many smooth future timelike geodesic pieces inside $E$. This lemma does not prove the existence of such a $z\in U_f$ for every $p\in E$.

## Statement references

[[def-causal-exterior-and-boundary-data]]

[[physics:def-gr-causal-curves-and-reachability]]

[[physics:lem-gr-push-up-rule|Push-up rule]]

[[physics:lem-gr-chronology-openness]]

[[physics:lem-gr-convex-normal-causality]]

[[physics:thm-gr-local-geodesics-and-exponential-map]]

[[math:def-axiom-of-choice]]

[[physics:thm-gr-convex-normal-neighborhoods]]

[[physics:thm-gr-normal-neighborhood-causal-cone]]

[[math:thm-heine-borel-rn]]

[[math:thm-lebesgue-number-lemma]]

[[physics:lem-gr-causal-curve-calculus]]

[[math:thm-choice-implies-dependent-implies-countable-choice]]

## Facts & Assumptions

[F1] Chronology, the causal exterior and causal curves have the stated meanings; timelike--causal concatenation obeys push-up, and chronological futures and pasts are open. [[def-causal-exterior-and-boundary-data]] [[physics:def-gr-causal-curves-and-reachability]] [[physics:lem-gr-push-up-rule|Push-up rule]] [[physics:lem-gr-chronology-openness]]

[F2] Local smooth geodesics and their exponential maps exist. Every point in an open neighborhood $O$ has a strictly convex normal neighborhood $C\subset O$ that is normal at every one of its points, with a unique contained geodesic between each pair of points. For every $x\in C$, the cone theorem gives $I_C^+(x)=\exp_x(\mathcal T_x^+)$; thus endpoints chronologically related by a timelike curve in $C$ are joined by the smooth future timelike radial geodesic in $C$. The fixed-base ball lemma also records this cone characterization at its specified base point. [[physics:thm-gr-local-geodesics-and-exponential-map]] [[physics:thm-gr-convex-normal-neighborhoods]] [[physics:thm-gr-normal-neighborhood-causal-cone]] [[physics:lem-gr-convex-normal-causality]]

[F3] A closed bounded real interval is compact by Heine--Borel. Every relatively open cover of that interval has a finite subcover and a Lebesgue number $\delta>0$: every nonempty subset of diameter less than $\delta$ lies in one cover member. [[math:thm-heine-borel-rn]] [[math:thm-lebesgue-number-lemma]]

[F4] Restrictions to nondegenerate compact subintervals preserve local absolute continuity and the almost-everywhere timelike or causal velocity condition directly from the curve definition. Increasing affine reparametrizations preserve these curve classes, and finite concatenations of smooth future timelike pieces are future timelike curves. [[physics:def-gr-causal-curves-and-reachability]] [[physics:lem-gr-causal-curve-calculus]]

[A1] Work in ZFC. AC implies Dependent Choice and Countable Choice, supplying the inherited choice hypotheses of the causal results in [F1], [F2] and [F4]. [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]]

## Proof

**Given:** The stated data and explicit hypotheses.

**Goal:** Establish the stated causal convexity and conditional geodesic replacement.

1.1 Every point of the open set $U$ has a short future and past timelike segment remaining in $U$, by local geodesic existence in [F2], so it lies in $I^-(U)\cap I^+(U)$. If a causal segment has endpoints $p,q\in E$ and passes through $y$, its restrictions give $p\le y\le q$, including equality at the endpoints. Choose $u_-\ll p$ and $q\ll u_+$ with $u_\pm\in U$. Push-up gives $u_-\ll y\ll u_+$, so $y\in E$. Also $I^\pm(U)$ are unions of open pointwise chronological futures or pasts, so $E$ is open. This proves causal convexity without a timelike stationary-field assumption on $U$. [F1, F2, F4, A1]

2.1 Under the explicit accessibility hypothesis choose a future timelike curve $\gamma:[a,b]\to M$, $a<b$, with endpoints $p$ and $z$. Both endpoints lie in $E$ by step 1.1, so its entire image lies in $E$. Since $E$ is open, [F2] supplies a cover of this image by strictly convex normal neighborhoods $C\subset E$. The inverse images $\gamma^{-1}(C)$ form a relatively open cover of $[a,b]$, because $\gamma$ is continuous. By [F3] take a finite subcover and a Lebesgue number $\delta>0$ for that subcover on the compact metric interval $[a,b]$. Choose a finite partition $a=t_0<\cdots<t_m=b$ of mesh less than $\delta$. Each $[t_{j-1},t_j]$ then lies in some $\gamma^{-1}(C_j)$, so $\gamma([t_{j-1},t_j])\subset C_j\subset E$. [given, F1, F2, F3, A1, step 1.1]

3.1 The restriction of $\gamma$ to $[t_{j-1},t_j]$, affinely reparametrized to $[0,1]$, is future timelike in $C_j$ by [F4]. Its endpoints are therefore chronologically related in $C_j$, not merely in the ambient spacetime. Apply the cone theorem of [F2] with base point $\gamma(t_{j-1})$, which is legitimate because $C_j$ is normal at every one of its points. The inverse-exponential displacement to $\gamma(t_j)$ is future timelike, and the radial geodesic is smooth, future timelike and contained in $C_j$. Replace each restricted curve by this geodesic and affinely parametrize it on $[t_{j-1},t_j]$. [F2, F4, A1, step 2.1]

4.1 The finitely many geodesic pieces have matching endpoints. Their concatenation is a future timelike curve by [F4], is smooth on each piece, stays in $E$ and has the original endpoints $p,z$. This establishes the asserted conditional replacement. No access to the far tail was inferred merely from access to $U$. [F4, step 3.1] ∎
