---
title: A compact-target boundary point has a null geodesic segment
status: published
research_item: lem-author-2632702918ef-compact-target-null-segment
dependency_level: 3
sources:
  references:
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://s3.cern.ch/inspire-prod-files-7/7a575d682fd15aaad8463a778fac1609
      locator: Section 4.5.4, Theorem 4.123 (Avez–Seifert) and its proof, printed/PDF
        p. 148 of 202; section 2.1, geodesic convention and equations
        (2.1)–(2.3), printed/PDF pp. 25–26.
      statement: In a globally hyperbolic spacetime, distinct points $p\le q$ are
        joined by a causal geodesic attaining the finite Lorentzian distance.
        Section 2.1 uses closed affine parameter intervals for connecting
        geodesics and gives their coordinate equation and affine
        reparametrization law.
      hypotheses: A time-oriented Lorentzian manifold with the source’s C2 metric
        regularity, global hyperbolicity, and distinct causally related
        endpoints. Here the metric is smooth. No acausality assumption on the
        target is needed.
      reading_limits: Read Theorem 4.123 and its printed proof on PDF p. 148, and
        section 2.1 through equation (2.3) on PDF pp. 25–26. Import geodesic
        existence and the affine convention; the limit-curve and
        upper-semicontinuity results were not reconstructed. Endpoint smoothness
        for the smooth metric is deduced below.
---

## Prerequisites

- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [physics:def-gr-fx-future-null-geodesic-completeness](https://alphabetamath.cc/physics/item/def-gr-fx-future-null-geodesic-completeness)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [` E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22 (2019), article 3 · Section 4.5.4, Theorem 4.123 (Avez–Seifert) and its proof, printed/PDF p. 148 of 202; section 2.1, geodesic convention and equations (2.1)–(2.3), printed/PDF pp. 25–26. `](https://s3.cern.ch/inspire-prod-files-7/7a575d682fd15aaad8463a778fac1609)


## Statement

Under the hypotheses of the compact-target causal-endpoint lemma, $p$ is joined to some $c\in C$ by a nonconstant future null geodesic segment. The segment may be affinely parametrized on $[0,1]$ and is smooth up to both endpoints.

## Facts & Assumptions

[A1] Work in ZFC; the axiom of choice includes the countable and dependent choice assumptions of the causal suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The smooth spacetime, global hyperbolicity and causal relations are those of [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data).

[F2] The target surface has the smooth embedded spacelike meaning of [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data).

[F3] There is a distinct $c\in C$ with $p\le_Ec$, and $p\notin I_E^-(C)$. [lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)

[F4] The External input is the Avez–Seifert theorem for two distinct causally related points in a globally hyperbolic spacetime, with the affine geodesic-segment convention of the source’s section 2.1.

[F5] A future null affine geodesic is a smooth nonconstant curve with nonzero future null tangent and $D_s\dot\gamma=0$; positive affine changes preserve its orientation. Only this definition, not any completeness assertion, is used. [physics:def-gr-fx-future-null-geodesic-completeness](https://alphabetamath.cc/physics/item/def-gr-fx-future-null-geodesic-completeness)

[F6] The metric-selected connection is smooth and metric-compatible: along a curve, $\frac{d}{ds}g(V,V)=2g(D_sV,V)$. It is the Levi–Civita connection used by the imported geodesic equation. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the asserted conclusion.

1.1 Apply [F4] in $(E,g)$ to the pair provided by [F3]. Global hyperbolicity holds, and the endpoints are distinct and causally related. In the source’s section 2.1 convention this gives a nonconstant future causal affine geodesic segment $\gamma:[a,b]\to E$, $a<b$, with $\gamma(a)=p$ and $\gamma(b)=c$; both endpoints are included in the segment. [F1, F2, F3, F4, F6, given]

2.1 By [F6] and the affine geodesic equation, $\frac{d}{ds}g(\dot\gamma,\dot\gamma)=2g(D_s\dot\gamma,\dot\gamma)=0$. Thus the squared speed is constant. If it were negative, the future causal geodesic would be timelike from $p$ to $c$, contrary to [F3]. Its tangent is therefore null everywhere, with the nonzero future tangent required in [F5]. [step 1.1, F1, F3, F5, F6, algebra]

3.1 Put $\eta(t)=\gamma(a+(b-a)t)$ for $0\le t\le1$. The chain rule gives $\eta\prime=(b-a)\dot\gamma$ and $D_t\eta\prime=(b-a)^2D_s\dot\gamma=0$, so this is the desired positive affine normalization. The imported segment has included endpoints, rather than merely an asymptotic endpoint. In endpoint charts its equation is $x^{\mu\prime\prime}=-\Gamma^\mu_{\alpha\beta}(x)x^{\alpha\prime}x^{\beta\prime}$, with smooth coefficients by [F6]; starting with its twice differentiable geodesic solution, this equation successively gives derivatives of every order, with one-sided derivatives at included endpoints. Hence $\gamma$ and its affine reparametrization are smooth up to both endpoints, as asserted. [step 1.1, step 2.1, F4, F5, F6, algebra] ∎

## External input

Import Theorem 4.123 for the distinct points $p\le_Ec$ in the smooth globally hyperbolic spacetime $E$, using section 2.1’s affine geodesic-segment convention. It supplies a causal geodesic; maximality of length is unused. The endpoint lemma supplies the causal pair and chronological exclusion. Nullness, normalization and smooth endpoint regularity are deduced above; boundary containment and orthogonality belong to separate local lemmas.
