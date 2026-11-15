---
id: pthm-causal-finite-time-escape
title: Causal speed and finite-section-time escape estimates
kind: physics-theorem
status: draft
origin: pipeline
domain: physics
proof_strategy: direct
deps:
  - pthm-global-harrison-one-form
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-harrison-normalization
  - def-stationary-maximal-graph
  - def-stationary-section-time
  - def-spacelike-maximal-hypersurface-data
  - def-causal-exterior-and-boundary-data
  - pthm-complete-maximal-slices
  - pthm-positive-transformed-lapse
  - pthm-adm-temporality
  - pthm-transformed-end-geometries
  - lem-author-eb8e266b8b92-adm-time-speed
  - lem-author-eb8e266b8b92-collar-nonarrival
  - lem-author-eb8e266b8b92-proper-radius-control
  - lem-author-eb8e266b8b92-interior-compact-confinement
  - lem-author-eb8e266b8b92-compact-causal-endpoint
  - math:def-axiom-of-choice
  - math:lem-schwartz-cutoffs-from-the-standard-smooth-step
dependency_roles:
  pthm-global-harrison-one-form: physical-result
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-stationary-maximal-graph: mathematical-premise
  def-stationary-section-time: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  pthm-complete-maximal-slices: physical-result
  pthm-positive-transformed-lapse: physical-result
  pthm-adm-temporality: physical-result
  pthm-transformed-end-geometries: physical-result
  lem-author-eb8e266b8b92-adm-time-speed: mathematical-premise
  lem-author-eb8e266b8b92-collar-nonarrival: mathematical-premise
  lem-author-eb8e266b8b92-proper-radius-control: mathematical-premise
  lem-author-eb8e266b8b92-interior-compact-confinement: mathematical-premise
  lem-author-eb8e266b8b92-compact-causal-endpoint: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:lem-schwartz-cutoffs-from-the-standard-smooth-step: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pages 23–24, proof of Lemma 4.1 and equation (4.3)
      reading_limits: "Retained prior source-input or attribution record: Retained
        attribution only: The article derives the causal ADM speed inequality,
        the collar and end escape estimates, and an endpoint on the remaining
        compact region. Attributed setting: The regular stationary construction
        and positive-parameter maximal section used in the article's proof. Read
        the frozen extracted article text at the cited passage. This reference
        attributes the claim and is not used as a proof premise. Fresh
        maintenance limits: current item and supplier contracts and the local
        applications were checked; no new reading of the external proof or PDF
        images is claimed."
    - title: John M. Lee, Introduction to Riemannian Manifolds, second edition (2018)
      url: https://pierre.ag.gerard.web.ulb.be/textbooks/books/IntroductionToRiemannianManifo.pdf
      locator: Theorem 5.25 and normal-tube definitions, printed p. 133 (PDF p. 145);
        Corollary 6.39, p. 180 (PDF p. 192); Theorem 6.40, p. 181 (PDF p. 193);
        Example 6.44, p. 183 (PDF p. 195).
      statement: The normal exponential map gives a uniform tubular neighborhood for a
        compact embedded submanifold. Its normal-length coordinate equals
        ambient distance there and has unit gradient off the submanifold.
        Boundary normal coordinates follow by smoothly extending the metric to
        the double and restricting Fermi coordinates to the inward side.
      hypotheses: The tubular and distance results concern an embedded submanifold of
        a smooth Riemannian manifold without boundary; compactness gives uniform
        radius, and Theorem 6.40 assumes the ambient manifold connected. Example
        6.44 assumes a smooth Riemannian manifold with nonempty boundary and
        supplies the double/metric-extension construction. Here the section is
        smooth and spacelike up to its compact boundary S; its connected double
        with the extended induced Riemannian metric meets those hypotheses. No
        spacetime causality or field equation is assumed in this input.
      reading_limits: "Retained prior source-input or attribution record: Consulted
        the PDF extracted text at the stated definitions, theorem statements,
        Corollary 6.39 and Theorem 6.40 distance arguments, and Example 6.44.
        Used these established geometric inputs without auditing their earlier
        supporting results or reconstructing the smooth metric-extension
        theorem. The intrinsic-distance comparison and causal application are
        proved locally below. Fresh maintenance limits: current item and
        supplier contracts and the local applications were checked; no new
        reading of the external proof or PDF images is claimed."
