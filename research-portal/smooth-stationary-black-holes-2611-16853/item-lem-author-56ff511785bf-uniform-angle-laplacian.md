---
title: Uniform scalar angle inequalities from local background tensors
status: draft
research_item: lem-author-56ff511785bf-uniform-angle-laplacian
dependency_level: 2
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum, arXiv:2610.09729v1
      url: https://arxiv.org/pdf/2610.09729v1
      locator: Appendix B, Lemma B.1, pp.35–36 (hypotheses); proof p.38, (B.8), the
        following unnumbered scalar inequality, and the transition to (B.9).
      statement: "Method attribution: normal-angle differentiation and Codazzi give
        the scalar Laplacian estimate before the restriction v>2 is imposed for
        the subsequent arcosh argument."
      hypotheses: The cited lemma concerns C2-convergent smooth Lorentz metrics near a
        fixed compact set, a fixed smooth temporal function with uniformly
        timelike gradient, and maximal hypersurfaces with compact
        nonnegative-height portions. Those global hypotheses are not imported
        into this locally proved result.
      reading_limits: Consulted the retrieved PDF text of the lemma hypotheses on
        pp.35–36 and the proof passage on p.38 from (B.8) through (B.9).
        Screenshot retrieval failed; no image reading is claimed. This item uses
        neither log v nor arcosh v. Its pointwise proof uses the two local
        geometric suppliers; its compact-family proof uses the stated common
        compact sets and topology. No weighted normal estimate is imported.
---

## Prerequisites

