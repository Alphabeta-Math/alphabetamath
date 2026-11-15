---
id: lem-compact-target-achronal-generator-input
title: Compact-target null generators and the required endpoint conditions
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-causal-exterior-and-boundary-data
  - def-null-screen-expansion-and-focal-data
  - lem-author-2632702918ef-compact-target-causal-endpoint
  - lem-author-2632702918ef-compact-target-null-segment
  - lem-author-2632702918ef-target-segment-boundary-containment
  - lem-author-2632702918ef-target-endpoint-orthogonality
  - lem-author-2632702918ef-target-interior-focal-exclusion
  - physics:lem-gr-achronal-boundaries-lipschitz-graphs
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-causal-curve-calculus
  - math:def-topological-space
  - math:def-axiom-of-choice
dependency_roles:
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  lem-author-2632702918ef-compact-target-causal-endpoint: mathematical-premise
  lem-author-2632702918ef-compact-target-null-segment: mathematical-premise
  lem-author-2632702918ef-target-segment-boundary-containment: mathematical-premise
  lem-author-2632702918ef-target-endpoint-orthogonality: mathematical-premise
  lem-author-2632702918ef-target-interior-focal-exclusion: mathematical-premise
  physics:lem-gr-achronal-boundaries-lipschitz-graphs: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  math:def-topological-space: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: E. Minguzzi, Lorentzian causality theory
      url: https://link.springer.com/article/10.1007/s41114-019-0019-x
      locator: Definition 2.86 and Theorem 2.87(iii)
      statement: An achronal boundary is the boundary of a future set and is locally a
        Lipschitz topological hypersurface.
      hypotheses: Lorentzian causality setting of the cited definition and theorem;
        the corresponding past-set statement follows by time reversal.
      reading_limits: Read Definition 2.86 and Theorem 2.87(iii) and the local graph
        proof. The reference is not claimed to prove the compact-target
        endpoint, orthogonality or focal assertions.
dependency_level: 6
---

## Statement

Let $(E,g,N)$ be a smooth globally hyperbolic time-oriented Lorentzian four-manifold and let $C\subset E$ be a compact spacelike two-surface, meaning a smooth embedded two-manifold without boundary with positive-definite induced metric. If $p\in\partial_E I_E^-(C)$ and some temporal function $\tau$ satisfies $\tau(p)<\min_C\tau$, then $p$ is joined to a point of $C$ by a future null geodesic whose entire segment lies in that boundary. Its final tangent is orthogonal to $C$, and there is no focal point to $C$ strictly between its endpoints, with focality measured from $C$ toward $p$. Achronal boundaries are locally Lipschitz. Choosing one of the two null normal directions, proving a closed endpoint domain, and controlling endpoint-map regularity require additional arguments specific to the chosen cylinder and cut.

## Facts & Assumptions

[A1] Work in ZFC; the axiom of choice includes the countable and dependent choice assumptions of the causal suppliers. [[math:def-axiom-of-choice]]

[F1] The chronological and causal relations, boundary, global hyperbolicity and temporal function are relative to $E$ as in [[def-causal-exterior-and-boundary-data]].

[F2] The surface and focal notions are those of [[def-null-screen-expansion-and-focal-data]].

[F3] Compactness and boundary membership give a distinct causal endpoint $c\in C$, with $p\notin I_E^-(C)$. [[lem-author-2632702918ef-compact-target-causal-endpoint]]

[F4] There is a future null geodesic segment from $p$ to such a target point. [[lem-author-2632702918ef-compact-target-null-segment]]

[F5] The whole segment is contained in the chronological boundary. [[lem-author-2632702918ef-target-segment-boundary-containment]]

[F6] Its target tangent is orthogonal to $C$ without assuming $C$ acausal. [[lem-author-2632702918ef-target-endpoint-orthogonality]]

[F7] No focal point to $C$ occurs strictly inside the segment. [[lem-author-2632702918ef-target-interior-focal-exclusion]]

[F8] The boundary of an open future set is locally a Lipschitz graph, and the time-reversed assertion holds for an open past set. [[physics:lem-gr-achronal-boundaries-lipschitz-graphs]]

[F9] Each chronological past $I_E^-(c)$ is open in $E$, by clause (a) of [[physics:lem-gr-chronology-openness]].

[F10] Finite concatenation of future timelike curves and positive affine reparametrization preserve the future timelike curve class, by clauses (d) and (e) of [[physics:lem-gr-causal-curve-calculus]].

[F11] Arbitrary unions of open sets are open, by topology axiom (T2) in [[math:def-topological-space]].

## Proof

**Given:**The data and hypotheses in the Statement.

**Goal:** Establish the asserted conclusion.

1.1 Apply [F3]–[F4] using the globally hyperbolic spacetime $E$, compact smooth target $C$, and the strict temporal separation in the Statement. These supply a nonconstant future null geodesic to a point of $C$. Apply [F5] to get containment of its whole closed segment in $\partial_E I_E^-(C)$; [F6] gives endpoint orthogonality and [F7] excludes interior focal points measured from that endpoint. Each use retains precisely the same domain and causal relations. [given, F1, F2, F3, F4, F5, F6, F7]

1.2 Put $P:=I_E^-(C)=\bigcup_{c\in C}I_E^-(c)$. Each set in this union is open by [F9], so $P$ is open by [F11]. If $x\in I_E^-(P)$, some $y\in P$ and $c\in C$ satisfy $x\ll_E y\ll_E c$. Positively affinely reparametrize the two joining timelike curves to adjoining compact intervals and concatenate them using [F10]. This gives $x\ll_E c$, hence $I_E^-(P)\subseteq P$. [F1, F9, F10, F11, A1]

2.1 Conversely, if $x\in P$, choose a future timelike curve $\gamma:[a,b]\to E$ from $x$ to some $c\in C$ and an interior parameter $s\in(a,b)$. Restriction to $[a,s]$ and $[s,b]$ preserves local absolute continuity and the nonzero future timelike velocity condition almost everywhere, directly from the curve definition in [F1]; thus $x\ll_E\gamma(s)\ll_E c$. It follows that $\gamma(s)\in P$ and $x\in I_E^-(P)$. Together with step 1.2 this gives $I_E^-(P)=P$. Therefore $P$ is an open past set in [F8]'s sense; reversing the time orientation makes it an open future set, with the same topological boundary. Apply [F8] to obtain the local Lipschitz property of $\partial_E P$. The argument does not choose a null-normal branch or assert regularity of an endpoint map; those remain the separate obligations in the Statement. [step 1.1, step 1.2, F1, F8, A1] ∎

## External input

Minguzzi's theorem gives the local Lipschitz property of achronal boundaries; the compact-target endpoint, orthogonality and focal conclusions above use the declared local suppliers.