physical_scope: Conditional causal geometry of the smooth stationary vacuum
  model and its positive-parameter Harrison-transformed metrics; no observation
  or measurement is asserted.
dependency_level: 23
---

## Statement

Adopt the regular mass-one stationary vacuum construction with maximal original exterior section and $T|_S\not\equiv0$, and assume the Axiom of Choice. Fix $q\in(0,1]$ and a complete smooth spacelike maximal graph section $\Sigma_q$ supplied by [[pthm-complete-maximal-slices]]. Its compact boundary is the bifurcation sphere $S$. Let $v=v_q$ be stationary section time, and write the stationary metric as $g_q=-N^2dv^2+h_{ij}(dx^i+X^idv)(dx^j+X^jdv)$, with positive lapse $N$, induced Riemannian metric $h$, and shift $X$.

A causal curve is locally absolutely continuous with nonzero causal velocity almost everywhere. A future causal curve admits section-time parameterization and obeys $h_{ij}((x^i)'+X^i)((x^j)'+X^j)\le N^2$ almost everywhere. Near $S$, let $\rho$ be the $h$-distance to $S$, extended constantly along the stationary flow. In a sufficiently small collar, $N=O(\rho)$ and $X(\rho)=O(\rho)$, and hence $|d\rho/dv|\le C\rho$ almost everywhere and $\rho(v)\ge\rho(v_0)e^{-C|v-v_0|}$ while the curve remains in the collar. On the asymptotic end, for the original radial coordinate $r$, $|r'|\le |dr|_h(N+|X|_h)\le C$ sufficiently far out. Constants may depend on the fixed $q$.

A causal curve cannot reach $S$ or escape to infinity in finite section time. If its spatial projection remains in an interior compact set and its section time approaches a finite endpoint, the curve has an endpoint in the exterior. Thus an inextendible causal curve has section-time image $\mathbb R$. These assertions concern section time, not geodesic affine completeness.

## Facts & Assumptions

**Given:** The model, choice convention, positive parameter, supplied section and causal curve in the Statement.

**Goal:** Prove the speed, collar, end and endpoint assertions.

[A1] The regular data supply the compact sphere $S$, the stationary field tangent to both transverse horizon branches, and the one-ended exterior. The mass normalization and stationary model specify the transformed family. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]] [[def-harrison-normalization]]

[A2] Work in ZFC, including the choice assumptions inherited by the mathematical suppliers. [[math:def-axiom-of-choice]]

[F1] The section theorem supplies a smooth spacelike graph with boundary $S$, complete up to that boundary, and normalized end derivatives tending to zero. The graph and section-time definitions identify the exterior with the stationary product and define $v$. [[pthm-complete-maximal-slices]] [[def-stationary-maximal-graph]] [[def-stationary-section-time]]

[F2] The lapse theorem gives $N>0$ in the interior and $N=0$ on $S$. The ADM theorem gives the displayed stationary metric; the shift is the section-tangent part of $T=Nn+X$. [[pthm-positive-transformed-lapse]] [[pthm-adm-temporality]] [[def-spacelike-maximal-hypersurface-data]]

[F3] Apply the additional positive-parameter conclusion of [[pthm-transformed-end-geometries]] for the actual smooth primitive of [[pthm-global-harrison-one-form]] in the standing regular mass-one construction, with maximal original exterior section and $T|_S\not\equiv0$. The pole, normalized contraction and single family are unchanged; only $(W_0)_i=O_5(r^{-3})$ is required, not equality with the exact radial integral. For this fixed $q>0$, the normalized metric is $-1+O_5(r_q^{-1})$ in its time-time component, $O_5(r_q^{-2})$ in its mixed components and $\delta_{ij}+O_5(r_q^{-1})$ spatially. These are the end bounds used below.

[F4] The causal section-time speed lemma supplies the causal reparameterization, the displayed speed inequality, and $|(f\circ x)'|\le N|df|_h+|X(f)|$ for smooth $f$. Causal relations and endpoints are relative to the exterior. [[lem-author-eb8e266b8b92-adm-time-speed]] [[def-causal-exterior-and-boundary-data]]

