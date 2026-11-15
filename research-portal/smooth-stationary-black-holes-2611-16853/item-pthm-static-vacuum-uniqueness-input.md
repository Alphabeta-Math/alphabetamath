---
title: Static vacuum Schwarzschild classification contract
status: published
research_item: pthm-static-vacuum-uniqueness-input
dependency_level: 5
sources:
  references:
    - title: G. L. Bunting and A. K. M. Masood-ul-Alam, Nonexistence of multiple black
        holes in asymptotically Euclidean static vacuum space-time, General
        Relativity and Gravitation 19 (1987), 147–154
      url: https://www.academia.edu/114578365/Nonexistence_of_multiple_black_holes_in_asymptotically_Euclidean_static_vacuum_space_time
      locator: p.148, static-data assumptions, equations (2)–(5) and Assumption 1;
        p.150, Theorem 2; p.153, Riemannian doubling and conclusion of the main
        proof
      statement: The regular complete asymptotically Euclidean three-dimensional
        static vacuum data with positive lapse in the interior, zero lapse on
        compact boundary and normalized lapse at infinity have Schwarzschild
        spatial geometry; in particular the black-hole boundary is connected.
        Theorem 2 phrases the spacetime conclusion for a maximally extended
        static spacetime; the Riemannian data conclusion is the one imported
        here, with its standard explicit restatement in Miao, p.2.
      hypotheses: Connected oriented three-dimensional spatial exterior, compact C3
        boundary; metric and lapse smooth in the interior and C2 on its closure;
        static vacuum equations; positive lapse inside and zero on boundary,
        nonzero boundary lapse gradient; complete spatial exterior with compact
        core and a single asymptotically Euclidean end. Assumption 1 requires
        metric perturbation O(r^-1), first derivatives O(r^-2), lapse 1-m/r+v
        with v=O(r^-2), first derivatives O(r^-3), second metric derivatives in
        L^q_{-lambda-2} and second v derivatives in L^q_{-lambda-3}, for some
        lambda>0 and 4<q<infinity; m>0. The local helpers establish the weighted
        conditions and positivity from the stated stronger pointwise bounds.
      reading_limits: Read all eight original-paper HTML page transcriptions from the
        author upload; visually inspected the source images for p.148 weighted
        exponents and C2 regularity, p.150 Theorem 2 and its maximal-extension
        wording, and p.153 doubling regularity and Riemannian conclusion. The
        original source bytes/images are retained run-locally. This is a
        statement/hypothesis/application reading, not an audit or reconstruction
        of the positive-mass theorem, conformal doubling proof, or cited final
        classification argument.
    - title: P. Miao, A Remark on Boundary Effects in Static Vacuum Initial Data sets,
        arXiv:gr-qc/0504081v1
      url: https://arxiv.org/pdf/gr-qc/0504081v1
      locator: pp.1–2, static equations (1) and paragraph beginning “A classic result
        of Bunting and Masood-ul-Alam”; p.3, boundary-regularity qualification
        for Miao’s different minimal-boundary theorem
      statement: For a one-ended asymptotically flat three-dimensional static vacuum
        manifold with nonempty compact boundary, if its normalized static
        potential vanishes on the boundary, the Bunting–Masood-ul-Alam theorem
        makes the spatial manifold isometric to (R3 minus the open ball of
        radius m/2, (1+m/(2|x|))^4 delta) with m>0; the boundary is a connected
        two-sphere.
      hypotheses: The Bunting–Masood-ul-Alam zero-lapse boundary case, with its source
        regularity and asymptotics verified from the original paper. Miao’s
        separate generalization assuming only minimal boundary is not imported;
        its p.3 C3 metric hypothesis is not substituted for the original
        theorem’s C2 boundary regularity.
      reading_limits: Read the downloaded full PDF’s pp.1–3 by text extraction,
        especially the explicit classical Riemannian restatement and the
        separate C3 assumption on p.3. No proof of Miao’s generalized
        minimal-boundary theorem or any claimed weaker regularity result was
        read or reconstructed.
external_input: true
---

## Prerequisites

