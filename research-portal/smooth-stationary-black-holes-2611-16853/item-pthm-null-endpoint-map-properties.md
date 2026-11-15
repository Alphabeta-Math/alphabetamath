---
title: Closed generator set and nonintersection before the cut
status: published
research_item: pthm-null-endpoint-map-properties
dependency_level: 27
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p.25, paragraph following Lemma 4.3
      attribution: The selected initial set A is closed, every cut point is reached
        without an interior focal point, and distinct generators do not
        intersect before the cut though endpoints may coincide; F is the
        endpoint map used next.
      hypotheses: The Section4 regular positive-parameter stationary vacuum Harrison
        construction and localized compact cut.
      reading_limits: Historical reading note retained from the current source; this
        maintenance revision claims no fresh article or external full-text
        reading. Consulted the frozen extracted article text at PDF p. 25, Lemma
        4.3 and the following paragraph. Attribution only; neither the PDF
        images nor the surrounding proof were independently verified in this
        assignment. The continuous-dependence sentence is not an
        endpoint-compactness premise.
    - title: E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22
        (2019), article 3
      url: https://s3.cern.ch/inspire-prod-files-7/7a575d682fd15aaad8463a778fac1609
      locator: Theorem 2.22 and its proof, PDF pp. 35–36 of 202; ambient regularity
        convention, PDF p. 3
      statement: If a continuous causal curve connects distinct points p and q and
        there is no timelike curve from p to q, then the given curve is an
        achronal lightlike geodesic up to reparametrization.
      hypotheses: A time-oriented spacetime in the source smooth causal setting and a
        continuous causal curve with distinct endpoints; no global
        hyperbolicity, target acausality or affine completeness is required. The
        present spacetime and curves are smooth or finitely piecewise smooth.
      reading_limits: Consulted Theorem 2.22 and its full printed proof on PDF pp.
        35–36 through the browser PDF text, and the C2-metric convention on p.
        3. Imported only the no-timelike-connection rigidity clause. The
        convex-normal-neighborhood inputs in its proof were not reconstructed or
        independently reviewed.
---