[F5] The normal-tube, distance-gradient and boundary-normal-coordinate results of Lee are recorded in External input below. Together they supply the geometry used to construct the intrinsic boundary-distance collar in step 1.2. [Lee, Theorem 5.25, Corollary 6.39, Theorem 6.40 and Example 6.44](https://pierre.ag.gerard.web.ulb.be/textbooks/books/IntroductionToRiemannianManifo.pdf).

[F6] The compact-confinement lemma combines a boundary collar barrier and a proper-radius bound; the compact-endpoint lemma supplies a limit at a finite time endpoint for a trajectory confined to an interior compact set. [[lem-author-eb8e266b8b92-interior-compact-confinement]] [[lem-author-eb8e266b8b92-compact-causal-endpoint]]

[F7] Given a smooth compact-boundary collar with coordinate $\rho$, smooth positive-definite $h$ up to its boundary, and $N\le A\rho$, $|X(\rho)|\le A\rho$, $|d\rho|_h\le A$, the collar-barrier lemma gives $b(x(v))\ge b(x(v_0))e^{-(A^2+A)|v-v_0|}$ for $b=\min(\rho,a)$ in the collar, extended by $a$ outside it, where $0<a$ is smaller than the collar width. Its proof uses the absolute-continuity fundamental theorem and both orientations of Gronwall, including curves that leave and re-enter the collar. [[lem-author-eb8e266b8b92-collar-nonarrival]]

[F8] In the stationary ADM setting, suppose the connected section has compact boundary, $h$ extends smoothly and positively to that boundary, $N$ and $X$ extend smoothly, and a supplied smooth nonnegative radius $R$ has compact sublevels. If $|dR|_h(N+|X|_h)$ is bounded outside a compact set, the proper-radius lemma gives $|R(x(v))-R(x(v_0))|\le C_R|v-v_0|$ for all section times. Its sufficient end realization is a compact core with finitely many product ends having compact cross sections, with $R$ equal to the unbounded end coordinate outside a larger compact core. [[lem-author-eb8e266b8b92-proper-radius-control]]

[F9] The smooth-cutoff lemma supplies $\eta\in C_c^\infty(\mathbb R)$ with $0\le\eta\le1$, $\eta=1$ on $|s|\le1$, and $\eta=0$ on $|s|\ge2$, by taking $n=1$. [[math:lem-schwartz-cutoffs-from-the-standard-smooth-step]]

## External input

Lee's normal-tube theorem gives a uniform normal-exponential diffeomorphism around a compact embedded submanifold in a smooth Riemannian manifold. In that tube the normal-length function equals ambient distance and has unit gradient away from the submanifold. Example 6.44 supplies smooth extension of a boundary metric to the double and restriction to inward boundary normal coordinates. These are imported premises; the intrinsic-distance comparison and the causal deductions below are local applications. The exact hypotheses, locators and reading limits are in the Lee source entry.

## Proof

1.1 Fix the parameter and section. The graph supplies the global stationary product, while the positive lapse and ADM form satisfy the hypotheses of the section-time speed lemma. It follows that future causal curves have strictly increasing $v$ and that their section-time parameterizations satisfy the displayed quadratic speed inequality almost everywhere. [A1, A2, F1, F2, F4]

1.2 The induced Riemannian metric $h$ is smooth and positive definite up to the compact boundary $S$. Use the boundary construction in [F5] to extend it smoothly to the connected double, with extended metric $\widehat h$. The compact normal-tube theorem gives a common $\epsilon>0$ for which $F(p,s)=\exp_p^{\widehat h}(s\nu_p)$, $p\in S$, $|s|<\epsilon$, is a diffeomorphism onto a normal tube, where $\nu$ is the inward unit normal. Shrink $\epsilon$ so that its inward half is a collar in the original section. The distance and gradient results in [F5] give $d_{\widehat h}(F(p,s),S)=s$ and $|ds|_h=1$ for $0<s<\epsilon$. Every curve confined to the section is also an ambient curve, so $d_h(F(p,s),S)\ge s$; the inward normal segment lies in the section and has length $s$, proving the reverse inequality. Thus the intrinsic boundary distance $\rho$ is exactly the smooth inward coordinate $s$, including at $S$. [F1, F5, A2]

2.1 The unit normal and the lapse and shift are smooth up to $S$. Since $T$ is tangent to both transverse horizon branches, $T|_S\in TS$. The lapse vanishes on $S$, so $X|_S=T|_S\in TS$ and $X(\rho)|_S=0$. In the collar of step 1.2, smoothness and compactness give $N\le A\rho$ and $|X(\rho)|\le A\rho$ on a smaller collar, with $A\ge1$. The scalar speed inequality and $|d\rho|_h=1$ give $|\rho'|\le2A\rho$ almost everywhere. All hypotheses of [F7] now hold. Choose $a$ smaller than this collar's width and apply that lemma to the truncated coordinate $b$. On the inner collar $\rho<a$, where $b=\rho$, its estimate is the stated exponential lower bound, with $C=A^2+A\ge2A$, on every interval contained in that collar. The global bound for $b$ also handles arbitrary departures and returns. [A1, A2, F1, F2, F4, F7, step 1.1, step 1.2]

2.2 In the normalized end chart, the metric coefficients tend to Minkowski values and the section graph derivatives tend to zero. Pulling the metric back to the graph shows that $h$ and $h^{-1}$ are uniformly bounded there. The lapse and shift, computed from the stationary metric and graph normal, are likewise bounded: the normalizing timelike covector has squared norm bounded away from zero for sufficiently large radius. Since $r$ differs from normalized radius by the fixed positive factor $q^{-1}$, $|dr|_h$ is bounded. The speed inequality consequently gives $|r'|\le |dr|_h(N+|X|_h)\le C$ on the end. [F1, F2, F3, F4, step 1.1, algebra]

3.1 Use the compact-core one-ended section data in [A1, F1, F2]. On its product end choose radii $0<r_1<r_2$ beyond the compact core and put $\delta=(r_2-r_1)/2>0$. For the one-dimensional cutoff $\eta$ in [F9], define $\chi(r)=0$ for $r\le r_1$ and $\chi(r)=1-\eta((r-r_1)/\delta)$ for $r>r_1$. On a neighborhood of $r_1$ both pieces are identically zero, so they join smoothly. Thus $0\le\chi\le1$, $\chi=0$ for $r\le r_1+\delta$, and $\chi=1$ for $r\ge r_2$. Define $R=r_1+\chi(r)(r-r_1)$ on the end and $R=r_1$ on the remaining core. These formulas agree near the gluing region, so $R$ is smooth, nonnegative and equals $r$ for $r\ge r_2$. The compact core and compact spherical cross sections give the sufficient end realization of [F8], hence compact sublevels. The smooth positive-definite extension of $h$ and the smooth extensions of $N,X$ were established in steps 1.2 and 2.1. Outside a larger compact set, $R=r$ and step 2.2 gives $|dR|_h(N+|X|_h)\le C$. Thus every hypothesis of [F8] holds, and its conclusion supplies the global estimate $|R(x(v))-R(x(v_0))|\le C_R|v-v_0|$, including portions of the curve in the compact remainder. [A1, A2, F1, F2, F8, F9, step 1.1, step 1.2, step 2.1, step 2.2, construct]

4.1 Steps 1.2 and 2.1 give the smooth collar data and global truncated-coordinate barrier required by [F6], and step 3.1 gives its proper-radius data and estimate. The compact-confinement lemma therefore places any bounded section-time segment in a compact subset of the section interior; in particular it cannot reach $S$ or escape along the end at finite section time. If a finite endpoint of the section-time interval existed for an inextendible curve, the compact-endpoint lemma would give a limit in the exterior, contradicting inextendibility. Reversing the time direction treats the other endpoint, so the image is all of $\mathbb R$. [A1, A2, F1, F4, F6, F7, F8, step 1.1, step 1.2, step 2.1, step 2.2, step 3.1] ∎

## Source notes

The article reference attributes the original estimate. The argument uses the completed section, lapse, end and mathematical causal suppliers; the article's claim is not used as its own proof.
