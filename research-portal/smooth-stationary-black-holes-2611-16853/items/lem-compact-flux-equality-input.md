---
id: lem-compact-flux-equality-input
title: Compact flux saturation and pointwise density rigidity
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-smooth-differential-k-form
  - math:prop-local-coordinate-expression-for-a-differential-form
  - math:def-riemannian-volume-form-on-an-oriented-manifold
  - math:thm-linearity-of-the-lebesgue-integral-on-l-one
  - math:prop-order-and-scalar-rules-for-the-nonnegative-integral
  - math:thm-integral-triangle-inequality
  - math:def-compact-space
  - math:def-connected-space
  - math:def-smooth-manifold
  - math:def-oriented-smooth-manifold-and-oriented-chart
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-topology-of-uniform-convergence
  - math:thm-coordinate-differentials-form-the-dual-cotangent-basis
  - math:lem-wedge-monomials-in-a-dual-basis-form-a-basis
  - math:thm-compactness-under-continuous-maps
  - math:cor-heine-borel-in-the-product-topology
  - math:def-borel-sigma-algebra
  - math:thm-continuous-preimages-of-borel-sets-are-borel
  - math:def-integrable-real-and-complex-functions-and-their-integrals
  - math:def-integral-of-a-nonnegative-simple-function
  - math:prop-the-nonnegative-integral-agrees-with-the-simple-integral
  - math:thm-integration-against-a-density
  - math:def-countable-choice
  - math:def-borel-measurable-nonnegative-density-on-a-manifold
  - math:thm-density-measure-is-independent-of-the-chart-gluing
  - math:thm-lebesgue-measure-of-a-box-of-every-kind
  - math:thm-finite-and-countable-subadditivity-of-measures
dependency_roles:
  math:def-smooth-differential-k-form: mathematical-premise
  math:prop-local-coordinate-expression-for-a-differential-form: mathematical-premise
  math:def-riemannian-volume-form-on-an-oriented-manifold: mathematical-premise
  math:thm-linearity-of-the-lebesgue-integral-on-l-one: mathematical-premise
  math:prop-order-and-scalar-rules-for-the-nonnegative-integral: mathematical-premise
  math:thm-integral-triangle-inequality: mathematical-premise
  math:def-compact-space: mathematical-premise
  math:def-connected-space: mathematical-premise
  math:def-smooth-manifold: mathematical-premise
  math:def-oriented-smooth-manifold-and-oriented-chart: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-topology-of-uniform-convergence: mathematical-premise
  math:thm-coordinate-differentials-form-the-dual-cotangent-basis: mathematical-premise
  math:lem-wedge-monomials-in-a-dual-basis-form-a-basis: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:cor-heine-borel-in-the-product-topology: mathematical-premise
  math:def-borel-sigma-algebra: mathematical-premise
  math:thm-continuous-preimages-of-borel-sets-are-borel: mathematical-premise
  math:def-integrable-real-and-complex-functions-and-their-integrals: mathematical-premise
  math:def-integral-of-a-nonnegative-simple-function: mathematical-premise
  math:prop-the-nonnegative-integral-agrees-with-the-simple-integral: mathematical-premise
  math:thm-integration-against-a-density: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-borel-measurable-nonnegative-density-on-a-manifold: mathematical-premise
  math:thm-density-measure-is-independent-of-the-chart-gluing: mathematical-premise
  math:thm-lebesgue-measure-of-a-box-of-every-kind: mathematical-premise
  math:thm-finite-and-countable-subadditivity-of-measures: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Assume countable choice $\mathrm{AC}_\omega$.

Let $S$ be a compact connected oriented smooth surface without boundary, $d\mu$ a smooth positive measure, and $e,b$ continuous real functions. Here a smooth positive measure has a smooth strictly positive density in every coordinate chart. If $\int_S1\,d\mu=4\pi$, $\int_Se\,d\mu=4\pi$, and $\int_S(e^2+b^2)\,d\mu\le4\pi$, then $e=1$ and $b=0$ everywhere.

Moreover, let $q_j$ and $q$ be smooth Riemannian metrics on the fixed oriented compact surface $S$, with $q_j\to q$ uniformly in local coordinates, and let smooth real two-forms $\alpha_j,\beta_j$ converge uniformly in local coordinates to smooth two-forms $\alpha,\beta$. Define $e_j,b_j,e,b$ by $\alpha_j=e_jd\mu_{q_j}$, $\beta_j=b_jd\mu_{q_j}$, $\alpha=ed\mu_q$, and $\beta=bd\mu_q$. Then the areas, the integrals of $e_j$ and $b_j$, and the integrals of $e_j^2+b_j^2$ with respect to $d\mu_{q_j}$ converge to their corresponding limiting values. In particular this applies to smooth metric convergence and continuous two-form convergence. The result is independent of global causal geometry.

