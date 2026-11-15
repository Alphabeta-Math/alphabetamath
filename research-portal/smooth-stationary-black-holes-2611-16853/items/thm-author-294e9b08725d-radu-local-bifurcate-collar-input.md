---
id: thm-author-294e9b08725d-radu-local-bifurcate-collar-input
title: External local boost collar and canonical temporal splice
kind: theorem
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-a4a441da4986-working-partial-cauchy-collar
  - def-regular-stationary-vacuum-spacetime
  - lem-author-294e9b08725d-regular-positive-stationary-mass
dependency_roles:
  lem-author-a4a441da4986-working-partial-cauchy-collar: mathematical-premise
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  lem-author-294e9b08725d-regular-positive-stationary-mass: mathematical-premise
provenance:
  statement: ai-altered
  proof: literature-derived
sources:
  references:
    - title: Alexandru F. Radu, On rigidity of stationary black holes under a
        nontrapping assumption
      url: https://arxiv.org/pdf/2609.23872v2
      locator: GR/SBS pp3–4; Proposition2.1 p7; Lemma2.2 statement pp9–10, exact boost
        coordinates (2.4) pp10–11 and cutoff construction pp11–12,
        quotient-escape conclusion p13; nonrotating specialization pp13–14
      statement: Under GR and SBS, a local Hawking field K=T+Omega Z has exact boost
        form K=kappa(V partial_V−U partial_U), kappa>0, with K=0 on S; in
        rotation Z is a commuting periodic local field. There is an acausal
        canonical outward section and a proper stationary collar R×Sigma_loc in
        E; its r→0 end leaves every compact quotient set. The proof constructs a
        temporal function equal to (V−U)/2 near S and the original Cauchy
        temporal function away from a compact neighborhood.
      hypotheses: The source GR package requires a smooth oriented time-oriented
        Ricci-flat four-manifold, positive ADM mass, the stated O6 stationary
        end with T future, globally hyperbolic DOC E, complete T-orbits in E
        meeting Sigma1, and an acausal edgeless partial section with both
        chronological end intersections Sigma1. SBS requires the smooth
        transverse nonexpanding bifurcate horizons and T tangent. The specified
        local conclusions use GR and SBS only, not NT or global axisymmetry. In
        the nonrotating case set K=T, Omega=0 and omit Z.
      reading_limits: Read full actual GR/SBS, Lemma2.2 statement and the displayed
        coordinate/cutoff and properness passages in its proof, plus the
        nonrotating specialization. Imported local results and construction; no
        proof review, nontrapping conclusion or global rotational field is
        asserted.
external_input: true
dependency_level: 8
---

## Statement

Assume the source GR and SBS hypotheses, including positive ADM mass and the acausal edgeless partial section with both chronological end intersections equal to its exterior part. Then near the bifurcation surface $S$ there are smooth double-normal coordinates $(U,V,p)$, a constant $\kappa>0$ and a Killing field $K$ with $K=\kappa(V\partial_V-U\partial_U)$ and $K|_S=0$. In rotation $K=T+\Omega Z$ with a commuting local circle field $Z$ preserving $U,V$; in the nonrotating case $K=T$. The outward section $\Sigma_{\rm loc}=\{U=V=r,0<r<\delta\}$ is spacelike and acausal, and its complete $T$-saturation is an embedded product collar in $E$. As $r\downarrow0$ this collar leaves every compact subset of the stationary quotient. The source cutoff construction gives a temporal function on $D(\Sigma_0)$ equal to $(V-U)/2$ near $S$ and to a Cauchy temporal function with zero level $\Sigma_0$ outside a compact neighborhood. No global horizon-generating field on $E$ is claimed.

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[F1] The adopted working collar supplies the required partial-Cauchy section and the original exterior. [[lem-author-a4a441da4986-working-partial-cauchy-collar]] [[def-regular-stationary-vacuum-spacetime]]

[F2] The general regular vacuum geometry has the positive stationary ADM mass needed in GR. [[lem-author-294e9b08725d-regular-positive-stationary-mass]]

## External input

Import the cited external results only under the exact hypotheses in the Statement and source records. Their proofs are not reconstructed or independently reviewed here.
