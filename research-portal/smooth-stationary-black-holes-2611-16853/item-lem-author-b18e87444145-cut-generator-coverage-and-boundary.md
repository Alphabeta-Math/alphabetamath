---
title: The selected endpoints cover the compact cut and remain on its past boundary
status: draft
research_item: lem-author-b18e87444145-cut-generator-coverage-and-boundary
dependency_level: 6
---

## Prerequisites

- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)


## Statement

Work in ZFC. Let $(E,g,N)$ be a time-oriented smooth Lorentzian four-manifold with its metric-selected connection, and compute all causal relations and boundaries in $E$. Let $v:E\to\mathbb R$ be smooth and temporal, with $dv(X)>0$ for every nonzero future causal vector $X$. Let $C\subset E$ be a smooth spacelike two-surface with $\min_Cv>0$, and let $D\subset\{v=0\}\cap\partial_E I_E^-(C)$ be compact. Choose a smooth future null-normal ray field on $C$. For each $c\in C$, let $\gamma_c:I_c\to E$ be a maximal affinely parametrized null geodesic with $\gamma_c(0)=c$ and initial past tangent on the opposite ray. Use its portion with parameter $s\ge0$ as the selected past ray.

Assume every $p\in D$ has a future null geodesic segment to some $c\in C$ whose final tangent is on the chosen future ray, whose interior has no focal point to $C$, and which lies on $\partial_E I_E^-(C)$. Define $A=\{c\in C:\gamma_c(s)\in D\text{ for some }s\in I_c\cap[0,\infty)\}$ and let $F(c)$ be that hit for $c\in A$. Then the hit is unique and $F(A)=D$. Every selected segment from $F(c)$ to $c$, for any $c\in A$, lies on the same past boundary. If the null-generator input excludes interior focal points on all such boundary segments, every selected segment has that exclusion.

## Statement references

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets)

[def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[A1] The axiom of choice is assumed, as in the focal-data interface. It implies dependent choice and countable choice, meeting the choice hypotheses of the causal and geodesic suppliers. It also permits selecting a nonzero initial vector on each supplied ray; no additional choice of a family of connecting segments is needed in the pointwise coverage argument. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F1] A prescribed initial vector determines a unique maximal geodesic. Affine reversal and positive rescaling give the same geodesic ray with the corresponding initial tangent, and short geodesics with any prescribed timelike initial vector exist smoothly. These conclusions apply with $M=E$. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F2] In the smooth time-oriented manifold $E$, push-up gives $x\le_Ey\ll_Ez\Rightarrow x\ll_Ez$ and $x\ll_Ey\le_Ez\Rightarrow x\ll_Ez$. Each $I_E^-(c)$ is open, so their union $I_E^-(C)$ is open. [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule) [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[F3] Causal relations, the time orientation and relative boundary have the exterior interface's meanings. The endpoint convention uses the unique hit of a chosen past ray on the temporal zero-level; only this endpoint convention, rather than the stationary remainder construction, is used here. Null normals and focal points have the supplied focal-data meanings, with time orientation reversed for the past congruence from $C$. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F4] Restrictions of a smooth future null segment are future causal curves in the stipulated locally absolutely continuous class. A smooth segment with future timelike tangent is a future timelike curve in that class. [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

## Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish unique hits, coverage, boundary containment and the conditional focal conclusion.

1.1 Along every selected past null ray, $(v\circ\gamma_c)'=dv(\dot\gamma_c)<0$, since its nonzero tangent is past causal. Thus $v\circ\gamma_c$ is strictly decreasing. Since $v(c)>0$ and $D\subset\{v=0\}$, a hit with $D$ has strictly positive parameter and is unique. Hence $F:A\to D$ is a function with the endpoint convention in [F3]. [given, F3]

2.1 For $p\in D$, take the supplied future null segment ending at $c\in C$, reverse it, and scale its affine parameter by a positive constant so that its initial tangent equals $\dot\gamma_c(0)$. This is possible because the final future tangent and $-\dot\gamma_c(0)$ lie on the same chosen ray. Maximal-geodesic uniqueness and scaling in [F1] identify the reversed segment with a restriction of $\gamma_c$, including its hit at $p$. Thus $c\in A$ and, by uniqueness of the hit, $F(c)=p$. The opposite inclusion $F(A)\subset D$ is the definition of $F$, proving $F(A)=D$. The segment is chosen for each fixed $p$, without choosing a family simultaneously. [given, A1, F1, F3, step 1.1]

2.2 Fix $c\in A$, let $p=F(c)$, and orient the selected segment from $p$ to $c$ toward the future. For any point $r$ on it, restrictions give $p\le_Er\le_Ec$, including the endpoints by reflexivity. Since $p\in\partial_E I_E^-(C)$ and $I_E^-(C)$ is open, $p\notin I_E^-(C)$. If $r\in I_E^-(C)$, there would be $c'\in C$ with $r\ll_Ec'$, and push-up would give $p\ll_Ec'$, a contradiction. Thus every such $r$ is outside $I_E^-(C)$. [given, A1, F2, F3, F4, step 1.1]

3.1 For each such $r$, [F1] gives a smooth geodesic $\eta$ in $E$ with $\eta(0)=r$ and $\dot\eta(0)=-N_r$. At zero, $g(\dot\eta,\dot\eta)<0$ and $g(\dot\eta,N)>0$. By continuity, both strict inequalities persist on a sufficiently short interval $[0,\delta]$ in its domain, so its tangent is past timelike there. For $0<\varepsilon<\delta$, set $r_\varepsilon=\eta(\varepsilon)$. Reversing the short segment gives a smooth future timelike curve from $r_\varepsilon$ to $r$, admitted by [F4], so $r_\varepsilon\ll_Er$. Push-up with $r\le_Ec$ gives $r_\varepsilon\ll_Ec$, also when $r=c$. Since $r_\varepsilon\to r$, this proves $r\in\overline{I_E^-(C)}^{\,E}$. Together with step 2.2 and openness, it gives $r\in\partial_E I_E^-(C)$. Thus the entire selected segment lies on the boundary, using neither global hyperbolicity nor compactness of $C$. [A1, F1, F2, F3, F4, step 2.2]

4.1 If the stipulated universal boundary-segment focal-exclusion input is assumed, apply it to each selected segment, whose boundary containment was proved in step 3.1. It excludes every interior focal point to $C$ on that segment. Together with steps 1.1 and 2.1 this establishes all assertions. [given, F3, step 1.1, step 2.1, step 3.1] ∎