## Statement references

[[math:def-smooth-differential-k-form]]

[[math:prop-local-coordinate-expression-for-a-differential-form]]

[[math:def-riemannian-volume-form-on-an-oriented-manifold]]

[[math:def-compact-space]]

[[math:def-connected-space]]

[[math:def-smooth-manifold]]

[[math:def-oriented-smooth-manifold-and-oriented-chart]]

[[math:def-riemannian-metric-and-riemannian-manifold]]

[[math:def-topology-of-uniform-convergence]]

[[math:def-countable-choice]]

[[math:def-borel-measurable-nonnegative-density-on-a-manifold]]

[[math:thm-density-measure-is-independent-of-the-chart-gluing]]

[[math:thm-lebesgue-measure-of-a-box-of-every-kind]]

## Facts & Assumptions

[A1] Countable choice $\mathrm{AC}_\omega$ is assumed. Its uses here are the chart-restriction theorem in [F11] and the Euclidean rectangle-measure theorem in [F12]; no necessity claim is made. [[math:def-countable-choice]]

[F1] A smooth real two-form on $S$ is a smooth section of $\bigwedge^2T^*S$. In a surface chart it has the unique expression $a\,dx^1\wedge dx^2$ with smooth real coefficient $a$. [[math:def-smooth-differential-k-form]] [[math:prop-local-coordinate-expression-for-a-differential-form]]

[F2] The oriented area form is $d\mu_q=\sqrt{\det q}\,dx^1\wedge dx^2$ in a positive chart and is nowhere zero. Scalar integration is against the Borel measure associated to its positive density, with chart restriction as in [F11]. [[math:def-riemannian-volume-form-on-an-oriented-manifold]]

[F3] The integral is linear on integrable functions, the nonnegative integral is monotone, and the modulus of an integral is bounded by the integral of the modulus. [[math:thm-linearity-of-the-lebesgue-integral-on-l-one]] [[math:prop-order-and-scalar-rules-for-the-nonnegative-integral]] [[math:thm-integral-triangle-inequality]]

[F4] A smooth surface without boundary is a smooth manifold of dimension two; its charts have open domains in $S$ and open images in $\mathbb R^2$. The specified orientation selects positive charts. Compactness means that every open cover of $S$ has a finite subcover, and connectedness means that $S$ has no separation into two disjoint nonempty open sets. [[math:def-smooth-manifold]] [[math:def-oriented-smooth-manifold-and-oriented-chart]] [[math:def-compact-space]] [[math:def-connected-space]]

[F5] A smooth Riemannian metric is a smooth symmetric covariant two-tensor positive definite at every point. For real coefficient functions on a fixed set $K$, uniform convergence means that for every $\varepsilon>0$ one index $J$ makes $|f_j(x)-f(x)|<\varepsilon$ for all $j\ge J$ and all $x\in K$. For the local-coordinate convergence here, apply this condition to every metric or form coefficient on each compact subset of a coordinate domain. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:def-topology-of-uniform-convergence]]

[F6] At each point of a surface chart, $dx^1,dx^2$ are dual to the coordinate tangent basis, and $dx^1\wedge dx^2$ is a basis of the alternating two-covectors. This is a pointwise linear-algebra statement, requiring no smoothness of the alternating covector field. [[math:thm-coordinate-differentials-form-the-dual-cotangent-basis]] [[math:lem-wedge-monomials-in-a-dual-basis-form-a-basis]]

[F7] A continuous real function on a nonempty compact topological space attains finite extrema; a strictly positive such function therefore has a strictly positive minimum. Continuous images of compact spaces are compact. Closed bounded rectangles in $\mathbb R^2$ are compact in its usual topology. [[math:thm-compactness-under-continuous-maps]] [[math:cor-heine-borel-in-the-product-topology]]

[F8] The Borel sigma-algebra is generated by the open sets. A continuous map between topological spaces has Borel preimages of Borel sets, so continuous real functions on $S$ are measurable for its Borel measures and also for their completions. [[math:def-borel-sigma-algebra]] [[math:thm-continuous-preimages-of-borel-sets-are-borel]]

