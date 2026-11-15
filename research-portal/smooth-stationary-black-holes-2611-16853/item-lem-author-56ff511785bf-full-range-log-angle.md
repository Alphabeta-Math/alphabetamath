---
title: Logarithmic angle inequality through the full range v at least one
status: draft
research_item: lem-author-56ff511785bf-full-range-log-angle
dependency_level: 3
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum, arXiv:2610.09729v1
      url: https://arxiv.org/pdf/2610.09729v1
      locator: Appendix B, Lemma B.1 hypotheses, printed pp.35–36; proof (B.8)–(B.11),
        printed pp.38–39 (PDF pages 35–36 and 38–39).
      statement: "Methodological attribution: normal-angle differentiation and Codazzi
        yield a scalar Laplacian bound; trace-free three-dimensional algebra
        retains a positive gradient term in the subsequent arcosh calculation."
      hypotheses: The cited lemma uses C2-convergent Lorentz metrics near a compact
        set, a fixed uniformly temporal function and compact nonnegative-height
        hypersurface portions. Its arcosh calculation assumes v>2.
      reading_limits: Consulted the online PDF text of these hypotheses and
        (B.8)–(B.11) in this repair; no rendered images were read. This citation
        supplies background attribution only. The all-range logarithmic
        inequality is proved locally from the declared geometric and scalar
        suppliers and operator definitions. No global weighted estimate or
        compact-positive-portion hypothesis is imported.
---

## Prerequisites

- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [lem-author-56ff511785bf-trace-free-angle-coercivity](item-lem-author-56ff511785bf-trace-free-angle-coercivity)
- [lem-author-56ff511785bf-uniform-angle-laplacian](item-lem-author-56ff511785bf-uniform-angle-laplacian)
- [lem-author-56ff511785bf-boost-frame-bounds](item-lem-author-56ff511785bf-boost-frame-bounds)
- [math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function)
- [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)
- [` Alexandru F. Radu, Rigidity of stationary black holes with small ADM angular momentum, arXiv:2610.09729v1 · Appendix B, Lemma B.1 hypotheses, printed pp.35–36; proof (B.8)–(B.11), printed pp.38–39 (PDF pages 35–36 and 38–39). `](https://arxiv.org/pdf/2610.09729v1)


## Statement

Let $U$ be a smooth future unit timelike field on a Lorentzian four-region with a uniform bound $|DU|_e+|D^2U|_e+|\operatorname{Ric}|_e\le K$, where $e=g+2U^\flat\otimes U^\flat$. For every smooth spacelike maximal hypersurface in the region, let $v=-g(n,U)$. There is a constant $C$ depending only on the background bound and dimension such that $\Delta_\Sigma\log v\ge\tfrac14|\nabla_\Sigma\log v|^2-Cv^2$ at every point, including the entire range $1\le v\le2$. For the compact-family assertion, let $P$ be a nonempty compact metric parameter space and let $(g_p,U_p)$ be smooth Lorentzian metrics and future unit timelike observer fields on one common open ambient domain. Assume continuity in the $C^2$ compact-open topology: in each fixed chart the components and all spatial derivatives through order two vary continuously with $p$, uniformly on every compact subset of the chart. Fix a common compact ambient set $L$ covered by finitely many nonempty compact coordinate sets $L_j$ contained in those open chart domains. Then on $L$ the constant $C$ can be chosen independently of $p$ and of the candidate hypersurface. In particular this applies to jointly smooth data on a neighborhood of a compact parameter set and the common compact ambient set. If a common background bound $K$ is explicitly supplied on the whole region for all family members, the constant is uniform on that region without requiring compactness of the parameter space. No hypersurface boundary, compact positive-height portion, bound on the candidate second fundamental form or temporal cutoff is needed for this pointwise conclusion.

## Facts & Assumptions

[F1] Maximality makes the symmetric three-dimensional form $k$ trace free. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F2] The trace-free spectral/gradient inequality is [lem-author-56ff511785bf-trace-free-angle-coercivity](item-lem-author-56ff511785bf-trace-free-angle-coercivity).

[F3] The uniform all-range scalar estimates, including $\nabla_\Sigma v=kZ+Q$, $|Z|^2=v^2-1$, $|Q|\le K_1v^2$ and the compact-family scope, are [lem-author-56ff511785bf-uniform-angle-laplacian](item-lem-author-56ff511785bf-uniform-angle-laplacian).

