---
id: def-author-ad064c44a1cc-weighted-pk-condition
title: The weighted AIK perturbation hypothesis PK
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-author-ad064c44a1cc-perturbative-gr-sbs
  - def-author-ad064c44a1cc-weighted-mars-simon
  - def-author-ad064c44a1cc-perturbative-effective-constant
  - def-spacelike-maximal-hypersurface-data
  - physics:def-gr-local-frame-and-tetrad-fields
  - math:thm-gram-schmidt-orthonormalisation
dependency_roles:
  def-author-ad064c44a1cc-perturbative-gr-sbs: mathematical-premise
  def-author-ad064c44a1cc-weighted-mars-simon: mathematical-premise
  def-author-ad064c44a1cc-perturbative-effective-constant: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  physics:def-gr-local-frame-and-tetrad-fields: mathematical-premise
  math:thm-gram-schmidt-orthonormalisation: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: "S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth
        stationary black holes in vacuum: small perturbations of the Kerr
        spaces"
      url: https://arxiv.org/html/0904.0982v1
      locator: §1.1 PK (1.4); §2.1 (2.5); §2.3 (2.18)–(2.19)
      reading_limits: Consulted arXiv:0904.0982v1 HTML section 1.1, including GR/SBS
        and PK (1.4), section 2.1 through (2.5), and section 2.3 (2.13)-(2.19)
        with the following weighted-smoothness sentence. The HTML has a
        malformed tensor glyph in that sentence; the existing weighted-tensor
        supplier gives the explicit polynomial and local smoothness proof. No
        PDF image inspection or rigidity-proof review was performed. The
        selected-frame convention and smooth Gram-Schmidt application below are
        local clarifications, not attributed source constructions.
      statement: PK (1.4) bounds the modulus of every component of
        (1-sigma)S(T,e_a,e_b,e_c) on Sigma0 intersect closure(E), in an
        orthonormal frame with e_0 the future unit normal. Its tolerance is
        sufficiently small depending only on Abar of (2.5). Equations
        (2.18)-(2.19) define S and the following sentence records the smooth
        weighted extension.
      hypotheses: The source GR/SBS stationary vacuum four-dimensional data, the
        specified spacelike slice and normalized Ernst/curvature data near
        Sigma0 intersect closure(E), a selected adapted orthonormal frame, and
        the quantitative chart package (2.1)-(2.5). This imports the PK
        formulation and parameter dependence, not the Main Theorem or its proof.
dependency_level: 5
proof_strategy: direct
---

## Definition

For the AIK GR/SBS and quantitative chart packages, use the smooth weighted tensor $\mathcal W$ on a neighborhood of $\Sigma^0\cap\overline E$. Let $h=g|_{T\Sigma^0}$ and let $n$ be the future unit normal. Fix, as part of the PK data, one smooth adapted orthonormal frame $e=(e_0,e_1,e_2,e_3)$ along $\Sigma^0$: $e_0=n$, $e_i\in T\Sigma^0$ and $h(e_i,e_j)=\delta_{ij}$ for $i,j\in\{1,2,3\}$. Such a frame exists; one available choice is the ordered Gram–Schmidt orthonormalization of the three tangent coordinate fields supplied by the global slice parametrization $\Phi_0$. The frame is held fixed when testing the inequality. Local tests use restrictions of that selected frame, agreeing on overlaps; a different selection may require a tolerance adjustment.

The **PK smallness condition at tolerance $\overline\varepsilon>0$**, relative to this selected frame, requires at every point of the displayed slice portion and for every displayed index triple:
$$|\mathcal W(T,e_a,e_b,e_c)|\le\overline\varepsilon\quad\hbox{on }\Sigma^0\cap\overline E,\qquad a,b,c\in\{0,1,2,3\}.$$
The bars denote modulus of a complex scalar, not a Lorentzian tensor norm. In the source notation this is $|(1-\sigma)\mathcal S(T,e_a,e_b,e_c)|\le\overline\varepsilon$, using the smooth weighted extension at $\sigma=1$. For the rigidity theorem the tolerance must be sufficiently small depending only on the fixed $\overline A_{\rm PK}$ from the preceding package. This is not generic smallness of $g-g_{\rm Kerr}$, not a bound only on $S_0$, and not merely small ADM angular momentum. This definition asserts no rigidity from the inequality without the separately imported source theorem.

## Definition references

[[def-author-ad064c44a1cc-perturbative-gr-sbs]]