[F9] A measurable real function $f$ is integrable exactly when $\int |f|$ is finite. For a measurable set $E$ and finite $C>0$, the nonnegative integral of the simple function $C\mathbf1_E$ is $C\nu(E)$, including when $\nu(E)$ is infinite; for $C=0$ the integral is zero. In particular $\int_S1\,d\nu=\nu(S)$. [[math:def-integrable-real-and-complex-functions-and-their-integrals]] [[math:def-integral-of-a-nonnegative-simple-function]] [[math:prop-the-nonnegative-integral-agrees-with-the-simple-integral]]

[F10] For nonnegative measurable $r$ and $f$ on a measure space, $\int f\,d(r\,d\nu)=\int fr\,d\nu$. [[math:thm-integration-against-a-density]]

[F11] A nonnegative Borel density has Borel chart coefficients satisfying the absolute-Jacobian transition law. Under [A1], on a Hausdorff second-countable smooth $n$-manifold its intrinsic Borel measure satisfies $\mu_r(E)=\int_{x(E)}r_x\,d\lambda_n$ for every Borel $E$ contained in a chart $x:U\to x(U)$. Here $S$ has these manifold properties by [F4], and $n=2$. The area density in [F2] has smooth positive coefficient $v=\sqrt{\det q}$, hence Borel by [F8], and the density transition law is part of the volume-form construction in [F2]. Thus this theorem supplies $\mu_q(E)=\int_{x(E)}v\,d\lambda_2$, and likewise for each $q_j$. For the given smooth positive measure $\mu$, the meaning of its chart density $\rho_x$ is $\mu(E)=\int_{x(E)}\rho_x\,d\lambda_2$; this is the stated measure-density hypothesis, not a new assumption about $\mu$. [[math:def-borel-measurable-nonnegative-density-on-a-manifold]] [[math:thm-density-measure-is-independent-of-the-chart-gluing]]

[F12] Under [A1], every bounded rectangle $Q=\prod_{i=1}^2[a_i,b_i]$, with $a_i\le b_i$, is Borel and has Lebesgue measure $\lambda_2(Q)=(b_1-a_1)(b_2-a_2)<\infty$; this is strictly positive if both side lengths are positive. The same formula holds with open faces. This is the box-measure theorem with $n=2$ and finite real endpoints. [[math:thm-lebesgue-measure-of-a-box-of-every-kind]]

[F13] For a measure and finitely many measurable sets, the measure of their union is at most the sum of their measures. [[math:thm-finite-and-countable-subadditivity-of-measures]]

## Proof

**Given:** Countable choice and the surface, measure, functions, metrics and forms in the statement, with the stated convergence and integral hypotheses.

**Goal:** Prove pointwise rigidity, well-definedness of the density quotients and convergence of the listed integrals.

**Proof technique:** direct.

1.1 For the rigidity assertion $S$ is nonempty because its stated total mass is $4\pi$. By [F7], each continuous real function on $S$ is bounded. More generally, for any finite Borel measure $\nu$ on $S$ (or its completion) and bounded continuous real $f$, [F8] makes $f$ and $|f|$ measurable. Choose a finite $C>0$ bounding $|f|$; [F3] and [F9] give $\int_S|f|\,d\nu\le\int_SC\,d\nu=C\nu(S)<\infty$, hence $f\in L^1(\nu)$. Apply this to the given smooth positive measure $\mu$, whose local densities specify its Borel measure, with $\mu(S)=\int_S1\,d\mu=4\pi$. Put $h=(e-1)^2+b^2$. All functions in this expansion are continuous, bounded and integrable by the preceding argument. Expanding the square and applying linearity gives $\int_Sh\,d\mu=\int_S(e^2+b^2)\,d\mu-2\int_Se\,d\mu+\int_S1\,d\mu\le0$. Nonnegativity gives the reverse inequality, so this integral is zero. [given, F3, F7, F8, F9, algebra]

1.2 In a positive chart, write $\alpha_j=a_j\,dx^1\wedge dx^2$ and $\beta_j=c_j\,dx^1\wedge dx^2$ using [F1], and put $v_j=\sqrt{\det q_j}>0$. Then $e_j=a_j/v_j$ and $b_j=c_j/v_j$ satisfy the required two-form equalities by [F2]; the same formulas define $e,b$ with $v=\sqrt{\det q}$. These smooth local functions agree on overlaps: at each point each is the unique scalar multiplying the same nonzero intrinsic area form to give the specified two-form. Thus the quotients define unique global smooth real functions for arbitrary two-forms on $S$, without an ambient spacetime. [given, F1, F2, algebra]

