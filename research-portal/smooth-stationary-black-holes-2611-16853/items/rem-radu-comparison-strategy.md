---
id: rem-radu-comparison-strategy
title: Reported comparison and Bertotti–Robinson strategy
kind: remark
status: published
origin: pipeline
domain: physics
deps:
  - thm-harrison-electrovacuum-construction-input
  - def-spacelike-maximal-hypersurface-data
  - def-null-screen-expansion-and-focal-data
  - def-source-free-geometric-electrovacuum-data
  - def-stationary-lorentzian-data
  - def-kerr-metric
  - def-bifurcate-killing-horizon-data
  - math:def-mean-curvature-vector
  - physics:prop-gr-fx-null-raychaudhuri
  - physics:def-gr-energy-conditions
dependency_roles:
  thm-harrison-electrovacuum-construction-input: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-null-screen-expansion-and-focal-data: mathematical-premise
  def-source-free-geometric-electrovacuum-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-kerr-metric: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  math:def-mean-curvature-vector: mathematical-premise
  physics:prop-gr-fx-null-raychaudhuri: mathematical-premise
  physics:def-gr-energy-conditions: formulation-prerequisite
provenance:
  statement: ai-altered
  proof: not-applicable
physical_scope: The reported strategy concerns a smooth stationary,
  asymptotically flat vacuum black-hole geometry and its conditional source-free
  Einstein–Maxwell transformations; it reports no observation or experiment.
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p. 6, §1.4, paragraphs beginning “The strategy of Radu” and “Our
        strategy”; continuation on PDF p. 7
      statement: The authors describe Radu's comparison with a stable minimal sphere
        on a maximal slice, its charge-based area bound, a limiting null-cone
        rigidity argument, and the subsequent use of small angular momentum;
        they contrast their own comparison with the bifurcation sphere.
      hypotheses: This is attribution of the article's account in its mass-one,
        stationary vacuum black-hole setting and its Harrison family; it is not
        an independent proof of the reported implications.
      reading_limits: Read the frozen extracted article text at the stated passage.
        The passage is reported as the authors' account; no independent
        verification of the complete comparison or rigidity argument is claimed.
    - title: Rigidity of stationary black holes with small ADM angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: §1.2, equality discussion; §3.1, equation (3.8) and following
        paragraph; §4.2, Lemma 4.2
      statement: The Bertotti–Robinson product used in the discussion has a
        two-dimensional Lorentzian factor of curvature minus one and a unit
        round sphere; the paper discusses recovery of the Kerr end in its
        equality case with the stationary normalization retained.
      hypotheses: The product description uses the unit normalization in the cited
        passage. The equality-case conclusion is subject to the hypotheses of
        the cited lemma and is not established by the product description alone.
      reading_limits: Read the indicated product descriptions and the statement and
        opening of Lemma 4.2 in the arXiv HTML. The complete equality-case proof
        and its hypotheses were not independently checked for this item.
    - title: Otis Chodosh, Stable Minimal Surfaces and Positive Scalar Curvature (Math
        258, Stanford, Fall 2021)
      url: https://web.stanford.edu/~ochodosh/Math258-min-surf.pdf
      locator: "§1, PDF pp. 2–3: two-sided hypersurface setup, variation convention
        before Lemma 1.2, Definition 1.4 and Proposition 1.5"
      statement: A smooth two-sided minimal hypersurface in a smooth Riemannian
        manifold is stable when its area has nonnegative second derivative at
        zero for every smooth compactly supported normal variation.
      hypotheses: The hypersurface has no boundary and admits a smooth unit normal.
        Variations are smooth families of immersions through the inclusion,
        fixed outside a compact subset. Applied only to the closed two-sided
        comparison sphere inside its Riemannian spacelike slice; no
        scalar-curvature assumption is required for this definition.
      reading_limits: Read PDF text on pp. 2–3 through Proposition 1.5 using the web
        PDF extraction. Only the setup and stability definition are imported; no
        visual inspection, existence theorem, area-charge bound or rigidity
        result is claimed.
dependency_level: 6
---

## Statement

In §1.4 the article reports the following strategy of Radu [36]. In the mass-one Harrison family $g_q$, one compares suitable spheres $C_q$ with a stable minimal two-sphere in a maximal spacelike slice bounded by the bifurcation sphere and $C_q$. The article reports a lower bound $4\pi(1-q^2)$ for the stable sphere's area, arising from the electric flux, and says that $T$ must be timelike at $C_q$ to control the slice's slope there. It explains that constructing the slice directly for $g_0$ may fail because the end is asymptotically cylindrical, so the comparison is made for sufficiently small positive $q$ and then passed to the limit.