PDF p. 25: ` Paragraph after Lemma 4.3 `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)
- [pthm-past-boundary-localization](item-pthm-past-boundary-localization)
- [pthm-past-boundary-null-generators](item-pthm-past-boundary-null-generators)
- [pthm-transformed-cauchy-sections](item-pthm-transformed-cauchy-sections)
- [pthm-adm-temporality](item-pthm-adm-temporality)
- [pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates)
- [lem-author-2632702918ef-target-interior-focal-exclusion](item-lem-author-2632702918ef-target-interior-focal-exclusion)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-b18e87444145-temporal-normalized-null-flow](item-lem-author-b18e87444145-temporal-normalized-null-flow)
- [lem-author-b18e87444145-compact-diamond-closed-hit-domain](item-lem-author-b18e87444145-compact-diamond-closed-hit-domain)
- [lem-author-b18e87444145-transverse-null-hit-extensions](item-lem-author-b18e87444145-transverse-null-hit-extensions)
- [lem-author-b18e87444145-cut-generator-coverage-and-boundary](item-lem-author-b18e87444145-cut-generator-coverage-and-boundary)
- [lem-author-b18e87444145-boundary-generators-do-not-cross](item-lem-author-b18e87444145-boundary-generators-do-not-cross)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [def-stationary-section-time](item-def-stationary-section-time)
- [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)
- [math:cor-euclidean-closed-balls-and-spheres-are-compact](https://alphabetamath.cc/item/cor-euclidean-closed-balls-and-spheres-are-compact)
- [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)
- [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)
- [pthm-harrison-component-asymptotics](item-pthm-harrison-component-asymptotics)
- [pthm-harrison-denominator-asymptotics](item-pthm-harrison-denominator-asymptotics)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:thm-logarithm-derivative-and-integral](https://alphabetamath.cc/item/thm-logarithm-derivative-and-integral)
- [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)
- [` E. Minguzzi, Lorentzian causality theory, Living Reviews in Relativity 22 (2019), article 3 · Theorem 2.22 and its proof, PDF pp. 35–36 of 202; ambient regularity convention, PDF p. 3 `](https://s3.cern.ch/inspire-prod-files-7/7a575d682fd15aaad8463a778fac1609)


## Statement

In the standing regular mass-one stationary vacuum Harrison construction, with original maximal outer section, $T|_S\not\equiv0$, and fixed sufficiently small positive $q$, choose $t$ sufficiently large for the past-boundary localization result and for $\min_{C_t}v_q>0$. Let the compact cut $D\subset\Sigma^\circ=\{v_q=0\}$ and comparison sphere $C_t$ be those of the near-horizon past-boundary definition, and let $L_{q,t}$ be the normalized future outward null normal supplied by the coordinate-null-normal result. For each $c\in C_t$, take the unique maximal affinely parametrized geodesic $\gamma_c:I_c\to\mathcal E$ for $g_q$ with $\gamma_c(0)=c$ and $\dot\gamma_c(0)=-L_{q,t}(c)$, and use its portion with parameter $s\in I_c\cap[0,\infty)$ as the selected past ray. This specifies the maximal-family instance of that definition. Put $A=\{c\in C_t:\gamma_c(s)\in D\text{ for some }s\in I_c\cap[0,\infty)\}$ and let $F:A\to D$ send each initial point to that unique hit. Every point of $D$ is reached by a selected past generator without an interior focal point. The set $A$ is closed, hence compact and Borel. The map $F$ is surjective, continuous and has local smooth extensions into the smooth section, hence countably many Lipschitz pieces and the measurable Jacobian and multiplicity data needed for the ensuing area comparison. For distinct initial points $c,c'\in A$, their selected segments from $C_t$ to $D$ are disjoint away from $D$, although they may meet at $D$. In particular, distinct maximal unparametrized generators do not intersect strictly between $C_t$ and $D$. No multiplicity-one conclusion for $F$ is asserted.

## Statement references

[def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets)

[pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates)

[physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[def-stationary-section-time](item-def-stationary-section-time)

[def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)

## Facts & Assumptions

[F1] Use the exact interface and hypotheses of [post-stationary-vacuum-model](item-post-stationary-vacuum-model).

[F2] Use the exact interface and hypotheses of [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime).

[F3] Use the exact interface and hypotheses of [def-harrison-normalization](item-def-harrison-normalization).

[F4] Use the exact interface and hypotheses of [def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets).

[F5] Use the exact interface and hypotheses of [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data).

[F6] Use the exact interface and hypotheses of [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data).

[F7] Use the exact interface and hypotheses of [pthm-past-boundary-localization](item-pthm-past-boundary-localization).

[F8] Use the exact interface and hypotheses of [pthm-past-boundary-null-generators](item-pthm-past-boundary-null-generators).

[F9] Use the exact interface and hypotheses of [pthm-transformed-cauchy-sections](item-pthm-transformed-cauchy-sections).

[F10] Use the exact interface and hypotheses of [pthm-adm-temporality](item-pthm-adm-temporality).

[F11] Use the exact interface and hypotheses of [pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates).

[F12] Use the exact interface and hypotheses of [lem-author-2632702918ef-target-interior-focal-exclusion](item-lem-author-2632702918ef-target-interior-focal-exclusion).

[F13] Use the exact interface and hypotheses of [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice).

[F14] Use the exact interface and hypotheses of [lem-author-b18e87444145-temporal-normalized-null-flow](item-lem-author-b18e87444145-temporal-normalized-null-flow).

[F15] Use the exact interface and hypotheses of [lem-author-b18e87444145-compact-diamond-closed-hit-domain](item-lem-author-b18e87444145-compact-diamond-closed-hit-domain).

[F16] Use the exact interface and hypotheses of [lem-author-b18e87444145-transverse-null-hit-extensions](item-lem-author-b18e87444145-transverse-null-hit-extensions).

[F17] Use the exact interface and hypotheses of [lem-author-b18e87444145-cut-generator-coverage-and-boundary](item-lem-author-b18e87444145-cut-generator-coverage-and-boundary).

[F18] Use the exact interface and hypotheses of [lem-author-b18e87444145-boundary-generators-do-not-cross](item-lem-author-b18e87444145-boundary-generators-do-not-cross).

[F19] Import only the causal-curve rigidity clause of Minguzzi Theorem 2.22, specified under External input below.

[F20] A prescribed position and tangent determine a unique maximal geodesic on an open interval containing zero; any geodesic with those initial data is its restriction, including any supplied finite segment. Affine reversal and nonzero constant rescaling have the stated maximal-domain identities. Apply clauses (a) and (c) with $M=\mathcal E$ and its metric-selected connection. The inherited countable-choice hypothesis follows from [F13]: restrict a full choice function to any countable family. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F21] The smooth section time is $v_q(\tau,x)=\tau-u_q(x)$ on the product exterior, and the stationary flow is $\phi_t^T(\tau,x)=(\tau+t,x)$; in particular $Tv_q=1$ and $v_q(\phi_t^T(c))=t+v_q(c)$. [def-stationary-section-time](item-def-stationary-section-time)

[F22] For fixed positive $q$, the comparison sphere in the supplied original end chart is $C_0=\{\tau=0,|x|=R\}$, where $R=R_0q^{-2/3}>a>0$, and $C_t=\phi_t^T(C_0)=\{\tau=t,|x|=R\}$. [def-coordinate-comparison-spheres](item-def-coordinate-comparison-spheres)

[F23] Every Euclidean sphere in $\mathbb R^n$, $n\ge1$, with positive radius is compact. [math:cor-euclidean-closed-balls-and-spheres-are-compact](https://alphabetamath.cc/item/cor-euclidean-closed-balls-and-spheres-are-compact)

[F24] A continuous real-valued function on a nonempty compact metric space has a finite attained minimum and maximum. [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)

[F25] On a smooth time-oriented Lorentzian four-manifold, its metric-selected connection is metric-compatible: $X(g(Y,Z))=g(\nabla_XY,Z)+g(Y,\nabla_XZ)$. The supplier's intrinsic construction establishes existence and uniqueness of this connection. Apply this to $(\mathcal E,g_q)$; its inherited countable-choice convention is supplied by [F13]. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F26] Use the uniform differentiated component estimates for the very same specified Harrison family already required by [F11], including its mass-one end, supplied original maximal section, pole and spatial-decay hypothesis $(W_0)_i=O_5(r^{-3})$ in the same original chart. With $a=q+r^{-1}$ and $d=d_q$, they give $g_{00}=-d^2/(16a^2)+a^{-4}O_5(q^2r^{-1}+qr^{-2}+r^{-3})$, $g_{0i}=d a^{-1}O_5(r^{-2})$, and $g_{ij}=a^2\delta_{ij}+O_5(q^2r^{-1}+qr^{-2}+r^{-3})$. The denominator supplier gives $0<d_*\le d_q\le d^*<\infty$ uniformly in $q$. The radial case and the supplied decaying-primitive alternative are both allowed by those estimates. The bound is required for the same primitive defining the metric; no identification with the exact radial integral is made. [pthm-harrison-component-asymptotics](item-pthm-harrison-component-asymptotics) [pthm-harrison-denominator-asymptotics](item-pthm-harrison-denominator-asymptotics)

[F27] The chain rule applies to totally differentiable maps between Euclidean open sets. The real logarithm has derivative $1/u$ for $u>0$. The mean value theorem applies to real functions continuous on a compact interval and differentiable in its interior; in particular a nonnegative derivative implies monotonicity and a zero derivative implies constancy. All functions used below are smooth on their open coordinate domains and restricted to finite closed parameter intervals. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) [math:thm-logarithm-derivative-and-integral](https://alphabetamath.cc/item/thm-logarithm-derivative-and-integral) [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

## Proof

**Given:**The hypotheses in the Statement.

**Goal:** Establish the asserted conclusions.

1.1 In the original stationary end chart, [F22] identifies $C_0$ with the Euclidean sphere $|x|=R$ in $\mathbb R^3$, where $R=R_0q^{-2/3}>a>0$. Give $C_0$ the metric $d_0(c,c')=|x(c)-x(c')|$; the chart identifies this metric topology with its manifold subspace topology. This metric space is compact by [F23] and nonempty, since the coordinate point $x=(R,0,0)$ lies on it. The smooth function $v_q$ is continuous on $C_0$, so [F24] gives the finite attained minimum $m=\min_{C_0}v_q$. The stationary translation in [F21] gives $v_q(\phi_t^T(c))=t+v_q(c)$ and hence $\min_{C_t}v_q=t+m$. Choose $t$ beyond the localization threshold in [F7] and with $t>-m$. Localization and the strict time ordering therefore hold simultaneously for every sufficiently late $t$, without any additional geometric assumption. [given, F7, F21, F22, F23, F24, algebra]

1.2 We first rule out two target initial points on one oriented maximal generator by a local end calculation. Follow the future outward affine geodesic from any $c\in C_t$, writing its affine parameter as $s=0$ at $c$, and put $p_\mu=g_{\mu\nu}\dot x^\nu$ in the stationary Cartesian chart $(\tau,x)$. The geodesic equation and the Christoffel formula supplied by [F25], after differentiating this pairing, give $\dot p_\mu=\tfrac12(\partial_\mu g_{\alpha\beta})\dot x^\alpha\dot x^\beta$. Stationarity therefore gives $p_\tau=-E=-d/4$ throughout any end portion, by the normal normalization in [F11]. Differentiating the inverse-matrix identity then gives the equivalent equations $\dot x^i=\partial_{p_i}H$ and $\dot p_i=-\partial_{x^i}H$ for $H=\tfrac12g^{\mu\nu}p_\mu p_\nu=0$, with $p_\tau=-E$ held fixed. Write $p=(p_1,p_2,p_3)$, with Euclidean norm $|p|$. Since $q^2r^{-1}+qr^{-2}+r^{-3}\le a^2/r$, [F26] gives, after scaling the time basis vector by $4a/d$ and spatial basis vectors by $a^{-1}$, a metric matrix $\eta+O(r^{-1})$, where $\eta=\operatorname{diag}(-1,1,1,1)$. Its inverse is also $\eta+O(r^{-1})$: write its inverse difference as $-(\eta+e)^{-1}e\eta$ for the error matrix $e$. A spatial rotation differentiates $e$ to $O(r^{-1})$ by the differentiated estimates; differentiating the inverse identity preserves that bound. Thus, at fixed $p_\tau=-d/4$, $H=H_0+\mathcal R$, where $H_0=\tfrac12(-a^2+a^{-2}|p|^2)$ and $|\mathcal R|\le Cr^{-1}(a^2+a^{-2}|p|^2)$. The quadratic coefficients also give $|\partial_p\mathcal R|\le Cr^{-1}(1+a^{-2}|p|)$. For $i<j$, define $\mathcal Q_{ij}=x^i\partial_{x^j}-x^j\partial_{x^i}+p_i\partial_{p_j}-p_j\partial_{p_i}$. The same rotation bounds give $|\mathcal Q_{ij}\mathcal R|\le Cr^{-1}(a^2+a^{-2}|p|^2)$. All constants here are independent of $q$, angle and sufficiently large $r$. [F11, F25, F26, F27, algebra]

2.1 Localization supplies compact $D\subset\Sigma^\circ\cap\partial_{\mathcal E}I^-_{g_q}(C_t)$ inside the cylinder at level $v_q=0$; step 1.1 gives $0<\min_{C_t}v_q$. The completed Cauchy and temporality suppliers give a smooth globally hyperbolic $(\mathcal E,g_q)$ and temporal $v_q$. The normalized outward initial null vector $L_{q,t}$ depends smoothly on $c\in C_t$ by its explicit smooth branch and nonzero normalization. Apply [F20] in $\mathcal E$ to these initial data. Differentiating in a coordinate chart and using the metric compatibility in [F25] gives $\frac{d}{ds}g_q(\dot\gamma_c,\dot\gamma_c)=2g_q(D_s\dot\gamma_c,\dot\gamma_c)=0$; uniqueness excludes a zero tangent on this nonconstant geodesic, so it remains past null. The chosen family is therefore maximal in the exterior, exactly as required by the endpoint lemmas; a truncated supplied curve would only be a restriction and is not the family defining $A$ here. Thus every hypothesis of the normalized-null-flow and compact-diamond lemmas is met, relative to the exterior. They give unique hits and closed $A$. Their compactness argument keeps the lifted rays over $J^+(D)\cap J^-(C_t)$ and normalizes $dv_q(w)=1$; it never assumes affine completeness or an unproved uniform affine parameter bound. [given, F4, F5, F7, F9, F10, F11, F13, F14, F15, F20, F25, step 1.1]

2.2 Put $p_r=r^{-1}\sum_i x^ip_i$, $\ell_{ij}=x^ip_j-x^jp_i$ for $i<j$, and $J=(\sum_{i<j}\ell_{ij}^2)^{1/2}$. The algebraic identity $|p|^2=p_r^2+J^2/r^2$ follows by expanding both sides. Nullity and step 1.2 imply $|p|^2/a^4=1+O(r^{-1})$ by absorbing the error in $-a^2+a^{-2}|p|^2=O(r^{-1})(a^2+a^{-2}|p|^2)$. The Hamilton equations give $\dot r=a^{-2}p_r+O(r^{-1})$. They also give $\dot\ell_{ij}=-\mathcal Q_{ij}H=-\mathcal Q_{ij}\mathcal R$, since the simultaneous rotation fixes $r$ and $|p|^2$, and hence $|\dot\ell_{ij}|\le Ka^2/r$. Initially [F11] gives $p=(L_q)_r x/r$ with $(L_q)_r=a^2(1+O(R^{-1}))>0$, so $J(0)=0$ and $p_r(0)>0$, where $R=R_0q^{-2/3}$. On any exterior interval with $J/(a^2r)\le1/2$, continuity keeps $p_r$ on its positive branch: for a common sufficiently large radius, $p_r^2/a^4=1+O(r^{-1})-J^2/(a^4r^2)\ge2/3$. Consequently $\dot r\ge1/2$ on that interval. This uses only finite portions of the existing geodesic. [F11, F26, F27, step 1.2, algebra]

3.1 Apply the transverse-hit lemma to obtain local smooth endpoint extensions, continuity, compact/Borel domain and countably many chart-Lipschitz pieces. This is the precise regularity needed by the endpoint-area interface, even if $D$ is nonsmooth or the derivative loses rank at a focal endpoint. The Jacobian is the nonnegative Gram two-Jacobian, and coincident endpoints are counted with their actual multiplicities. No image-smoothness or almost-everywhere injectivity is inferred from compactness. [F6, F16, step 2.1]

3.2 For every $p\in D$, the completed past-boundary generator theorem gives a future null segment to $C_t$ ending on the prescribed normalized outward ray and without an interior focal point. Reverse and positively affinely rescale that segment to give initial tangent $-L_{q,t}(c)$. By [F20] it is a restriction of the chosen maximal $\gamma_c$, including its endpoint in $D$; hence $c\in A$ and $F(c)=p$, proving $F(A)=D$. Conversely any selected segment from a hit in $D$ to $C_t$ stays on the past boundary by the cut-coverage lemma; the completed universal boundary focal-exclusion supplier rules out any interior focal point on it. [F4, F8, F12, F17, F20, step 2.1]

3.3 For $r\ge R$, define $B_q(r)=q^2\log(r/R)+2q(R^{-1}-r^{-1})+\tfrac12(R^{-2}-r^{-2})$. Then $B_q(R)=0$, $B_q\ge0$, and $B_q'(r)=a^2/r$, by [F27]. While the bound in step 2.2 holds, $dB_q(r(s))/ds\ge a^2/(2r)$. Therefore the derivatives of $2KB_q(r(s))\pm\ell_{ij}(s)$ are nonnegative, and the mean value theorem gives $|\ell_{ij}(s)|\le2KB_q(r(s))$. In particular $J\le2\sqrt3 K B_q$. Since $a^2r=q^2r+2q+r^{-1}\ge4q$ and also $a^2r\ge q^2r$, the estimate $\log z\le z$ for $z\ge1$ gives $B_q(r)/(a^2r)\le3/(2R)+1/(8qR^2)$. The logarithmic estimate itself follows by differentiating $z-\log z$ and using [F27]. Hence $J/(a^2r)\le C(R^{-1}+(qR^2)^{-1})=C(q^{2/3}/R_0+q^{1/3}/R_0^2)$. Choose the already sufficiently small positive $q$ so that this bound is less than $1/4$, and $R$ exceeds the preceding common end thresholds. This choice is independent of $t$. Starting with $J=0$, a first failure of $J/(a^2r)<1/2$ on any finite exterior segment is impossible, because the improved bound is less than $1/4$ and the fields are continuous. Thus $\dot r\ge1/2$ persists. The ray cannot return to $r=R$: before any putative first return it stays in this exterior chart with strictly increasing $r$. No assertion of affine completeness or continuation to infinite affine parameter is used. In particular an outward ray through one point of $C_t$ cannot later pass through another point of $C_t$. [F22, F26, F27, step 2.2, algebra]

4.1 Apply the independent causal-curve rigidity input [F19] to the smooth time-oriented exterior. As in the noncrossing lemma [F18], a meeting with nonparallel future tangents at a point interior to both boundary segments would produce a causal corner from $D$ to $C_t$, contradicting rigidity and boundary membership from step 3.2. A proportional-tangent meeting identifies the oriented maximal geodesics by [F20]. Their distinct initial points on $C_t$ would then be ordered along that geodesic by temporal $v_q$; the earlier one's future outward continuation reaches the later one, contrary to step 3.3. If a common point outside $D$ is the $C_t$ endpoint of just one selected segment and interior to the other, concatenate the first segment's past leg from $D$ with the other's future leg to its target in $C_t$. Rigidity again forces matching tangent directions there, so the same uniqueness and no-return argument excludes this case. A point in $D$ cannot be interior to either segment because $v_q$ strictly increases from zero to its positive target value. Thus selected segments from distinct initial points are disjoint away from $D$, covering the full stated nonintersection claim. Meetings at $D$ remain possible; the area interface retains their actual multiplicities. [F6, F10, F17, F18, F19, F20, step 3.2, step 3.3] ∎

## External input

Import the exact rigidity implication of Minguzzi Theorem 2.22 (PDF pp.35–36): for a continuous causal curve between distinct endpoints, absence of a timelike connecting curve forces that very curve to be an achronal null geodesic up to parametrization. The application is to a finite concatenation of smooth null segments in the smooth time-oriented exterior. This independent input supplies the hypothesis of the fifth local lemma; the five local prerequisites supply endpoint compactness, smooth hitting regularity, coverage and the application. No source result establishing closedness of $A$, no affine completeness and no global acausality of $C_t$ is imported.

## Source notes

The original paragraph attributes the claims. Closedness here follows from compact causal diamonds and the temporal-normalized geodesic flow, not continuous dependence alone. The local end calculation also rules out a second comparison-cylinder visit by an outward normal ray, closing the same-generator loophole without assuming global acausality of $C_t$. It uses the exact component-estimate hypotheses already inherited through the specified coordinate-null-normal construction. All original nonintersection and endpoint claims are retained, with endpoint multiplicity allowed. This is an authoring proposal, not independent proof review or mathematical acceptance.