2.1 If $h(p)>0$ at some point, continuity gives a coordinate neighborhood on which $h\ge c>0$. Its coordinate image contains a closed rectangle $Q$ with finite endpoints and strictly positive side lengths, so $0<\lambda_2(Q)<\infty$ by [F12]. By [F7], $Q$ is compact and the smooth strictly positive chart density $\rho_x$ of $\mu$ has a positive minimum $m$ on $Q$. The chart preimage $R$ of $Q$ is closed in the open chart domain $U$; thus $R=U\setminus V$ for some open $V$ in $S$, making $R$ Borel by [F8]. By [F11], [F3] and [F9], $\mu(R)=\int_Q\rho_x\,d\lambda_2\ge m\lambda_2(Q)>0$. Monotonicity gives $\int_Sh\,d\mu\ge c\mu(R)>0$, a contradiction. Hence $h=0$ everywhere, and its two nonnegative square terms give $e=1$ and $b=0$ pointwise. [given, step 1.1, F3, F4, F7, F8, F9, F11, F12, algebra]

2.2 If $S$ is empty all convergence assertions are immediate; otherwise, around each point choose a positive chart and an open coordinate rectangle whose closed rectangle is contained in the chart image. These open patches cover $S$, so [F4] gives finitely many of them. Each closed rectangle is compact by [F7], and its inverse chart image is compact by the continuous-image assertion of [F7]. On each closed rectangle, the continuous positive $v$ has a positive minimum by [F7]; all limiting metric and form coefficients are bounded there by the same fact. Uniform convergence of the metric coefficients implies uniform convergence of their determinants, hence $v_j\to v$ uniformly, with $v_j$ eventually bounded away from zero. The assumed coefficient convergence and the formulas of step 1.2 therefore give $e_j\to e$ and $b_j\to b$ uniformly on each patch and then on $S$. The global ratio $r_j=v_j/v=d\mu_{q_j}/d\mu_q$ converges uniformly to $1$. Consequently $r_j$, $e_jr_j$, $b_jr_j$, and $(e_j^2+b_j^2)r_j$ converge uniformly to $1$, $e$, $b$, and $e^2+b^2$, respectively. [given, F1, F2, F4, F5, F7, step 1.2, algebra]

3.1 The fixed measure $\mu_q(S)$ is finite: on each closed coordinate rectangle $Q$ of the finite cover in step 2.2, [F7] bounds the local density $v$ above by a finite $M>0$. Its inverse chart image $R$ is Borel as in step 2.1, and [F11], [F12], [F3] and [F9] give $\mu_q(R)=\int_Qv\,d\lambda_2\le M\lambda_2(Q)<\infty$. These finitely many sets cover $S$, so finite subadditivity in [F13] gives $\mu_q(S)<\infty$. The functions in the four global pairs in step 2.2 and their differences are continuous, hence bounded and Borel measurable by [F7] and [F8]. The finite-measure argument of step 1.1 makes them integrable for $\mu_q$ and, likewise, for each $\mu_{q_j}$, whose total mass is finite by the same finite-cover argument. The coordinate identity $v_j=r_jv$ gives the measure identity $d\mu_{q_j}=r_jd\mu_q$: on each Borel subset of a chart, [F11] and [F10] identify both measures with the integral of $r_jv=v_j$ against $\lambda_2$, and a finite disjoint Borel refinement of the chart cover gives the identity globally. For each pair $u_j,u$ among the four uniformly convergent pairs in step 2.2, linearity, the integral triangle inequality and monotonicity give $|\int_Su_j\,d\mu_q-\int_Su\,d\mu_q|\le\mu_q(S)\sup_S|u_j-u|\to0$. Applying [F10] to the nonnegative integrands, and separately to the positive and negative parts of the signed integrands using [F9], rewrites these integrals as area, the two flux integrals and the squared-density integral for $\mu_{q_j}$. This proves all claimed integral limits. [F2, F3, F7, F8, F9, F10, F11, F12, F13, step 1.1, step 2.1, step 2.2, algebra]

4.1 No derivative of a two-form coefficient was used in steps 1.2–3.1. For continuous two-forms, meaning alternating covector fields with continuous coefficients in smooth coordinate frames, the pointwise basis in [F6] gives unique coefficients $a_j,c_j,a,c$; these are continuous by the stated meaning of continuity in a coordinate frame. Division by the smooth positive $v_j,v$ gives continuous density quotients, and uniqueness again makes them agree on overlaps. Uniform coefficient convergence therefore gives exactly the same uniform bounds and integral limits. In particular the claimed smooth-metric and continuous-two-form convergence case follows. [F2, F5, F6, step 1.2, step 2.2, step 3.1] ∎