- [def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)
- [lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction)
- [lem-author-f247c641a714-static-end-weighted-integrability](item-lem-author-f247c641a714-static-end-weighted-integrability)
- [lem-author-f247c641a714-static-boundary-and-positive-mass](item-lem-author-f247c641a714-static-boundary-and-positive-mass)
- [lem-author-f247c641a714-schwarzschild-static-data-lift](item-lem-author-f247c641a714-schwarzschild-static-data-lift)
- [physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)
- [` G. L. Bunting and A. K. M. Masood-ul-Alam, Nonexistence of multiple black holes in asymptotically Euclidean static vacuum space-time, General Relativity and Gravitation 19 (1987), 147–154 · p.148, static-data assumptions, equations (2)–(5) and Assumption 1; p.150, Theorem 2; p.153, Riemannian doubling and conclusion of the main proof `](https://www.academia.edu/114578365/Nonexistence_of_multiple_black_holes_in_asymptotically_Euclidean_static_vacuum_space_time)
- [` P. Miao, A Remark on Boundary Effects in Static Vacuum Initial Data sets, arXiv:gr-qc/0504081v1 · pp.1–2, static equations (1) and paragraph beginning “A classic result of Bunting and Masood-ul-Alam”; p.3, boundary-regularity qualification for Miao’s different minimal-boundary theorem `](https://arxiv.org/pdf/gr-qc/0504081v1)


## Statement

In the zero-cosmological-constant vacuum Einstein model, let the spacetime exterior be the globally static product $g=-V^2dt^2+h$ on $\mathbb R_t\times X$. Assume the regular static exterior data: $\overline X$ is a connected oriented three-dimensional exterior complete up to nonempty compact smooth boundary $B$, $V>0$ inside and $V=0$ on $B$, the interior data are smooth and extend at least $C^2$ to $B$, and $dV\ne0$ there. The single asymptotically Euclidean end is the complement of a compact core, with $h-\delta=O_2(r^{-1})$ and $V=1-m/r+O_2(r^{-2})$, and there is no other end or deleted interior boundary. No connectedness of $B$ is assumed.

Then the exterior is globally isometric to the Schwarzschild exterior of mass $m>0$, and $B$ is a connected two-sphere. Staticity and this global static product must already have been established; this theorem does not turn an arbitrary non-rotating stationary spacetime into a static one. The classification is of the given exterior; it does not assert a maximal analytic extension beyond its horizon.

## Statement references

[def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)

[lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction)

[lem-author-f247c641a714-static-end-weighted-integrability](item-lem-author-f247c641a714-static-end-weighted-integrability)

[lem-author-f247c641a714-static-boundary-and-positive-mass](item-lem-author-f247c641a714-static-boundary-and-positive-mass)

[lem-author-f247c641a714-schwarzschild-static-data-lift](item-lem-author-f247c641a714-schwarzschild-static-data-lift)

[physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)

## Facts & Assumptions

[A1] The classical field law is adopted on the smooth spacetime interior with zero stress-energy and zero cosmological constant. Tracing $\operatorname{Ric}(g)-\tfrac12\operatorname{Scal}(g)g=0$ in dimension four gives $\operatorname{Ric}(g)=0$. [physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)

[F1] The regular static data, their reduced spatial equations, original weighted-end conditions, boundary geometry, positive mass coefficient, and lifting from Schwarzschild spatial data are the following locally authored application suppliers: [def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data) [lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction) [lem-author-f247c641a714-static-end-weighted-integrability](item-lem-author-f247c641a714-static-end-weighted-integrability) [lem-author-f247c641a714-static-boundary-and-positive-mass](item-lem-author-f247c641a714-static-boundary-and-positive-mass) [lem-author-f247c641a714-schwarzschild-static-data-lift](item-lem-author-f247c641a714-schwarzschild-static-data-lift)

[F2] The complete static-data Schwarzschild classification is an established external input: Bunting–Masood-ul-Alam, p.148 hypotheses and Assumption 1, p.150 Theorem 2, and p.153 Riemannian conclusion, with Miao pp.1–2 giving its explicit spatial-data formulation.

## External input

The classification theorem, including connectedness and the Schwarzschild spatial geometry, is imported from the two independent-source records. The five local prerequisites supply the application chain: the adopted vacuum law gives the spatial static equations, the differentiated pointwise decay implies Assumption 1 with $q=6$ and $\lambda=1/2$, the boundary and energy identity give regular boundary data and $m>0$, and the global product lifts the spatial Schwarzschild classification to the stated spacetime exterior. The spatial classification is used on complete data, as explicitly restated by Miao; the “maximally extended” spacetime wording of the original Theorem 2 is not used to infer that an arbitrary ambient spacetime has such an extension. No local proof of the imported classification or of the positive-mass theorem is claimed.

## Source notes

The original theorem’s weighted second derivatives were resolved by reading its source image, not by guessing from corrupted OCR. Miao’s later minimal-boundary theorem with a C3 metric is not substituted for the original C2 zero-lapse-boundary result.
