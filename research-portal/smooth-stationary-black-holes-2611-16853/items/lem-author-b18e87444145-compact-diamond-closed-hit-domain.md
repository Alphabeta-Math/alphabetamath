---
id: lem-author-b18e87444145-compact-diamond-closed-hit-domain
title: Compact causal diamonds close the selected-generator endpoint domain
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-b18e87444145-temporal-normalized-null-flow
  - math:def-axiom-of-choice
  - math:thm-extreme-value-metric
  - math:thm-topological-manifolds-are-metrizable-and-paracompact
  - math:thm-metric-compactness-equivalences
  - math:thm-metric-sequential-closure
  - math:def-embedded-submanifold-and-slice-chart
dependency_roles:
  lem-author-b18e87444145-temporal-normalized-null-flow: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-extreme-value-metric: mathematical-premise
  math:thm-topological-manifolds-are-metrizable-and-paracompact: mathematical-premise
  math:thm-metric-compactness-equivalences: mathematical-premise
  math:thm-metric-sequential-closure: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3 — dimension-independent causal conventions
      url: https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609
      locator: Sections 1.2–1.3, PDF pp. 6–7; sections 1.5 and 1.7, pp. 9–11; sections
        1.10–1.11, pp. 15–16; section 2.3, p. 28; Definition 4.74, p. 131;
        Definition 4.117 and following traditional-definition paragraph, pp.
        146–147.
      statement: In arbitrary spacetime dimension, use signature (-,+,...,+), nonzero
        future causal vectors, causal curves with locally absolutely continuous
        coordinates and future causal velocity almost everywhere, reflexive
        causal reachability, and set futures/pasts given by unions of point
        futures/pasts. Strong causality means arbitrarily small causally convex
        neighborhoods. The traditional global-hyperbolicity convention is strong
        causality plus compact point diamonds.
      hypotheses: Smooth Hausdorff second-countable manifolds without boundary, with
        time-oriented Lorentzian metric. The review assumes a C2 metric. Its
        spacetime convention is connected and noncompact; the local argument
        applies the imported results to each connected component and proves
        noncompactness using the supplied temporal function.
      reading_limits: Read the listed passages in browser-extracted PDF text,
        including Definition 1.6 and the AC-curve convention. No full-paper
        reading, source-proof reconstruction or independent review is claimed.
        PDF screenshots were unavailable. Temporal and geodesic conventions come
        from the existing normalized-flow supplier, not from this citation.
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3 — closed compact-set cones and compact causal hulls
      url: https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609
      locator: Theorem 4.12 (i)–(iv), PDF pp. 109–110; Definition 4.117, its final
        compact-set assertion and proof, p. 146; traditional-definition
        paragraph, pp. 146–147.
      statement: Theorem 4.12 equates closedness of the causal relation, closedness of
        all point futures/pasts, closedness of futures/pasts of every compact
        set, and closedness of all point diamonds. Definition 4.117 concludes
        that, in a globally hyperbolic spacetime, J+(K) intersect J-(K) is
        compact for every compact K.
      hypotheses: A connected noncompact time-oriented smooth Lorentzian manifold in
        any finite spacetime dimension, with C2 metric. For the compact-hull
        assertion assume global hyperbolicity. Strong causality and compact
        point diamonds are the traditional sufficient formulation stated
        immediately after Definition 4.117; compact point diamonds are closed in
        the Hausdorff manifold, so Theorem 4.12 applies.
      reading_limits: Read Theorem 4.12 and its printed proof, and Definition 4.117
        with its printed proof and following traditional-definition paragraph in
        browser PDF text. Import only the stated closed-cone and
        same-compact-set hull conclusions; do not claim reconstruction of their
        source prerequisites. The two-distinct-compact-set consequence and
        disconnected-manifold application are proved locally below. No
        four-dimensional restriction is present in these statements.
dependency_level: 1
---

## Statement

