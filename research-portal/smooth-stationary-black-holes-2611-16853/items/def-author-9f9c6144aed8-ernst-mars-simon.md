---
id: def-author-9f9c6144aed8-ernst-mars-simon
title: Ernst sublevels and the Mars–Simon tensor interface
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-complex-self-dual-two-form-data
  - math:def-interior-product-of-a-form-by-a-vector-field
  - physics:def-gr-metric-volume-form-and-current-flux
  - math:def-smooth-embedding
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  math:def-interior-product-of-a-form-by-a-vector-field: mathematical-premise
  physics:def-gr-metric-volume-form-and-current-flux: mathematical-premise
  math:def-smooth-embedding: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Ionescu–Klainerman, On the uniqueness of smooth, stationary black holes
        in vacuum
      url: https://arxiv.org/pdf/0711.0040
      locator: §4.2, (4.11), (4.15), (4.17) and the normalization paragraph after
        (4.18), printed pp. 22–23; §4.3, (4.19)–(4.21), (4.27), Definition 4.3
        (4.29), printed pp. 23–24; §7, (7.3), printed p. 35; Appendix A.3,
        opening curvature-component formula, printed p. 54 (PDF p. 54).
      statement: Definitions of the Killing two-form, complex self-dual form, Ernst
        differential, normalized potential, reciprocal potential and Mars–Simon
        tensor, and the Riemann curvature sign and slot convention used in these
        formulas.
      hypotheses: The cited development assumes a smooth oriented four-dimensional
        vacuum spacetime, a Killing field and an existing Ernst potential; 1−σ
        is nonzero on the reciprocal/tensor domain. Only the displayed
        definitions are adopted here for stationary Lorentzian data with a
        supplied potential; no vacuum identity or existence theorem is imported.
      reading_limits: Read the PDF text at the listed definition equations and
        normalization paragraph, including (7.3), and the opening curvature
        formula of Appendix A.3 on printed p. 54. Compared that formula with the
        stationary-data supplier. The end parametrization, quantified limit and
        complex-linear extension are local formulation details. No PDF image
        inspection, analytic proof reconstruction or independent proof review is
        claimed.
dependency_level: 1
---

## Definition

Use the stationary Lorentzian data, metric connection and index conventions, together with the complex self-dual-form conventions. Let $F_{ab}=\nabla_aT_b$, $\mathcal F=F+i\star F$, and $\mathcal F^2=\mathcal F_{ab}\mathcal F^{ab}$ without conjugation. For a complex two-form $U+iV$ with real $U,V$, use the interior product extended complex linearly: $\iota_T(U+iV)=\iota_TU+i\iota_TV$, so $(\iota_T\mathcal F)_b=T^a\mathcal F_{ab}$.

As normalization data, choose $R_0>0$ and a smooth embedding $e:\{x\in\mathbb R^3:|x|>R_0\}\to M$. Its image is the chosen parametrized spatial end, with radial coordinate $r(e(x))=|x|$. This end datum specifies where the limit is taken and imposes no metric decay conditions. For this interface an **Ernst potential** is a supplied smooth complex scalar $\sigma$ satisfying $d\sigma=2\iota_T\mathcal F$, normalized by $\sigma\to1$ along this end. Precisely, for every $\varepsilon>0$ there is $R>R_0$ such that $|\sigma(e(x))-1|<\varepsilon$ for all $|x|>R$, uniformly in angular direction. Existence of the end datum and of such a potential is supplied, not proved here.

On the open set $N=\{1-\sigma\ne0\}$ define $P=(1-\sigma)^{-1}$ and $y=\operatorname{Re}P$. Write $\epsilon=\mathrm{vol}_g$ for the oriented metric volume tensor: in every positively oriented coordinate chart, $\mathrm{vol}_g=\sqrt{|\det(g_{ab})|}\,dx^0\wedge dx^1\wedge dx^2\wedge dx^3$. Use the same orientation for this tensor and the Hodge star. Write $R_{ab cd}$ for the curvature convention used in the cited source; let $\mathcal R_{ab cd}=R_{ab cd}+\frac i2\epsilon_{cd}{}^{ef}R_{ab ef}$ and $\mathcal I_{ab cd}=(g_{ac}g_{bd}-g_{ad}g_{bc}+i\epsilon_{ab cd})/4$. The **Mars–Simon tensor in the IK convention** is $\mathcal S_{ab cd}=\mathcal R_{ab cd}+6(1-\sigma)^{-1}(\mathcal F_{ab}\mathcal F_{cd}-\mathcal F^2\mathcal I_{ab cd}/3)$. Curvature and orientation conventions must be transported together when applying this formula.

## Definition references

[[def-stationary-lorentzian-data]]

[[def-complex-self-dual-two-form-data]]

[[math:def-interior-product-of-a-form-by-a-vector-field]]

[[physics:def-gr-metric-volume-form-and-current-flux]]

[[math:def-smooth-embedding]]

## Justification

The Killing equation makes $F$ alternating, using [[def-stationary-lorentzian-data]]. The supplied self-dual-form interface [[def-complex-self-dual-two-form-data]] defines the complex contractions. The real interior product in [[math:def-interior-product-of-a-form-by-a-vector-field]] is smooth and inserts $T$ into the first slot; its complex-linear extension is well defined because the real and imaginary parts are unique. The end embedding, in the sense of [[math:def-smooth-embedding]], makes $\sigma\circ e$ a specified function on a Euclidean exterior; the quantified limit is therefore a predicate on the supplied data, rather than an assertion that stationary geometry provides an end or a normalized potential.

Clause (a) of [[physics:def-gr-metric-volume-form-and-current-flux]] supplies the smooth normalized metric volume form on an oriented Lorentzian four-manifold. Raising its indices uses the given inverse metric. On $N$ the smooth nonzero denominator permits the reciprocal and tensor formula, so they define smooth fields there. This construction does not assert a wave equation, vanishing or a Kerr characterization.

Appendix A.3 of Ionescu–Klainerman, printed p. 54, fixes $R_{ab cd}=g(e_a,\nabla_{e_c}\nabla_{e_d}e_b-\nabla_{e_d}\nabla_{e_c}e_b-\nabla_{[e_c,e_d]}e_b)$. This is the curvature operator of [[def-stationary-lorentzian-data]] with its output index lowered: in a coordinate frame $R_{ab cd}=g_{ae}R^e{}_{bcd}$. Thus the imported convention agrees with that supplier without a sign reversal or slot permutation.

## External input

Ionescu–Klainerman supplies the displayed definition formulas in §4.2–§4.3, printed pp. 22–24, and the reciprocal potential in §7, equation (7.3), printed p. 35. Appendix A.3, printed p. 54, supplies the curvature convention compared above. Its normalization is at infinity along the chosen section. The embedding and quantified angularly uniform limit above specify that convention locally. Only definitions are adopted from the source's vacuum setting; no potential-existence or analytic theorem is inferred.
