---
id: lem-author-f247c641a714-static-end-weighted-integrability
title: The pointwise static end bounds imply the original weighted hypotheses
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-author-f247c641a714-regular-static-exterior-data
  - math:thm-polar-coordinates-formula-for-lebesgue-measure
  - math:def-countable-choice
dependency_roles:
  def-author-f247c641a714-regular-static-exterior-data: mathematical-premise
  math:thm-polar-coordinates-formula-for-lebesgue-measure: mathematical-premise
  math:def-countable-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: G. L. Bunting and A. K. M. Masood-ul-Alam, Nonexistence of multiple black
        holes in asymptotically Euclidean static vacuum space-time, General
        Relativity and Gravitation 19 (1987), 147–154
      url: https://www.academia.edu/114578365/Nonexistence_of_multiple_black_holes_in_asymptotically_Euclidean_static_vacuum_space_time
      locator: p.148, Assumption 1, equations (4)–(5), the following derivative
        conditions and definition of the weighted space
      statement: The asymptotic part of Assumption 1 requires a compact-core Euclidean
        end with metric perturbation H=O(r^-1), first derivatives O(r^-2), lapse
        V=1-m/r+v with v=O(r^-2) and first derivatives O(r^-3), and second
        derivatives of H in L^q_{-lambda-2} and of v in L^q_{-lambda-3}, for
        some lambda>0 and 4<q<infinity. Its convention is finiteness of the
        integral of |f|^q r^(-alpha q-3) against Cartesian volume.
      hypotheses: This is the specified end-data contract, not a classification
        theorem. It is read in the end chart outside a compact cutoff. The
        source separately states positivity of m; that assertion, the static
        vacuum equations and boundary assumptions are not derived by this
        integrability lemma.
      reading_limits: In this adjudication, read the online transcription around
        Assumption 1 and visually inspected the retained original-paper image
        bunting-page-2.jpg (printed p.148), including both weighted subscripts,
        q range, first-derivative conditions and weight convention. The
        transcription corrupts the subscripts; the image supplies them. No
        classification proof or positive-mass proof was read or reconstructed
        for this assignment.
dependency_level: 2
---

## Statement

Assume the Axiom of Countable Choice. Let $H_{ij}=h_{ij}-\delta_{ij}$ and $v=V-1+m/r$ in the end of the regular static exterior data, and fix an end cutoff $R>R_0$. For $4<q<\infty$ and $0<\lambda<1$, define $L^q_\alpha$ on $r>R$ by finiteness of $\int_{r>R}|f|^q r^{-\alpha q-3}\,dx$. Then
$$\partial_k\partial_\ell H_{ij}\in L^q_{-\lambda-2},\qquad \partial_k\partial_\ell v\in L^q_{-\lambda-3}.$$
Thus the differentiated pointwise falloff supplies the weighted second-derivative hypotheses in Bunting–Masood-ul-Alam's Assumption 1 (p.148), for example with $q=6$ and $\lambda=1/2$. The compact-core end topology and the zeroth- and first-derivative falloff in that asymptotic contract are also supplied by the regular static exterior data. This comparison concerns the end conditions; positivity of $m$, the static vacuum equations and boundary conditions require their separate arguments.

## Statement references

[[def-author-f247c641a714-regular-static-exterior-data]]

[[math:thm-polar-coordinates-formula-for-lebesgue-measure]]

[[math:def-countable-choice]]

## Facts & Assumptions

[F1] The regular static exterior data have a single Cartesian end outside a compact core, with $H=O_2(r^{-1})$ and $v=O_2(r^{-2})$; the $O_2$ convention gives uniform Cartesian derivative bounds through order two. [[def-author-f247c641a714-regular-static-exterior-data]]

[F2] In dimension three the polar integration formula applies to every nonnegative Borel function on $\mathbb R^3$, with volume element $r^2\,dr\,d\sigma$ and finite Borel measure $\sigma$ on $S^2$. The cited theorem assumes Countable Choice. [[math:thm-polar-coordinates-formula-for-lebesgue-measure]]

[A1] Adopt the Axiom of Countable Choice to meet precisely the choice hypothesis of [F2]. [[math:def-countable-choice]]

[F3] The imported asymptotic contract is Bunting–Masood-ul-Alam, p.148, Assumption 1 and its weighted-space definition, as recorded in the External input section and the source reference.

## External input

Only the end-data formulation is imported here: outside a compact core the end is Euclidean in topology, $H=O(r^{-1})$, $\partial H=O(r^{-2})$, $V=1-m/r+v$, $v=O(r^{-2})$, $\partial v=O(r^{-3})$, and for some $\lambda>0$ and $4<q<\infty$ one requires $\partial^2H\in L^q_{-\lambda-2}$ and $\partial^2v\in L^q_{-\lambda-3}$. The weighted convention is $\int |f|^q r^{-\alpha q-3}\,dx<\infty$. These are the conditions read on p.148, Assumption 1, with $H$ here denoting the source's metric perturbation. The local proof below verifies these end conditions from [F1]; no static classification theorem or mass-positivity assertion is imported as a premise of this mathematical lemma.

## Proof

**Given:** The Cartesian end and $O_2$ bounds of [F1], the polar integration theorem [F2] under [A1], and the external formulation [F3].

**Goal:** Verify the two weighted integrability assertions and the stated comparison of end conditions.

1.1 The differentiated bounds give $|\partial^2H|\leq Cr^{-3}$ and $|\partial^2v|\leq Cr^{-4}$ uniformly in angle for $r>R_1$, where $R_1>R$. Extend each nonnegative weighted component integrand by zero off $r>R_1$; smoothness on the end makes this extension Borel measurable. Apply [F2] with $n=3$, using [A1] at this invocation. The first weighted $q$th power is at most $C^q\sigma(S^2)\int_{R_1}^\infty r^{-3q}r^{(\lambda+2)q-3}r^2\,dr=C^q\sigma(S^2)\int_{R_1}^\infty r^{q(\lambda-1)-1}\,dr$. This last integral is $R_1^{q(\lambda-1)}/(q(1-\lambda))<\infty$, since $\lambda<1$. The finite sum of components does not affect convergence. [given, F1, F2, A1]

2.1 For the lapse remainder the same polar formula bounds its weighted $q$th power by $C^q\sigma(S^2)\int_{R_1}^\infty r^{-4q}r^{(\lambda+3)q-3}r^2\,dr=C^q\sigma(S^2)\int_{R_1}^\infty r^{q(\lambda-1)-1}\,dr<\infty$. On the compact annulus $R\leq r\leq R_1$ all component second derivatives and weights are bounded, and its Cartesian volume is finite, also by [F2]. Adding the annular integrals proves both claims on $r>R$. [given, F1, F2, A1, step 1.1]

3.1 The order-zero and order-one parts of [F1] give exactly $H=O(r^{-1})$, $\partial H=O(r^{-2})$, $v=O(r^{-2})$ and $\partial v=O(r^{-3})$, while its compact-core chart gives the required end topology. The weight in [F3] agrees with the Statement, so steps 1.1 and 2.1 verify its second-derivative requirements. Choosing $q=6$ and $\lambda=1/2$ meets $4<q<\infty$ and $\lambda>0$ simultaneously. Enlarging the compact cutoff only discards a compact annulus, whose finite integral was checked in step 2.1. This establishes the asserted end comparison without claiming that a borderline $O(r^{-2})$ second derivative would suffice. [given, F1, F3, step 1.1, step 2.1] ∎