- [lem-author-56ff511785bf-boost-frame-bounds](item-lem-author-56ff511785bf-boost-frame-bounds)
- [lem-author-56ff511785bf-local-angle-gauss-codazzi](item-lem-author-56ff511785bf-local-angle-gauss-codazzi)
- [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)
- [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [` Alexandru F. Radu, Rigidity of stationary black holes with small ADM angular momentum, arXiv:2610.09729v1 · Appendix B, Lemma B.1, pp.35–36 (hypotheses); proof p.38, (B.8), the following unnumbered scalar inequality, and the transition to (B.9). `](https://arxiv.org/pdf/2610.09729v1)


## Statement

Use the local normal-angle setting, and define the positive comparison metric $e=g+2U^\flat\otimes U^\flat$. Suppose $|DU|_e+|D^2U|_e+|\operatorname{Ric}|_e\le K$ on the ambient region under consideration. Then for every $\varepsilon>0$ there are constants $K_1,C_\varepsilon$ depending only on $K$, $\varepsilon$ and dimension such that $\nabla v=kZ+Q$, $|Z|^2=v^2-1$, $|Q|\le K_1v^2$, and $\Delta v\ge(1-\varepsilon)|k|^2v-C_\varepsilon v^3$ at every point of every smooth spacelike maximal hypersurface in that region. These estimates require neither $v>2$ nor compactness of any candidate portion. The compact-family assertion has the following precise scope. Let $P$ be a nonempty compact metric parameter space and let $(g_p,U_p)$ be smooth Lorentzian metrics and future unit timelike observer fields on one common open ambient domain. Assume the family is continuous in the $C^2$ compact-open topology: in every fixed chart, its coordinate components and all spatial derivatives of order at most two vary continuously with $p$, uniformly on each compact subset of the chart. Fix a common compact ambient set $L$ covered by finitely many nonempty compact coordinate sets $L_j$ contained in those open chart domains. Then there is a single finite background bound $K_L$ on $L$ for all $p\in P$, and the estimates hold there with constants independent of $p$ and of the candidate hypersurface. In particular this applies to jointly smooth data on a neighborhood of a compact parameter set and the common compact ambient set. No uniformity up to the boundary of an open chart is asserted without such compact containment or an explicitly supplied common background bound.

## Facts & Assumptions

[F1] Observer-frame component bounds and tensor norms are [lem-author-56ff511785bf-boost-frame-bounds](item-lem-author-56ff511785bf-boost-frame-bounds).

[F2] The exact angle, Gauss and contracted Codazzi identities are [lem-author-56ff511785bf-local-angle-gauss-codazzi](item-lem-author-56ff511785bf-local-angle-gauss-codazzi). In particular the contracted curvature term is Ricci, not an uncontracted curvature component estimated in a boosted frame.

[F3] A finite product of compact spaces is compact by [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces). A continuous real-valued function on a nonempty compact metric space is bounded and attains its extrema by [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric). These results will be applied to the parameter space and the fixed compact coordinate sets in the Statement, not to open charts.

[F4] The Lorentzian Christoffel formula, curvature operator and Ricci trace are supplied by [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection), Definition (d)–(e). These are mathematical constructions for the given smooth nondegenerate metrics; no physical postulate or field equation is used.

## Proof

**Given:** The stated background bound and arbitrary smooth maximal hypersurface. **Goal:** Obtain the uniform scalar inequalities at every $v\ge1$.

1.1 In [F2], set $Q_a=-g(n,D_{e_a}U)$. By [F1], $|n|_e\le\sqrt2v$ and $|e_a|_e\le\sqrt2v$, while the metric pairing has operator norm one in an $e$-orthonormal observer frame. Thus $|Q|\le K_1v^2$. The other first-derivative term is $kZ$, and [F1] gives $|Z|^2=v^2-1$. [F1, F2, given, algebra]

2.1 The contracted Codazzi term satisfies $|\operatorname{Ric}(n,e_b)|\le CKv^2$; multiplying by the three components $Z_b$, whose total norm is at most $v$, bounds its contribution by $CKv^3$. The $DU$ term in the Laplacian formula is bounded by $CK|k|v^2$. The $D^2U$ term has one $n$ and two tangent vector slots, so is bounded by $CKv^3$. Consequently $\Delta v\ge |k|^2v-CK|k|v^2-CKv^3$. [F1, F2, step 1.1, given, algebra]

3.1 Apply the elementary inequality $ab\le\varepsilon a^2+b^2/(4\varepsilon)$ to $a=|k|\sqrt v$ and $b=CKv^{3/2}$, absorbing constants. This yields the displayed $(1-\varepsilon)|k|^2v-C_\varepsilon v^3$ bound for the given background bound. No bound on the candidate $k$ was assumed or used. [F1, F2, step 2.1, algebra]

4.1 For the family assertion, work in any one of the fixed charts on its compact coordinate set $L_j$. The $C^2$ compact-open continuity gives jointly continuous coordinate components of $g_p,U_p$ and their spatial derivatives through order two on $P\times L_j$: the change in $p$ is controlled uniformly on $L_j$, and for fixed $p$ these components are continuous in the spatial point. Matrix inversion is continuous wherever the determinant is nonzero, by the adjugate formula. Use the Christoffel formula in [F4], with parameter subscripts suppressed for the coordinate calculation. Differentiating $g^{-1}g=I$ gives $\partial_i g^{-1}=-g^{-1}(\partial_i g)g^{-1}$, so $\Gamma$ and $\partial\Gamma$ are finite sums of products of entries of $g^{-1}$ and spatial derivatives of $g$ through order two. Put $A^a{}_j=(D_jU)^a=\partial_jU^a+\Gamma^a{}_{jb}U^b$. The definition of $D^2U$ in [F2] gives $(D^2U)^a{}_{ij}=\partial_iA^a{}_j+\Gamma^a{}_{ib}A^b{}_j-\Gamma^b{}_{ij}A^a{}_b$. Expanding the curvature operator of [F4] on commuting coordinate fields gives $R^a{}_{bij}=\partial_i\Gamma^a{}_{jb}-\partial_j\Gamma^a{}_{ib}+\Gamma^a{}_{ic}\Gamma^c{}_{jb}-\Gamma^a{}_{jc}\Gamma^c{}_{ib}$, and $\operatorname{Ric}_{bj}=\sum_aR^a{}_{baj}$ is its finite contraction. Thus the components of $D^{(p)}U_p$, $(D^{(p)})^2U_p$ and $\operatorname{Ric}(g_p)$ use only finite sums and products of those jointly continuous metric entries and spatial derivatives of $U_p$ through order two, and are jointly continuous. Likewise $e_p=g_p+2U_p^\flat\otimes U_p^\flat$ and its inverse vary continuously; each $e_p$ is positive definite by [F1]. Their finite-dimensional tensor operator norms consequently vary continuously: near any fixed positive metric, its quadratic form is uniformly comparable to that fixed metric, with comparison factors tending to one as its entries converge, and the same holds for the inverse and tensor products. Thus $B_j(p,x)=|D^{(p)}U_p|_{e_p}+|(D^{(p)})^2U_p|_{e_p}+|\operatorname{Ric}(g_p)|_{e_p}$ is continuous on $P\times L_j$. By [F3] this product is compact; the metric $\max\{d_P(p,p'),|x-x'|\}$ induces its product topology, since its balls are products of balls. The extreme value theorem in [F3] gives a finite maximum of $B_j$. Take $K_L$ to be the largest of the finitely many such maxima. Steps 1.1–3.1 now apply on $L$ to every family member with this same $K_L$, proving the stated uniformity independently of the candidate. [F1, F2, F3, F4, step 1.1, step 2.1, step 3.1, given, algebra] ∎

## Source notes

The Radu citation records the scalar differentiation method, including the scalar estimate preceding the restricted arcosh argument. It is attribution, not an imported premise: the pointwise estimates and the compact-family application above are proved locally from the declared suppliers.