[F4] For a future unit observer and future unit hypersurface normal, $e$ is positive definite and $v=-g(n,U)\ge1$; use the induced $e$ tensor operator norms. [lem-author-56ff511785bf-boost-frame-bounds](item-lem-author-56ff511785bf-boost-frame-bounds)

[F5] With $h=g|_{T\Sigma}$, the intrinsic gradient is defined by $h(\nabla_\Sigma f,X)=df(X)$ for tangent $X$. [math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function)

[F6] The intrinsic Laplacian uses the positive-divergence convention $\Delta_\Sigma f=\operatorname{tr}_h\operatorname{Hess}_h f=\operatorname{div}_h\nabla_\Sigma f$, where $\operatorname{Hess}_h f(X,Y)=h(\nabla^h_X\nabla_\Sigma f,Y)$. [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)

## Proof

**Given:** The smooth observer, background bound and arbitrary maximal hypersurface. **Goal:** Prove the displayed inequality for all $v\ge1$.

1.1 By [F1], the induced metric $h$ is Riemannian and $k$ is symmetric and trace free; identify $k$ with its $h$-raised endomorphism. By [F4], $e$ is positive definite and $v\ge1$. Hence $\log v$ is smooth. For tangent $X$, [F5] gives $h(\nabla_\Sigma\log v,X)=d(\log v)(X)=v^{-1}dv(X)=h(v^{-1}\nabla_\Sigma v,X)$, so $v\nabla_\Sigma\log v=\nabla_\Sigma v$. [F1, F4, F5, given, algebra]

2.1 Fix $\varepsilon=1/11$ and put $G=|\nabla_\Sigma\log v|_h^2$. By [F3] and $v\ge1$, $\Delta_\Sigma v/v\ge\tfrac{10}{11}|k|_h^2-C_1v^2$. Step 1.1 and the vector identity and bounds in [F3] satisfy the hypotheses of [F2] with $A=\nabla_\Sigma\log v$, so $G\le\tfrac{8}{11}|k|_h^2+C_2v^2$. The second inequality rearranges to $\tfrac{10}{11}|k|_h^2\ge\tfrac54G-\tfrac54C_2v^2$, with constants depending only on the background bound and dimension. [F2, F3, step 1.1, choose, algebra]

2.2 Using step 1.1 and the connection product rule in the Hessian formula of [F6], for tangent $X,Y$ one has $\operatorname{Hess}_h(\log v)(X,Y)=h(\nabla^h_X(v^{-1}\nabla_\Sigma v),Y)=v^{-1}\operatorname{Hess}_h v(X,Y)-v^{-2}dv(X)dv(Y)$. By [F5], tracing $dv\otimes dv$ gives $|\nabla_\Sigma v|_h^2$. Taking the trace as prescribed in [F6] therefore yields $\Delta_\Sigma\log v=\Delta_\Sigma v/v-G$. [F5, F6, step 1.1, algebra]

3.1 Insert step 2.1 into step 2.2 to obtain $\Delta_\Sigma\log v\ge\tfrac14G-(C_1+\tfrac54C_2)v^2$. No division by $\sqrt{v^2-1}$ occurred, so step 1.1 makes this calculation valid also at $v=1$ and throughout $1\le v\le2$. Under the stated compact-family hypotheses, [F3] gives a single finite background bound $K_L$ on $L$ for all $p\in P$. The same calculation therefore gives one $C$ on $L$, independently of $p$ and the candidate hypersurface. With an explicitly supplied common background bound $K$ on the whole region, the calculation instead gives one $C$ there. The algebra uses fixed $\varepsilon$ and numerical coefficients only. No hypersurface boundary, compact positive-height portion, candidate second-fundamental-form bound or temporal cutoff was used. [F3, step 1.1, step 2.1, step 2.2, algebra] ∎

## Source notes

The cited Appendix B uses normal-angle differentiation, Codazzi and trace-free three-dimensional algebra, then restricts to $v>2$ for its arcosh argument. This is methodological attribution only; the all-range logarithmic conclusion above is proved from the declared local suppliers and operator definitions.