The article further reports that the spheres can be arranged so their limiting sphere $C$ has a future $g_0$ null cone extending to infinity without focal or cut points and with limiting area $4\pi$. Its account uses the Raychaudhuri equation and the dominant energy condition to obtain equality of the area of $C$ with $4\pi$, zero expansion and zero shear. It then reports an identification of the transformed asymptotic region with Bertotti–Robinson geometry and recovery of Kerr by the inverse transformation. In this account angular-momentum smallness is not imposed in that step; it is imposed later to obtain a smallness condition on the bifurcation sphere and invoke [3]. These are reported steps of a strategy, not a proof here of the comparison, its limiting construction, or the rigidity conclusion.

## Statement references

[[thm-harrison-electrovacuum-construction-input]]

[[def-spacelike-maximal-hypersurface-data]]

[[def-null-screen-expansion-and-focal-data]]

[[def-source-free-geometric-electrovacuum-data]]

[[def-stationary-lorentzian-data]]

[[def-kerr-metric]]

[[def-bifurcate-killing-horizon-data]]

[[math:def-mean-curvature-vector]]

[[physics:prop-gr-fx-null-raychaudhuri]]

[[physics:def-gr-energy-conditions]]

[Chodosh, §1, Definition 1.4](https://web.stanford.edu/~ochodosh/Math258-min-surf.pdf)

## Terminology and scope

The family supplier specifies the mass-one hypotheses and its actual scope: $g_q$ and the Maxwell form are constructed for $0\le q\le1$, with the electrovacuum equations asserted on the exterior. It does not by itself supply the maximal slices, comparison spheres, limiting cone, or rigidity argument described above. Here the bifurcation sphere is the spacelike two-sphere where the two smooth null Killing-horizon branches meet transversely and their common horizon Killing field vanishes; that field need not be the stationary field $T$. The stationary field $T$ is Killing, meaning that its local flow preserves the metric; timelike at a point means $g_q(T,T)<0$ there. A spacelike slice has positive-definite induced metric, and it is maximal when its mean curvature vanishes. For the smooth inclusion of a two-sphere in the slice with its induced Riemannian metric, mean curvature is the averaged mean curvature vector, one half of the trace of its second fundamental form. A minimal two-sphere in that slice has zero mean curvature vector; stability means that the second variation of its area is nonnegative for every smooth compactly supported normal variation. Variations here are within the Riemannian slice, through smooth immersions that agree with the inclusion at parameter zero and outside a fixed compact subset. The comparison sphere is closed and two-sided, with a smooth unit normal. These conditions do not assert that such a sphere exists.

The electric charge of an oriented closed surface is $Q_E=(4\pi)^{-1}\int_S\star_{g_q}F_q$, with the orientation and Hodge-star conventions of the charge supplier. The family supplier gives $Q_E=\sqrt{1-q^2}$ on the stated outward end spheres. This normalization explains the numerical charge-squared expression in the reported area bound; it does not establish the bound for the comparison sphere or the required flux identification.

For a null congruence normal to a spacelike two-surface, expansion is the trace of its null second fundamental form and shear is its trace-free part. A focal point is a point at which the normal screen Jacobi map loses rank. A boundary cut point is defined using the endpoint of the segment remaining on the future causal boundary; absence of focal points and absence of cut points are distinct conditions. A non-expanding cone has vanishing expansion along its regular generators. For a smooth symmetric stress-energy tensor $\mathsf T$ on an open matter domain in the time-oriented Lorentzian four-spacetime, the energy-momentum flux vector for a future timelike observer $v$ is $J_v=-(\mathsf T(v,\cdot))^{\sharp_{g_q}}$. The dominant energy condition requires $J_v$ to be future causal or zero at every point for every such $v$. This uses the energy-condition supplier only for terminology; it does not assume or prove that the transformed fields satisfy that condition. The Bertotti–Robinson product referred to in the comparison has a two-dimensional Lorentzian factor of constant curvature $-1$ and a unit round two-sphere in this normalization; Kerr denotes the metric family in the cited definition.

The null Raychaudhuri supplier gives the evolution identity for a smooth, affinely parametrized null geodesic hypersurface congruence from a spacelike two-surface, on the regular interval before its first focal instant. Its focusing bound additionally assumes a nonnegative null Ricci contraction, negative initial expansion and existence through the comparison parameter. No energy condition or field equation is inferred by that mathematical supplier, and it does not by itself establish the reported limiting construction or equality-case rigidity.

## Source note

Radu's cited equality discussion retains the normalization of the stationary field when recovering Kerr. The brief account above does not assert that a product geometry alone determines the Kerr angular momentum, nor that the source's detailed hypotheses follow solely from the terminology given here.

## External input

Chodosh’s §1 setup and Definition 1.4 supply the stability terminology for the smooth closed two-sided sphere in its Riemannian slice. This imports only the definition for compactly supported normal variations, not the existence of a comparison sphere or an area inequality.