Work in ZFC. Let $(E,g)$ be a smooth time-oriented Lorentzian manifold without boundary, of arbitrary finite dimension, globally hyperbolic in the convention below. Let $v$ be smooth temporal with $dv$ positive on nonzero future causal vectors. Let $C\subset E$ be a compact smooth embedded surface (a two-dimensional submanifold) with its induced smooth structure and subspace topology, and suppose $\min_Cv>0$. Choose a smooth future null vector $L_c$ at each $c\in C$. Let $D\subset\{v=0\}$ be compact. Use the maximal past geodesic from $c$ with initial tangent $-L_c$, and let $A\subset C$ consist of initial points whose geodesic meets $D$. Then $A$ is closed in $C$. A meeting is unique, and every selected segment between $D$ and $C$ is contained in the compact set $J^+(D)\cap J^-(C)$. No affine completeness or a uniform affine hit-time bound is assumed.

## Facts & Assumptions

[F1] On a connected noncompact time-oriented Lorentzian manifold of arbitrary finite spacetime dimension with a smooth metric, global hyperbolicity gives closed $J^+(B)$ and $J^-(B)$ and compact $J^+(B)\cap J^-(B)$ for every compact $B$. These are the imported conclusions of Minguzzi Theorem 4.12 and Definition 4.117, as specified under External input.

[F2] The normalized null flow has smooth dependence and cannot terminate at a finite temporal time while over a compact set. [[lem-author-b18e87444145-temporal-normalized-null-flow]]

[F3] Use the dimension-independent Lorentzian, temporal and geodesic conventions of the normalized-flow supplier. A future causal curve has locally absolutely continuous coordinates and nonzero future causal velocity almost everywhere. Put $p\le q$ if $p=q$ or a future causal curve joins them, $J^+(B)=\{q:\exists p\in B,\ p\le q\}$ and $J^-(B)=\{p:\exists q\in B,\ p\le q\}$. Strong causality means arbitrarily small open neighborhoods that a causal curve cannot leave and re-enter; global hyperbolicity means strong causality and compact point diamonds $J^+(p)\cap J^-(q)$. These dimension-independent causal conventions are imported from Minguzzi. Work in ZFC. Full AC supplies the countable-choice and dependent-choice hypotheses of the cited results: restrict a choice function to a countable family for countable choice; for dependent choice, choose a successor at each point of a set with a serial relation and recursively iterate the chosen successor from the prescribed initial point. [[lem-author-b18e87444145-temporal-normalized-null-flow]] [[math:def-axiom-of-choice]]

[F4] Under AC and countable choice, every topological manifold is metrizable. The smooth manifold $E$ has the underlying Hausdorff, second-countable manifold topology used by this result. [[math:thm-topological-manifolds-are-metrizable-and-paracompact]]

[F5] Under countable choice and dependent choice, compactness and sequential compactness are equivalent for a metric space. [[math:thm-metric-compactness-equivalences]]

[F6] Under countable choice, a subset of a metric space is closed if and only if every sequence in it converging in the ambient metric space has its limit in that subset. [[math:thm-metric-sequential-closure]]

[F7] An embedded smooth surface $C\subset E$ is a two-dimensional submanifold in slice charts. It has the subspace topology inherited from $E$ and the smooth structure induced by the restricted slice charts. [[math:def-embedded-submanifold-and-slice-chart]]

[F8] A continuous real-valued function on a nonempty compact metric space attains a maximum. [[math:thm-extreme-value-metric]]

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the asserted conclusions.

1.1 Apply [F4] to $E$ and choose a compatible metric $d$. For any subset $B\subset E$, the restricted metric has balls $B\cap B_d(b,r)$ for $b\in B$ and $r>0$. These form a neighborhood base for the subspace topology: an ambient open neighborhood of $b$ contains such an ambient ball, and each ambient ball is open. By [F7], the given topology on $C$ is this subspace topology; $D$ also carries its subspace topology. Thus both topologies agree with those of the restricted metrics. In particular $D$ is a compact metric space and is sequentially compact by [F5]. The choice assumptions are supplied by [F3]. [F3, F4, F5, F7, given]

