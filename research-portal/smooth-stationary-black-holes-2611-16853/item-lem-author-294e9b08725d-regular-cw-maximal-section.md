---
title: Maximal bifurcation-boundary section under the original regular hypotheses
status: published
research_item: lem-author-294e9b08725d-regular-cw-maximal-section
dependency_level: 16
sources:
  references:
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609
      locator: Section 3.2, Definition 3.29, Remark 3.31, Proposition 3.33 (3.8), and
        Corollary 3.34, printed/PDF pp. 93–95.
      statement: For closed achronal A in a spacetime W, the timelike domain is W iff
        the causal domain is W; continuous causal curves give the same causal
        domain.
      hypotheses: A closed achronal subset of a time-oriented smooth Lorentzian
        spacetime; all curves and domains are relative to that spacetime.
      reading_limits: Read the listed PDF-text passages and Corollary 3.34 argument;
        imported only this equivalence and continuous-curve convention. No full
        proof review. Screenshots unavailable. The parameter interface and
        application are local.
---

## Prerequisites

- [lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing](item-lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing)
- [lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice)
- [lem-author-294e9b08725d-band-domain-of-dependence-is-exterior](item-lem-author-294e9b08725d-band-domain-of-dependence-is-exterior)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [lem-author-9e5789a3d617-end-holder-interface](item-lem-author-9e5789a3d617-end-holder-interface)
- [thm-stationary-maximal-slice-existence-input](item-thm-stationary-maximal-slice-existence-input)
- [lem-author-a4a441da4986-cauchy-closure-double-boundary](item-lem-author-a4a441da4986-cauchy-closure-double-boundary)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [physics:lem-gr-maximal-geodesics-and-extension](https://alphabetamath.cc/physics/item/lem-gr-maximal-geodesics-and-extension)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions)
- [physics:lem-gr-causal-curve-conventions](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-conventions)
- [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)
- [` E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22 (2019), article 3 · Section 3.2, Definition 3.29, Remark 3.31, Proposition 3.33 (3.8), and Corollary 3.34, printed/PDF pp. 93–95. `](https://inspirehep.net/files/7a575d682fd15aaad8463a778fac1609)


## Statement

Under the article regular stationary-vacuum hypotheses, there is a smooth spacelike maximal section $\Sigma_{\max}\subset E$ whose closure has boundary $S$ and whose interior is Cauchy in $E$. It lies in an exterior-preserving smooth stationary vacuum strongly causal ambient spacetime with complete stationary flow. Its stationary translates foliate $E$. On its original end it is a CW asymptotically flat graph: at falloff exponent one, its height and differentiated weighted bounds allow logarithmic growth. No stronger normalized end-gauge estimate is asserted in this lemma.

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[F1] The glued ambient is smooth, strongly causal, vacuum and has complete stationary field with connected closed acausal section $C_0\cup S$. [lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing](item-lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing) [lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice)

[F2] The band-domain lemma establishes $\operatorname{int}D^{\mathrm{tim}}_{M_*}(C_0\cup S)=E$ for the CW convention in which every inextendible timelike curve through a point must meet the section; it also supplies the required chronological end exclusion. Its separate causal-curve conclusion is not substituted for this source convention. The adopted general Cauchy-closure interface confines any further original-ambient closure points of an exterior Cauchy section to the double boundary $S$. [lem-author-294e9b08725d-band-domain-of-dependence-is-exterior](item-lem-author-294e9b08725d-band-domain-of-dependence-is-exterior) [lem-author-a4a441da4986-cauchy-closure-double-boundary](item-lem-author-a4a441da4986-cauchy-closure-double-boundary)

[F3] The original O6 end supplies the CW differentiated Hölder interface, and the existing exact CW existence input gives maximal boundary sections. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) [lem-author-9e5789a3d617-end-holder-interface](item-lem-author-9e5789a3d617-end-holder-interface) [thm-stationary-maximal-slice-existence-input](item-thm-stationary-maximal-slice-existence-input)

[F4] For a closed achronal subset $A$ of a spacetime $W$, $D^{\mathrm{tim}}_W(A)=W$ if and only if $D^{\mathrm{caus}}_W(A)=W$. The causal domain may equivalently be tested with continuous causal curves; see External input.

[F5] Every causal curve in the declared locally absolutely continuous convention is a geodesically connectible continuous causal curve. A smooth function with past timelike gradient strictly increases along every future causal curve in its domain. Push-up gives $r\ll z\le q\Rightarrow r\ll q$. [physics:lem-gr-causal-curve-conventions](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-conventions) [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions) [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[F6] Maximal timelike geodesics through a specified point are inextendible in the no-endpoint-limit convention, and chronological futures and pasts are open. Smooth embedded hypersurfaces admit local slice coordinates. [physics:lem-gr-maximal-geodesics-and-extension](https://alphabetamath.cc/physics/item/lem-gr-maximal-geodesics-and-extension) [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness) [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

[A1] Retain the ZFC convention of the regular data. It supplies Countable Choice and Dependent Choice for the causal suppliers in F5 and F6. These are mathematical suppliers. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

## Proof

**Given:**The data and hypotheses of the Statement.

**Goal:** The asserted conclusion with its stated scope.

[F1] The glued ambient is smooth, strongly causal, vacuum and has complete stationary field with connected closed acausal section $C_0\cup S$. [lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing](item-lem-author-294e9b08725d-hausdorff-causal-stationary-collar-gluing) [lem-author-294e9b08725d-canonical-outer-cauchy-splice](item-lem-author-294e9b08725d-canonical-outer-cauchy-splice)

[F2] The band-domain lemma establishes $\operatorname{int}D^{\mathrm{tim}}_{M_*}(C_0\cup S)=E$ for the CW convention in which every inextendible timelike curve through a point must meet the section; it also supplies the required chronological end exclusion. Its separate causal-curve conclusion is not substituted for this source convention. The adopted general Cauchy-closure interface confines any further original-ambient closure points of an exterior Cauchy section to the double boundary $S$. [lem-author-294e9b08725d-band-domain-of-dependence-is-exterior](item-lem-author-294e9b08725d-band-domain-of-dependence-is-exterior) [lem-author-a4a441da4986-cauchy-closure-double-boundary](item-lem-author-a4a441da4986-cauchy-closure-double-boundary)

[F3] The original O6 end supplies the CW differentiated Hölder interface, and the existing exact CW existence input gives maximal boundary sections. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) [lem-author-9e5789a3d617-end-holder-interface](item-lem-author-9e5789a3d617-end-holder-interface) [thm-stationary-maximal-slice-existence-input](item-thm-stationary-maximal-slice-existence-input)



1.1 The section has one Euclidean end and a compact interior with boundary $S$, and its data agree with the original stationary end. The stationary field is tangent to $S$ and equals $\partial_t$ in the end. Use order five and any fixed Hölder exponent in $(0,1)$: the sixth differentiated end bounds imply the required order-five weighted Hölder bounds. Together with the ambient construction and the identified domain of dependence, every class-(b) and exclusion hypothesis of the existing CW input is supplied. In the source convention, $U=\operatorname{int}D^{\mathrm{tim}}_{M_*}(C_0\cup S)$, with all inextendible timelike curves taken in the glued ambient. The timelike-curve conclusion in F2 gives exactly $U=E$ and $(B\cup W)\cap U=\varnothing$. This checks the source exclusion for its own domain, without assuming that a causal-curve domain and a timelike-curve domain coincide in general. [F1, F2, F3, algebra]

2.1 Apply the existence input with the hypotheses checked in step 1.1. It gives smooth maximal sections $\widehat\Sigma_s$ with fixed boundary $S$, interiors $C_s$ covering $E$ and Cauchy there in the source convention, and the stated end graph bounds. For the Cauchy assertion use only the source conclusion that $C_s$ is achronal and every inextendible timelike curve in $E$ meets it exactly once. Vacuum gives zero Ricci tensor, hence the timelike-convergence condition and the stationary foliation conclusion. This invokes the nonlinear existence theorem as an external prerequisite and does not reconstruct it or infer stronger end gauge from its logarithmic graph estimate. [F1, F2, F3, step 1.1, algebra]

3.1 Fix $s$. The hypersurface $C_s$ is closed in $E$: if $p\in\overline{C_s}^{\,E}\setminus C_s$, a maximal timelike geodesic through $p$, taken in $E$, meets $C_s$ at a point $q\ne p$ by the source Cauchy conclusion. Thus $q\ll_E p$ or $p\ll_E q$. The corresponding open chronological neighborhood of $p$ meets $C_s$ at another point, contradicting achronality. Moreover $D^{\mathrm{tim}}_E(C_s)=E$ by that same source conclusion. Apply F4 with $W=E$ and $A=C_s$, obtaining $D^{\mathrm{caus}}_E(C_s)=E$. By the continuous-curve interface in F5, every inextendible locally absolutely continuous causal curve in $E$ is among the continuous causal curves tested by this imported conclusion: its image is unchanged and its ends still have no point limit in $E$. Consequently every declared causal curve meets $C_s$. [A1, F4, F5, F6, step 2.1]

4.1 The intersection counts exactly one parameter value. Indeed, near any $p\in C_s$ choose slice coordinates $(f,x)$ with $C_s=\{f=0\}$. Since $C_s$ is spacelike, the coordinates can be chosen with $\partial_f$ future timelike and $\nabla f$ past timelike at $p$, and both properties persist after shrinking to a product coordinate box. For a future causal curve $\gamma$ through $p$ at parameter $a$, temporal monotonicity in F5 gives $f(\gamma(t))>0$ on a short interval after $a$. A point $z=\gamma(t)$ on that interval is chronologically above some $r\in C_s$, using the coordinate fiber with $x$ fixed from $f=0$ to $f(z)>0$. If a later parameter $b>a$ also gave $q=\gamma(b)\in C_s$, choose $a<t<b$ in that interval. Push-up gives $r\ll_E z\le_E q$, hence $r\ll_E q$, contradicting achronality when $r\ne q$ and strong causality when $r=q$. Thus two distinct parameter visits are impossible. Together with step 3.1, this establishes the declared causal Cauchy condition. [A1, F1, F5, F6, step 2.1, step 3.1]

5.1 The local right germ at $S$ is shared with the original spacetime. Now that $C_s$ is Cauchy in the declared sense, the general Cauchy-closure interface applies in the original geometry and excludes further original-ambient accumulation points away from the double boundary $S$. The fixed smooth boundary supplied in step 2.1 already includes all of $S$, so the closure boundary is exactly $S$. All maximality, stationary covariance, foliation and end bounds from step 2.1 are retained. [F1, F2, step 2.1, step 4.1] ∎

## External input

Import Minguzzi's Corollary 3.34 and Remark 3.31: F4's equivalence and continuous-curve convention, requiring closedness and achronality. Apply them with $W=E$ and $A=C_s$.
