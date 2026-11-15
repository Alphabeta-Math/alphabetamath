---
id: def-author-ad064c44a1cc-adm-maximal-section
title: Maximality and smooth boundary in the ADM theorem
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-author-ad064c44a1cc-adm-gr-sbs
  - def-spacelike-maximal-hypersurface-data
dependency_roles:
  def-author-ad064c44a1cc-adm-gr-sbs: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: §1.1 definitions of h and k, maximality equation and smooth-extension
        sentence immediately after SBS
      statement: For the future unit normal T_0 to Sigma^0, set h=g restricted to T
        Sigma^0 and k(Y,V)=-g(D_Y T_0,V) for tangent Y,V. The additional
        maximality hypothesis is tr_h k=0 on Sigma_1; its induced geometry
        extends smoothly to S_0 within Sigma^0. These are conditions on the
        given slice, not an existence assertion for another slice.
      hypotheses: "The connected oriented time-oriented smooth stationary vacuum
        four-spacetime of signature (-,+,+,+) and the GR/SBS slice data of
        section 1.1: Sigma^0 is the supplied embedded spacelike partial Cauchy
        hypersurface, Sigma_1=Phi_0(E_1), and S_0=Phi_0({|x|=1}). Maximality and
        smooth extension are additional assumptions, separate from the later
        angular-momentum restriction and quantitative smallness conditions."
      reading_limits: Freshly retrieved the indicated arXiv HTML version and read the
        exact formulation and adjacent hypothesis definitions. This citation
        attributes the locally transcribed definition; no theorem proof or
        supplier proof review was performed.
dependency_level: 5
---

## Definition

For the Radu ADM package let $n$ be the future unit normal to $\Sigma^0$, $h=g|_{T\Sigma^0}$ and $k(Y,V)=-g(\nabla_Yn,V)$ for fields tangent to the slice. The additional **original maximality and boundary condition** is
$$\operatorname{tr}_h k=0\quad\hbox{on }\Sigma_1,$$
and smooth extension of the induced geometry to $\overline\Sigma_1=\Sigma_1\cup S_0$ within $\Sigma^0$. The trace is $h^{ij}k_{ij}$. This concerns the original stationary slice; it does not assert existence of any transformed maximal slice or impose maximality as part of the nontrapping theorem.

## Facts & Assumptions

[F1] [[def-author-ad064c44a1cc-adm-gr-sbs]] provides the source slice and its specified sphere. [[def-spacelike-maximal-hypersurface-data]] provides its future unit normal, induced positive metric and the same negative-sign second fundamental form convention.

## Justification

The normal and tangential derivatives along the supplied smooth hypersurface determine $k$ and $h$. Positive definiteness gives the inverse used in the trace, and the zero trace is an unambiguous predicate; its zero value is unchanged if a source uses the opposite sign for the second fundamental form. Here the displayed sign is exactly the ADM source's convention. The specified smooth boundary extension is an additional regularity predicate, not a consequence of trace zero or an assertion that new hypersurfaces have been constructed.