2.1 The imported results in [F1] apply componentwise. Indeed each connected component $H$ of a manifold is open: a connected coordinate ball about any point of $H$ lies in $H$. Components are also closed, since their complement is a union of the other open components. A connected curve cannot leave its component, so point diamonds and strong causality in $H$ are exactly the restrictions of those in $E$. No such $H$ is compact: otherwise [F8], with the restricted metric from step 1.1, gives a maximum of $v|_H$, where the derivatives in every coordinate direction vanish by the one-variable difference quotients at a maximum. This contradicts the nonzero differential of the temporal function. Thus each component meets the connectedness and noncompactness conventions of [F1]. A compact $B\subset E$ meets only finitely many components, since the components are an open cover. Each $B\cap H$ is compact: to any ambient open cover of it add $E\setminus H$ and use compactness of $B$. Therefore [F1] in these finitely many components gives closed $J^\pm(B)$ and compact $J^+(B)\cap J^-(B)$ in $E$. A set closed in the closed component is closed in $E$, and the finite unions here remain closed or compact respectively; the latter follows by taking a finite subcover in each component. [F1, F3, F8, step 1.1]

3.1 Temporal monotonicity gives uniqueness of any hit at $v=0$. Orient a selected segment from its endpoint $p\in D$ to $c\in C$ towards the future. For each interior point $x$, the restrictions from $p$ to $x$ and from $x$ to $c$ are smooth with nonzero future null tangents, hence are causal curves by the curve definition. Thus $x\in J^+(p)\cap J^-(c)$ directly; at either endpoint use the reflexive alternative in causal reachability. The whole segment therefore lies in $K=J^+(D)\cap J^-(C)$. By step 2.1, $K$ is closed. The set $B=D\cup C$ is compact by combining finite subcovers of $D$ and $C$, and $K\subset J^+(B)\cap J^-(B)$, which is compact by step 2.1. Hence $K$ is compact: adjoin the open complement of $K$ to any ambient open cover of $K$, obtain a finite cover of this compact hull, and discard the complement. If $A$ is empty its closedness is immediate; otherwise let $c_j\in A$ converge to $c\in C$. Write $p_j\in D$ for the unique hit of the selected ray from $c_j$. Sequential compactness of $D$ permits passage to a subsequence with $p_j\to p\in D$. [F1, F3, step 1.1, step 2.1, given]

4.1 Normalize initial future tangents as $w_j=L_{c_j}/dv(L_{c_j})$. Smoothness gives $w_j\to w=L_c/dv(L_c)$. Run the normalized flow backwards from these data. The $j$th orbit exists over the temporal interval $[0,v(c_j)]$ and lies over $K$. By smooth ODE dependence, on every compact subinterval of the limiting maximal backward orbit before temporal time zero these flows converge to it. At each such time its base lies in closed $K$. If this limiting orbit terminated at a positive temporal time or precisely at zero, the compact-lift continuation in [F2] would extend it. Therefore it exists through zero. Smooth dependence, now on a neighborhood of the complete finite limiting segment, and $v(c_j)\to v(c)$ give convergence of its zero-time endpoint to $p$. [F1, F2, step 3.1]

5.1 The zero-time endpoint of the selected ray from $c$ consequently equals $p\in D$, so $c\in A$. Every sequence in $A$ converging in $C$ has limit in $A$. Apply [F6] to $C$ with the restricted compatible metric of step 1.1 to conclude that $A$ is closed in $C$. The proof bounds temporal lengths and normalized velocities on a compact causal diamond rather than asserting an affine bound. [F2, F3, F6, step 1.1, step 3.1, step 4.1] ∎

## External input

Import only the dimension-independent causal conventions and the closed-cone and same-compact-set hull statements recorded in the two Minguzzi references. The metric is smooth, hence satisfies the source C2 regularity requirement. Step 2.1 matches its connected, noncompact spacetime convention without adding these restrictions to E. Step 3.1 derives compactness for the two different compact sets D and C. The endpoint-domain closedness remains the locally authored normalized-flow argument; it is not imported from Minguzzi. No physical field equation or conclusion of the article under study is used as a premise.
