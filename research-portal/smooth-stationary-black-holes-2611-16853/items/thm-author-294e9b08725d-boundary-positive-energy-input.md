---
id: thm-author-294e9b08725d-boundary-positive-energy-input
title: External boundary positive-energy theorem without maximality
kind: theorem
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-294e9b08725d-complete-boundary-initial-data-interface
  - lem-author-294e9b08725d-vacuum-section-dominant-energy
  - lem-author-294e9b08725d-bifurcation-boundary-zero-expansions
  - def-regular-stationary-vacuum-spacetime
dependency_roles:
  lem-author-294e9b08725d-complete-boundary-initial-data-interface: mathematical-premise
  lem-author-294e9b08725d-vacuum-section-dominant-energy: mathematical-premise
  lem-author-294e9b08725d-bifurcation-boundary-zero-expansions: mathematical-premise
  def-regular-stationary-vacuum-spacetime: mathematical-premise
provenance:
  statement: ai-altered
  proof: literature-derived
sources:
  references:
    - title: Dan A. Lee, Martin Lesourd and Ryan Unger, Density and positive mass
        theorems for initial data sets with boundary
      url: https://arxiv.org/pdf/2112.12017v2
      locator: Definition 2.1 p.5; expansion convention p.6; Theorem 4.3 p.25
      statement: Complete AF initial data in dimensions 3 through 7, with nonempty
        compact boundary, DEC, and each boundary component weakly outer trapped
        or weakly inner untrapped, have E>0; in dimension 3 assume additionally
        tr k=O(r^-gamma) for gamma>2.
      hypotheses: AF means locally C2,alpha x C1,alpha, h=delta+O2(r^-q),
        k=O1(r^-q-1), q>(n-2)/2, and integrable constraint densities. Boundary
        normal points into the manifold; theta±=±H+tr_boundary k. No maximality,
        axisymmetry, strict expansion, outermost condition or stability
        condition is assumed.
      reading_limits: Read the actual full theorem, Definition 2.1 and expansion
        conventions, introduction discussion distinguishing Theorems 1.3, 1.4
        and 4.3, and nearby proof setup. Not an independent reconstruction or
        review of the source proof.
external_input: true
dependency_level: 6
---

## Statement

Let $(Q^n,h,k)$ be complete asymptotically flat initial data, $3\le n\le7$, with nonempty compact boundary, locally $C^{2,\alpha}\times C^{1,\alpha}$, end bounds $h-\delta=O_2(r^{-q})$, $k=O_1(r^{-1-q})$, $q>(n-2)/2$, and integrable constraint densities. Suppose $\mu\ge|J|_h$ and each boundary component has either $\theta_+=H+\operatorname{tr}_{\partial Q}k\le0$ or $\theta_-=-H+\operatorname{tr}_{\partial Q}k\ge0$, using the normal into $Q$. For $n=3$, suppose additionally $\operatorname{tr}_h k=O(r^{-\gamma})$ for some $\gamma>2$. Then its ADM energy satisfies $E>0$. This external input does not require maximality or axisymmetry.

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[A1] For the intended vacuum exterior-section application only, assume the regular stationary-vacuum hypotheses. Clause 3 requires the two transverse null horizons through $S$ to have vanishing null expansion. [[def-regular-stationary-vacuum-spacetime]]

[F1] Under the application hypotheses [A1], the vacuum exterior section has the required complete initial-data, end-decay and constraint interfaces. [[lem-author-294e9b08725d-complete-boundary-initial-data-interface]] [[lem-author-294e9b08725d-vacuum-section-dominant-energy]]

[F2] Under [A1], the boundary-expansion lemma gives both expansion expressions zero with the specified into-manifold normal; its zero-horizon-expansion hypothesis is supplied by clause 3. [[lem-author-294e9b08725d-bifurcation-boundary-zero-expansions]] [[def-regular-stationary-vacuum-spacetime]]

## External input

This is an external input under exactly the hypotheses stated above. The cited result is imported; its proof is not reconstructed here.
