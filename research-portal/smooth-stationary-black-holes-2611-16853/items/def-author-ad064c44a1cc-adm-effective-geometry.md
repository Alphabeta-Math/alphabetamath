---
id: def-author-ad064c44a1cc-adm-effective-geometry
title: The actual geometric constant in the small-ADM theorem
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-ad064c44a1cc-adm-gr-sbs
  - def-author-ad064c44a1cc-adm-angular-momentum-parameters
  - def-author-ad064c44a1cc-adm-maximal-section
  - def-stationary-asymptotic-decay-data
dependency_roles:
  def-author-ad064c44a1cc-adm-gr-sbs: mathematical-premise
  def-author-ad064c44a1cc-adm-angular-momentum-parameters: mathematical-premise
  def-author-ad064c44a1cc-adm-maximal-section: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1
      locator: "§1.1: setup, GR and (1.1), SBS and the separate maximality paragraph;
        quantitative-coordinate paragraphs immediately before (1.2), equations
        (1.2)–(1.3), and Theorem 1.1 for mass-one application."
      reading_limits: Retrieved arXiv HTML v1 and read §1.1 from the spacetime setup
        through GR, (1.1), SBS, maximality, the quantitative-coordinate
        paragraphs, (1.2)–(1.3), and Theorem 1.1 with its adjacent
        qualification. Used only to check this definition and its application
        hypotheses. The interpolation construction in reference [5], rigidity
        proof, and existence of the quantitative package for any particular
        spacetime were not reviewed or reconstructed.
      statement: The quantitative package uses A_1, R_1>=max(R_0,A_1^4), epsilon_0>0,
        spatial metric comparability on Phi_0(E_{3/4}), and differentiated
        remainder coefficients bounded by A_1. Its extension
        Phi_1:(-epsilon_0,epsilon_0) x E_{1-epsilon_0}->Mtilde interpolates
        between the slice unit normal and T, agrees with the stationary chart
        for r>2R_1, and satisfies sum_i|g_0i|+|g_00+1|<=A_1/(R_1+r). Equation
        (1.3) defines Abar as the maximum of R_1, epsilon_0^{-1}, (M^2-J)^{-1}
        and the supremum on Mtilde of all metric and stationary-field component
        derivatives through spacetime order six, summed over indices.
      hypotheses: The smooth stationary Ricci-flat four-spacetime with signature
        (-,+,+,+), source GR/SBS, the given maximal slice with smooth boundary
        geometry, and J<M^2. Supply the stated chart and quantitative bounds;
        finite Abar is required for a bounded-geometry application. Theorem 1.1
        uses mass-one data. The source M is denoted M_0 locally.
dependency_level: 6
---

## Definition

For the Radu ADM source choose its chart data $A_1,R_1,\varepsilon_0$, with $R_1\ge\max(R_0,A_1^4)$ and $\varepsilon_0>0$. Require $A_1^{-1}|v|^2\le h_{ij}v^iv^j\le A_1|v|^2$ on $\Phi_0(E_{3/4})$, and differentiated coefficients of the three remainders in its end expansion bounded by $A_1$ (at order $m\le6$ their weights are $r^{m+1}$, $r^{m+2}$ and $r^{m+3}$ for spatial, temporal and mixed remainders respectively). Supply the source extension chart $\Phi_1:(-\varepsilon_0,\varepsilon_0)\times E_{1-\varepsilon_0}\to\widetilde M$, built by interpolation between the slice unit normal and $T$, agreeing with the stationary chart for $r>2R_1$, and obeying
$$\sum_{i=1}^3|g_{0i}|+|g_{00}+1|\le A_1/(R_1+r).$$
Under $J<M_0^2$ set
$$\overline A_{\rm ADM}=\max\left\{R_1,\varepsilon_0^{-1},(M_0^2-J)^{-1},\sup_{\widetilde M}\sum_{m=0}^6\left(\sum_{a,b=0}^3|\partial^m g_{ab}|+\sum_{a=0}^3|\partial^mT^a|\right)\right\}.$$
Here all spacetime coordinate derivatives and components are summed, and the supremum is required finite. The source's quantitative condition is a bound on this actual normalized chart package. It is not a claim that small $J$ alone controls curvature, chart radius, horizon collar width or the distance to extremality.

## Facts & Assumptions

[F1] [[def-author-ad064c44a1cc-adm-gr-sbs]] fixes the end and charts; [[def-author-ad064c44a1cc-adm-angular-momentum-parameters]] fixes $M_0,J$ and the mass-one labels. [[def-author-ad064c44a1cc-adm-maximal-section]] fixes the original maximal section.

[F2] [[def-stationary-asymptotic-decay-data]] defines componentwise spatial Cartesian differentiated decay estimates and uniform constants on the exterior chart.

[F3] Radu, §1.1, the quantitative-coordinate paragraphs and (1.2)–(1.3), specifies the interpolated chart package and effective constant. The finite supremum of spacetime coordinate derivatives on that chart is an explicit hypothesis of the Definition, to be supplied for each application; it is not inferred from the spatial decay notation in [F2].

## Justification

Every term is computed from the specified source chart, metric, field and positive parameters. The strict parameter inequality makes the inverse gap finite, and the explicit supremum condition makes the last term finite. A maximum of this finite list is a unique finite positive number. The ancillary chart and remainder conditions remain part of the package; merely writing down a maximum on an unrelated chart would not instantiate the source theorem. The chart choices and all their bounds must be supplied for each application.
