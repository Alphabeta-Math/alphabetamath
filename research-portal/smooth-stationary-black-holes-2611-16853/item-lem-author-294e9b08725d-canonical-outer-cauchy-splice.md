---
title: Canonical bifurcation collar joined to the original exterior Cauchy section
status: published
research_item: lem-author-294e9b08725d-canonical-outer-cauchy-splice
dependency_level: 9
sources:
  references:
    - title: Alexandru F. Radu, On rigidity of stationary black holes under a
        nontrapping assumption
      url: https://arxiv.org/pdf/2609.23872v2
      locator: Section 2.2, Lemma 2.2 proof, printed pp. 10–12, equation (2.4) and
        logarithmic cutoff; nonrotating extension, pp. 13–14, equation (2.5);
        GR/SBS, pp. 3–4.
      statement: The chart is exp_p(((V-U)e_0+(V+U)e_1)/2), with orthonormal
        future/outward normals and exterior U,V>0. For a fixed sufficiently
        small outer tubular radius r_2, the logarithmic cutoff becomes temporal
        by choosing r_1 sufficiently small; the perturbation estimate is uniform
        under scaling in [0,1].
      hypotheses: GR and SBS, as matched by the existing local-boost supplier; a
        Cauchy temporal tau_0 vanishing on the working section and the local
        normal time tau_1. The cited construction uses no NT conclusion.
      reading_limits: Read GR/SBS, equation (2.4), the cutoff calculation through its
        acausality conclusion, and the nonrotating specialization. Only these
        coordinate/localization premises are imported; no independent proof
        review is claimed.
---

## Prerequisites