[[def-author-ad064c44a1cc-weighted-mars-simon]]

[[def-author-ad064c44a1cc-perturbative-effective-constant]]

[[def-spacelike-maximal-hypersurface-data]]

[[physics:def-gr-local-frame-and-tetrad-fields]]

[[math:thm-gram-schmidt-orthonormalisation]]

[AIK, PK (1.4), effective constant (2.5), and weighted tensor (2.18)–(2.19)](https://arxiv.org/html/0904.0982v1)

## Facts & Assumptions

[F1] [[def-author-ad064c44a1cc-perturbative-gr-sbs]] fixes the slice, its global parametrization $\Phi_0$ and $E$; [[def-spacelike-maximal-hypersurface-data]] fixes its smooth normal and positive induced metric. The inherited Axiom of Choice convention of the hypersurface supplier remains in force.

[F2] [[def-author-ad064c44a1cc-weighted-mars-simon]] supplies the smooth complex covariant four-tensor, including its polynomial value at $\sigma=1$. [[def-author-ad064c44a1cc-perturbative-effective-constant]] fixes the actual constant controlling the source tolerance.

[F3] [[physics:def-gr-local-frame-and-tetrad-fields]], whose domain is mathematics, supplies local-frame, orthonormal-tetrad and adapted-frame terminology; here the fields are along the slice, with smooth ambient components in slice charts. Its countable-choice convention is covered by the inherited Axiom of Choice convention. [[math:thm-gram-schmidt-orthonormalisation]] supplies the finite positive-definite Gram–Schmidt recursion and its nonzero denominators. Its application to smooth tangent fields is justified below.

[F4] AIK PK (1.4), (2.5), and (2.18)–(2.19) supply the weighted component formulation and the dependence of the tolerance on the fixed effective constant, with the exact citation contract recorded in the source reference and External input.

## Justification

**Given:** The slice, parametrization, metric and normal of [F1], tensor and effective constant of [F2], frame terminology and finite Gram–Schmidt result of [F3], and source PK formulation of [F4].

1.1 Let $v_i=(\Phi_0)_*(\partial/\partial x^i)$, $i=1,2,3$, be the globally defined smooth independent tangent fields from the supplied slice parametrization. Apply [F3] in each positive-definite tangent space with $u_i=v_i-\sum_{1\le j<i}h(v_i,e_j)e_j$ and $e_i=u_i/\sqrt{h(u_i,u_i)}$, starting with the empty sum. The cited recursion gives $u_i\ne0$ and an $h$-orthonormal basis. The coefficients are smooth by finite sums, products and division by a positive smooth square root, inductively for the three fields. The same formula on the whole parametrized slice agrees on every overlap. Appending $e_0=n$ gives the required smooth adapted frame along the slice. No ambient extension, global tetrad on $M$, or additional choice of a frame at each point is needed. [F1, F3, construct]

2.1 Evaluation of the smooth tensor of [F2] on $T,e_a,e_b,e_c$ gives a smooth complex scalar along the slice, with ordinary nonnegative modulus. The polynomial value of $\mathcal W$ keeps it defined at $\sigma=1$. To compare any other selected adapted frame $\widetilde e$ with $e$, orthonormality and the common $e_0=n$ give $\widetilde e_0=e_0$ and $\widetilde e_i=\sum_{j=1}^3R_i{}^j e_j$ for a pointwise orthogonal matrix $R$. Every entry has modulus at most one. Expansion in the three varying tensor slots has at most $3^3=27$ terms, so a component bound $\overline\varepsilon$ in one frame gives a component bound $27\overline\varepsilon$ in the other, uniformly on the entire slice portion; the inverse comparison has the same bound. Thus the fixed-tolerance predicate is unambiguous, and sufficiently small tolerances transfer after a universal factor, preserving dependence only on the previously fixed $\overline A_{\rm PK}$. This establishes well-definedness and the stated frame convention, without deducing rigidity from the definition. [F1, F2, F3, F4, step 1.1, algebra] ∎

## External input

[AIK, section 1.1 PK (1.4), section 2.1 (2.5), and section 2.3 (2.18)–(2.19)](https://arxiv.org/html/0904.0982v1) supplies the source-specific weighted component inequality and its effective-constant dependence. The reference records its statement, hypotheses and reading limits. The frame construction and comparison in Justification are local arguments; the source rigidity theorem is not proved or imported by this definition.
