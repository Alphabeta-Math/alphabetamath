---
id: lem-author-b18e87444145-boundary-generators-do-not-cross
title: Distinct boundary generators cannot cross strictly before a spacelike cut
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - physics:thm-gr-local-geodesics-and-exponential-map
  - lem-author-b18e87444145-cut-generator-coverage-and-boundary
  - physics:lem-gr-causal-curve-calculus
  - physics:lem-gr-temporal-functions-and-time-functions
  - physics:lem-gr-chronology-openness
  - math:def-axiom-of-choice
  - math:thm-choice-implies-dependent-implies-countable-choice
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:thm-gr-local-geodesics-and-exponential-map: mathematical-premise
  lem-author-b18e87444145-cut-generator-coverage-and-boundary: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  physics:lem-gr-temporal-functions-and-time-functions: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 7
---

## Statement

Work in ZFC. Let $(E,g,N)$ be a time-oriented smooth Lorentzian four-manifold with its metric-selected connection, and let $v:E\to\mathbb R$ be smooth and temporal. Let $C\subset E$ and $D\subset\{v=0\}\cap\partial_E I_E^-(C)$. All causal relations, curves and boundaries are relative to $E$, with the causal-data interface's conventions applied to this ambient manifold. Let selected nonconstant future null geodesic segments from $D$ to $C$ lie on that boundary. Assume the causal rigidity input that every future causal curve in $E$ between distinct endpoints not timelike related is a null geodesic up to reparametrization. Then two distinct maximal unparametrized generators of these selected segments cannot intersect at a point interior to both selected segments, strictly between $D$ and $C$. At an intersection with proportional future tangents they are the same maximal geodesic by uniqueness. Distinct generators may meet on $D$; no injectivity of the endpoint map on initial points is asserted.

## Statement references

[[def-causal-exterior-and-boundary-data]]

[[math:def-axiom-of-choice]]

## Facts & Assumptions

[A1] The axiom of choice is assumed. It implies dependent choice and countable choice, meeting the stated choice hypotheses of the causal-curve calculus, temporal-function and chronology-openness suppliers and the inherited countable-choice convention of the geodesic supplier. These are the choice uses in the argument. [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]]

[F1] The causal rigidity clause in the Statement is an explicit hypothesis, to be supplied by an independently established theorem in an application. The causal-data conventions are applied with ambient manifold $E$; thus $p\ll_E c$ means a future timelike curve in $E$, and $\partial_E$ denotes the boundary in its manifold topology. [[def-causal-exterior-and-boundary-data]]

[F2] In $E$, a prescribed initial position and tangent determine a unique maximal geodesic. Positive affine rescaling gives the same unparametrized ray. These are clauses (a) and (c) of the geodesic supplier; completeness is not assumed. [[physics:thm-gr-local-geodesics-and-exponential-map]]

[F3] The selected boundary segments and their target endpoints are the segment data used in the cut-coverage interface. Only these data are used here; their boundary containment and endpoint membership are explicit hypotheses of the present Statement. [[lem-author-b18e87444145-cut-generator-coverage-and-boundary]]

[F4] Smooth future null segments are causal curves in the locally absolutely continuous class, and a finite concatenation of such curves with matching endpoints is future causal, by clauses (c) and (d). Apply the supplier with $M=E$. [[physics:lem-gr-causal-curve-calculus]]

[F5] A temporal function strictly increases on every nonconstant future causal curve, by clause (b), with $M=E$ and $u=v$. [[physics:lem-gr-temporal-functions-and-time-functions]]

[F6] Each $I_E^-(c)$ is open in $E$ by clause (a). Consequently $I_E^-(C)=\bigcup_{c\in C}I_E^-(c)$ is open, and none of its points belongs to its boundary, which is closure minus interior in the causal-data convention. [[physics:lem-gr-chronology-openness]] [[def-causal-exterior-and-boundary-data]]

## Proof

**Given:** The hypotheses in the Statement, including ZFC and the explicit causal rigidity hypothesis.

**Goal:** Establish the asserted noncrossing and proportional-tangent conclusions, retaining the endpoint qualifications.

1.1 Suppose two selected segments meet at a point $z$ interior to both, and their future tangents there are not proportional. Let $p\in D$ be the first segment's initial endpoint and $c\in C$ the second segment's final endpoint. Restrict to the subsegments from $p$ to $z$ and from $z$ to $c$, and positively affinely reparametrize their compact parameter intervals to $[0,1]$ and $[1,2]$. By [F4] their concatenation is a continuous future causal curve in $E$. By [F5], $0=v(p)<v(z)<v(c)$, so $p$ and $c$ are distinct. This curve has a genuine null corner: its one-sided tangent rays at $z$ differ, whereas a smooth nonconstant geodesic has a unique tangent ray there. Thus it is not a null geodesic up to reparametrization. The rigidity hypothesis [F1] therefore gives $p\ll_E c$. Since $c\in C$, this places $p$ in the open set $I_E^-(C)$, contradicting $p\in\partial_E I_E^-(C)$ by [F6]. Hence nonproportional interior crossings are impossible. [given, A1, F1, F3, F4, F5, F6]

2.1 If the future tangents at an intersection are proportional, translate the affine parameters to put that intersection at parameter zero and positively rescale one so the tangent vectors agree. Initial-value uniqueness and scaling [F2] then make both segments restrictions of the same maximal unparametrized null geodesic. Together with step 1.1, this proves that distinct maximal generators cannot cross in the interiors of their selected portions. The corner argument needs an incoming segment from a cut point strictly before $z$; at $z\in D$ this is absent, so it does not exclude coincident endpoints. Nor does it assert that a target surface never meets the same maximal generator twice, or that the endpoint map is injective on initial points. [A1, F2, F3, step 1.1] ∎