- [lem-author-294e9b08725d-regular-positive-stationary-mass](item-lem-author-294e9b08725d-regular-positive-stationary-mass)
- [lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar)
- [thm-author-294e9b08725d-radu-local-bifurcate-collar-input](item-thm-author-294e9b08725d-radu-local-bifurcate-collar-input)
- [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [physics:lem-gr-partial-cauchy-development](https://alphabetamath.cc/physics/item/lem-gr-partial-cauchy-development)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)
- [physics:lem-gr-maximal-geodesics-and-extension](https://alphabetamath.cc/physics/item/lem-gr-maximal-geodesics-and-extension)
- [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [physics:lem-gr-parallel-transport-and-geodesic-speed](https://alphabetamath.cc/physics/item/lem-gr-parallel-transport-and-geodesic-speed)
- [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)
- [math:thm-compactly-supported-vector-fields-are-complete](https://alphabetamath.cc/item/thm-compactly-supported-vector-fields-are-complete)
- [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)
- [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [math:cor-intermediate-value-theorem-topological](https://alphabetamath.cc/item/cor-intermediate-value-theorem-topological)
- [` Alexandru F. Radu, On rigidity of stationary black holes under a nontrapping assumption · Section 2.2, Lemma 2.2 proof, printed pp. 10–12, equation (2.4) and logarithmic cutoff; nonrotating extension, pp. 13–14, equation (2.5); GR/SBS, pp. 3–4. `](https://arxiv.org/pdf/2609.23872v2)


## Statement

Under the regular stationary-vacuum hypotheses, there is a smooth spacelike Cauchy section $C_0$ of $E$ whose closure $C_0\cup S$ is complete with compact boundary $S$, agrees with the original section on the stationary end, and equals the canonical section $U=V>0$ in a neighborhood of $S$ from the local boost input. It is obtained by changing the original working section in a compact neighborhood of $S$. The section need not be transverse to $T$ away from this collar.

## Facts & Assumptions

**Given:** The regular stationary-vacuum hypotheses, in the stated ZFC convention.

**Goal:** Construct the stated canonical exterior Cauchy section without changing its stationary end.

[F1] Write $W=M\prime$ and $A=\Sigma\prime$ for the supplied working spacetime and section; thus $C=A\cap E$ is the original exterior Cauchy section. The section $A$ is closed in $W$, smooth, spacelike, acausal and edgeless (including closedness proved in the working-collar argument, Proof 3.1). Its two chronological end intersections are $C$. The working exterior and the local horizon germs are the original ones. All geometry is in the ZFC convention of the regular-spacetime definition. [lem-author-a4a441da4986-working-partial-cauchy-collar](item-lem-author-a4a441da4986-working-partial-cauchy-collar) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F2] Under the regular stationary-vacuum hypotheses, the positive-mass supplier gives $M_0=E_{\mathrm{ADM}}>0$ without maximality or axisymmetry. The working restriction leaves the stationary end unchanged, so this supplies the positive ADM mass required by source GR for both the local-boost input and the supplementary chart and cutoff construction. [lem-author-294e9b08725d-regular-positive-stationary-mass](item-lem-author-294e9b08725d-regular-positive-stationary-mass) The existing local-boost input applies to $A$ as the source section denoted $\Sigma_0$: it supplies a Cauchy temporal function $\tau_0$ with zero level $A$ on its domain of dependence and a temporal splice equal to $\tau_1=(V-U)/2$ near $S$. The independently checked normal-exponential formula and the freedom to fix the outer cutoff radius inside a smaller chart are recorded in External input. [thm-author-294e9b08725d-radu-local-bifurcate-collar-input](item-thm-author-294e9b08725d-radu-local-bifurcate-collar-input)

[F3] The original closure $C\cup S$ is the radial exterior with compact radial truncations, one Euclidean end and complete induced length metric with boundary included. [lem-author-a4a441da4986-exact-outer-cauchy-section](item-lem-author-a4a441da4986-exact-outer-cauchy-section)

[F4] For a closed acausal edgeless hypersurface, the causal domain of dependence is open and causally convex and the hypersurface is Cauchy there. Push-up composes a timelike segment with a causal segment in either order. Causal curves admit restriction, concatenation, increasing reparametrization and endpoint extension; maximal nonconstant timelike geodesics have no endpoint limit. A temporal function strictly increases on every future causal curve. Chronological futures and pasts are open, and a continuous real function on an interval attains every intermediate value. The declared choice hypotheses all follow from ZFC. [physics:lem-gr-partial-cauchy-development](https://alphabetamath.cc/physics/item/lem-gr-partial-cauchy-development) [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule) [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus) [physics:lem-gr-maximal-geodesics-and-extension](https://alphabetamath.cc/physics/item/lem-gr-maximal-geodesics-and-extension) [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions) [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness) [math:cor-intermediate-value-theorem-topological](https://alphabetamath.cc/item/cor-intermediate-value-theorem-topological)

[F5] The metric exponential has unique geodesics with prescribed initial data, and the squared speed and causal character of a nonconstant geodesic are constant. These apply to the normal-exponential rays in the independently checked chart. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map) [physics:lem-gr-parallel-transport-and-geodesic-speed](https://alphabetamath.cc/physics/item/lem-gr-parallel-transport-and-geodesic-speed)

[F6] Smooth vector fields have unique smooth local flows, and compactly supported smooth vector fields are complete under Countable Choice. The inverse function theorem gives local smooth level graphs when the differential is nonzero. A smooth positive metric has uniform positive lower and finite upper Euclidean comparison bounds on a compact set in a coordinate chart. [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows) [math:thm-compactly-supported-vector-fields-are-complete](https://alphabetamath.cc/item/thm-compactly-supported-vector-fields-are-complete) [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds) [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

## Proof

1.1 Use the causal domain $D=D_W(A)$, with the one-sided causal-domain convention of [F4]. It is open, contains $A$, is causally convex in $W$, and has $A$ as a Cauchy hypersurface. We first prove $E\subset D$. If $p\in E\setminus D$, there are a past-inextendible and a future-inextendible causal half-curve in $W$ through $p$, both avoiding $A$. Concatenate them at $p$. The maximal connected segment of this curve in the open set $E$ containing $p$ is inextendible in $E$: a limit in $E$ at an interior cut would permit continuation in $E$, and a limit at an original end would be a limit in $W$. But $C$ is Cauchy in $E$, so that segment meets $C\subset A$, a contradiction. Thus every relevant exterior point lies in the very domain on which the splice is defined. [F1, F4, construct, contradiction]

1.2 Choose a normal-coordinate box $O$ around compact $S$, with compact closure contained in $D$ and in the horizon neighborhood of [F1]. The verified formula in External input writes its points as $\exp_p(w)$, where $w=((V-U)e_0+(V+U)e_1)/2$, and fixes the right exterior as $U,V>0$. The two smooth null horizon sheets have germs $U=0$ and $V=0$. Indeed their null radical field $L$ satisfies $\nabla_LL\in\mathbb RL$: differentiating $g(L,Y)=0$ for tangent $Y$, and using metric compatibility and torsion-freeness, makes $\nabla_LL$ orthogonal to the entire null tangent hyperplane. Reparametrization therefore makes its integral curves geodesic. Uniqueness in [F5] identifies them with the corresponding null normal rays; their parametrizations cover the sheets near $S$. The future-sheet label $U=0$ is fixed by the source normalization, and the other sheet is $V=0$. [F1, F2, F5, algebra]

2.1 For clarity put $P=I^-_W(M^{\rm end})$ and $Q=I^+_W(M^{\rm end})$. Their boundaries in $O$ are respectively $U=0$ and $V=0$ by step 1.2. Each connected half-box on either side of such a sheet is wholly inside or wholly outside the corresponding open chronological set, since it contains no boundary point. The right wedge belongs to both sets, so $U>0$ lies in $P$ and $V>0$ lies in $Q$. The opposite half-box cannot also belong to $P$: a future timelike normal-coordinate segment from a point on $U=0$ enters $U<0$, and membership of that future point in the past set $P$ would put the boundary point itself in $P$. Similarly a past timelike segment from $V=0$ enters $V<0$ and excludes that half-box from the future set $Q$. The needed segment directions are $-\partial_U+\partial_V$, which are future timelike on a sufficiently small box by their value at $S$. Hence $P\cap O=\{U>0\}$ and $Q\cap O=\{V>0\}$. [F1, F2, F4, step 1.2, algebra]

2.2 Fix the cutoff outer radius inside $O$ before choosing its inner radius. By [F2] and External input, $\tau=\tau_0+\chi(\tau_1-\tau_0)$ is temporal and equals $\tau_0$ outside a fixed compact subset of $O$. Set $\tau_\lambda=\tau_0+\lambda\chi(\tau_1-\tau_0)$, $0\le\lambda\le1$. Its differential has a convex timelike part $(1-\lambda\chi)d\tau_0+\lambda\chi d\tau_1$ and error $\lambda(\tau_1-\tau_0)d\chi$; the same uniform cone margin and logarithmic error bound used for $\tau$ prove temporality for every $\lambda$. Each $\tau_\lambda-\tau_0$ is uniformly bounded. Since $\tau_0$ tends to the appropriate infinite limits on every inextendible causal curve in $D$, so does $\tau_\lambda$. Strict monotonicity and the intermediate value theorem make $H_\lambda=\tau_\lambda^{-1}(0)$ Cauchy and acausal in $D$; nonzero timelike differential and the inverse function theorem make it smooth and spacelike. All $H_\lambda$ contain $S$, $H_0=A$, and $H=H_1$ is $U=V$ near $S$. [F2, F4, F6, step 1.1, construct, algebra]

3.1 The zero levels form an actual compactly supported isotopy fixing $S$. Namely put $N_\lambda=\nabla\tau_\lambda/g(\nabla\tau_\lambda,\nabla\tau_\lambda)$ and $X_\lambda=-(\partial_\lambda\tau_\lambda)N_\lambda$. Then $\partial_\lambda\tau_\lambda+d\tau_\lambda(X_\lambda)=0$, and $X_\lambda$ has common compact support in $O$ and vanishes on $S$. Its time-dependent flow exists smoothly through $0\le\lambda\le1$: temporality persists for a slightly larger parameter interval by the uniform compact margin, and the suspension on that interval times $D$ can be cut off in parameter and space to be a compactly supported autonomous vector field. Take the spatial cutoff equal to one on a relatively compact neighborhood of the common support; trajectories starting there cannot exit through its stationary collar, so this suspension has parameter speed one along every moving trajectory. Completeness and uniqueness from [F6] supply the flow and its backward inverse. Thus its diffeomorphisms $F_\lambda$ satisfy $F_\lambda(A)=H_\lambda$, fix $S$, and are identity outside $O$. They extend by identity to the original ambient $M$. [F2, F6, step 2.2, construct, algebra]

4.1 The normal ray $s\mapsto\exp_p(sw)$ has squared speed $g_p(w,w)=UV$. By [F5] it is timelike when $UV<0$ and null when $UV=0$ with $(U,V)\ne(0,0)$. These rays stay in $O\subset D$; their endpoints are causally related to $p\in S$. Acausality of every $H_\lambda$ therefore excludes all such points. Consequently $H_\lambda\cap O\setminus S$ lies in the disjoint right and left wedges. An isotopy trajectory from $A\setminus S$ cannot switch wedge, since it never meets $S$ or either nonzero axis, and it cannot exit $O$ through the fixed collar of the support. Originally the outward component $C$ lies in the right wedge and the inner component lies in the left wedge wherever they meet the deformation region, by [F1] and step 2.1. It follows that $C_0=F_1(C)$ is the connected outward component, and that $H\cap P=H\cap Q=C_0$. Outside $O$ the same equalities are exactly the old ones of [F1]. In particular $H\cap E=C_0$. [F1, F3, F5, step 2.1, step 2.2, step 3.1, algebra]

5.1 Let $\gamma$ be inextendible causal in $E$. Extend it to an inextendible causal curve $\Gamma$ in $D$ as follows. An end with no limit in $D$ already needs no extension. At an end having a limit in $D$, first use an increasing smooth reparametrization to a finite parameter end, then [F4] to adjoin the endpoint and a short causal extension, and append an appropriate half of a maximal timelike geodesic. That half has no limit in $D$. Do the same at the other end when necessary; concatenation preserves the curve class. The original $\gamma$ is the maximal connected $E$ segment containing any of its points, since its endpoint limits, if added, are outside $E$. The Cauchy property of $H$ gives $q\in\Gamma\cap H$. If $q$ is after a point $p\in\gamma$, choose $a\in M^{\rm end}$ with $a\ll_W p$; push-up gives $a\ll_W q$, hence $q\in Q$. If $q$ is before $p$, choose $b\in M^{\rm end}$ with $p\ll_W b$ and use push-up to get $q\in P$. By step 4.1 either case puts $q\in C_0\subset E$. Moreover $E=P\cap Q$ is causally convex in $W$: for a causal segment $x\le z\le y$ with endpoints in $E$, end paths $a\ll x$ and $y\ll b$ and push-up give $a\ll z\ll b$. Thus the segment from $p$ to $q$ stays in $E$, and $q$ belongs to the original maximal $E$ segment $\gamma$. Acausality gives exactly one meeting. [F1, F4, step 1.1, step 2.2, step 4.1, construct]

6.1 Because $F_1$ extends to an ambient diffeomorphism fixing $S$, [F3] gives $\overline{C_0}^{\,M}=F_1(C\cup S)=C_0\cup S$. This is a smooth connected manifold with compact boundary $S$, the same compact radial truncations up to diffeomorphism, and the same stationary end. Pull its induced metric back to $C\cup S$. It is smooth and positive definite through $S$ and agrees with the original complete metric outside a compact set. On the remaining compact set, [F6] compares both metrics in the original spatial chart on the boundaryless section $A$; this yields constants $0<c\le C<\infty$ bounding one metric above and below by the other. They also apply outside that set after enlarging the constants. The resulting intrinsic length distances are bounded above and below by the square roots of these constants. Hence a Cauchy sequence for the new distance is Cauchy for the complete original distance and converges also in the new distance. This proves completeness with boundary included. The canonical collar and the compact support were established in step 2.2, and no step required transversality to $T$ away from that collar. [F2, F3, F6, step 2.2, step 3.1, step 4.1, step 5.1, algebra] ∎

## External input

The supplementary imported premises are the explicit normal-exponential chart and the localized logarithmic cutoff in Radu, Section 2.2, equation (2.4) and the subsequent construction, with the nonrotating specialization (2.5). Their precise statement, hypotheses and reading limits are in the reference record. They supplement the existing local-boost supplier. The causal-domain inclusion, horizon-side identification, isotopy, Cauchy restriction and completeness arguments above are local deductions; the present lemma is not an external-input theorem.
