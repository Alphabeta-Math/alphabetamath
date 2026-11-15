---
title: Maximal slices, causal cuts and stability
description: Assemble the analytic and geometric inputs for maximal-slice
  continuation, causal completeness, null-boundary cuts, area comparison and
  horizon flux rigidity. Use the common data and the preceding field inputs
  while retaining every local argument and imported-premise qualification.
status: published
dependency_level: 1
---

**Purpose:** Assemble the analytic and geometric inputs for maximal-slice continuation, causal completeness, null-boundary cuts, area comparison and horizon flux rigidity. Use the common data and the preceding field inputs while retaining every local argument and imported-premise qualification.

## Divergence comparison in a smooth compact boundary collar

[Open item](item-lem-thin-collar-divergence-area-input) · level 0


### Statement

Work in ZFC. Let $(N,h)$ be a smooth Riemannian three-manifold with compact boundary $S$, and suppose a smooth collar diffeomorphism $F:S\times[0,\eta_0]\to U\subset N$ satisfies $F(p,0)=p$ and $\rho(F(p,t))=t$, where $|\nabla\rho|_h=1$ and $|\Delta_h\rho|\le C$ on $U$, for constants $\eta_0>0$ and $C\ge0$. Here $\nabla\rho$ is the metric gradient and $\Delta_h\rho=\operatorname{div}_h(\nabla\rho)$; area and volume are integrals of the induced Riemannian densities.

For $0<\eta\le\eta_0$, let $\Omega\subset U\cap\{0\le\rho\le\eta\}$ be a compact smooth three-dimensional region with boundary the disjoint union $S\sqcup D$, and assume that $\Omega$ contains the inward side of $S$. Here a smooth region is supplied as an embedded smooth submanifold with boundary of $N$, whose inclusion $\iota:\Omega\hookrightarrow N$ is a smooth embedding and whose metric is $\iota^*h$. Its intrinsic interior $\Omega^\circ$ is open in $N^\circ$ with the restricted smooth structure, and its displayed boundary is its intrinsic manifold boundary. Containing the inward side means that a neighborhood of $S$ in $N$ lies in $\Omega$, with the restricted manifold-with-boundary smooth structure there. The outer boundary $D$ may be disconnected. Then $|S|\le |D|+C\operatorname{Vol}_h(\Omega)$.

If the collar volume density has the form $F^*dV_h=J(p,t)\,dA_S(p)\,dt$ with $J\le K$ for a constant $K$, then $\operatorname{Vol}_h(\Omega)\le K\eta |S|$, so $|S|\le |D|+CK\eta |S|$. In particular, for fixed collar data the error is $O(\eta)$, uniformly over such regions.

### Facts & Assumptions

[A1] ZFC supplies the countable choice required by the cited integration, measure and partition results. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] A Riemannian metric is smooth and positive definite; the gradient is the metric dual of the differential, and the Laplace–Beltrami operator is the trace of the Hessian. Its value is the divergence of the gradient. [math:def-riemannian-divergence](https://alphabetamath.cc/item/def-riemannian-divergence) [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function) [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian) [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)

[F2] Riemannian densities are defined locally by the square root of the metric determinant. Compactly supported density integration is local, linear, nonnegative and invariant under diffeomorphisms, without an orientation. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation)

[F3] On an oriented Riemannian manifold with boundary, the integral of the divergence of a smooth compactly supported vector field equals its outward normal flux. A smooth partition of unity subordinate to a boundary-chart cover exists under countable choice. [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem) [math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary)

[F4] Cauchy–Schwarz bounds the absolute inner product by the product of the norms. Tonelli's theorem permits iterated integration of a nonnegative measurable function over a product of sigma-finite measure spaces. [math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces) [math:thm-tonelli-and-fubini-for-completed-product-measures](https://alphabetamath.cc/item/thm-tonelli-and-fubini-for-completed-product-measures)

[F5] The boundary of a smooth positive-dimensional manifold is a closed embedded smooth boundaryless hypersurface, and its tangent space is the boundary-tangent hyperplane. Pullback of a Riemannian metric by an immersion is Riemannian. [math:thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold](https://alphabetamath.cc/item/thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold) [math:prop-tangent-space-of-the-boundary-is-the-boundary-tangent-hyperplane](https://alphabetamath.cc/item/prop-tangent-space-of-the-boundary-is-the-boundary-tangent-hyperplane) [math:prop-pullback-of-a-riemannian-metric-is-riemannian-exactly-for-immersions](https://alphabetamath.cc/item/prop-pullback-of-a-riemannian-metric-is-riemannian-exactly-for-immersions)

[F6] Under countable choice a positive smooth density defines a compact-finite, sigma-finite Borel measure. On a Borel subset of a chart its measure is the Lebesgue integral of the density coefficient. For a nonnegative Borel function the integral is the sum of the partition-weighted chart integrals; for a smooth compactly supported function it agrees with smooth density integration. [math:thm-a-positive-smooth-density-defines-a-locally-finite-radon-measure](https://alphabetamath.cc/item/thm-a-positive-smooth-density-defines-a-locally-finite-radon-measure) [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing) [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)

[F7] Euclidean Lebesgue measures are sigma-finite, and the product of the measures in dimensions two and one agrees with three-dimensional Lebesgue measure on Borel sets. [math:prop-lebesgue-measure-is-sigma-finite-and-finite-on-bounded-sets](https://alphabetamath.cc/item/prop-lebesgue-measure-is-sigma-finite-and-finite-on-bounded-sets) [math:thm-lebesgue-product-measure-agrees-with-euclidean-lebesgue-on-borel-sets](https://alphabetamath.cc/item/thm-lebesgue-product-measure-agrees-with-euclidean-lebesgue-on-borel-sets)

[F8] Under countable choice a positive-codimension immersed submanifold of a smooth manifold is null in ambient coordinates. Thus its Borel image has zero measure for a smooth density by the chart formula in [F6]. [math:cor-positive-codimension-immersed-submanifolds-are-null](https://alphabetamath.cc/item/cor-positive-codimension-immersed-submanifolds-are-null)

[F9] Nonnegative measurable integrals are monotone and homogeneous for positive finite scalars; the zero function has integral zero. [math:prop-order-and-scalar-rules-for-the-nonnegative-integral](https://alphabetamath.cc/item/prop-order-and-scalar-rules-for-the-nonnegative-integral)

[F10] A diffeomorphism is a bijective smooth map with smooth inverse. This definition applies to the supplied closed-interval parametrization onto its smooth image $U$. [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[F11] Under countable choice, every closed interval $[a,b]$ with real $a\le b$ has one-dimensional Lebesgue measure $b-a$. In particular, the degenerate interval $[c,c]=\{c\}$ is Borel and has measure zero for every real $c$. [math:thm-lebesgue-measure-of-a-box-of-every-kind](https://alphabetamath.cc/item/thm-lebesgue-measure-of-a-box-of-every-kind)

[F12] An embedded smooth submanifold with boundary is a subset supplied with a manifold-with-boundary smooth structure for which its inclusion is a smooth embedding. An embedding is an immersion and a homeomorphism onto its image; its differential is injective on the full tangent spaces, including at boundary points. This definition does not assert that the intrinsic boundary equals the intersection with the ambient boundary. [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary) [math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-immersion-and-embedding-for-manifolds-with-boundary)

### Proof

**Given:** The collar, region and bounds in the statement, working in ZFC as in [A1].

**Goal:** Prove the area inequality and the stated uniform volume estimate.

1.1 If $S$ is empty, the collar and $\Omega$ are empty and all conclusions hold with zero integrals. Otherwise [F12] makes the inclusion $\iota:\Omega\hookrightarrow N$ a smooth embedding and hence an immersion. Apply [F5] to $N$ and to the supplied manifold with boundary $\Omega$. It gives the smooth embedded surfaces $S$ and $D$ and identifies their tangent spaces with the boundary hyperplanes of $\Omega$; at $S$ the stated region convention gives the same smooth structure as the boundary of $N$. Their inclusions into $N$ are immersions, so the induced metrics and their area densities are smooth and positive. The metric on $\Omega$ is $\iota^*h$, smooth and positive up to its boundary by [F5]. [A1, F1, F2, F5, F12, given]

2.1 Cover $\Omega$ by coordinate neighborhoods in the manifold with boundary $\Omega$ and take a subordinate smooth partition of unity. Compactness and local finiteness leave finitely many nonzero terms $\chi_i$, each supported compactly inside its chart. Orient each chart and apply the oriented divergence theorem to $\chi_i\nabla\rho$ there. On that oriented chart the volume and outward boundary forms integrate as the corresponding positive densities. Sum using locality, linearity and orientation independence of density integration. The product rule and $\sum_i\chi_i=1$ give $\sum_i\operatorname{div}(\chi_i\nabla\rho)=\operatorname{div}(\nabla\rho)=\Delta_h\rho$. Hence $\int_\Omega\Delta_h\rho\,dV_h=\int_{\partial\Omega}h(\nabla\rho,\nu)\,dA$, where $\nu$ is the outward unit normal. This also covers nonorientable $\Omega$. [A1, F1, F2, F3, step 1.1, given]

2.2 Write $B_\eta=F(S\times[0,\eta])$. Let $\mu$ be the Borel measure of the smooth positive density $dV_h$ on $N$ supplied by [F6]; $B_\eta$ and $\Omega$ are compact and hence Borel, and $\mu(B_\eta)<\infty$. The intrinsic smooth volume of each region equals its ambient density measure. Indeed, for $\Omega$ the stated region convention identifies the interior smooth structure with the ambient restriction, and its metric is the pullback through its embedding as in step 1.1; for $B_\eta$ use the supplied smooth collar image and [F10]. Thus on each interior the charts and density coefficients agree, so [F6] gives the same measure there. The remaining boundary has zero three-dimensional measure intrinsically: in a boundary chart it is a Borel coordinate face, each of whose normal sections is either empty or a singleton. By [F11], $\lambda_1(\{c\})=\lambda_1([c,c])=0$ for every real $c$. The sigma-finite factors and Euclidean product identification in [F7] therefore allow Tonelli from [F4] to give zero three-dimensional measure for the face. The same is true in ambient boundary charts for $S$. The surface $D$ lies in the interior of $N$ and is an immersed two-manifold there, so [F8] makes it ambient-null; the same argument applies to the upper collar surface $F(S\times\{\eta\})$. Coordinate-null Borel sets have zero smooth-density measure by [F6]. Finally apply the smooth-integral agreement of [F6] to the constant function one on each compact region. Since $\Omega\subset B_\eta$, measure additivity and nonnegativity give $\operatorname{Vol}_h(\Omega)=\mu(\Omega)\le\mu(B_\eta)=\operatorname{Vol}_h(B_\eta)$. [A1, F4, F5, F6, F7, F8, F10, F11, F12, step 1.1, given]

3.1 At $S$ the restriction of $\rho$ is zero, so its differential vanishes on the tangent hyperplane from step 1.1. The gradient-dual identity makes $\nabla\rho$ perpendicular to that hyperplane. It is unit and points inward: $\rho$ is nonnegative on $\Omega$, and $d\rho(\nabla\rho)=1$, with $\Omega$ containing the inward side of $S$. Thus $h(\nabla\rho,\nu)=-1$ at $S$. On $D$, Cauchy–Schwarz and $|\nabla\rho|=|\nu|=1$ imply $h(\nabla\rho,\nu)\le1$. The identity in step 2.1 and $|\Delta_h\rho|\le C$ now yield $|S|=\int_D h(\nabla\rho,\nu)\,dA-\int_\Omega\Delta_h\rho\,dV_h\le |D|+C\operatorname{Vol}_h(\Omega)$. [F1, F2, F4, F5, step 1.1, step 2.1, given]

3.2 To compute this last volume assume the stated factorization $F^*dV_h=J\,dA_S\,dt$. Its coefficient $J$ is smooth and positive, being the ratio of positive smooth densities. Choose a finite smooth chart partition $(x_i,\psi_i)$ on the compact surface $S$, with $x_i:V_i\to x_i(V_i)\subset\mathbb R^2$. Write $dA_S=a_i(u)|du^1du^2|$ in this chart. On $S\times(0,\eta)$ use the product charts and the partition $\psi_i(p)$, and extend each coefficient $g_i(u,t)=\psi_i(x_i^{-1}u)a_i(u)J(x_i^{-1}u,t)$ by zero outside $x_i(V_i)\times(0,\eta)$. Each extension is nonnegative Borel: its coefficient is smooth on an open set, and the extension is zero on its Borel complement. The measures $\lambda_2$ and $\lambda_1$ are sigma-finite by [F7], so Tonelli applies to these Borel functions, also on the completed product. The product identification in [F7] equates their three-dimensional chart integrals with the product-measure integrals. The end surfaces have zero volume by step 2.2. Density diffeomorphism invariance, the chart formula of [F6], and the finite partition sum consequently give $\operatorname{Vol}_h(B_\eta)=\sum_i\int_0^\eta\int_{x_i(V_i)}g_i(u,t)\,d\lambda_2(u)\,dt=\int_0^\eta\int_S J(p,t)\,d\mu_S(p)\,dt$, where $\mu_S$ is the finite Borel measure of $dA_S$ and $\mu_S(S)=|S|$. This derives the iterated-integral formula from chart integrals rather than assuming a product-measure identity for manifold densities. [A1, F2, F3, F4, F6, F7, F10, step 2.2, given]

4.1 By $J\le K$ and [F9], the inner integral in step 3.2 is at most $K\mu_S(S)=K|S|$. All quantities are finite by compactness and [F6]; thus integrating over an interval of length $\eta$ gives $\operatorname{Vol}_h(B_\eta)\le K\eta|S|$. Combining steps 2.2 and 3.1 proves $|S|\le |D|+CK\eta|S|$. With the collar, $C,K$ and $|S|$ fixed, this error is $O(\eta)$ independently of the smooth region or its disconnected outer boundary. [F6, F9, step 3.1, step 2.2, step 3.2, given] ∎


## Compact flux saturation and pointwise density rigidity

[Open item](item-lem-compact-flux-equality-input) · level 0


### Statement

Assume countable choice $\mathrm{AC}_\omega$.

Let $S$ be a compact connected oriented smooth surface without boundary, $d\mu$ a smooth positive measure, and $e,b$ continuous real functions. Here a smooth positive measure has a smooth strictly positive density in every coordinate chart. If $\int_S1\,d\mu=4\pi$, $\int_Se\,d\mu=4\pi$, and $\int_S(e^2+b^2)\,d\mu\le4\pi$, then $e=1$ and $b=0$ everywhere.

Moreover, let $q_j$ and $q$ be smooth Riemannian metrics on the fixed oriented compact surface $S$, with $q_j\to q$ uniformly in local coordinates, and let smooth real two-forms $\alpha_j,\beta_j$ converge uniformly in local coordinates to smooth two-forms $\alpha,\beta$. Define $e_j,b_j,e,b$ by $\alpha_j=e_jd\mu_{q_j}$, $\beta_j=b_jd\mu_{q_j}$, $\alpha=ed\mu_q$, and $\beta=bd\mu_q$. Then the areas, the integrals of $e_j$ and $b_j$, and the integrals of $e_j^2+b_j^2$ with respect to $d\mu_{q_j}$ converge to their corresponding limiting values. In particular this applies to smooth metric convergence and continuous two-form convergence. The result is independent of global causal geometry.

### Statement references

[math:def-smooth-differential-k-form](https://alphabetamath.cc/item/def-smooth-differential-k-form)

[math:prop-local-coordinate-expression-for-a-differential-form](https://alphabetamath.cc/item/prop-local-coordinate-expression-for-a-differential-form)

[math:def-riemannian-volume-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-riemannian-volume-form-on-an-oriented-manifold)

[math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[math:def-connected-space](https://alphabetamath.cc/item/def-connected-space)

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:def-oriented-smooth-manifold-and-oriented-chart](https://alphabetamath.cc/item/def-oriented-smooth-manifold-and-oriented-chart)

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[math:def-topology-of-uniform-convergence](https://alphabetamath.cc/item/def-topology-of-uniform-convergence)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:def-borel-measurable-nonnegative-density-on-a-manifold](https://alphabetamath.cc/item/def-borel-measurable-nonnegative-density-on-a-manifold)

[math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing)

[math:thm-lebesgue-measure-of-a-box-of-every-kind](https://alphabetamath.cc/item/thm-lebesgue-measure-of-a-box-of-every-kind)

### Facts & Assumptions

[A1] Countable choice $\mathrm{AC}_\omega$ is assumed. Its uses here are the chart-restriction theorem in [F11] and the Euclidean rectangle-measure theorem in [F12]; no necessity claim is made. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F1] A smooth real two-form on $S$ is a smooth section of $\bigwedge^2T^*S$. In a surface chart it has the unique expression $a\,dx^1\wedge dx^2$ with smooth real coefficient $a$. [math:def-smooth-differential-k-form](https://alphabetamath.cc/item/def-smooth-differential-k-form) [math:prop-local-coordinate-expression-for-a-differential-form](https://alphabetamath.cc/item/prop-local-coordinate-expression-for-a-differential-form)

[F2] The oriented area form is $d\mu_q=\sqrt{\det q}\,dx^1\wedge dx^2$ in a positive chart and is nowhere zero. Scalar integration is against the Borel measure associated to its positive density, with chart restriction as in [F11]. [math:def-riemannian-volume-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-riemannian-volume-form-on-an-oriented-manifold)

[F3] The integral is linear on integrable functions, the nonnegative integral is monotone, and the modulus of an integral is bounded by the integral of the modulus. [math:thm-linearity-of-the-lebesgue-integral-on-l-one](https://alphabetamath.cc/item/thm-linearity-of-the-lebesgue-integral-on-l-one) [math:prop-order-and-scalar-rules-for-the-nonnegative-integral](https://alphabetamath.cc/item/prop-order-and-scalar-rules-for-the-nonnegative-integral) [math:thm-integral-triangle-inequality](https://alphabetamath.cc/item/thm-integral-triangle-inequality)

[F4] A smooth surface without boundary is a smooth manifold of dimension two; its charts have open domains in $S$ and open images in $\mathbb R^2$. The specified orientation selects positive charts. Compactness means that every open cover of $S$ has a finite subcover, and connectedness means that $S$ has no separation into two disjoint nonempty open sets. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:def-oriented-smooth-manifold-and-oriented-chart](https://alphabetamath.cc/item/def-oriented-smooth-manifold-and-oriented-chart) [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) [math:def-connected-space](https://alphabetamath.cc/item/def-connected-space)

[F5] A smooth Riemannian metric is a smooth symmetric covariant two-tensor positive definite at every point. For real coefficient functions on a fixed set $K$, uniform convergence means that for every $\varepsilon>0$ one index $J$ makes $|f_j(x)-f(x)|<\varepsilon$ for all $j\ge J$ and all $x\in K$. For the local-coordinate convergence here, apply this condition to every metric or form coefficient on each compact subset of a coordinate domain. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-topology-of-uniform-convergence](https://alphabetamath.cc/item/def-topology-of-uniform-convergence)

[F6] At each point of a surface chart, $dx^1,dx^2$ are dual to the coordinate tangent basis, and $dx^1\wedge dx^2$ is a basis of the alternating two-covectors. This is a pointwise linear-algebra statement, requiring no smoothness of the alternating covector field. [math:thm-coordinate-differentials-form-the-dual-cotangent-basis](https://alphabetamath.cc/item/thm-coordinate-differentials-form-the-dual-cotangent-basis) [math:lem-wedge-monomials-in-a-dual-basis-form-a-basis](https://alphabetamath.cc/item/lem-wedge-monomials-in-a-dual-basis-form-a-basis)

[F7] A continuous real function on a nonempty compact topological space attains finite extrema; a strictly positive such function therefore has a strictly positive minimum. Continuous images of compact spaces are compact. Closed bounded rectangles in $\mathbb R^2$ are compact in its usual topology. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps) [math:cor-heine-borel-in-the-product-topology](https://alphabetamath.cc/item/cor-heine-borel-in-the-product-topology)

[F8] The Borel sigma-algebra is generated by the open sets. A continuous map between topological spaces has Borel preimages of Borel sets, so continuous real functions on $S$ are measurable for its Borel measures and also for their completions. [math:def-borel-sigma-algebra](https://alphabetamath.cc/item/def-borel-sigma-algebra) [math:thm-continuous-preimages-of-borel-sets-are-borel](https://alphabetamath.cc/item/thm-continuous-preimages-of-borel-sets-are-borel)

[F9] A measurable real function $f$ is integrable exactly when $\int |f|$ is finite. For a measurable set $E$ and finite $C>0$, the nonnegative integral of the simple function $C\mathbf1_E$ is $C\nu(E)$, including when $\nu(E)$ is infinite; for $C=0$ the integral is zero. In particular $\int_S1\,d\nu=\nu(S)$. [math:def-integrable-real-and-complex-functions-and-their-integrals](https://alphabetamath.cc/item/def-integrable-real-and-complex-functions-and-their-integrals) [math:def-integral-of-a-nonnegative-simple-function](https://alphabetamath.cc/item/def-integral-of-a-nonnegative-simple-function) [math:prop-the-nonnegative-integral-agrees-with-the-simple-integral](https://alphabetamath.cc/item/prop-the-nonnegative-integral-agrees-with-the-simple-integral)

[F10] For nonnegative measurable $r$ and $f$ on a measure space, $\int f\,d(r\,d\nu)=\int fr\,d\nu$. [math:thm-integration-against-a-density](https://alphabetamath.cc/item/thm-integration-against-a-density)

[F11] A nonnegative Borel density has Borel chart coefficients satisfying the absolute-Jacobian transition law. Under [A1], on a Hausdorff second-countable smooth $n$-manifold its intrinsic Borel measure satisfies $\mu_r(E)=\int_{x(E)}r_x\,d\lambda_n$ for every Borel $E$ contained in a chart $x:U\to x(U)$. Here $S$ has these manifold properties by [F4], and $n=2$. The area density in [F2] has smooth positive coefficient $v=\sqrt{\det q}$, hence Borel by [F8], and the density transition law is part of the volume-form construction in [F2]. Thus this theorem supplies $\mu_q(E)=\int_{x(E)}v\,d\lambda_2$, and likewise for each $q_j$. For the given smooth positive measure $\mu$, the meaning of its chart density $\rho_x$ is $\mu(E)=\int_{x(E)}\rho_x\,d\lambda_2$; this is the stated measure-density hypothesis, not a new assumption about $\mu$. [math:def-borel-measurable-nonnegative-density-on-a-manifold](https://alphabetamath.cc/item/def-borel-measurable-nonnegative-density-on-a-manifold) [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing)

[F12] Under [A1], every bounded rectangle $Q=\prod_{i=1}^2[a_i,b_i]$, with $a_i\le b_i$, is Borel and has Lebesgue measure $\lambda_2(Q)=(b_1-a_1)(b_2-a_2)<\infty$; this is strictly positive if both side lengths are positive. The same formula holds with open faces. This is the box-measure theorem with $n=2$ and finite real endpoints. [math:thm-lebesgue-measure-of-a-box-of-every-kind](https://alphabetamath.cc/item/thm-lebesgue-measure-of-a-box-of-every-kind)

[F13] For a measure and finitely many measurable sets, the measure of their union is at most the sum of their measures. [math:thm-finite-and-countable-subadditivity-of-measures](https://alphabetamath.cc/item/thm-finite-and-countable-subadditivity-of-measures)

### Proof

**Given:** Countable choice and the surface, measure, functions, metrics and forms in the statement, with the stated convergence and integral hypotheses.

**Goal:** Prove pointwise rigidity, well-definedness of the density quotients and convergence of the listed integrals.

**Proof technique:** direct.

1.1 For the rigidity assertion $S$ is nonempty because its stated total mass is $4\pi$. By [F7], each continuous real function on $S$ is bounded. More generally, for any finite Borel measure $\nu$ on $S$ (or its completion) and bounded continuous real $f$, [F8] makes $f$ and $|f|$ measurable. Choose a finite $C>0$ bounding $|f|$; [F3] and [F9] give $\int_S|f|\,d\nu\le\int_SC\,d\nu=C\nu(S)<\infty$, hence $f\in L^1(\nu)$. Apply this to the given smooth positive measure $\mu$, whose local densities specify its Borel measure, with $\mu(S)=\int_S1\,d\mu=4\pi$. Put $h=(e-1)^2+b^2$. All functions in this expansion are continuous, bounded and integrable by the preceding argument. Expanding the square and applying linearity gives $\int_Sh\,d\mu=\int_S(e^2+b^2)\,d\mu-2\int_Se\,d\mu+\int_S1\,d\mu\le0$. Nonnegativity gives the reverse inequality, so this integral is zero. [given, F3, F7, F8, F9, algebra]

1.2 In a positive chart, write $\alpha_j=a_j\,dx^1\wedge dx^2$ and $\beta_j=c_j\,dx^1\wedge dx^2$ using [F1], and put $v_j=\sqrt{\det q_j}>0$. Then $e_j=a_j/v_j$ and $b_j=c_j/v_j$ satisfy the required two-form equalities by [F2]; the same formulas define $e,b$ with $v=\sqrt{\det q}$. These smooth local functions agree on overlaps: at each point each is the unique scalar multiplying the same nonzero intrinsic area form to give the specified two-form. Thus the quotients define unique global smooth real functions for arbitrary two-forms on $S$, without an ambient spacetime. [given, F1, F2, algebra]

2.1 If $h(p)>0$ at some point, continuity gives a coordinate neighborhood on which $h\ge c>0$. Its coordinate image contains a closed rectangle $Q$ with finite endpoints and strictly positive side lengths, so $0<\lambda_2(Q)<\infty$ by [F12]. By [F7], $Q$ is compact and the smooth strictly positive chart density $\rho_x$ of $\mu$ has a positive minimum $m$ on $Q$. The chart preimage $R$ of $Q$ is closed in the open chart domain $U$; thus $R=U\setminus V$ for some open $V$ in $S$, making $R$ Borel by [F8]. By [F11], [F3] and [F9], $\mu(R)=\int_Q\rho_x\,d\lambda_2\ge m\lambda_2(Q)>0$. Monotonicity gives $\int_Sh\,d\mu\ge c\mu(R)>0$, a contradiction. Hence $h=0$ everywhere, and its two nonnegative square terms give $e=1$ and $b=0$ pointwise. [given, step 1.1, F3, F4, F7, F8, F9, F11, F12, algebra]

2.2 If $S$ is empty all convergence assertions are immediate; otherwise, around each point choose a positive chart and an open coordinate rectangle whose closed rectangle is contained in the chart image. These open patches cover $S$, so [F4] gives finitely many of them. Each closed rectangle is compact by [F7], and its inverse chart image is compact by the continuous-image assertion of [F7]. On each closed rectangle, the continuous positive $v$ has a positive minimum by [F7]; all limiting metric and form coefficients are bounded there by the same fact. Uniform convergence of the metric coefficients implies uniform convergence of their determinants, hence $v_j\to v$ uniformly, with $v_j$ eventually bounded away from zero. The assumed coefficient convergence and the formulas of step 1.2 therefore give $e_j\to e$ and $b_j\to b$ uniformly on each patch and then on $S$. The global ratio $r_j=v_j/v=d\mu_{q_j}/d\mu_q$ converges uniformly to $1$. Consequently $r_j$, $e_jr_j$, $b_jr_j$, and $(e_j^2+b_j^2)r_j$ converge uniformly to $1$, $e$, $b$, and $e^2+b^2$, respectively. [given, F1, F2, F4, F5, F7, step 1.2, algebra]

3.1 The fixed measure $\mu_q(S)$ is finite: on each closed coordinate rectangle $Q$ of the finite cover in step 2.2, [F7] bounds the local density $v$ above by a finite $M>0$. Its inverse chart image $R$ is Borel as in step 2.1, and [F11], [F12], [F3] and [F9] give $\mu_q(R)=\int_Qv\,d\lambda_2\le M\lambda_2(Q)<\infty$. These finitely many sets cover $S$, so finite subadditivity in [F13] gives $\mu_q(S)<\infty$. The functions in the four global pairs in step 2.2 and their differences are continuous, hence bounded and Borel measurable by [F7] and [F8]. The finite-measure argument of step 1.1 makes them integrable for $\mu_q$ and, likewise, for each $\mu_{q_j}$, whose total mass is finite by the same finite-cover argument. The coordinate identity $v_j=r_jv$ gives the measure identity $d\mu_{q_j}=r_jd\mu_q$: on each Borel subset of a chart, [F11] and [F10] identify both measures with the integral of $r_jv=v_j$ against $\lambda_2$, and a finite disjoint Borel refinement of the chart cover gives the identity globally. For each pair $u_j,u$ among the four uniformly convergent pairs in step 2.2, linearity, the integral triangle inequality and monotonicity give $|\int_Su_j\,d\mu_q-\int_Su\,d\mu_q|\le\mu_q(S)\sup_S|u_j-u|\to0$. Applying [F10] to the nonnegative integrands, and separately to the positive and negative parts of the signed integrands using [F9], rewrites these integrals as area, the two flux integrals and the squared-density integral for $\mu_{q_j}$. This proves all claimed integral limits. [F2, F3, F7, F8, F9, F10, F11, F12, F13, step 1.1, step 2.1, step 2.2, algebra]

4.1 No derivative of a two-form coefficient was used in steps 1.2–3.1. For continuous two-forms, meaning alternating covector fields with continuous coefficients in smooth coordinate frames, the pointwise basis in [F6] gives unique coefficients $a_j,c_j,a,c$; these are continuous by the stated meaning of continuity in a coordinate frame. Division by the smooth positive $v_j,v$ gives continuous density quotients, and uniqueness again makes them agree on overlaps. Uniform coefficient convergence therefore gives exactly the same uniform bounds and integral limits. In particular the claimed smooth-metric and continuous-two-form convergence case follows. [F2, F5, F6, step 1.2, step 2.2, step 3.1] ∎


## Gradient Hölder control by differentiated flux and one-dimensional lifting

[Open item](item-lem-author-db87cb8e0bab-divergence-gradient-holder) · level 0


### Statement

Let $P(y,p)$ be a smooth flux on a coordinate ball times $|p|\le p_0$; assume $P_p$ symmetric with $\lambda I\le P_p\le\Lambda I$ and $|P_y|\le K$. Let $w$ be a smooth scalar solution of $\operatorname{div}P(y,Dw)=0$ with $|Dw|\le p_0$. On each strictly smaller ball there exist $0<\beta<1$ and $C$, depending only on dimension, ellipticity, $K,p_0$ and the interior separation, such that $\|Dw\|_{C^{0,\beta}}\le C$. No uniform second-derivative bound is assumed.

### Facts & Assumptions

[F1] Hölder norms and classical derivatives are as in the Euclidean interface. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F2] On an open Euclidean set, $H^1=W^{1,2}$ consists of almost-everywhere classes of square-integrable functions with square-integrable first weak derivatives; use the real scalar case here. [math:def-hk-and-hk-zero-notation](https://alphabetamath.cc/item/def-hk-and-hk-zero-notation)

[F3] For a bounded measurable uniformly elliptic real matrix $B$ on an open set $U$, the homogeneous local weak equation $\operatorname{div}(B Du)=0$ means $u\in H^1(U)$ and $\int_U (B Du)\cdot D\varphi=0$ for every $\varphi\in C_c^\infty(U)$; this is the supplier convention with operator $-\operatorname{div}(B D)$, zero lower-order coefficients and zero datum, without a boundary condition. [math:def-local-weak-solution-for-a-divergence-form-operator](https://alphabetamath.cc/item/def-local-weak-solution-for-a-divergence-form-operator)

[A1] Work in ZFC, including choice for the imported analytic input and the Countable Choice assumptions of the Sobolev and weak-solution interfaces. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F20] Use the scalar homogeneous divergence-form De Giorgi–Nash estimate from Theorem 3.17 as recorded in External input, in one additional Euclidean dimension.

### Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the asserted estimate with the stated uniform dependence.

1.1 For each $k$, put $z=D_kw$, $a(y)=P_p(y,Dw(y))$ and $F(y)=-P_{y_k}(y,Dw(y))$, with $P_{y_k}$ the partial derivative at fixed $p$. Differentiating the flux equation gives $\operatorname{div}(a Dz)=\operatorname{div}F$. The matrix $a$ is measurable, symmetric and uniformly elliptic, $|z|\le p_0$ and $|F|\le K$. Smoothness justifies the differentiation without any uniform Hessian estimate. [given, F1, algebra]

2.1 Write $n$ for the coordinate dimension. Here is a local reduction of this inhomogeneous equation to the exact homogeneous source statement. If $M=\|z\|_\infty+\|F\|_\infty$ is zero there is nothing to prove. Otherwise put $Z(y,t)=z(y)/M+t$ and $H=F/M$. On a cylinder strictly inside the coordinate ball times $(-1,1)$ use the symmetric matrix $B=\begin{pmatrix}a&-H\\-H^T&L\end{pmatrix}$, where $L=1+2/\lambda$. Its quadratic form is at least $(\lambda/2)|\xi|^2+|\tau|^2$, since $|H|\le1$ and $2|\tau H\cdot\xi|\le(\lambda/2)|\xi|^2+(2/\lambda)\tau^2$. It has a uniform upper bound too. Direct distributional differentiation, using independence of $t$, gives $\operatorname{div}_{y,t}(B DZ)=\operatorname{div}_y(a Dz/M-H)=0$. [step 1.1, given, algebra]

3.1 Let $U$ be any $(n+1)$-dimensional ball with closure in this cylinder. The smooth function $Z$ and all its first classical derivatives are bounded on $\overline U$, so they are square-integrable on $U$; integration by parts against compactly supported tests identifies these classical derivatives as its weak derivatives. Thus $Z\in H^1(U)$, without requiring a uniform bound on its $H^1$ norm. For each $\varphi\in C_c^\infty(U)$, integration by parts in the divergence identity of step 2.1 gives $\int_U (B DZ)\cdot D\varphi=0$. Hence $Z$ is a scalar homogeneous weak solution with exactly the convention and coefficient hypotheses needed in F20. [step 2.1, F2, F3, F20, A1, algebra]

4.1 Apply the imported homogeneous theorem in dimension $n+1$ on the balls of step 3.1, after translation and dilation to the unit ball. Since $|Z|$ has a universal bound on the fixed cylinder, its $L^2$ norm is uniformly bounded on each such ball. Restrict the resulting Hölder estimate to $t=0$ and multiply by $M$. A finite cover of every smaller coordinate ball yields $\|z\|_{C^{0,\beta}}\le C(\|z\|_\infty+\|F\|_\infty)$. Doing this for the finitely many $k$ proves the assertion. The exponent may be decreased below one; no value of the prescribed later Schauder exponent is assumed here. [F20, A1, step 3.1, F1] ∎

### External input

[F20] Imported established input: For a weak solution $z\in H^1(B_1)$ of $\operatorname{div}(A Dz)=0$, with measurable symmetric matrix $\lambda I\le A\le\Lambda I$, there are $\beta>0$ and $C$ depending only on dimension and ellipticity such that $\|z\|_{C^{0,\beta}(B_{1/2})}\le C\|z\|_{L^2(B_1)}$. Scalar real-valued weak solution on a Euclidean ball; bounded measurable uniformly elliptic coefficients; the symmetric case suffices here. Used in dimension $n+1$ for an $n$-dimensional coordinate ball after a local lifting, not directly on the nonlinear graph equation. Reading limits: Checked the extracted statement, hypotheses and immediate proof note of Theorem 3.17 on printed p. 93 (PDF p. 99) in the author-hosted PDF. The underlying De Giorgi–Nash argument was not read or reconstructed. The local lifting, weak-solution verification and graph application are authored here.


## Linear fourth derivative bound with controlled realized coefficients

[Open item](item-lem-author-db87cb8e0bab-linear-fourth-derivative-estimate) · level 0


### Statement

Work in ZFC. Let $n\ge2$ be an integer, $0<\alpha<1$, and let $A',A\subset\mathbb R^n$ be fixed bounded Euclidean annuli with $\overline{A'}\subset A$. Let $z$ be smooth on $A$ and solve $Lz=a^{ij}z_{ij}+b^jz_j+cz=f$, with summation over $i,j=1,\dots,n$. Suppose $a$ is symmetric and $\lambda|\xi|^2\le a^{ij}(x)\xi_i\xi_j\le\Lambda|\xi|^2$ for all $x\in A$ and $\xi\in\mathbb R^n$, where $0<\lambda\le\Lambda<\infty$. Suppose every component of $a,b,c$ has $C^{2,\alpha}(A)$ norm at most $M<\infty$, and $f\in C^{2,\alpha}(A)$. Then
$$\|z\|_{C^{4,\alpha}(A')}\le C\bigl(\|z\|_{L^\infty(A)}+\|f\|_{C^{2,\alpha}(A)}\bigr).$$
Here $C$ depends only on $n,\alpha,\lambda,\Lambda,M$ and the fixed annular geometry, including the positive separation $\operatorname{dist}(\overline{A'},\partial A)$. The coefficients are the realized functions of position, even if originally obtained by evaluating a nonlinear operator at $z,Dz$; their stated bounds must hold as functions of position. In particular the same $C$ works for any family with these common bounds.

### Facts & Assumptions

[F1] The interior linear Schauder estimate applies on a ball to a bounded classical solution of a uniformly elliptic equation with controlled $C^{0,\alpha}$ coefficients, including first-order and zeroth-order terms. Its constant depends only on dimension, exponent, ellipticity and the stated scaled coefficient bounds. [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations)

[F2] Use the Euclidean Hölder norms and their scaled ball versions. The product estimate needed below follows directly from $p(x)q(x)-p(y)q(y)=p(x)(q(x)-q(y))+q(y)(p(x)-p(y))$: $[pq]_{0,\alpha}\le\|p\|_\infty[q]_{0,\alpha}+\|q\|_\infty[p]_{0,\alpha}$. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F3] The repeated-index expression $L=a^{ij}\partial_i\partial_j+b^j\partial_j+c$ and the constants $\lambda,\Lambda$ have the uniformly elliptic nondivergence-operator convention. Differentiating the equation keeps this same principal operator. [math:def-uniformly-elliptic-nondivergence-operator](https://alphabetamath.cc/item/def-uniformly-elliptic-nondivergence-operator)

[A1] Work in ZFC. Full Choice implies the Countable Choice assumed by the Schauder supplier; that implication is the use of Choice in each invocation of [F1]. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the asserted estimate with the stated uniform dependence.

1.1 If $\|z\|_{L^\infty(A)}$ is infinite, the claimed inequality is automatic in the extended sense, so assume it finite and put $N=\|z\|_{L^\infty(A)}+\|f\|_{C^{2,\alpha}(A)}$. Fix intermediate open sets with $A'\Subset U_2\Subset U_1\Subset A$, where $V\Subset W$ means $\overline V$ is compact and contained in $W$. For any of these three successive inclusions, positive separation allows balls of a common fixed radius centered in the smaller set and contained in the larger set. Apply [F1] on these balls and convert its scaled norms to ordinary norms. The local derivative bounds give the global suprema on the smaller set. For Hölder quotients, pairs closer than half a target-ball radius lie in one target ball; separated pairs are bounded by twice the derivative supremum divided by that fixed distance to the power $\alpha$. A finite cover of the compact closure gives the same bounds, with constants depending only on the fixed geometry. The coefficient $C^{0,\alpha}$ bounds needed on each ball follow from the assumed $C^{2,\alpha}$ bounds and the derivative bounds on that convex ball. Consequently [F1] applied to $Lz=f$ gives $\|z\|_{C^{2,\alpha}(U_1)}\le CN$. [F1, F2, F3, A1, given, algebra]

2.1 Differentiate once in coordinate $k$. The equation is $Lz_k=f_k-a^{ij}_kz_{ij}-b^j_kz_j-c_kz$. On the balls contained in $U_1$, its right-hand side has $C^{0,\alpha}$ norm at most $CN$ by step 1.1, the coefficient bounds and the product estimate [F2]. Also $\|z_k\|_{L^\infty(U_1)}\le CN$. Applying [F1] with the same elliptic operator and assembling the ball estimates as in step 1.1 yields $\|z\|_{C^{3,\alpha}(U_2)}\le CN$. [step 1.1, F1, F2, F3, A1, given, algebra]

3.1 Differentiate twice. The equation for $z_{k\ell}$ has the same left-hand operator $L$ and right-hand side $f_{k\ell}-a^{ij}_{k\ell}z_{ij}-a^{ij}_kz_{ij\ell}-a^{ij}_\ell z_{ijk}-b^j_{k\ell}z_j-b^j_kz_{j\ell}-b^j_\ell z_{jk}-c_{k\ell}z-c_kz_\ell-c_\ell z_k$. On balls contained in $U_2$ its $C^{0,\alpha}$ norm is at most $CN$ by step 2.1, [F2] and the coefficient bounds; the same bound holds for $\|z_{k\ell}\|_\infty$. Apply [F1] to every $z_{k\ell}$ and assemble the estimates on $A'$ by step 1.1. This bounds $z$ in $C^{4,\alpha}(A')$ by $CN$. All constants depend only on the listed geometry, dimension, exponent, ellipticity and realized coefficient bounds, so the asserted family uniformity follows. [step 1.1, step 2.1, F1, F2, F3, A1, given, algebra] ∎


## Compact-domain comparison with a nonnegative potential

[Open item](item-lem-author-58255dfd955f-compact-comparison) · level 0


### Statement

Let $D$ be a relatively compact smooth domain in a smooth Riemannian manifold $(M,h)$, with $\overline C\cap\partial D\ne\varnothing$ for each connected component $C$ of $D$. Here $N=\overline D$ is the smooth compact closure of the domain, regarded as an embedded full-dimensional manifold with boundary, and $\partial D=\partial N$ is its intrinsic manifold boundary. The smooth-domain convention includes $N\setminus D\subseteq\partial N$. The ambient manifold $M$ may have boundary; put $\Omega=D\cap M^\circ$. Points inherited from $\partial M$ belong to $\partial N$, as verified below. Let $V\ge0$ be bounded and smooth, and $w\in C^2(D)\cap C^1(\overline D)$ be real. Use the positive-divergence convention $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. If $(\Delta_h-V)w\ge0$ on $\Omega$ and $w\le0$ on $\partial D$, then $w\le0$ in $D$. Equivalently, supersolutions dominate subsolutions with ordered boundary data for this operator, when their difference has the stated regularity. Work in ZFC.

### Facts & Assumptions

**Given:** The Riemannian manifold and Laplacian are those of [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) and [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian). Write $v_\epsilon=(w-\epsilon)^+=\max(w-\epsilon,0)$ for $\epsilon>0$. We assume [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice), hence Countable Choice, for the partition and Sobolev suppliers below.

[F1] In an interior chart of dimension $n\ge1$, put $m=\sqrt{\det(h_{ij})}$, $A^{ij}=mh^{ij}$ and $q=mV$. The gradient formula in [math:def-riemannian-gradient](https://alphabetamath.cc/item/def-riemannian-gradient), the divergence formula in [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence), and the trace-of-Hessian convention give $\Delta_hw=m^{-1}\partial_i(A^{ij}\partial_jw)$. These suppliers state smooth-input formulas; step 1.2 verifies their use for $C^2$ functions. The Riemannian density is $d\mu_h=m\,dx$ by [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density); it requires no orientation.

[F2] Under Countable Choice, [math:thm-smooth-partitions-of-unity-exist-on-manifolds](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds) supplies a nonnegative, locally finite smooth partition subordinate to a cover of $\Omega$ by coordinate balls $U=x^{-1}(B)$, where $x:O\to x(O)$ is an interior chart and $B\subset\mathbb R^n$ is a bounded open ball with $\overline B\subset x(O\cap\Omega)$. Thus $\overline U$ is compact and contained in the larger chart $O$ and in $\Omega$. Only finitely many partition supports meet any fixed compact subset. A square partition suitable for the particular cutoff tests is constructed in step 3.1.

[F3] We use real $H^1=W^{1,2}$ classes with weak coordinate derivatives as in [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm) and [math:def-hk-and-hk-zero-notation](https://alphabetamath.cc/item/def-hk-and-hk-zero-notation). On each coordinate ball $U=x^{-1}(B)$ in [F2], the coordinate representative $w\circ x^{-1}$ belongs to $H^1(B)$. Indeed, this function and its coordinate first derivatives extend continuously to the compact set $\overline B$ inside $x(O\cap\Omega)$ and are therefore bounded there. Since $B$ is bounded it has finite Lebesgue measure, so these functions are square integrable; classical integration by parts against compactly supported smooth tests identifies the weak derivatives. The supplier [math:lem-positive-part-is-an-admissible-weak-test-by-truncation](https://alphabetamath.cc/item/lem-positive-part-is-an-admissible-weak-test-by-truncation) gives $Dv_\epsilon=\mathbf 1_{\{w>\epsilon\}}Dw$ almost everywhere and admissibility of $\eta^2v_\epsilon$ for $\eta\in C_c^\infty$ in the local weak inequality when its source is $L^2_{\mathrm{loc}}$. We use exactly these compactly supported tests, with source $-qw$, which is continuous and hence locally square integrable. No trace characterization or general boundary-test assertion is needed.

[F4] By [math:thm-zero-weak-gradient-implies-componentwise-constancy](https://alphabetamath.cc/item/thm-zero-weak-gradient-implies-componentwise-constancy), under AC an element of $W^{1,2}_{\mathrm{loc}}(G)$ with all weak derivatives zero on an open Euclidean set $G\subseteq\mathbb R^n$, $n\ge1$, is almost everywhere constant on each component. For our continuous truncation, this gives pointwise local constancy on coordinate balls in $\Omega$; step 4.1 explains its extension to $D$ using the boundary condition.

### Proof

**Given:** The hypotheses of the Statement and the suppliers in Facts & Assumptions.

**Goal:** Prove the compact-domain maximum and comparison assertions.

**Proof technique:** direct.

1.1 If $D$ is empty the assertion is vacuous. In dimension zero the manifold is discrete, so each component of $D$ is a closed singleton and cannot have closure meeting $\partial D$; thus the hypotheses force $D$ to be empty. In positive dimension, $N\cap\partial M\subseteq\partial N$. Indeed, if an ambient-boundary point were an intrinsic interior point of $N$, an ambient boundary coordinate $r\ge0$ would restrict to a smooth function on an open neighborhood in $N$ with an interior minimum zero. Its differential there would vanish. But the inclusion of the full-dimensional embedded $N$ has an invertible tangent map, so the nonzero differential $dr$ of that boundary coordinate would restrict to a nonzero differential, a contradiction. Hence $D\setminus\Omega\subseteq\partial D$, and $N\setminus\partial D\subseteq\Omega$ by the smooth-domain convention. [given, algebra]

1.2 Fix an interior point $p\in\Omega$ and replace $w$ in its coordinates by the polynomial with the same value and first and second derivatives at $p$. Metric duality gives $(\operatorname{grad}_hw)^i=h^{ij}\partial_jw$. Its first derivatives depend only on the two-jet of $w$, so the trace of its covariant derivative agrees at $p$ with that of the smooth polynomial. The density-divergence formula for a $C^1$ vector field follows likewise by replacing its coordinate coefficients by affine functions with the same one-jet. Consequently the smooth formulas in [F1] imply $\Delta_hw=m^{-1}\partial_i(A^{ij}\partial_jw)$ for the stated $C^2$ function in every interior chart. [F1, given, algebra]

2.1 In a coordinate ball $U=x^{-1}(B)$ as in [F2], the differential inequality becomes $-\partial_i(A^{ij}\partial_jw)+qw\le0$. Multiply by a nonnegative $\varphi\in C_c^\infty$ and integrate in chart coordinates. Each product $A^{ij}\partial_jw\,\varphi$ is $C^1$ and compactly supported, so extension by zero and one-dimensional integration of its $i$th derivative give $\int(A^{ij}\partial_jw\partial_i\varphi+qw\varphi)\,dx\le0$. This has local source $-qw\in L^2_{\mathrm{loc}}$. Thus [F3] extends it to each nonnegative test $\varphi=\eta^2v_\epsilon$, with the stated truncation and product derivative formulas. All tests are supported in the interior, so no manifold-boundary integration or boundary-chart approximation occurs. [F2, F3, step 1.2, given, algebra]

3.1 Fix $\epsilon>0$. The set $K=\{x\in\overline D:w(x)\ge\epsilon\}$ is compact and disjoint from $\partial D$, so step 1.1 gives $K\subset\Omega$ and $\operatorname{supp}v_\epsilon\subseteq K$ (support taken in $N$). If $K$ is empty then $v_\epsilon=0$. Otherwise take a locally finite partition $(\chi_a)$ from [F2], subordinate to the coordinate balls $U=x^{-1}(B)$ of [F2], and put $s=(\sum_a\chi_a^2)^{1/2}$ and $\eta_a=\chi_a/s$. The locally finite sum is smooth and strictly positive because $\sum_a\chi_a=1$; each $\eta_a$ is smooth, has compact support in its chart, and $\sum_a\eta_a^2=1$. Only finitely many supports meet $K$. Apply step 2.1 with each corresponding $\eta_a^2v_\epsilon$ and sum. With the density from [F1] the result is $\int_\Omega(\langle\nabla_hw,\nabla_hv_\epsilon\rangle_h+Vwv_\epsilon)\,d\mu_h\le0$: the terms containing partition derivatives cancel because $\sum_a\nabla_h(\eta_a^2)=0$ near $K$, and $v_\epsilon$ and its weak derivatives vanish off $K$. [F1, F2, F3, step 1.1, step 2.1, algebra, construct]

4.1 The integrand in step 3.1 equals $\mathbf 1_{\{w>\epsilon\}}|\nabla_hw|_h^2+Vwv_\epsilon$ almost everywhere. Both terms are nonnegative, so the weak gradient of $v_\epsilon$ is zero almost everywhere. On each coordinate ball $U=x^{-1}(B)$ of [F2], smooth positive definiteness and the positive density imply equivalence with zero Euclidean weak derivatives. Apply [F4] on that ball. Its almost everywhere constant value is its value everywhere by continuity of $v_\epsilon$, since every nonempty coordinate ball has positive measure. Thus $v_\epsilon$ is locally constant on $\Omega$. At any $q\in D\setminus\Omega$, step 1.1 places $q$ in $\partial D$, so $w(q)\le0<\epsilon$. Continuity supplies a relative neighborhood of $q$ in $D$ on which $w<\epsilon$, and $v_\epsilon=0$ there. Consequently $v_\epsilon$ is locally constant on all of $D$, and connectedness makes it a single constant on each component $C$. Choose $p\in\overline C\cap\partial D$; continuity on $\overline D$ and $w(p)\le0$ show that this constant is $v_\epsilon(p)=0$. Hence $v_\epsilon=0$ throughout $D$ for every $\epsilon>0$, and $w\le0$. For a subsolution $u_-$ and supersolution $u_+$ satisfying $(\Delta_h-V)u_-\ge0$, $(\Delta_h-V)u_+\le0$ and ordered boundary values, apply the established assertion to $w=u_--u_+$, whose operator and boundary signs are exactly those required. [F2, F3, F4, step 1.1, step 3.1, given, algebra] ∎


## Imported unit-ball Harnack inequality with bounded potential

[Open item](item-thm-author-58255dfd955f-bounded-potential-harnack-input) · level 0


### Statement

Let $n\ge2$. On $B_1\subset\mathbb R^n$, let $A$ be real measurable symmetric with $\xi^TA\xi\ge|\xi|^2$ and $\sum_{i,j}|A^{ij}|\le\Lambda$, and let $Q_0$ be real measurable with $0\le Q_0\le Q$. A nonnegative weak solution $v\in W^{1,2}(B_1)$ of $-\operatorname{div}(A\nabla v)+Q_0v=0$ satisfies $\operatorname{ess\,sup}_{B_{1/2}}v\le C\operatorname{ess\,inf}_{B_{1/2}}v$, with $C$ depending only on $n,\Lambda,Q$.

### Facts & Assumptions

**Given:** Work in ZFC, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice); this includes the countable choice assumed by the formulation suppliers below. The open ball is Euclidean.

[F1] Use $W^{1,2}(B_1;\mathbb R)$ as the space of almost-everywhere classes with square-integrable weak first derivatives from [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm). The gradient $\nabla v$ consists of the weak derivatives in [math:def-weak-derivative-of-a-locally-integrable-function](https://alphabetamath.cc/item/def-weak-derivative-of-a-locally-integrable-function); $v\ge0$ means almost everywhere.

[F2] All null sets and integrals use Lebesgue measure $\lambda_n$ from [math:def-lebesgue-measure-and-the-lebesgue-sigma-algebra](https://alphabetamath.cc/item/def-lebesgue-measure-and-the-lebesgue-sigma-algebra). Measurability of each real coefficient on $B_1$ means that its extension by zero to $\mathbb R^n$ is Lebesgue measurable in the sense of [math:def-borel-and-lebesgue-measurable-function-on-rn](https://alphabetamath.cc/item/def-borel-and-lebesgue-measurable-function-on-rn). Coefficient bounds are understood almost everywhere.

[F3] A weak solution means $\int_{B_1}(A\nabla v\cdot\nabla\varphi+Q_0v\varphi)\,d\lambda_n=0$ for every real smooth function $\varphi$ compactly supported in $B_1$. For measurable $E\subseteq B_1$, set $\operatorname{ess\,sup}_E v=\inf\{a\in\mathbb R:\lambda_n(\{x\in E:v(x)>a\})=0\}$ and $\operatorname{ess\,inf}_E v=\sup\{a\in\mathbb R:\lambda_n(\{x\in E:v(x)<a\})=0\}$, with extended-real infimum and supremum conventions. These expressions ignore changes on null sets.

[F4] The independent Simon reference supplies the analytic Harnack conclusion with the coefficient and weak-solution hypotheses in External input. It is imported, rather than proved locally.

### External input

Let $n\ge2$. On $B_1\subset\mathbb R^n$, let $A$ be real measurable symmetric with $\xi^TA\xi\ge|\xi|^2$ and $\sum_{i,j}|A^{ij}|\le\Lambda$, and let $Q_0$ be real measurable with $0\le Q_0\le Q$. A nonnegative weak solution $v\in W^{1,2}(B_1)$ of $-\operatorname{div}(A\nabla v)+Q_0v=0$ satisfies $\operatorname{ess\,sup}_{B_{1/2}}v\le C\operatorname{ess\,inf}_{B_{1/2}}v$, with $C$ depending only on $n,\Lambda,Q$.


## Compact sets admit relatively compact open neighborhoods and finite chart pieces

[Open item](item-lem-author-89004136b63c-compact-neighborhood-localization) · level 0


### Statement

Let $B$ be an open subset of a smooth Hausdorff manifold without boundary, and let $Q\subset B$ be compact. There are open sets $V,W$ with $Q\subset V$, $\overline V\subset W$ and $\overline W$ compact and contained in $B$. Every compact $K\subset B$ is covered by finitely many compact sets $K_j$ each contained in one smooth coordinate chart. Here closures are in the ambient manifold; a relatively compact set has compact closure.

### Statement references

[math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[math:lem-coordinate-balls-form-a-basis-of-a-topological-manifold](https://alphabetamath.cc/item/lem-coordinate-balls-form-a-basis-of-a-topological-manifold)

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary)

[math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

[math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

### Facts & Assumptions

[F1] Compactness means finite subcovers, including the ambient-cover formulation. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[F2] In any topological manifold, every point has an open coordinate-ball neighborhood whose closure in that manifold is compact. We will apply this also with an open chart subdomain as the manifold. [math:lem-coordinate-balls-form-a-basis-of-a-topological-manifold](https://alphabetamath.cc/item/lem-coordinate-balls-form-a-basis-of-a-topological-manifold)

[F3] A smooth manifold has an underlying topological manifold and a specified maximal smooth atlas; a smooth chart is a member of that atlas. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[F4] A topological manifold without boundary is Hausdorff, second countable and locally Euclidean of fixed dimension. [math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary)

[F5] In a topological space, the closure of a set is the intersection of all closed sets containing it, hence its smallest closed superset. [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

[F6] Distinct points of a Hausdorff space have disjoint open neighborhoods. [math:def-hausdorff-space](https://alphabetamath.cc/item/def-hausdorff-space)

[F7] The open sets of a subspace are traces of ambient open sets, and its closed sets are traces of ambient closed sets. If the subspace is open, its relatively open subsets are also ambient open subsets. [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

### Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the conclusions in the Statement.

1.1 Write $M$ for the ambient Hausdorff manifold. We first record the compactness consequences used below. If $C$ is compact in an open subspace $D\subset M$, every ambient open cover restricts to an open cover in $D$, so $C$ is compact in $M$. Any compact $C\subset M$ is closed: for $x\notin C$, the open sets disjoint from some open neighborhood of $x$ cover $C$ by Hausdorff separation; take finitely many of these sets covering $C$ and intersect the corresponding finitely many neighborhoods of $x$. This gives a neighborhood of $x$ disjoint from $C$. A closed subset of a compact space is compact, since adjoining its open complement to an open cover gives a cover of the compact space and hence a finite subcover. [given, F1, F6, F7]

2.1 Let $p\in O$ with $O\subset M$ open, and choose a smooth chart $(U,\varphi)$ containing $p$. The open set $D=U\cap O$ is a topological manifold: it is Hausdorff and second countable as an open subspace, and restricting charts gives local Euclidean coordinates. Apply F2 to $D$ at $p$ to obtain an open $T\subset D$ containing $p$ with $C=\overline T^{\,D}$ compact in $D$. Since $D$ is open in $M$, $T$ is open in $M$. By step 1.1, $C$ is compact and closed in $M$, so the ambient closure $\overline T$ is contained in $C\subset D\subset O\cap U$ and is a closed subset of compact $C$, hence compact. Thus the closure lies in the prescribed open set and in the original smooth chart domain. [F1, F2, F3, F4, F5, F6, F7, step 1.1]

3.1 Apply step 2.1 with $O=B$. The family of all neighborhoods $T$ obtained there covers $Q$, so choose finitely many $T_1,\ldots,T_r$ covering $Q$ and put $W=\bigcup_{i=1}^r T_i$. It is open and contains $Q$. The closure of a finite union is the union of the closures, so $\overline W=\bigcup_{i=1}^r\overline{T_i}\subset B$. This union is compact: restrict any open cover to each compact member, take finitely many covering sets for each, and combine these finite lists. [F1, F5, step 2.1]

4.1 Repeat step 3.1 with the open set $W$ in place of $B$ to obtain an open $V$ containing $Q$ with compact $\overline V\subset W$. For a compact $K\subset B$, use step 2.1 and compactness to obtain finitely many open $T_j$ covering $K$ such that each compact $\overline{T_j}$ lies in a smooth chart domain $U_j$. Set $K_j=K\cap\overline{T_j}$. Each $K_j$ is closed in compact $K$, hence compact by step 1.1, and is contained in $U_j$; these sets cover $K$ because the $T_j$ do. If $Q$ is empty take $V=W=\varnothing$, and if $K$ is empty use the empty family of pieces. [F1, F3, F5, F7, step 1.1, step 2.1, step 3.1] ∎


## Compact timelike-length bounds restrict to open subdomains

[Open item](item-lem-author-89004136b63c-compact-length-restriction) · level 0


### Statement

Assume countable choice for the usual Lebesgue-measure convention. Let $g$ be a $C^2$ Lorentz metric on an open subset $B$ of a smooth four-manifold and let $N$ be a continuous timelike time-orientation field. Here $T_pB$ is the derivation tangent space. A $C^2$ Lorentz metric means an assignment of symmetric nondegenerate bilinear forms $g_p:T_pB\times T_pB\to\mathbb R$ of signature $(-,+,+,+)$ whose coefficients $g_{ij}=g(\partial_{x^i},\partial_{x^j})$ are $C^2$ in every smooth chart. A continuous timelike orientation field means an assignment $N_p\in T_pB$ with continuous coordinate components and $g_p(N_p,N_p)<0$. At each point it selects the timelike component containing $N_p$; future-directed nonzero causal vectors are the nonzero vectors in the closure of that component, equivalently $g_p(v,v)\le0$ and $g_p(v,N_p)<0$. The pointwise equivalence and its applicability to these regularities are justified below. For a continuous curve $c:[a,b]\to B$, at an interior time $t$ where a coordinate representative $x\circ c$ is differentiable, define its velocity by $\dot c(t)=\sum_{i=1}^4(x^i\circ c)^{\prime}(t)\,\partial_{x^i}|_{c(t)}\in T_{c(t)}B$. Both existence at that time and this vector are independent of the smooth chart, as proved below. In this item a future Lipschitz curve is a continuous curve $c:[a,b]\to B$, locally Lipschitz in coordinates, with nonzero future-directed velocity almost everywhere. For such a curve uniformly timelike in its chosen parameter, meaning $g(\dot c,\dot c)\le-\epsilon_c<0$ almost everywhere for one constant $\epsilon_c>0$, define $L_g(c)=\int_a^b\sqrt{-g(\dot c,\dot c)}\,dt$ using the nonnegative Lebesgue integral, with integrand zero on a measurable null set containing the exceptional times and the parameter endpoints. The value is independent of this null-set choice. Suppose each compact $C\subset B$ has a finite constant $L_C$ bounding $L_g(c)$ for all such curves with image in $C$. Every open $W\subset B$ inherits precisely the same property, with $g,N$ restricted to $W$. The constants are uniform over curves in each compact set, while $\epsilon_c$ may depend on the curve.

### Statement references

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:def-derivation-at-a-point-and-tangent-space](https://alphabetamath.cc/item/def-derivation-at-a-point-and-tangent-space)

[math:thm-coordinate-derivations-form-a-basis-of-the-tangent-space](https://alphabetamath.cc/item/thm-coordinate-derivations-form-a-basis-of-the-tangent-space)

[math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map)

[math:thm-coordinate-formula-for-the-differential](https://alphabetamath.cc/item/thm-coordinate-formula-for-the-differential)

[math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space)

[math:def-ck-and-multi-index-notation-in-several-variables](https://alphabetamath.cc/item/def-ck-and-multi-index-notation-in-several-variables)

[physics:def-lorentz-form-and-inertia](https://alphabetamath.cc/physics/item/def-lorentz-form-and-inertia)

[physics:def-causal-classification-of-lorentz-vectors](https://alphabetamath.cc/physics/item/def-causal-classification-of-lorentz-vectors)

[physics:def-time-orientation-and-future-causal-sets](https://alphabetamath.cc/physics/item/def-time-orientation-and-future-causal-sets)

[physics:lem-lorentz-form-has-orthonormal-basis](https://alphabetamath.cc/physics/item/lem-lorentz-form-has-orthonormal-basis)

[physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components)

[math:thm-cauchy-schwarz-finite](https://alphabetamath.cc/item/thm-cauchy-schwarz-finite)

[math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction)

[math:def-nonnegative-lebesgue-integral](https://alphabetamath.cc/item/def-nonnegative-lebesgue-integral)

[math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure](https://alphabetamath.cc/item/prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:thm-lebesgue-measure-is-a-complete-measure](https://alphabetamath.cc/item/thm-lebesgue-measure-is-a-complete-measure)

[math:thm-borel-sets-are-lebesgue-measurable](https://alphabetamath.cc/item/thm-borel-sets-are-lebesgue-measurable)

[math:thm-continuous-preimages-of-borel-sets-are-borel](https://alphabetamath.cc/item/thm-continuous-preimages-of-borel-sets-are-borel)

[math:thm-sequential-suprema-infima-limsup-liminf-and-pointwise-limits-are-measurable](https://alphabetamath.cc/item/thm-sequential-suprema-infima-limsup-liminf-and-pointwise-limits-are-measurable)

[math:thm-coordinatewise-measurability-into-r-n](https://alphabetamath.cc/item/thm-coordinatewise-measurability-into-r-n)

[math:thm-composition-with-borel-functions-preserves-measurability](https://alphabetamath.cc/item/thm-composition-with-borel-functions-preserves-measurability)

[math:def-measure-null-set-and-almost-everywhere](https://alphabetamath.cc/item/def-measure-null-set-and-almost-everywhere)

[math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)

[math:cor-integral-over-a-null-set-vanishes](https://alphabetamath.cc/item/cor-integral-over-a-null-set-vanishes)

[math:lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets](https://alphabetamath.cc/item/lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets)

[math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

### Facts & Assumptions

[F1] At each point the metric is a Lorentz form, timelike means $g_p(v,v)<0$, and causal means nonzero with $g_p(v,v)\le0$. A pointwise time orientation chooses a component of the timelike set; future causal vectors are the nonzero vectors in its closure. Here the chosen component contains $N_p$. These are definitions on a four-dimensional real vector space, with no smooth-field hypothesis. [physics:def-lorentz-form-and-inertia](https://alphabetamath.cc/physics/item/def-lorentz-form-and-inertia) [physics:def-causal-classification-of-lorentz-vectors](https://alphabetamath.cc/physics/item/def-causal-classification-of-lorentz-vectors) [physics:def-time-orientation-and-future-causal-sets](https://alphabetamath.cc/physics/item/def-time-orientation-and-future-causal-sets)

[F2] Compactness is intrinsic to the subspace topology. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[F3] Lipschitz continuity means a uniform distance-ratio bound in coordinates. The nonnegative integral is the supremum of the integrals of nonnegative simple minorants of a measurable integrand. [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction) [math:def-nonnegative-lebesgue-integral](https://alphabetamath.cc/item/def-nonnegative-lebesgue-integral)

[F4] An open subset carries the canonical smooth structure generated by restricted charts, independent of the presenting atlas. Apply this first to $B$ in the given four-manifold, and then to $W$ in $B$. [math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure](https://alphabetamath.cc/item/prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure)

[F5] Countable choice is assumed only for the standard Lebesgue-measure suppliers: Lebesgue measure is a complete measure and all Borel sets are Lebesgue measurable. These results apply in dimension one to the parameter variable. Restricting the measure and sigma-algebra to $[a,b]$ preserves these properties. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) [math:thm-lebesgue-measure-is-a-complete-measure](https://alphabetamath.cc/item/thm-lebesgue-measure-is-a-complete-measure) [math:thm-borel-sets-are-lebesgue-measurable](https://alphabetamath.cc/item/thm-borel-sets-are-lebesgue-measurable)

[F6] Continuous maps have Borel preimages of Borel sets. Sequential limsups of measurable functions are measurable. A finite-dimensional real map is measurable exactly when its coordinates are measurable, and composition of measurable maps is measurable. [math:thm-continuous-preimages-of-borel-sets-are-borel](https://alphabetamath.cc/item/thm-continuous-preimages-of-borel-sets-are-borel) [math:thm-sequential-suprema-infima-limsup-liminf-and-pointwise-limits-are-measurable](https://alphabetamath.cc/item/thm-sequential-suprema-infima-limsup-liminf-and-pointwise-limits-are-measurable) [math:thm-coordinatewise-measurability-into-r-n](https://alphabetamath.cc/item/thm-coordinatewise-measurability-into-r-n) [math:thm-composition-with-borel-functions-preserves-measurability](https://alphabetamath.cc/item/thm-composition-with-borel-functions-preserves-measurability)

[F7] An almost-everywhere condition holds outside a measurable null set containing all its exceptional points. In the curve class here, existence of the nonzero future-directed velocity almost everywhere is already required. [math:def-measure-null-set-and-almost-everywhere](https://alphabetamath.cc/item/def-measure-null-set-and-almost-everywhere)

[F8] The closed bounded parameter interval is compact and every open cover of it has a finite subcover. [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)

[F9] A nonnegative measurable function integrated over a measurable null set has integral zero. [math:cor-integral-over-a-null-set-vanishes](https://alphabetamath.cc/item/cor-integral-over-a-null-set-vanishes)

[F10] A $C^1$ map is locally Lipschitz in coordinates near a compact coordinate subset; for a chart transition one may take the compact set to be a singleton in the overlap. The total-derivative chain rule applies at each parameter where the coordinate curve is differentiable. [math:lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets](https://alphabetamath.cc/item/lem-a-c1-map-is-locally-lipschitz-on-compact-coordinate-subsets) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F11] A smooth manifold has a maximal smooth atlas, its tangent space consists of derivations at a point, and the coordinate derivations form a basis. A type $(0,2)$ tensor at a point is a bilinear map on that tangent space. In this item the metric's $C^2$ regularity and the field's continuity mean exactly the coordinate conditions in the Statement; $C^2$ coefficients have continuous iterated partial derivatives through order two. No smoothness of either field is assumed. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:def-derivation-at-a-point-and-tangent-space](https://alphabetamath.cc/item/def-derivation-at-a-point-and-tangent-space) [math:thm-coordinate-derivations-form-a-basis-of-the-tangent-space](https://alphabetamath.cc/item/thm-coordinate-derivations-form-a-basis-of-the-tangent-space) [math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space) [math:def-ck-and-multi-index-notation-in-several-variables](https://alphabetamath.cc/item/def-ck-and-multi-index-notation-in-several-variables)

[F12] The differential of a smooth map acts on derivations by precomposing germs, and its matrix in coordinate tangent bases is the Jacobian of its coordinate representative. These facts concern smooth maps of the underlying smooth manifolds, independently of metric regularity. [math:def-differential-of-a-smooth-map](https://alphabetamath.cc/item/def-differential-of-a-smooth-map) [math:thm-coordinate-formula-for-the-differential](https://alphabetamath.cc/item/thm-coordinate-formula-for-the-differential)

[F13] Every four-dimensional Lorentz form has an orthonormal basis. In such a basis the two timelike components are $v^0>|v_s|$ and $v^0<-|v_s|$, with closures $v^0\ge|v_s|$ and $v^0\le-|v_s|$; here $|v_s|=\sqrt{\sum_{i=1}^3(v^i)^2}$. These component and closure descriptions are independent of the orthonormal basis. The finite Cauchy-Schwarz inequality gives $|\sum_{i=1}^3 u^iv^i|\le|u_s||v_s|$. [physics:lem-lorentz-form-has-orthonormal-basis](https://alphabetamath.cc/physics/item/lem-lorentz-form-has-orthonormal-basis) [physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components) [math:thm-cauchy-schwarz-finite](https://alphabetamath.cc/item/thm-cauchy-schwarz-finite)

### Proof

**Given:** The hypotheses in the Statement, including countable choice for the Lebesgue-measure convention.

**Goal:** Establish the measurable length convention and the asserted restriction property.

1.1 Use [F11] and [F4] to equip $B$ and $W$ with their restricted smooth structures. A chart of the ambient manifold restricts first to $B$ and then to $W$; the resulting coordinate functions and transition maps are unchanged wherever defined. For the inclusion $W\hookrightarrow B$ the coordinate map is the identity on an open set, so its tangent map is the identity in these coordinates by [F12]. Consequently the restrictions of $g$ and $N$ have the same coefficient functions, signature, regularity and time orientation. This supplies the smooth-manifold and tangent identifications used below. [F4, F11, F12]

1.2 Fix $p$ and apply [F13] to the four-dimensional space $T_pB$ of [F11]. In an orthonormal basis write $N_p=(n^0,n_s)$, reversing the time basis vector if necessary so that $n^0>|n_s|$. The component containing $N_p$ is then $T_+$ of [F13]. If $v\in\operatorname{cl}(T_+)\setminus\{0\}$, then $v^0\ge|v_s|$ and $v^0>0$, so $g_p(v,N_p)=-v^0n^0+\sum_{i=1}^3v^in^i\le-v^0(n^0-|n_s|)<0$ by the finite Cauchy-Schwarz inequality in [F13]. On $\operatorname{cl}(T_-)\setminus\{0\}$ the pairing is positive by applying this calculation to $-v$. Every nonzero causal vector is in exactly one of those two closed cones by [F1] and [F13], proving the equivalence asserted in the Statement. All pairings are intrinsic evaluations of bilinear forms. Their coordinate expressions vary continuously with $p$ and the vector components because $g$ and $N$ have continuous coefficients. Thus the strict future inequality defines an open condition, restricted to the causal vectors, at precisely the stated regularities. The pointwise argument chooses a basis only at the fixed point; no field of bases, smooth orientation field, or stronger choice principle is used. [given, F1, F11, F13, algebra]

1.3 Let $t\in(a,b)$, put $p=c(t)$, and suppose $y\circ c$ is differentiable at $t$ in one smooth chart $y$ about $p$. For any other smooth chart $x$ about $p$, continuity of $c$ permits restriction to a parameter neighborhood whose image lies in the overlap. The transition $x\circ y^{-1}$ is smooth, so the Euclidean chain rule [F10] gives differentiability of $x\circ c$ at $t$ and $(x^i\circ c)^{\prime}(t)=\sum_{\alpha=1}^4 A^i_{\alpha}(y^{\alpha}\circ c)^{\prime}(t)$, where $A^i_{\alpha}=\partial(x^i\circ y^{-1})/\partial y^{\alpha}$ is evaluated at $y(p)$. Apply [F12] to the smooth identity map on the overlap, represented in these two charts, to obtain $\partial_{y^{\alpha}}|_p=\sum_i A^i_{\alpha}\partial_{x^i}|_p$. The coordinate basis in [F11] makes each proposed velocity a derivation in $T_pB$, and substitution gives $\sum_i(x^i\circ c)^{\prime}(t)\partial_{x^i}|_p=\sum_{\alpha}(y^{\alpha}\circ c)^{\prime}(t)\partial_{y^{\alpha}}|_p$. Interchanging the two charts proves equivalence of derivative existence as well as equality of the vectors. Thus the Statement defines an intrinsic velocity at every interior differentiability time. Here [F12] concerns the smooth identity map and [F10] concerns Euclidean maps differentiable at the one time under consideration. [given, F10, F11, F12, algebra]

1.4 Fix an eligible curve $c$. By local coordinate Lipschitz continuity, each parameter value has a relative open interval on which the image is in one chart and its coordinates satisfy one Lipschitz bound. Shrink such intervals to closed relative intervals $J_k$ whose relative interiors still cover $[a,b]$ and on each of which that chart and bound remain valid. By [F8] finitely many suffice. For each component $x^i$ of its coordinate curve on $J_k$, extend $x^i$ to $\mathbb R$ by keeping it constant beyond the two endpoints of $J_k$. The extension $\widetilde x^i$ is continuous and Lipschitz with the same bound. For integers $n\ge1$, the difference quotient $q_n^i(t)=n(\widetilde x^i(t+1/n)-\widetilde x^i(t))$ is continuous, hence Borel measurable by [F6], and Lebesgue measurable by [F5]. Its limsup $v_k^i$ is measurable by [F6] and finite everywhere because $|q_n^i|$ is bounded by that Lipschitz constant. At every interior parameter where $x^i$ is differentiable, $v_k^i=(x^i)'$. Choose a measurable null set $E$ containing the endpoints of these finitely many intervals and all exceptional times for the velocity and timelikeness conditions; such a set exists by [F7]. No differentiability theorem is being inferred from the Lipschitz definition: derivative existence almost everywhere is part of the stated curve class. The case $a=b$ has the zero integrand and zero integral. [given, F3, F5, F6, F7, F8]

2.1 On $J_k$, every coefficient $g_{ij}(c(t))$ in its chart is continuous, hence measurable by [F5] and [F6]. Combine these coefficients with the measurable finite coordinates $v_k^i$ into one measurable finite-dimensional map, using [F6]. The real function of these coefficients and coordinates given by $h_k(t)=\sqrt{\max\{0,-\sum_{i,j=1}^4g_{ij}(c(t))v_k^i(t)v_k^j(t)\}}$ is measurable: the map performing the displayed arithmetic, maximum and square root is continuous, so [F6] applies to its composition. Make a disjoint Borel partition by assigning each point to the first interval $J_k$ that contains it. Define $h=h_k$ on its assigned piece outside $E$ and $h=0$ on $E$. Each piece is measurable and there are finitely many, so preimages under this piecewise definition are finite unions of measurable sets. Thus $h$ is nonnegative measurable. Outside $E$, step 1.3 identifies the coordinate derivatives with the velocity defined in the Statement, and $g(\dot c,\dot c)<0$, so $h=\sqrt{-g(\dot c,\dot c)}$. For overlapping coordinates $x,y$, put $A^i_{\alpha}=\partial x^i/\partial y^{\alpha}$. By [F12] the coordinate tangent bases satisfy $\partial_{y^{\alpha}}=\sum_i A^i_{\alpha}\partial_{x^i}$. Bilinearity in [F11] gives $g^{(y)}_{\alpha\beta}=\sum_{i,j}A^i_{\alpha}A^j_{\beta}g^{(x)}_{ij}$. At each differentiability time outside $E$, the chain rule [F10] gives $\dot x^i=\sum_{\alpha}A^i_{\alpha}\dot y^{\alpha}$, hence $\sum_{\alpha,\beta}g^{(y)}_{\alpha\beta}\dot y^{\alpha}\dot y^{\beta}=\sum_{i,j}g^{(x)}_{ij}\dot x^i\dot x^j$. This derives the tensor transformation rule and the scalar's chart independence without differentiating $g$ or $N$. This establishes the claimed measurable length integrand with the stated null-set convention. [given, F5, F6, F7, F10, F11, F12, step 1.1, step 1.3, step 1.4]

3.1 Changing the chart intervals, their assignment, or the measurable exceptional null set gives another nonnegative measurable representative $h'$ equal to $h$ outside a measurable null set $Z$: take the union of the two exceptional sets and the finite interval endpoints. If $s$ is a nonnegative simple minorant of $h$, the function equal to $s$ off $Z$ and zero on $Z$ is a simple minorant of $h'$ with the same simple integral; its removed part is supported on $Z$ and has integral zero by [F9]. Taking the supremum over $s$ in [F3] gives $\int h\le\int h'$. Interchanging the representatives gives the reverse inequality. Hence the length is independent of all these auxiliary choices, including the measurable null set used for the zero values. [F3, F7, F9, step 2.1]

4.1 If $C\subset W$ is compact in $W$, the topology induced on $C$ from $W$ is the topology induced from $B$: both consist of the same iterated intersections of open sets with $C$. Thus $C$ is compact in $B$ by the intrinsic convention [F2]. The restricted atlas in step 1.1 gives exactly the same coordinate representatives of a curve into $C$ in either domain. Local coordinate Lipschitz continuity may be tested in this atlas: changing to any compatible chart composes with a smooth transition, which is locally Lipschitz by [F10]. The product of its local Lipschitz bound and that of the coordinate curve is a bound for the new coordinate representative. By step 1.2 the future condition is the pointwise pairing inequality at the given regularities. The velocity defined in the Statement is unchanged by this identification, since its coordinate derivatives and coordinate tangent bases agree by steps 1.1 and 1.3. The inequalities $g(\dot c,N)<0$ and $g(\dot c,\dot c)\le-\epsilon_c$ are unchanged under the identity tangent map. Choose the same chart intervals and exceptional set in step 2.1 for both domains; they give identical $h$ and therefore identical length. Step 3.1 removes dependence on that choice. [F2, F3, F10, step 1.1, step 1.2, step 1.3, step 2.1, step 3.1]

5.1 Apply the assumed bound $L_C$ in $B$ to each such curve into $C$. Step 4.1 shows that it is exactly an eligible curve in $B$ with the same length and the same individual constant $\epsilon_c$. The bound $L_C$ is therefore common to every eligible curve in $C$ in $W$, with no extra uniformity imposed on $\epsilon_c$. This proves the restriction property. [given, step 4.1] ∎


## Inversion is uniformly stable on compact chart families

[Open item](item-lem-author-89004136b63c-uniform-inverse-metric-continuity) · level 0


### Statement

Let $K_j$ be finitely many compact subsets of coordinate domains and let $G_j(x)$ be continuous invertible real $4\times4$ matrix fields there. Given $\eta>0$, there is $\delta>0$ such that any matrix fields $\widetilde G_j$ satisfying $\max_{a,b}|\widetilde G_{j,ab}(x)-G_{j,ab}(x)|<\delta$ on all $K_j$ are invertible there and satisfy $\max_{a,b}|(\widetilde G_j^{-1})^{ab}(x)-(G_j^{-1})^{ab}(x)|<\eta$. No derivatives of the perturbation enter this assertion.

### Statement references

[math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)

[math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[math:def-manifold-chart-coordinate-domain-and-coordinate-functions](https://alphabetamath.cc/item/def-manifold-chart-coordinate-domain-and-coordinate-functions)

[math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)

[math:cor-determinant-is-a-polynomial-in-the-matrix-entries](https://alphabetamath.cc/item/cor-determinant-is-a-polynomial-in-the-matrix-entries)

[math:thm-real-square-matrix-invertible-iff-determinant-nonzero](https://alphabetamath.cc/item/thm-real-square-matrix-invertible-iff-determinant-nonzero)

[math:lem-algebra-of-continuous-real-maps-on-a-space](https://alphabetamath.cc/item/lem-algebra-of-continuous-real-maps-on-a-space)

### Facts & Assumptions

[F1] If $U\subseteq\mathbb R^{16}$ is open and every matrix in $U$ has nonzero determinant, apply the matrix-inversion regularity lemma with $m=16$, $n=4$, $r=1$ to the identity matrix-valued map on $U$. Its entry functions have constant first partial derivatives, so inversion on $U$ is $C^1$, in particular continuous. [math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)

[F2] Compactness has its finite ambient-subcover meaning, including the indexed-cover version and the empty-set case. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[F3] A coordinate domain is open in its manifold; its chart image is open in Euclidean space. Continuity means that the inverse image of a neighborhood is a neighborhood, equivalently that each open target neighborhood contains the image of some open source neighborhood. Apply this definition to the matrix fields on their coordinate domains with the usual topology on their sixteen real entries. [math:def-manifold-chart-coordinate-domain-and-coordinate-functions](https://alphabetamath.cc/item/def-manifold-chart-coordinate-domain-and-coordinate-functions) [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)

[F4] For fixed finite size the determinant is a finite sum of signed products of entries, and a real square matrix is invertible exactly when its determinant is nonzero. [math:cor-determinant-is-a-polynomial-in-the-matrix-entries](https://alphabetamath.cc/item/cor-determinant-is-a-polynomial-in-the-matrix-entries) [math:thm-real-square-matrix-invertible-iff-determinant-nonzero](https://alphabetamath.cc/item/thm-real-square-matrix-invertible-iff-determinant-nonzero)

[F5] Finite sums and products of continuous real-valued maps on a topological space are continuous. [math:lem-algebra-of-continuous-real-maps-on-a-space](https://alphabetamath.cc/item/lem-algebra-of-continuous-real-maps-on-a-space)

### Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the conclusions in the Statement.

1.1 Identify $M_4(\mathbb R)$ with $\mathbb R^{16}$ and write $d_\infty(A,B)=\max_{a,b}|A_{ab}-B_{ab}|$. The inequalities $d_\infty(A,B)\le\|A-B\|_2\le4d_\infty(A,B)$ show that maximum-entry and Euclidean neighborhoods give the same topology. Each entry projection is continuous since its change is at most $d_\infty(A,B)$. Thus [F4] and [F5] make determinant continuous. At a matrix $A$ with nonzero determinant, continuity gives a neighborhood where $|\det B-\det A|<|\det A|/2$, so the determinant stays nonzero. By [F4], $\mathrm{GL}_4(\mathbb R)$ is therefore open, independently of inversion. [F3, F4, F5, algebra]

2.1 Apply [F1] to the open set $\mathrm{GL}_4(\mathbb R)$ from step 1.1. Inversion is continuous there, also for $d_\infty$. Consequently, for every invertible center matrix $A$ and the given $\eta>0$, some $r>0$ has the following property: $d_\infty(B,A)<2r$ implies that $B$ is invertible and $d_\infty(B^{-1},A^{-1})<\eta/2$. Indeed, intersect an open neighborhood of $A$ contained in $\mathrm{GL}_4(\mathbb R)$ with the inverse image under inversion of the radius-$\eta/2$ ball about $A^{-1}$, and take a sufficiently small ball in that intersection. [F1, F3, step 1.1]

3.1 For each coordinate domain $U_j$, use all pairs $(x,r)$ with $x\in K_j$ and $r>0$ satisfying step 2.1 for $A=G_j(x)$. The sets $V_{j,x,r}=\{y\in U_j:d_\infty(G_j(y),G_j(x))<r\}$ are open in $U_j$ by continuity of $G_j$ and cover $K_j$. This uses neighborhoods in the coordinate domain, without identifying that domain itself with a Euclidean open set. Using all admissible pairs requires no selection of a radius at every point. [given, F3, step 2.1]

4.1 If every $K_j$ is empty, take $\delta=1$. Otherwise, [F2] gives a finite indexed subcover of each nonempty $K_j$ from step 3.1. Set $\delta>0$ to the minimum of the associated finitely many positive radii over the finitely many $j$. For $y\in K_j$ choose a selected $V_{j,x,r}$ containing it. Then $d_\infty(G_j(y),G_j(x))<r$ and $d_\infty(\widetilde G_j(y),G_j(x))<\delta+r\le2r$. Step 2.1 makes both matrices invertible and puts both inverses within $\eta/2$ of $G_j(x)^{-1}$. The triangle inequality gives $d_\infty(\widetilde G_j(y)^{-1},G_j(y)^{-1})<\eta$. Empty sets impose no restriction, and no continuity or derivatives of the perturbation were used. [given, F2, step 2.1, step 3.1, algebra] ∎



## Finite smooth cutoffs relative to compact sets and boundary neighborhoods

[Open item](item-lem-author-423fe0348a31-finite-relative-cutoffs) · level 0


### Statement

On a compact smooth manifold with boundary $R$, let $K\subset V$ with $K$ compact and $V$ open. There is a smooth $\chi:R\to[0,1]$ equal to one on a neighborhood of $K$ and supported in $V$. If $K$ lies in the interior, the support may be compactly contained in the interior. Given finitely many coordinate neighborhoods covering a compact interior set $K$, there are finitely many smooth functions $\chi_j$ compactly supported in those neighborhoods with $\sum_j\chi_j=1$ near $K$.

### Facts & Assumptions

[F1] Support is the closure in $R$ of the nonzero locus. The manifold is Hausdorff, coordinate images are relatively open in a half-space, and smoothness at the boundary means local smooth Euclidean extension. [math:def-smooth-partition-of-unity-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-partition-of-unity-on-a-manifold-with-boundary) [math:def-topological-manifold-with-boundary](https://alphabetamath.cc/item/def-topological-manifold-with-boundary) [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:def-smooth-function-on-a-relatively-open-subset-of-a-half-space](https://alphabetamath.cc/item/def-smooth-function-on-a-relatively-open-subset-of-a-half-space)

[F2] For $n\ge1$ and $0<r<s$, there is a smooth $\rho:\mathbb R^n\to[0,1]$ equal to one on $\overline B_r(0)$ and supported in $B_s(0)$; translation gives the corresponding bump centered at any coordinate point. [math:lem-smooth-bump-between-concentric-euclidean-balls](https://alphabetamath.cc/item/lem-smooth-bump-between-concentric-euclidean-balls)

[F3] An indexed cover of a compact subset by ambient open sets has a finite subcover (claim 2), including the empty-set alternative. [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[F4] Closed bounded Euclidean sets are compact; metric and topological compactness agree. Continuous images of compact sets are compact (clause 1), and compact subsets of a Hausdorff space are closed (clause 3). Since $R$ is compact and Hausdorff, every closed subset of $R$ is compact (clause 4 of the Hausdorff compactness theorem). [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn) [math:thm-compactness-agrees-with-metric-compactness](https://alphabetamath.cc/item/thm-compactness-agrees-with-metric-compactness) [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps) [math:thm-compact-subset-of-a-hausdorff-space-is-closed](https://alphabetamath.cc/item/thm-compact-subset-of-a-hausdorff-space-is-closed)

[F5] Coordinate sum, product and quotient differentiation rules, iterated on smooth Euclidean extensions, preserve smoothness wherever the quotient denominator is nonzero. The half-space chain rule makes composition and change of boundary coordinates smooth. [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives) [math:prop-chain-rule-for-smooth-half-space-maps](https://alphabetamath.cc/item/prop-chain-rule-for-smooth-half-space-maps)

[F6] Write $R^\circ=\operatorname{Int}R$ for the manifold interior: in positive dimension its points have positive last boundary-chart coordinate, and in dimension zero every point is interior. For the smooth manifold with boundary $R$, this interior is open. [math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold) [math:thm-the-interior-is-an-open-smooth-n-manifold](https://alphabetamath.cc/item/thm-the-interior-is-an-open-smooth-n-manifold)

### Proof

**Given:** The hypotheses in the Statement.

**Goal:** Construct the asserted relative cutoff and a partition subordinate to the prescribed finite coordinate cover.

1.1 If $K=\varnothing$, take $\chi=0$ and take every function indexed by the prescribed finite coordinate cover to be zero; for an empty cover use the empty family. The required equalities near $K$ hold on the empty open neighborhood, and every support is empty. Henceforth suppose $K\ne\varnothing$. [given, F1, construct]

1.2 For an open neighborhood $W$ of a point $p$, take a boundary chart $\varphi:U\to O\subseteq\mathbb H^n$ and write $a=\varphi(p)$. In positive dimension choose $0<r<s$ with $\overline B_s(a)\cap\mathbb H^n\subseteq\varphi(U\cap W)$, using relative openness. By [F2] take a translated Euclidean bump equal to one on $\overline B_r(a)$ and supported in $B_s(a)$. Restrict it to $O$ and pull it back to $U$. The set $C=\varphi^{-1}(\overline B_s(a)\cap\mathbb H^n)$ is compact by [F4], closed in $R$, and contained in $U\cap W$. The pullback is zero on $U\setminus C$, so extension by zero on $R\setminus C$ is smooth: the two formulas agree on their open overlap, and the boundary-chart formula has a smooth ambient extension. Its support is closed in $R$, is therefore compact by [F4], lies in $C\subseteq W$, and it equals one on the open neighborhood $\varphi^{-1}(B_r(a)\cap\mathbb H^n)$ of $p$. In dimension zero, a singleton chart is open and closed, and its indicator is a smooth bump with that singleton as compact support. [F1, F2, F4, F5, construct]

2.1 Consider all the bumps and inner neighborhoods constructed in step 1.2 with $p\in K$ and $W=V$. Their inner neighborhoods form an indexed open cover of $K$; [F3] gives finitely many, with bumps $b_1,\ldots,b_N$. Set $\chi=1-\prod_{a=1}^N(1-b_a)$. This is smooth by the iterated product rule, takes values in $[0,1]$, and equals one on the union of the inner neighborhoods, since there one factor is zero. Its support lies in the finite union of the closed supports of the $b_a$, which is closed in $R$ and contained in $V$. Both this finite union and $\operatorname{supp}\chi$ are closed in compact Hausdorff $R$, hence compact by [F4]. If $K\subset R^\circ$, perform the same construction with $W=V\cap R^\circ$; the resulting support is compactly contained in $R^\circ$. This proves the first assertion and its interior refinement without taking a minimum or using a scalar cutoff. [given, F1, F3, F4, F5, F6, step 1.2, construct]

3.1 For the second assertion, write the prescribed coordinate neighborhoods as $U_1,\ldots,U_m$. Use all the local constructions of step 1.2 with $p\in K\cap U_j$ and $W=U_j\cap R^\circ$, retaining the index $j$. Their inner neighborhoods cover $K$, so [F3] gives finitely many bumps $b_a$, each with compact support in its assigned $U_{j(a)}\cap R^\circ$. Set $S=\sum_a b_a$ and $W_0=\{S>0\}\cap R^\circ$. This is open and contains $K$. Apply the already proved construction in step 2.1 with $V=W_0$ to obtain a smooth $\psi:R\to[0,1]$ equal to one near $K$ with compact support contained in $W_0$. [given, F1, F3, F5, F6, step 1.2, step 2.1, construct]

4.1 For $1\le j\le m$, define $\chi_j=\psi\bigl(\sum_{a:j(a)=j}b_a\bigr)/S$ on $W_0$, and set it to zero elsewhere; an empty numerator sum is zero. These functions are smooth on $W_0$ by [F5]. At every point outside $W_0$, the complement of the closed set $\operatorname{supp}\psi\subset W_0$ is a neighborhood on which both formulas are zero, proving smooth extension. Each $\chi_j$ is nonnegative and at most one. Its support lies in the intersection of $\operatorname{supp}\psi$ with the finite union of the supports assigned to $j$. This support is closed in $R$, so [F4] makes it compact; it is therefore compactly contained in $U_j\cap R^\circ$. Summing the formulas gives $\sum_j\chi_j=\psi$ on $W_0$, and both sides vanish off $W_0$. Thus the sum equals one near $K$, proving the second assertion. [F1, F4, F5, step 3.1, algebra] ∎



## Weak first derivatives and Riemannian chart norm comparison

[Open item](item-lem-author-423fe0348a31-chart-sobolev-comparison) · level 0


### Statement

Assume Countable Choice. Let $(R,k)$ be a smooth Riemannian manifold of dimension $n\ge0$, let $x:U\to\Omega\subseteq\mathbb R^n$ be an interior coordinate chart with compact closure in $R$, and fix a compact set $K\subset U$. For $n\ge1$, let $u\in W^{1,1}(\Omega;\mathbb R)$ vanish almost everywhere outside $x(K)$, and define $f=u\circ x$ on $U$, extended by zero to $R$. Here $u_i=D_i u$ are weak coordinate derivatives, $df=\sum_i(u_i\circ x)\,dx^i$ on $U$, and $df=0$ off $U$. These formulas define an almost-everywhere covector field independent of coordinates.

There are constants $0<c\le C<\infty$, depending on $K$, $x$, and $k$ but not on $u$, such that
$$c\|u\|_{W^{1,1}(\Omega)}\le\int_R(|f|+|df|_k)\,dV_k\le C\|u\|_{W^{1,1}(\Omega)},\qquad \|u\|_{W^{1,1}(\Omega)}=\int_\Omega\left(|u|+\sum_{i=1}^n|u_i|\right)\,dx.$$
The measure $dV_k$ is the Riemannian volume density, and $|df|_k$ is the dual metric norm. Essential supremum norms, possibly infinite, agree under the coordinate map, using Lebesgue measure on $\Omega$ and $dV_k$ on $U$. For any specified pointwise representative, its pointwise supremum on $U$ agrees with that of its coordinate expression on $\Omega$; this assertion does not identify representatives that differ on null sets.

Every real locally Lipschitz scalar function on $R$ has almost-everywhere classical coordinate derivatives equal to its weak derivatives, which assemble to the same coordinate-independent differential. More generally, the coordinate weak derivatives of a function that is $W^{1,1}_{\mathrm{loc}}$ in charts obey $d(\chi f)=\chi\,df+f\,d\chi$ for every smooth cutoff $\chi$. In particular this applies to the compactly supported functions above and to locally Lipschitz functions. For continuous representatives the pointwise and essential suprema of the absolute value also agree.

In dimension zero use the local convention $W^{1,1}(\mathbb R^0;\mathbb R)=\mathbb R$ with norm $|u|$, no first-derivative components, and volume one at the chart point; on the empty coordinate domain use the zero space. Then the same conclusions hold, with $df=0$ and $c=C=1$.

### Facts & Assumptions

[F1] The coordinate metric matrix $G=(k_{ij})$ is smooth and positive definite. Its inverse gives the dual metric: for a covector with component column $a$, $|a|_k^2=a^TG^{-1}a$. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:prop-riemannian-metrics-induce-metrics-on-dual-tensor-and-exterior-bundles](https://alphabetamath.cc/item/prop-riemannian-metrics-induce-metrics-on-dual-tensor-and-exterior-bundles)

[F2] The Riemannian volume density in a chart is $dV_k=\rho\,dx$, where $\rho=\sqrt{\det G}$ is smooth and positive; in dimension zero the empty determinant is one. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)

[F3] For positive dimension, weak first derivatives satisfy $\int u\,\partial_i\varphi\,dx=-\int u_i\varphi\,dx$ for every $\varphi\in C_c^\infty(\Omega)$. Under Countable Choice they are unique as almost-everywhere classes. The space $W^{1,1}$ requires $u$ and every $u_i$ to be integrable, with the sum norm displayed in the Statement; the local space requires this on relatively compact open subsets. [math:def-weak-derivative-of-a-locally-integrable-function](https://alphabetamath.cc/item/def-weak-derivative-of-a-locally-integrable-function) [math:lem-weak-derivatives-are-unique-almost-everywhere](https://alphabetamath.cc/item/lem-weak-derivatives-are-unique-almost-everywhere) [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm)

[F4] Assuming Countable Choice, a real locally Lipschitz function on an open subset of $\mathbb R^n$, $n\ge1$, is differentiable almost everywhere, with measurable weak partial derivatives, and $|Du|\le L$ almost everywhere wherever it is $L$-Lipschitz. Only this calculus conclusion of the supplier is used. [math:lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice](https://alphabetamath.cc/item/lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice)

[F5] Assuming Countable Choice, a $C^1$ diffeomorphism $T:A\to B$ of Euclidean open sets satisfies $\int_B h(y)\,dy=\int_A h(T(z))|\det DT(z)|\,dz$ for $h\in L^1(B)$. [Change of variables for integrable functions](https://alphabetamath.cc/item/cor-c-one-change-of-variables-for-l-one-functions)

[F6] For a real measurable function $h$ on a measure space $(X,\mathcal A,\mu)$, its essential supremum norm is $\|h\|_{\infty,\mu}=\inf\{M\in[0,\infty]:|h|\le M\text{ }\mu\text{-almost everywhere}\}$. [math:def-essential-supremum-with-respect-to-a-measure](https://alphabetamath.cc/item/def-essential-supremum-with-respect-to-a-measure)

[A1] Countable Choice is assumed for the Sobolev, weak-derivative uniqueness, Lipschitz-calculus, and Lebesgue change-of-variables suppliers; no stronger choice principle is asserted here. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

### Proof

**Given:** The chart, compact set, metric, function class, and Countable Choice in the Statement.

**Goal:** Establish the coordinate-independent weak differential, norm comparisons, and stated calculus in all dimensions.

1.1 Suppose first that $n\ge1$. We establish the coordinate transformation of weak derivatives locally. Let $T:A\to B$ be a smooth coordinate transition, write $z$ for the coordinates on $A$, put $J=|\det DT|$, and for a fixed $j$ set $b_i=J(DT^{-1})_{ij}$, where $DT^{-1}$ denotes the inverse matrix at $z$. Then $\sum_i\partial_i b_i=0$: on each connected component the sign of $\det DT$ is constant, and $b_i$ is that sign times the $(j,i)$ cofactor of $DT$. In its determinant expansion, differentiating a factor $\partial_\ell T_a$ in the cofactor for index $i$ pairs with the term differentiating $\partial_i T_a$ in the cofactor for index $\ell$; the signs are opposite and mixed second partials are equal. All terms cancel (for $n=1$ the cofactor is the constant one). For a coordinate function $u\in W^{1,1}_{\mathrm{loc}}(A)$, set $v=u\circ T^{-1}$. Change of variables on compact subsets makes $v$ and the proposed derivatives locally integrable. For $\varphi\in C_c^\infty(B)$, the smooth functions $b_i(\varphi\circ T)$ have compact support in $A$. The ordinary chain rule gives $\sum_i b_i\partial_i(\varphi\circ T)=J(\partial_j\varphi)\circ T$. Applying the weak identity to these tests, summing, and using the zero divergence just proved gives $$\int_B v\,\partial_j\varphi\,dy=-\int_B\left(\sum_i u_i(T^{-1}(y))\,\partial_j(T^{-1})_i(y)\right)\varphi(y)\,dy.$$ Thus $v_j=\sum_i(u_i\circ T^{-1})\partial_j(T^{-1})_i$ weakly. Uniqueness identifies this with any other weak derivative, so the covector expressions agree on overlaps. Applying change of variables to null-set indicators, with $J>0$, and then to the inverse transition shows that both directions preserve null sets; hence these statements are well defined for almost-everywhere classes. [F3, F5, A1, algebra]

2.1 For the compactly supported $u$ of the Statement, its restriction to $\Omega\setminus x(K)$ is zero almost everywhere. Its weak derivatives there are zero by the test identity and uniqueness. Therefore $u_i=0$ almost everywhere off $x(K)$. Step 1.1 patches the local differential within $U$; each point outside $U$ has a neighborhood disjoint from the closed set $K$, on which the zero extension is zero. Hence the extension has the asserted global weak differential and no boundary contribution. If $K$ is nonempty, compactness gives numbers $0<r\le s$ and $0<a\le b$ such that on $x(K)$, $r\le\rho\le s$ and $a|q|_2\le\sqrt{q^TG^{-1}q}\le b|q|_2$. Indeed the positive continuous density and the positive continuous function $\sqrt{q^TG^{-1}q}$ on the compact set $x(K)\times\{q:|q|_2=1\}$ have positive lower and finite upper bounds, by taking finite subcovers of neighborhoods where each has such bounds. No bound on the closure of the whole chart is used. Since $|q|_2\le\sum_i|q_i|\le\sqrt n|q|_2$, substituting [F1] and [F2] into the integral proves the inequalities with $c=r\min(1,a/\sqrt n)$ and $C=s\max(1,b)$. If $K$ is empty, $u$ and its derivatives are zero almost everywhere and $c=C=1$ suffices. [F1, F2, F3, step 1.1, algebra]

2.2 Apply [F4] locally to the coordinate expressions of any locally Lipschitz scalar function. Locally Lipschitz here means locally Lipschitz in smooth coordinates; this property is invariant because smooth transitions have bounded derivative on sufficiently small compact coordinate boxes. On each such box the function and its weak derivatives are integrable, so it is $W^{1,1}_{\mathrm{loc}}$. At points of classical differentiability the ordinary chain rule gives exactly the transformation in step 1.1. The null-set invariance proved there makes the resulting differential independent of chart as an almost-everywhere field. Second countability and [A1] give a countable subatlas, so these local null exceptions can be combined into one null set. For an arbitrary $W^{1,1}_{\mathrm{loc}}$ coordinate function and smooth $\chi$, use $\chi\varphi$ as the test in [F3]. Expanding $\partial_i(\chi\varphi)$ gives $$\int \chi u\,\partial_i\varphi\,dx=-\int(\chi u_i+u\,\partial_i\chi)\varphi\,dx.$$ The right-hand coefficient is locally integrable because the smooth factors are bounded on the support of each test. Thus $D_i(\chi u)=\chi u_i+u\partial_i\chi$, and step 1.1 makes this the stated global weak product rule. [F3, F4, A1, step 1.1, algebra]

3.1 The positive density $\rho$ has exactly the same null sets as coordinate Lebesgue measure: on each compact coordinate subset it is bounded above and below, and countably many relatively compact coordinate boxes cover $\Omega$. Therefore essential supremum norms agree. The equality of pointwise suprema for a specified representative follows directly from bijectivity of $x$. If that representative is continuous, any strict lower bound on its absolute value attained at a point holds on a neighborhood of that point, which has positive volume; hence its pointwise supremum is also its essential supremum, including the possible infinite value. [F2, F6, A1, step 2.1, algebra]

4.1 For $n=0$, a nonempty coordinate chart is a single point, its tangent and cotangent spaces are zero, and [F2] assigns that point volume one. Under the stated zero-dimensional convention both norms are $|u|$, all differential terms vanish, and the product rule is $0=0$. Null sets for this measure contain no chart point, so essential and pointwise suprema agree. The empty chart gives only zero norms. This proves all remaining cases. [given, F1, F2, F6, step 2.1, step 3.1, step 2.2] ∎


## Compactly supported chart mollification in uniform and first Sobolev norms

[Open item](item-lem-author-423fe0348a31-compact-chart-mollification) · level 0


### Statement

Work in ZFC. Let $n\ge1$, let $V\subset\mathbb R^n$ be open, and let $f:V\to\mathbb R$ be Lipschitz and compactly supported in $V$: the Euclidean closure $K=\overline{\{x\in V:f(x)\ne0\}}^{\mathbb R^n}$ is compact and contained in $V$. Its extension by zero $\widetilde f:\mathbb R^n\to\mathbb R$ is globally Lipschitz and belongs to $W^{1,1}(\mathbb R^n;\mathbb R)$. Write $f$ also for this zero extension whenever its argument ranges over $\mathbb R^n$; all $L^p$ and Sobolev spaces in this item are real. Fix a nonnegative $\rho\in C_c^\infty(\mathbb R^n)$ with $\int_{\mathbb R^n}\rho=1$ and $\operatorname{supp}\rho\subseteq\overline B_1(0)$, and for $\eta>0$ set $\rho_\eta(x)=\eta^{-n}\rho(x/\eta)$. The functions $f_\eta=\rho_\eta*f$ are smooth, supported in a fixed compact subset of $V$ for all sufficiently small $\eta$, and converge to $f$ both uniformly and in $W^{1,1}(\mathbb R^n)$. Such nonnegative unit-mass kernels exist in every dimension $n\ge1$.

### Facts & Assumptions

[F1] Real-valued locally Lipschitz functions are differentiable almost everywhere; their measurable partial derivatives are weak derivatives and satisfy $|Dh|\le L$ almost everywhere on every $L$-Lipschitz open region. [math:lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice](https://alphabetamath.cc/item/lem-ip-lipschitz-graph-area-and-calculus-under-countable-choice)

[F2] Convolution commutes with weak derivatives, including on all of Euclidean space for the zero extension. [math:lem-mollification-commutes-with-weak-derivatives-in-the-interior](https://alphabetamath.cc/item/lem-mollification-commutes-with-weak-derivatives-in-the-interior)

[F3] Translations are continuous in $L^p$ for $1\le p<\infty$; use $p=1$ for the function and its weak first derivatives. [math:thm-translation-is-continuous-in-l-p-for-one-le-p-less-infinity](https://alphabetamath.cc/item/thm-translation-is-continuous-in-l-p-for-one-le-p-less-infinity)

[F4] Convolution with a compactly supported smooth mollifier is smooth and differentiates under the integral. [math:thm-convolution-with-a-mollifier-is-smooth-and-differentiates-under-the-integral-sign](https://alphabetamath.cc/item/thm-convolution-with-a-mollifier-is-smooth-and-differentiates-under-the-integral-sign)

[F5] Work in ZFC, carrying the analytic suppliers' countable-choice assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F6] Membership in the real space $W^{1,1}(\mathbb R^n;\mathbb R)$ means that the function and each weak first derivative belong to $L^1$, and $\|u\|_{W^{1,1}}=\|u\|_1+\sum_{i=1}^n\|D_i u\|_1$. [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm)

[F7] The mollifier family is generated by the fixed kernel $\rho$ via $\rho_\eta(x)=\eta^{-n}\rho(x/\eta)$. Its mass is one, and the stated unit-ball support gives $\operatorname{supp}\rho_\eta\subseteq\overline B_\eta(0)$. [math:def-mollifier-family-generated-by-a-unit-mass-smooth-bump](https://alphabetamath.cc/item/def-mollifier-family-generated-by-a-unit-mass-smooth-bump)

[F8] For every $n\ge1$, a nonnegative smooth bump equals one on $\overline B_{1/2}(0)$ and has support in $B_1(0)$. [math:lem-smooth-bump-between-concentric-euclidean-balls](https://alphabetamath.cc/item/lem-smooth-bump-between-concentric-euclidean-balls)

[F9] In the Euclidean metrics, Lipschitz means that some $L\ge0$ satisfies $|f(x)-f(y)|\le L|x-y|$ for every pair in the domain. [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction)

[F10] For measurable functions, $(a*b)(x)=\int a(x-y)b(y)\,dy$ whenever the integrand is measurable and integrable. [math:def-convolution-of-two-functions-on-rn](https://alphabetamath.cc/item/def-convolution-of-two-functions-on-rn)

[F11] On sigma-finite measure spaces, if $F(x,z)$ is product-measurable and $\int\|F(\cdot,z)\|_1\,dz<\infty$, then $H(x)=\int|F(x,z)|\,dz$ belongs to $L^1$ and $\|H\|_1\le\int\|F(\cdot,z)\|_1\,dz$. This is the $p=1$ case of Minkowski's integral inequality. [math:thm-minkowski-integral-inequality](https://alphabetamath.cc/item/thm-minkowski-integral-inequality)

[F12] For an integrable real or complex function $u$, $|\int u|\le\int|u|$. [math:thm-integral-triangle-inequality](https://alphabetamath.cc/item/thm-integral-triangle-inequality)

[F13] Lebesgue measure is translation invariant, and an invertible linear map scales it by the absolute determinant. The corresponding integral substitutions follow first for indicator functions, then simple functions and their increasing limits; apply this also to positive and negative parts of integrable functions. In particular, $y=x-\eta z$ has volume factor $\eta^n$, and translations preserve $L^1$ norms. [math:thm-linear-change-of-variables-for-lebesgue-measure](https://alphabetamath.cc/item/thm-linear-change-of-variables-for-lebesgue-measure) [math:thm-lebesgue-outer-measure-and-measurability-are-translation-invariant](https://alphabetamath.cc/item/thm-lebesgue-outer-measure-and-measurability-are-translation-invariant)

[F14] A map from $\mathbb R^d$ to $\mathbb R^m$ is Borel measurable when it is measurable between their Borel sigma-algebras; use $m=1$ for real-valued functions. [math:def-borel-and-lebesgue-measurable-function-on-rn](https://alphabetamath.cc/item/def-borel-and-lebesgue-measurable-function-on-rn)

[F15] For a measure space, the real $L^1$ quotient norm is well defined and satisfies $\|u+v\|_1\le\|u\|_1+\|v\|_1$ and $\|a u\|_1=|a|\|u\|_1$. [math:thm-the-l-p-norm-descends-to-the-quotient-and-makes-l-p-a-normed-space](https://alphabetamath.cc/item/thm-the-l-p-norm-descends-to-the-quotient-and-makes-l-p-a-normed-space)

[F16] For a real-valued function $h$ on $\mathbb R^n$, $\operatorname{supp}h$ is the Euclidean closure of its nonzero set; compact support means that this closure is compact. Applied to the zero extension of $f:V\to\mathbb R$, its nonzero set is $\{x\in V:f(x)\ne0\}$, so its support is exactly the set $K$ specified in the Statement. [math:def-support-and-compactly-supported-riemann-integral-in-rn](https://alphabetamath.cc/item/def-support-and-compactly-supported-riemann-integral-in-rn)

[F17] The space $C_c(\mathbb R^n)$ consists of real-valued continuous functions on $\mathbb R^n$ with compact support, and $C_c^\infty(\mathbb R^n)$ is its subspace of smooth functions. [math:def-c-c-and-c-c-infinity-on-rn](https://alphabetamath.cc/item/def-c-c-and-c-c-infinity-on-rn)

### Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the stated construction or identity.

1.1 By [F8], choose a bump $b$ equal to one on $\overline B_{1/2}(0)$ with support in $B_1(0)$. Its integral is positive and finite, so $b/\int b$ is an admissible kernel, proving the existence assertion with the real smooth-function convention of [F17]; the rest of the proof applies to any fixed kernel in the Statement. By [F16], the set $K$ in the Statement is $\operatorname{supp}\widetilde f$. If $K$ is empty, all asserted functions are zero. Otherwise compactness gives $\eta_0>0$ such that $K+\overline B_{\eta_0}(0)$ is compact and contained in $V$; when $V=\mathbb R^n$, take any $\eta_0>0$. The zero extension $\widetilde f$ is globally Lipschitz: for $x\in V$ and $y\notin V$, approach the first exit point of the segment from $x$ to $y$ from within $V$. The function is zero near that exit point because $K$ stays away from the complement, so the Lipschitz inequality gives $|f(x)|\le L|x-y|$. Pairs in $V$ satisfy the original bound and pairs outside have zero difference. By [F1], $\widetilde f$ has bounded weak derivatives, zero almost everywhere off $K$, so the function and these derivatives are integrable and [F6] gives $\widetilde f\in W^{1,1}(\mathbb R^n)$. The support of $\rho_\eta*\widetilde f$ lies in $K+\overline B_\eta(0)$, hence in the fixed compact subset above for $0<\eta\le\eta_0$. [given, F1, F5, F6, F7, F8, F9, F10, F16, F17, construct, algebra]

2.1 By [F7], [F10] and the substitution in [F13], $f_\eta(x)-f(x)=\int\rho(z)(f(x-\eta z)-f(x))\,dz$. The integrand is integrable since $f$ is bounded and $\rho$ has compact support. Thus [F9] and [F12] give $\|f_\eta-f\|_\infty\le L\eta\int|z|\rho(z)\,dz$, proving uniform convergence. For the Sobolev estimate take $g=f$ or a representative of one of its weak first derivatives. For a derivative, choose the following Borel representative in the sense of [F14]: take the limit of the continuous difference quotients $m(f(x+e_i/m)-f(x))$ where the sequence converges and put zero elsewhere, where $e_i$ is the $i$th coordinate vector. The convergence set is Borel by the countable Cauchy criterion, and the resulting function is Borel measurable. It agrees almost everywhere with $D_i f$ by [F1]. The function $f$ itself is continuous. Consequently $F_\eta(x,z)=\rho(z)(g(x-\eta z)-g(x))$ is product-measurable for the Borel sigma-algebras: the product Borel sigma-algebra is the Euclidean Borel sigma-algebra because open rectangles from countable bases generate the product topology; compose the Borel functions with the continuous affine maps and take their difference and product. Each Euclidean Borel Lebesgue measure space is sigma-finite, being covered by bounded cubes. By [F13] and the $L^1$ norm triangle inequality and homogeneity from [F15], $\int\|F_\eta(\cdot,z)\|_1\,dz\le2\|g\|_1\int\rho(z)\,dz=2\|g\|_1<\infty$. All hypotheses of [F11] are therefore satisfied. [F1, F5, F6, F7, F9, F10, F11, F12, F13, F14, F15, step 1.1, construct, algebra]

3.1 Applying [F11] gives $H_\eta(x)=\int|F_\eta(x,z)|\,dz\in L^1$. Hence $F_\eta(x,\cdot)$ is integrable for almost every $x$, and the convolution substitution [F10], [F13], its unit mass [F7] and [F12] imply $|(\rho_\eta*g)(x)-g(x)|\le H_\eta(x)$ almost everywhere. It follows that $\|\rho_\eta*g-g\|_1\le\int\rho(z)\|g(\cdot-\eta z)-g\|_1\,dz$. Given $\varepsilon>0$, [F3] supplies $\delta>0$ such that $|h|<\delta$ implies $\|g(\cdot-h)-g\|_1<\varepsilon$. If $0<\eta<\delta$, every $z$ in the unit-ball support of $\rho$ satisfies this bound with $h=\eta z$, so the last integral is at most $\varepsilon\int\rho=\varepsilon$. This proves convergence for $f$ and each weak first derivative. Apply [F2] with $\Omega=\mathbb R^n$, $k=1$, $p=1$ and the kernel specified in the Statement; its hypotheses hold by step 1.1, so commutation of convolution with weak derivatives and [F6] prove the $W^{1,1}$ convergence. The smoothness supplier [F4] applies because $f$ is locally integrable and the fixed kernel is smooth, compactly supported and of mass one. Together with the support conclusion in step 1.1 and the uniform convergence in step 2.1, this proves every assertion. [F2, F3, F4, F5, F6, F7, F10, F11, F12, F13, step 1.1, step 2.1, algebra] ∎


## Formal adjoint of a real drift Laplacian on a closed manifold

[Open item](item-lem-author-1a44964f66ee-formal-adjoint) · level 0


### Statement

Let $(S,h)$ be a connected compact smooth Riemannian manifold without boundary, of positive dimension. For a smooth real vector field $t$ and smooth real function $c$, put $Lu=-\Delta_hu+2\langle t,\nabla u\rangle_h+cu$, with $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. The formal adjoint for $\langle f,g\rangle_{L^2}=\int_S\overline f g\,d\mu_h$ is $L^\dagger u=-\Delta_hu-2\langle t,\nabla u\rangle_h+(c-2\operatorname{div}_ht)u$. It has smooth real coefficients and the same negative-Laplacian principal part. The measure $d\mu_h$ is the positive Riemannian density, so no orientation assumption is needed.

### Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The supplied metric has its Levi–Civita connection. Gradient and Laplacian use $\operatorname{grad}_h u=(du)^\sharp$ and $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$; in coordinates $(\operatorname{grad}_h u)^i=h^{ij}\partial_j u$ and $\operatorname{div}_hX=\gamma^{-1}\partial_i(\gamma X^i)$, where $\gamma=\sqrt{\det(h_{ij})}$. Differential expressions extend complex-linearly, and contractions in them use the complex-bilinear extension of $h$. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry) [math:def-riemannian-gradient](https://alphabetamath.cc/item/def-riemannian-gradient) [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian) [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)

[F2] Density frames transform by absolute Jacobians. The local expressions $d\mu_h=\sqrt{\det(h_{ij})}\,|dx^1\cdots dx^n|$ therefore glue to a smooth positive density on $S$, independently of orientability. [math:def-density-bundle-and-smooth-density](https://alphabetamath.cc/item/def-density-bundle-and-smooth-density) [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:lem-the-riemannian-volume-density-is-coordinate-independent](https://alphabetamath.cc/item/lem-the-riemannian-volume-density-is-coordinate-independent)

[F3] Compactly supported smooth density integration is defined by chart partitions, is independent of those choices, is linear and local, and is strictly positive on any nonzero nonnegative density. Integrate complex coefficients by their real and imaginary parts. Compactness makes all smooth function multiples of $d\mu_h$ compactly supported. Work in ZFC: Choice supplies the countable-choice hypotheses of density integration and partitions. The $L^2$ notation here denotes the displayed pairing on smooth functions. [math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density) [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F4] A smooth partition of unity subordinate to a coordinate cover exists under countable choice. The divergence theorem is applied only on an oriented coordinate domain, with its restricted metric and a compactly supported vector field; that domain has no manifold boundary, so its divergence integral is zero. No orientation of $S$ is assumed. [math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary) [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F5] Here a formal adjoint of $L$ means a linear smooth-coefficient differential operator $A$ satisfying $\langle f,Lg\rangle_{L^2}=\langle Af,g\rangle_{L^2}$ for every $f,g\in C^\infty(S;\mathbb C)$. This is an identity of the density integrals just specified. Existence and uniqueness for this operator are proved below. [math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density) [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation)

[F6] For scalar coordinate operators built from the supplied gradient and divergence, use this symbol convention: for second-order part $-a^{ij}\partial_i\partial_j$, put $\sigma_2(P)(x,\xi)=a^{ij}(x)\xi_i\xi_j$. Thus the sign is the one obtained by replacing each top-order derivative by $i\xi_j$. This convention applies in every positive dimension; its value for the two operators is calculated in the proof. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-riemannian-gradient](https://alphabetamath.cc/item/def-riemannian-gradient) [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)

### Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The supplied metric has its Levi–Civita connection. Gradient and Laplacian use $\operatorname{grad}_h u=(du)^\sharp$ and $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$; in coordinates $(\operatorname{grad}_h u)^i=h^{ij}\partial_j u$ and $\operatorname{div}_hX=\gamma^{-1}\partial_i(\gamma X^i)$, where $\gamma=\sqrt{\det(h_{ij})}$. Differential expressions extend complex-linearly, and contractions in them use the complex-bilinear extension of $h$. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry) [math:def-riemannian-gradient](https://alphabetamath.cc/item/def-riemannian-gradient) [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian) [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)

[F2] Density frames transform by absolute Jacobians. The local expressions $d\mu_h=\sqrt{\det(h_{ij})}\,|dx^1\cdots dx^n|$ therefore glue to a smooth positive density on $S$, independently of orientability. [math:def-density-bundle-and-smooth-density](https://alphabetamath.cc/item/def-density-bundle-and-smooth-density) [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:lem-the-riemannian-volume-density-is-coordinate-independent](https://alphabetamath.cc/item/lem-the-riemannian-volume-density-is-coordinate-independent)

[F3] Compactly supported smooth density integration is defined by chart partitions, is independent of those choices, is linear and local, and is strictly positive on any nonzero nonnegative density. Integrate complex coefficients by their real and imaginary parts. Compactness makes all smooth function multiples of $d\mu_h$ compactly supported. Work in ZFC: Choice supplies the countable-choice hypotheses of density integration and partitions. The $L^2$ notation here denotes the displayed pairing on smooth functions. [math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density) [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F4] A smooth partition of unity subordinate to a coordinate cover exists under countable choice. The divergence theorem is applied only on an oriented coordinate domain, with its restricted metric and a compactly supported vector field; that domain has no manifold boundary, so its divergence integral is zero. No orientation of $S$ is assumed. [math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary) [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F5] Here a formal adjoint of $L$ means a linear smooth-coefficient differential operator $A$ satisfying $\langle f,Lg\rangle_{L^2}=\langle Af,g\rangle_{L^2}$ for every $f,g\in C^\infty(S;\mathbb C)$. This is an identity of the density integrals just specified. Existence and uniqueness for this operator are proved below. [math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density) [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation)

[F6] For scalar coordinate operators built from the supplied gradient and divergence, use this symbol convention: for second-order part $-a^{ij}\partial_i\partial_j$, put $\sigma_2(P)(x,\xi)=a^{ij}(x)\xi_i\xi_j$. Thus the sign is the one obtained by replacing each top-order derivative by $i\xi_j$. This convention applies in every positive dimension; its value for the two operators is calculated in the proof. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-riemannian-gradient](https://alphabetamath.cc/item/def-riemannian-gradient) [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)

**Proof technique:** direct.

1.1 Choose a smooth chart-subordinate partition $(\rho_a)$. Local finiteness and compactness make only finitely many supports nonempty: finitely many neighborhoods covering $S$ each meet only finitely many supports. Each $\rho_aX$ is compactly supported inside its chart domain $U_a$, which is oriented by its coordinates. There $d\mu_h$ and the positive coordinate Riemannian volume form have the same coefficient $\gamma$, so their integrals of a chart-supported scalar agree. The oriented divergence theorem on $U_a$ gives $\int_S\operatorname{div}_h(\rho_aX)\,d\mu_h=0$, using locality to extend the chart integral to $S$. The coordinate product rule gives $\operatorname{div}_h(\rho_aX)=\rho_a\operatorname{div}_hX+d\rho_a(X)$. Sum the finite family, using $\sum_a\rho_a=1$ and $\sum_a d\rho_a=0$, to obtain $\int_S\operatorname{div}_hX\,d\mu_h=0$. The same identity holds for complex vector fields by real and imaginary parts. [F1, F2, F3, F4]

2.1 Apply step 1.1 to $\overline f\operatorname{grad}_h g$ and then to $g\operatorname{grad}_h\overline f$. The product rule gives $\int_S\overline f(-\Delta_hg)\,d\mu_h=\int_Sh(\nabla\overline f,\nabla g)\,d\mu_h=\int_S\overline{(-\Delta_hf)}g\,d\mu_h$. Thus the negative Laplacian is formally symmetric for the stated first-variable-conjugate-linear pairing. [F1, F3, F5, step 1.1]

3.1 Apply step 1.1 to $\overline fgt$. Expanding its divergence yields $\int_S\overline f\,2t\cdot\nabla g\,d\mu_h=-\int_Sg(2t\cdot\nabla\overline f+2\operatorname{div}_ht\,\overline f)\,d\mu_h$. Combining this with step 2.1 and the real multiplication coefficient $c$ proves $\langle f,Lg\rangle_{L^2}=\langle Af,g\rangle_{L^2}$ for $Af=-\Delta_hf-2t\cdot\nabla f+(c-2\operatorname{div}_ht)f$. All these coefficients are smooth and real. [F1, F3, F5, step 1.1, step 2.1]

4.1 If $A$ and $B$ both satisfy the identity in F5, then for each smooth $f$ and every smooth $g$ one has $\langle (A-B)f,g\rangle_{L^2}=0$. Choose $g=(A-B)f$, which is smooth and compactly supported on compact $S$. The resulting integral $\int_S|(A-B)f|^2\,d\mu_h$ is zero, so strict positivity of the density integral forces $(A-B)f=0$ everywhere. Hence $A=B$, and the operator of step 3.1 is the formal adjoint $L^\dagger$. [F2, F3, F5, step 3.1]

5.1 The coordinate formulas give $\Delta_hu=\gamma^{-1}\partial_i(\gamma h^{ij}\partial_ju)$, whose second-order part is $h^{ij}\partial_i\partial_ju$. The drift and multiplication terms in $L$ and $L^\dagger$ have order at most one, so both have second-order part $-h^{ij}\partial_i\partial_j$. In the convention F6 their symbol is $h^{ij}\xi_i\xi_j=h^{-1}(\xi,\xi)=|\xi|_h^2>0$ for nonzero $\xi$. This is an intrinsic quadratic form, hence chart independent, and the calculation includes dimension one. This proves all assertions of the Statement without an orientation assumption. [F1, F6, step 3.1, step 4.1] ∎


## General spacelike two-surfaces, null gauges and fluxes

[Open item](item-def-author-97780c2fed82-general-spacelike-surface-data) · level 0


### Definition

Assume Countable Choice $\mathrm{AC}_\omega$. Let $(M,g,N)$ be a smooth oriented, time-oriented Lorentzian four-manifold with signature $(-,+,+,+)$ and a smooth metric connection $\nabla$, meaning any $g$-compatible affine connection; torsion freedom is not assumed. Let $i:S\hookrightarrow M$ be a nonempty compact oriented smooth embedded two-manifold without boundary with positive-definite induced metric $q=i^*g$. No containing spacelike hypersurface is required. Supply a global ordered pair of future null normal fields $\ell,k$ with $g(\ell,k)=-1$; the choice of $\ell$ labels the outgoing direction. The library convention $g(\ell,k)=-2$ is converted by halving its second normal.

For tangent fields $u,v$ on $S$, identify them with their images under $di$ in metric pairings and interpret $\nabla_u\ell$ as $(i^*\nabla)_u\ell$ in the pullback tangent bundle $i^*TM$. Put $\chi_\ell(u,v)=g(\nabla_u\ell,v)$, $\theta_{(\ell)}=\operatorname{tr}_q\chi_\ell$ and $\Omega(u)=-g(k,\nabla_u\ell)$. A marginal outer trapped surface (MOTS) means $\theta_{(\ell)}=0$ everywhere; no sign for the other null expansion is added. Write $d\mu_q$ for the positive area density and $A=\int_S d\mu_q$. For a smooth real two-form $F$, use the chosen orientations to define $F|_{TS}=b\,dA_q$ and $(\star_gF)|_{TS}=e\,dA_q$, where $dA_q$ is the positive oriented area form. Set $Q_M=(4\pi)^{-1}\int_SF=(4\pi)^{-1}\int_Sb\,d\mu_q$ and $Q_E=(4\pi)^{-1}\int_S\star_gF=(4\pi)^{-1}\int_Se\,d\mu_q$.

### Definition references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[math:def-riemannian-volume-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-riemannian-volume-form-on-an-oriented-manifold)

[math:prop-integration-over-an-oriented-embedded-submanifold](https://alphabetamath.cc/item/prop-integration-over-an-oriented-embedded-submanifold)

[physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold)

[math:def-pullback-connection](https://alphabetamath.cc/item/def-pullback-connection)

[math:thm-pullback-connection-is-well-defined-and-functorial](https://alphabetamath.cc/item/thm-pullback-connection-is-well-defined-and-functorial)

[math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density)

[math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

### Facts & Assumptions

[A1] Countable Choice is assumed for the smooth tangent-bundle and time-orientation conventions of the Lorentzian and null-screen suppliers, the Hodge supplier's background hypotheses, and the density-integral construction. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F1] The Lorentzian and null-screen suppliers fix the spacelike-surface and future-null-pair conventions. Metric compatibility means clause (a) of the connection supplier. Connection-dependent null-screen assertions are used only in the metric-selected case; no symmetry of $\chi_\ell$ is assumed for a general metric connection. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry) [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F2] The Riemannian area form obeys $|dA_q|=d\mu_q$. Integration of an ambient two-form over $S$ means integration of its pullback, with compact support required on $S$ itself; the oriented integral has its finite-chart construction. The Lorentzian Hodge star is a smooth bundle map fixed by $g$ and the ambient orientation. [math:def-riemannian-volume-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-riemannian-volume-form-on-an-oriented-manifold) [math:prop-integration-over-an-oriented-embedded-submanifold](https://alphabetamath.cc/item/prop-integration-over-an-oriented-embedded-submanifold) [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[F3] An affine connection is a connection on $TM$. For any smooth map $i$ and any connection on a vector bundle, the pullback prescription gives a frame-independent connection on the pullback bundle and satisfies $(i^*\nabla)_u(i^*s)=(\nabla s)(di(u))$ for local ambient sections $s$. No torsion or metric hypothesis is needed. [math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold) [math:def-pullback-connection](https://alphabetamath.cc/item/def-pullback-connection) [math:thm-pullback-connection-is-well-defined-and-functorial](https://alphabetamath.cc/item/thm-pullback-connection-is-well-defined-and-functorial)

[F4] Under Countable Choice, a compactly supported smooth density is integrated by a chart partition and the resulting finite sum of coefficient integrals is independent of charts and partition. This integral is finite, linear and strictly positive for a nonzero nonnegative density. [math:def-integral-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-smooth-density) [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation)

### Justification

**Given:** The objects and hypotheses in the Definition, including Countable Choice.

**Goal:** Establish the assertions and well-definedness stated there.

1.1 Multiplying the library second null normal by $1/2$ changes its pairing with the first from $-2$ to $-1$ and preserves its future null direction. These are the supplied smooth normal fields; no global pair is inferred from local existence. [given, A1, F1]

1.2 The area form $dA_q$ is nowhere zero and smooth. Both pulled-back two-forms are smooth, since $F$, the Hodge star and $i$ are smooth. Thus each is uniquely a smooth scalar multiple of $dA_q$: in a positive surface chart, divide its coefficient by $\sqrt{\det q}>0$. The ratios agree on overlaps by the top-form transformation law, giving global smooth $b,e$. [A1, F2]

2.1 Apply the pullback construction to the connection on $TM$ and the smooth embedding $i$. In any pulled-back frame $e_a$, write $\ell=\ell^ae_a$ and let $\omega^a{}_b$ be the ambient connection matrix. Then $(i^*\nabla)_u\ell$ has coefficients $u(\ell^a)+\omega^a{}_b(di(u))\ell^b$, which are smooth and depend only on the section along $S$. Frame independence is supplied by the pullback theorem. If a local ambient extension of $\ell$ is used, the section identity gives the same formula; two such extensions agree after pullback, so their tangential derivatives agree. The connection's function-linearity in $u$, smooth metric pairing and invertibility of the positive matrix $q$ now make $\chi_\ell$, its $q$-trace and $\Omega$ well-defined smooth tensors or functions. In the metric-selected case, $\chi_\ell$ and $\theta_{(\ell)}$ coincide with the null-screen definitions; $\Omega$ is the independent local definition above. The general argument uses no torsion restriction. [A1, F1, F3, step 1.1]

2.2 Compactness of $S$ makes $d\mu_q$, $b\,d\mu_q$, $e\,d\mu_q$ and the pulled-back top forms compactly supported on $S$. Choose a common chart partition in positive surface charts. The localized coefficients of $b\,dA_q$ and $b\,d\mu_q$ are the same functions $\rho_j b\sqrt{\det q}$; their respective form and density integrals therefore have identical finite chart sums. Replacing $b$ by $e$ gives the second equality. The submanifold integral convention then proves both stated flux identities, with finite integrals. [A1, F2, F4, step 1.2]

3.1 The area density is nonzero and nonnegative because $S$ is nonempty and $q$ is positive definite. Strict positivity of density integration gives $A>0$. With ambient orientation fixed, reversing the surface orientation negates $dA_q$ and both oriented flux integrals, while leaving $d\mu_q$ and $A$ unchanged; equivalently $b,e$ both change sign. Thus both charges change sign and their squares are unchanged. [F2, F4, step 1.2, step 2.2] ∎



## Mean-curvature variation and the stationary lapse equation

[Open item](item-thm-maximal-jacobi-lapse-input) · level 1


### Statement

Let $(M,g)$ be a smooth time-oriented Lorentzian four-manifold, and let $F_s$ be a smooth local variation through spacelike embeddings of a smooth spacelike hypersurface $\Sigma=F_0(\Sigma)$, with $F_0$ the inclusion. Write $n$ for the future unit normal, $h$ for the induced metric, $k(U,V)=-g(\nabla_U n,V)$, and $H=\operatorname{div}_g n=-\operatorname{tr}_h k$. Let the variational vector field be $V=a n+X$, where $X$ is tangent and $a=-g(V,n)$. Then the derivative at $s=0$ of the pulled-back mean curvature is $\Delta_h a-(|k|_h^2+\operatorname{Ric}(n,n))a+X(H)$. Here $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$ and $|k|_h^2=h^{ij}h^{pq}k_{ip}k_{jq}$.

If $H=0$ on $\Sigma$ and a Killing field $T$ decomposes along it as $T=Nn+X$, then $\Delta_hN=(|k|_h^2+\operatorname{Ric}(n,n))N$. This local identity asserts no boundary values or normalization at an end.

### Statement references

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)

[math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)

[physics:thm-gr-curvature-algebraic-symmetries](https://alphabetamath.cc/physics/item/thm-gr-curvature-algebraic-symmetries)

[math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)

### Facts & Assumptions

[F1] The spacelike hypersurface data give the future normal, induced metric, sign convention for $k$, mean curvature and normal–tangential decomposition. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F2] The mean-curvature map pulls the mean curvature of each admissible spacelike graph back to the original hypersurface. [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[F3] A Killing field has local flow preserving $g$, and the curvature convention is $R(U,V)W=\nabla_U\nabla_VW-\nabla_V\nabla_UW-\nabla_{[U,V]}W$, with $\operatorname{Ric}_{bd}=R^a{}_{bad}$. The Killing condition and curvature convention are supplied by the stationary data; flow invariance follows from vanishing metric Lie derivative on each local flow domain. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)

[F4] The smooth nondegenerate metric has a unique torsion-free metric-compatible connection, extended to tensor fields. [physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[F5] For the smooth induced Riemannian metric $h$, the intrinsic operators satisfy $h(\operatorname{grad}_h a,U)=U(a)$, $\operatorname{Hess}_h a(U,W)=h(\nabla^h_U\operatorname{grad}_h a,W)$, and $\operatorname{div}_h Z=\operatorname{tr}(U\mapsto\nabla^h_U Z)$, where $\nabla^h$ is the Levi–Civita connection of $h$. Thus $\Delta_h a=\operatorname{tr}_h\operatorname{Hess}_h a=\operatorname{div}_h\operatorname{grad}_h a$. [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas) [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)

[F6] The curvature tensor of a smooth time-oriented Lorentzian four-manifold with its metric-selected connection has the algebraic curvature symmetries, in particular $R(U,W)Z=-R(W,U)Z$, with the curvature and Ricci conventions used here. [physics:thm-gr-curvature-algebraic-symmetries](https://alphabetamath.cc/physics/item/thm-gr-curvature-algebraic-symmetries)

### Proof

**Given:** The variation and geometric data in the Statement.

**Goal:** Derive the variation formula and its consequence for a maximal hypersurface moved by a Killing flow.

1.1 First suppose $V=an$. In local coordinates $x^i$ on $\Sigma$, put $e_i=\partial_iF_s$ and $K_{ij}=g(\nabla_{e_i}n,e_j)=-k_{ij}$ at $s=0$. Differentiating $g(n,n)=-1$ and $g(n,e_i)=0$, using torsion-freeness and $[\partial_s,e_i]=0$, gives $\nabla_{\partial_s}n=\operatorname{grad}_h a$ at $s=0$. Metric compatibility also gives $\dot h_{ij}=2aK_{ij}$ and $\dot h^{ij}=-2aK^{ij}$. [given, F1, F4, F5]

2.1 Commuting the covariant derivatives by the curvature convention and differentiating $K_{ij}$ gives $\dot K_{ij}=\nabla^h_i\nabla^h_j a+a\,g(R(n,e_i)n,e_j)+aK_i{}^pK_{pj}$, where $\nabla^h$ is the Levi–Civita connection of $h$. Using $\operatorname{tr}_h\operatorname{Hess}_h a=\Delta_h a$ from F5, tracing this identity and including $\dot h^{ij}K_{ij}$ yields $\dot H=\Delta_h a-a|k|_h^2+a h^{ij}g(R(n,e_i)n,e_j)$. The displayed Ricci convention and the curvature symmetries of the metric-compatible torsion-free connection give $h^{ij}g(R(n,e_i)n,e_j)=-\operatorname{Ric}(n,n)$, proving the formula for a normal variation. [F1, F3, F4, F5, F6, step 1.1]

3.1 For a general variation, locally reparametrize the domain by a time-dependent diffeomorphism whose initial velocity cancels $X$. The resulting variation has initial velocity $an$; differentiating the scalar pullback under the inverse reparametrization adds $X(H)$. This proves the stated formula for arbitrary $V$; the graph mean-curvature map uses the same pullback convention. [given, F2, step 2.1]

4.1 By F3 the local flow of a Killing field consists of local isometries. Transporting $\nabla$ by a local isometry gives a torsion-free metric-compatible connection, which equals $\nabla$ by uniqueness in F4. The flow starts at the identity and hence preserves future direction on its local flow domain. It therefore carries the future normal and mean curvature of $\Sigma$ to those of the image hypersurface. Its pulled-back mean curvature is therefore constant in the flow parameter. Its variational field is $T=Nn+X$; if $H=0$, then $X(H)=0$, and the variation formula gives the stated lapse equation. The calculation is local and imposes no boundary or asymptotic condition. [given, F1, F3, F4, step 3.1] ∎

### External input

Gourgoulhon records the maximal-slicing lapse equation under the 3+1 Einstein-equation conventions; the more general geometric variation above is derived locally.


## Null optical comparison with affine and screen conventions

[Open item](item-lem-null-optics-jacobian-comparison-input) · level 1


### Statement

Assume the axiom of choice. In the null-screen setting, let $F:U\times J\to M$ be a smooth future-directed affinely parametrized null geodesic hypersurface congruence normal to a spacelike two-surface $S$, with $F(p,0)=p$ and $L=\partial_\lambda F$. Fix $p\in U$ and work on the connected interval containing $0$ on which the screen Jacobi map $A_\lambda:T_pS\to\mathscr S_\lambda=L^\perp/\mathbb RL$ is invertible. Put $B=A'A^{-1}$, $\theta=\operatorname{tr}B$, and $\sigma=B-\frac12\theta\,\mathrm{id}$. The positive area Jacobian is $J(\lambda)=\sqrt{\det(\bar\gamma(A_\lambda e_i,A_\lambda e_j))}$ for any orthonormal basis $(e_1,e_2)$ of $T_pS$; thus $J(0)=1$.

On this interval $\theta'=-\theta^2/2-|\sigma|^2-\operatorname{Ric}(L,L)$ and $(\log J)'=\theta$. If $\operatorname{Ric}(L,L)\ge0$ along the relevant segment and $\theta(0)<0$, a focal instant occurs by $2/|\theta(0)|$, provided the smooth congruence is defined through that parameter.

If instead $[a,0]\subset J$ is regular, $a<0$, $\operatorname{Ric}(L,L)\ge0$ on it and $\theta(0)>0$, then $\theta(\lambda)\ge\theta(0)>0$ for $a\le\lambda\le0$ and $0<J(\lambda_1)\le J(\lambda_2)\le1$ whenever $a\le\lambda_1\le\lambda_2\le0$. Thus moving from $S$ toward the past, with parameter $s=-\lambda$, reverses the expansion sign and makes the screen Jacobian nonincreasing. This is a pointwise comparison of regular screen Jacobians; applying it to nonsmooth cuts requires a separate applicable area formula and endpoint-map hypotheses.

### Statement references

[def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)

[physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)

[physics:prop-gr-fx-null-raychaudhuri](https://alphabetamath.cc/physics/item/prop-gr-fx-null-raychaudhuri)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### Facts & Assumptions

[A1] Assume the axiom of choice, including the countable and dependent choice used by the geometric suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The null-screen definition supplies the positive screen metric, metric screen derivative, invertible regular Jacobi map, optical endomorphism, and the initial identification of $T_pS$ with the screen. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data) [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)

[F2] The Ricci tensor is the contraction of the curvature tensor of the metric-selected connection, with the curvature convention used in null Raychaudhuri. [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors) For the stated null hypersurface congruence, null Raychaudhuri gives the displayed evolution equation and, under nonnegative null Ricci curvature and negative initial expansion, the stated focal bound when the congruence is defined through the bound. [physics:prop-gr-fx-null-raychaudhuri](https://alphabetamath.cc/physics/item/prop-gr-fx-null-raychaudhuri)

[F3] Under its stated causal hypotheses, a focal instant excludes sufficiently nearby later points of the future generator from the future horismos of $S$. This fact does not assert the existence or regularity of a cut. [physics:lem-gr-fx-null-focal-boundary-exclusion](https://alphabetamath.cc/physics/item/lem-gr-fx-null-focal-boundary-exclusion)

[F4] The derivative product, quotient and chain rules and the identity $(\log x)'=1/x$ for $x>0$ apply to the smooth scalar functions below. [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives) [math:thm-chain-rule](https://alphabetamath.cc/item/thm-chain-rule) [math:thm-logarithm-derivative-and-integral](https://alphabetamath.cc/item/thm-logarithm-derivative-and-integral)

[F5] A continuous function on a closed interval, differentiable in its interior, is nondecreasing when its derivative is nonnegative, by the mean value theorem. [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

### Proof

**Given:**The stated congruence, regular interval, and the hypotheses in each conditional assertion.

**Goal:** Establish the screen transport identity and the stated focal and past-directed comparisons.

1.1 Choose an orthonormal basis of $T_pS$ and a smooth orthonormal screen frame locally along the generator. Let $M$ be the resulting matrix of $A$, and let $\Omega$ be the connection matrix of the screen frame. Metric compatibility makes $\Omega$ skew-symmetric, and the matrix of $B$ is $(M'+\Omega M)M^{-1}$. Expanding the determinant of the invertible $2\times2$ matrix and differentiating its entries gives $(\det M)'=(\det M)\operatorname{tr}(M'M^{-1})$. Since $\operatorname{tr}\Omega=0$, the definition of $J$ gives $J'/J=\operatorname{tr}B=\theta$; the sign of $\det M$ is locally constant. The chain rule for $\log$ gives $(\log J)'=\theta$. The initial screen identification makes $J(0)=1$. [F1, F4, given, algebra]

1.2 The evolution equation and the focal conclusion under the stated nonnegative Ricci, negative initial expansion and existence hypotheses are precisely the applications of the null Raychaudhuri supplier. [F2, given]

2.1 On a regular interval $[a,0]$ with nonnegative null Ricci curvature, the evolution equation gives $\theta'\le0$ because the screen shear norm is nonnegative. Applying the mean value theorem to $-\theta$ yields $\theta(\lambda)\ge\theta(0)>0$ for $a\le\lambda\le0$. Step 1.1 then gives $J'=\theta J>0$; another application of the mean value theorem and $J(0)=1$ give the stated inequalities. Reparametrizing by $s=-\lambda$ changes $d(\log J)/ds$ to $-\theta$, giving the past-directed sign and monotonicity. [F1, F5, step 1.1, step 1.2, given, algebra] ∎

### Remarks

The screen metric is positive, so the Jacobian above is independent of the chosen orthonormal basis. At a smooth regular cut whose differential is identified with the screen Jacobi map, it is the corresponding pointwise area Jacobian. The statement makes no such identification for a nonsmooth cut and does not infer a global cut parameter from focal data. The focal-exclusion fact is recorded for the later causal application, with its own hypotheses.


## Annular scaling and fixed interior covers

[Open item](item-lem-author-db87cb8e0bab-annular-scaling) · level 1


### Statement

Let $n\ge1$ and $k\ge0$ be integers and $0<\alpha<1$. In $\mathbb R^n$ set $A=\{y:1/2<|y|<4\}$, $A'=\{y:1<|y|<2\}$ and $K=\overline{A'}=\{y:1\le|y|\le2\}$. For $R\ge1$ and $u\in C^k(RA;\mathbb R)$, where $RS=\{Ry:y\in S\}$, define $v(y)=u(Ry)$ and $w(y)=R^{-1}u(Ry)$ on $A$. Multi-index derivatives are taken in their canonical order. No boundary extension of $u$ to $\partial(RA)$ is assumed.

For every multi-index $\beta$ with $|\beta|\le k$ and every nonempty open $S\subseteq A$, the exact scaling identities are
$$D_y^\beta v(y)=R^{|\beta|}(D_x^\beta u)(Ry),\qquad D_y^\beta w(y)=R^{|\beta|-1}(D_x^\beta u)(Ry),$$
$$[D_y^\beta v]_{\alpha;S}=R^{|\beta|+\alpha}[D_x^\beta u]_{\alpha;RS},\qquad [D_y^\beta w]_{\alpha;S}=R^{|\beta|-1+\alpha}[D_x^\beta u]_{\alpha;RS}.$$
Here $[f]_{\alpha;S}=\sup_{y,z\in S,\,y\ne z}|f(y)-f(z)|/|y-z|^\alpha$; seminorms may equal $+\infty$.

For $h\in C^k(S;\mathbb R)$ use the ordinary norm convention
$$\|h\|_{C^{k,\alpha}(S)}=\sum_{j=0}^k\max_{|\beta|=j}\sup_S|D^\beta h|+\sum_{|\beta|=k}[D^\beta h]_{\alpha;S}.$$
Consequently the annular rescaling, with the same convention for any such $S$, satisfies
$$\|v\|_{C^{k,\alpha}(S)}=\sum_{j=0}^k R^j\max_{|\beta|=j}\sup_{RS}|D_x^\beta u|+R^{k+\alpha}\sum_{|\beta|=k}[D_x^\beta u]_{\alpha;RS},\qquad \|w\|_{C^{k,\alpha}(S)}=R^{-1}\|v\|_{C^{k,\alpha}(S)}.$$

There is a fixed finite family of centers $p_1,\ldots,p_N\in K$, depending only on $n$, such that the balls $B_r(p_i)$ cover $K$, where $r=1/16$, and every enlarged ball $B_{4r}(p_i)$ lies in $A$. In particular the smaller concentric balls $B_{2r}(p_i)$ also cover $K$. For every $h\in C^k(A;\mathbb R)$ with $M:=\max_i\|h\|_{C^{k,\alpha}(B_{2r}(p_i))}<\infty$,
$$\|h\|_{C^{k,\alpha}(A')}\le C_{n,k,\alpha} M,\qquad C_{n,k,\alpha}:=(k+1)+N_{n,k}\max\{1,2r^{-\alpha}\},\qquad N_{n,k}:=\#\{\beta\in\mathbb N^n:|\beta|=k\}.$$
Thus ball estimates on the smaller balls, obtained using these enlarged balls, imply a full annular estimate, including the global Hölder seminorm, with a constant independent of $R$.

The same conclusion applies to families indexed by $R$ and any further parameter whenever the local estimates have common constants on the specified parameter set; uniformity at a parameter endpoint is not inferred from separate pointwise estimates. In the three-dimensional exterior-chart setting $E=\{x:|x|>R_0\}$ with $R_0>0$, if $u$ is given only on $E$, require $R\ge1$ and $R/2>R_0$ so that $RA\subset E$. Uniform end bounds retain their common-chart, common-radius and common-constant meaning.

### Facts & Assumptions

[F1] The class $C^k$ requires continuous iterated coordinate derivatives through order $k$; $D^\beta$ uses the fixed canonical order. [math:def-ck-and-multi-index-notation-in-several-variables](https://alphabetamath.cc/item/def-ck-and-multi-index-notation-in-several-variables)

[F2] Ordinary Hölder seminorms and norms use Euclidean distances, derivative suprema and top-order difference quotients; scaled norms attach the indicated powers of radius. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F3] Exterior differentiated bounds and parameter uniformity require a specified Cartesian chart and common radii and constants on the specified parameter set. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F4] A closed bounded subset of $\mathbb R^n$, $n\ge1$, is compact in its Euclidean metric: every open cover has a finite subcover. [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)

### Proof

**Given:** The hypotheses and norm conventions in the Statement.

**Goal:** Prove the exact scaling identities and the full fixed-cover annular estimate.

1.1 If $k\ge1$, for any coordinate unit vector $e_i$ and any iterated coordinate derivative $q$ of $u$ of order less than $k$, the difference quotient after dilation is
$$\frac{q(R(y+t e_i))-q(Ry)}{t}=R\frac{q(Ry+Rt e_i)-q(Ry)}{Rt}\longrightarrow R(\partial_iq)(Ry)\quad(t\to0).$$
For $y\in A$ the points involved lie in $RA$ for sufficiently small $|t|$, since $RA$ is open. Apply this calculation successively to every coordinate-derivative word through order $k$; all required derivatives exist by [F1]. In particular, the canonical order gives the asserted identities for $D^\beta v$, and multiplication by the constant $R^{-1}$ gives those for $D^\beta w$. Each resulting derivative is continuous, since its derivative of $u$ is continuous and $|Ry-Rz|=R|y-z|$ makes dilation continuous. Thus $v,w\in C^k(A)$. Order zero is the defining identity, including when $k=0$. [given, F1, algebra]

1.2 The reverse triangle inequality $\big||y|-|z|\big|\le|y-z|$ shows directly that the complement of $K$ is open: at a point with $|y|<1$ take a ball of radius $(1-|y|)/2$, and at one with $|y|>2$ take radius $(|y|-2)/2$. Also $K\subset B_3(0)$, so [F4] makes $K$ compact. The balls $B_r(p)$, for $p\in K$ and $r=1/16$, form an open cover. Take a finite subcover with centers $p_1,\ldots,p_N$. For $y\in B_{4r}(p_i)$, the same triangle inequalities give $3/4<|y|<9/4$; thus $B_{4r}(p_i)\subset A$. All these balls are fixed in $y$ coordinates, independently of $R$, $u$ or any further parameter. [given, F4, construct, algebra]

2.1 Dilation maps $S$ bijectively onto $RS$, so the derivative identities give the corresponding supremum factors $R^{|\beta|}$ and $R^{|\beta|-1}$. For distinct $y,z\in S$, substitute $x=Ry$, $x'=Rz$; then $|x-x'|=R|y-z|$. Each difference quotient for $D_y^\beta v$ is therefore $R^{|\beta|+\alpha}$ times the corresponding quotient for $D_x^\beta u$, and the factor for $w$ is $R^{|\beta|-1+\alpha}$. The pair correspondence is bijective, so taking suprema proves both seminorm equalities, also if they are infinite. Summation in the stated norm convention proves the norm identities. [given, F2, step 1.1, algebra]

2.2 Put $M=\max_i\|h\|_{C^{k,\alpha}(B_{2r}(p_i))}$. Every $y\in A'$ belongs to some $B_r(p_i)\subset B_{2r}(p_i)$, so each derivative supremum in the norm on $A'$ is at most $M$. For distinct $y,z\in A'$ with $|y-z|<r$, choose $i$ with $|y-p_i|<r$. Then $|z-p_i|<2r$, and the $\alpha$-Hölder quotient of each $D^\beta h$ with $|\beta|=k$ is bounded by its seminorm on $B_{2r}(p_i)$, hence by $M$. Thus the fixed margin $r$ controls every nearby pair. [given, F1, F2, step 1.2, algebra]

3.1 For the remaining pairs, $|y-z|\ge r$, each numerator $|D^\beta h(y)-D^\beta h(z)|$ is at most $2M$, so its Hölder quotient is at most $2r^{-\alpha}M$. Together with step 2.2 this bounds each top-order seminorm by $\max\{1,2r^{-\alpha}\}M$. There are $N_{n,k}$ such multi-indices, and $k+1$ derivative-supremum terms. Summing gives exactly $\|h\|_{C^{k,\alpha}(A')}\le C_{n,k,\alpha}M$ as stated. [given, F2, step 2.2, algebra]

4.1 Apply the fixed-cover estimate to $h=v$ or $h=w$ and use the exact rescaling identities of step 2.1. If the local estimates are bounded by a common local constant times a given right-hand side, their finite maximum has that same bound, and step 3.1 multiplies it only by $C_{n,k,\alpha}$. Neither the balls nor this factor depend on $R$ or a further parameter. For an exterior chart in dimension three, $y\in A$ gives $|Ry|>R/2>R_0$, which verifies the domain condition; [F3] specifies precisely when end estimates and their constants are uniform. This proves all the claimed scaling and uniform annular conclusions. [given, F3, step 2.1, step 1.2, step 3.1, algebra] ∎



## Ellipticity and zero-slope forcing of the stationary maximal flux

[Open item](item-lem-author-db87cb8e0bab-stationary-flux-ellipticity) · level 1


### Statement

Fix $0<\alpha<1$, $R_0\ge1$, a bounded annulus $A=\{y\in\mathbb R^3:a<|y|<b\}$ with $0<a<b$, and $p_0>0$. For $R\ge R_0$, let $G_R(y)$ be a smooth symmetric Lorentzian metric matrix of signature $(-,+,+,+)$, independent of the time coordinate. Write $G_R^{\mu\nu}$ for its inverse entries, $J_R=\sqrt{-\det G_R}$, $C_R^{ij}=G_R^{ij}$, $d_R^i=G_R^{i0}$, and $Q_R(y,p)=-G_R^{00}+2d_R^jp_j-C_R^{jk}p_jp_k$, with spatial indices summed from $1$ to $3$. Assume, uniformly in $R$ and on $A\times\{|p|\le p_0\}$, that $Q_R\ge\kappa>0$, $C_R\ge\kappa I$, and $G_R,G_R^{-1},J_R,J_R^{-1}$ have common zeroth-order bounds $M$. Define $P_R^i(y,p)=J_R(C_R^{ij}p_j-d_R^i)/\sqrt{Q_R}$. Then $A_R^{ij}=\partial_{p_j}P_R^i$ is symmetric, with $\lambda I\le A_R\le\Lambda I$ for positive constants depending only on $\kappa,M,p_0$.

If, in addition, $\sup_{R\ge R_0}\|G_R\|_{C^{4,\alpha}(A)}\le M_4$, then $P_R$ has common joint $C^{4,\alpha}$ bounds in $(y,p)$ on this fixed product domain, depending only on $A,\alpha,p_0,\kappa,M,M_4$.

For the zero-slope conclusion, assume $h_R:=J_R/\sqrt{-G_R^{00}}$ has a common $C^{3,\alpha}(A)$ bound $H$ and $\|d_R\|_{C^{3,\alpha}(A)}\le K R^{-2}$. Then, with the $y$ derivatives taken at fixed $p$, $s_R(y,0):=\sum_i\partial_{y_i}P_R^i(y,0)$ satisfies $\|s_R(\cdot,0)\|_{C^{2,\alpha}(A)}\le C H K R^{-2}$, where $C$ depends only on $A,\alpha$. The preceding uniform $C^{4,\alpha}$ hypothesis on $G_R$ supplies the required bound on $h_R$; the zeroth-order hypotheses alone do not.

### Facts & Assumptions

[F1] The Lorentzian and stationary flow-graph conventions are those of the graph definition; maximality means zero mean curvature. This lemma proves analytic properties of the specified flux. Identifying that flux with a particular graph equation is a separate application. [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[F2] Coefficient norms are ordinary Euclidean Hölder norms, applied componentwise; joint norms differentiate in both $y$ and $p$. The parameter $R$ is not a differentiation variable. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F3] For composable totally differentiable Euclidean maps, $D(g\circ f)=Dg(f)Df$. It applies to the smooth coefficient maps here, repeatedly through order four. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F4] Scalar sums, products, quotients with nonzero denominator, compositions and positive integer powers have their usual derivative rules. Apply these rules on coordinate lines and iterate for partial derivatives. [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules)

[F5] Matrix inversion preserves every finite $C^k$ class where the determinant is nonzero, and the determinant is a fixed finite polynomial in the matrix entries. [math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity) [math:cor-determinant-is-a-polynomial-in-the-matrix-entries](https://alphabetamath.cc/item/cor-determinant-is-a-polynomial-in-the-matrix-entries)

[F6] A scalar function on an interval with bounded derivative is Lipschitz with that bound; it applies to restrictions along the piecewise smooth paths used below. [math:cor-bounded-derivative-implies-lipschitz](https://alphabetamath.cc/item/cor-bounded-derivative-implies-lipschitz)

[F7] For a square matrix over a commutative ring with invertible determinant, $A^{-1}=\det(A)^{-1}\operatorname{adj}(A)$. Apply this to the real $4\times4$ matrices $G_R$, whose determinants are nonzero by the Lorentzian hypothesis. [math:cor-inverse-matrix-by-adjugate](https://alphabetamath.cc/item/cor-inverse-matrix-by-adjugate)

### Proof

**Given:** The hypotheses in the Statement, retaining the additional regularity hypotheses for the corresponding conclusions.

**Goal:** Prove uniform ellipticity, coefficient regularity and the differentiated zero-slope estimate.

1.1 Fix $R$ and put $z_R=C_Rp-d_R$. Symmetry of $C_R$ gives $\partial_{p_j}Q_R=-2z_R^j$. The scalar derivative rules and chain rule give $A_R=J_R(C_R/\sqrt{Q_R}+z_R\otimes z_R/Q_R^{3/2})$. This is symmetric. For every $\xi\in\mathbb R^3$, $\xi^TA_R\xi\ge J_R\kappa|\xi|^2/\sqrt{Q_R}$. The zeroth-order bounds and fixed slope ball bound $Q_R$ above and $z_R$ in norm; also $J_R\ge M^{-1}$ and $Q_R\ge\kappa$. Thus this lower bound is uniform and positive, and the displayed formula gives a uniform upper bound. [given, F3, F4, algebra]

1.2 Assume the additional $C^{4,\alpha}$ bound on $G_R$. By [F5], inversion is smooth on the invertible locus and determinant is polynomial. The identities $\sqrt{t+u}-\sqrt t=u/(\sqrt{t+u}+\sqrt t)$ and $(\sqrt t)'=1/(2\sqrt t)$, together with [F4], give all higher derivatives of $t^{1/2}$ and $t^{-1/2}$ for $t>0$. Their derivatives of any fixed order are bounded when $t$ is bounded away from zero and above. The bound on $J_R^{-1}$ gives $-\det G_R\ge M^{-2}$. The cofactor-over-determinant formula in [F7] expresses every derivative of inversion in the matrix entries as a polynomial numerator divided by a power of the determinant. Bounded matrix entries and this determinant lower bound therefore give common bounds on these derivatives, also on a fixed neighborhood of the matrix values; polynomial increment estimates keep the determinant away from zero on that neighborhood. Repeated use of [F3] and [F4], and $Q_R\ge\kappa$, expresses every mixed derivative of $P_R$ through order four as a finite sum of bounded coefficient functions times derivatives of $G_R$ of order at most four and bounded slope monomials. This proves the required derivative supremum bounds. [given, F3, F4, F5, F7, algebra]

2.1 For scalar factors, $a(x)b(x)-a(x')b(x')=a(x)(b(x)-b(x'))+b(x')(a(x)-a(x'))$ gives $[ab]_\alpha\le\|a\|_\infty[b]_\alpha+\|b\|_\infty[a]_\alpha$. The same identity iterates over finite products. Lower-order derivatives of $G_R$ are uniformly Lipschitz on $A$: two points can be joined by a radial segment and a shorter circular arc at the smaller radius, of total length at most $(1+\pi/2)$ times their Euclidean distance; use [F3] and [F6] on these path pieces with the next-derivative bound. On the product domain the slope points can additionally be joined by a straight segment. Thus these lower derivatives have common Hölder bounds on the bounded domain. The smooth coefficient functions from step 1.2 are uniformly Lipschitz as functions of the bounded matrix entries and slopes: their derivatives are bounded on a common neighborhood, so nearby pairs use a straight segment and [F6], while separated pairs use their supremum bounds. Applying the product inequality to the differentiated expressions in step 1.2, using the assumed Hölder bound on fourth derivatives of $G_R$, proves the joint $C^{4,\alpha}$ bound. The identical argument through order three at $p=0$, where $-G_R^{00}=Q_R(y,0)\ge\kappa$, bounds $h_R$ uniformly under the additional metric hypothesis. [given, F2, F3, F4, F6, step 1.2, algebra]

3.1 For the zero-slope estimate use its explicit $C^{3,\alpha}$ hypotheses on $h_R,d_R$, whether supplied directly or obtained for $h_R$ in step 2.1. Since $P_R(y,0)=-h_Rd_R$, one has $s_R(y,0)=-\sum_i((\partial_i h_R)d_R^i+h_R\partial_i d_R^i)$. Differentiating this formula at most twice gives only finite products of derivatives of $h_R$ and $d_R$ of order at most three. The lower-order Hölder control and product inequality of step 2.1 yield $\|s_R(\cdot,0)\|_{C^{2,\alpha}(A)}\le C\|h_R\|_{C^{3,\alpha}(A)}\|d_R\|_{C^{3,\alpha}(A)}\le C H K R^{-2}$. All constants are independent of $R$. The graph terminology in [F1] imposes no additional equation in this analytic proof. [given, F1, F2, F4, F6, step 2.1, algebra] ∎


## Uniform coefficient regularity before the final graph estimate

[Open item](item-lem-author-db87cb8e0bab-coefficient-regularity) · level 1


### Statement

Work in ZFC, with integer coordinate dimension $n\ge1$. Let $0<\alpha<1$ and let $P$ and $w$ satisfy the preceding gradient lemma on a fixed annulus, with common joint $C^{4,\alpha}$ bounds for $P$, $|Dw|\le p_0$ and $\|w\|_\infty\le M_0$. Then on any fixed smaller annulus, $A(y)=P_p(y,Dw)$ and $b^j(y)=\int_0^1s_{p_j}(y,tDw)\,dt$, where $s(y,p)=\sum_iP^i_{y_i}(y,p)$, have common $C^{2,\alpha}$ bounds. The constants depend on the structural bounds and $M_0$, not on any initially unknown derivative norm of $w$.

### Facts & Assumptions

[F1] The differentiated-flux estimate supplies a uniform $C^{0,\beta}$ bound for $Dw$ for some $0<\beta<1$, on compactly contained coordinate balls under the smooth flux, uniform ellipticity and slope hypotheses inherited in the Statement. [lem-author-db87cb8e0bab-divergence-gradient-holder](item-lem-author-db87cb8e0bab-divergence-gradient-holder)

[F2] Use the ordinary Euclidean $C^{k,\gamma}$ norms and scaled ball norms. Product and composition estimates needed below are proved in step 1.1 from these seminorm definitions. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F3] Under Countable Choice and in dimension $n\ge2$, the library interior Schauder estimate applies to a bounded $C^2$ solution with uniformly elliptic $C^{0,\gamma}$ principal coefficients, $C^{0,\gamma}$ forcing and finite coefficient seminorms; its constant depends only on the stated quantitative bounds. We take both lower-order coefficients to be zero. [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations)

[F4] For totally differentiable maps between open Euclidean sets, $D(G\circ\Phi)=DG(\Phi)D\Phi$. Apply this successively to the smooth maps used here. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F5] A continuous real integrand on a compact rectangle whose parameter derivative is continuous there may be differentiated through its Riemann integral. Apply this componentwise, with other coordinates fixed, and then to first parameter derivatives. [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle)

[F6] For integrable real functions on $[0,1]$, a uniform difference bound $\eta$ implies that their integrals differ by at most $\eta$. This also bounds an integral by taking one integrand to be zero. [math:lem-uniform-integral-error-bound](https://alphabetamath.cc/item/lem-uniform-integral-error-bound)

[F7] The real mean value theorem applies to each smooth component along a closed line segment contained in its coordinate domain; a derivative bound therefore bounds its increment by the segment length times that bound. [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

[A1] Work in ZFC, including the Axiom of Choice used by the gradient supplier. In particular Countable Choice holds: for any sequence of nonempty sets, choose on its family of values and compose that choice function with the sequence. This supplies the first Schauder theorem's choice hypothesis. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F20] The imported Corollary 2.21 supplies the higher-order a priori estimate recorded in External input, for already smooth solutions with controlled $C^{k,\gamma}$ coefficients and forcing.

### Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the asserted estimate with the stated uniform dependence.

1.1 On bounded convex coordinate balls, subtracting products gives $[fg]_{0,\gamma}\le\|f\|_\infty[g]_{0,\gamma}+\|g\|_\infty[f]_{0,\gamma}$; iterating gives the finite-product version. The increment identity $\Delta(fg)=f\Delta g+g\Delta f+\Delta f\Delta g$ also proves the ordinary product differentiation rule by division and passage to the limit. By F7 along segments, bounded first derivatives make a smooth outer map $G$ Lipschitz. Thus $[G\circ\Psi]_{0,\gamma}\le\operatorname{Lip}(G)[\Psi]_{0,\gamma}$; if instead $G$ is $\gamma$-Hölder and $\Psi$ Lipschitz, then $[G\circ\Psi]_{0,\gamma}\le[G]_{0,\gamma}\operatorname{Lip}(\Psi)^\gamma$. These componentwise inequalities and F4 give all product and composition estimates below on ball times slope-ball domains. [F2, F4, F7, algebra]

2.1 First suppose $n\ge2$. Reduce the exponent in F1 so that $0<\beta\le\alpha$; on a fixed bounded set this costs only a fixed diameter factor in the seminorm. On smaller balls F1 and step 1.1 give uniform $C^{0,\beta}$ bounds for $A(y)=P_p(y,Dw)$ and $s(y,Dw)$, where $s(y,p)=\sum_iP^i_{y_i}(y,p)$ uses derivatives at fixed $p$. The chain rule expands the given flux equation as $A^{ij}w_{ij}=-s(y,Dw)$. The inherited symmetric ellipticity bounds hold for $A$; the lower-order coefficients are zero; $w$ is smooth and bounded by $M_0$; and A1 supplies Countable Choice. All hypotheses of F3 are now satisfied, with $\gamma=\beta$. Its scaled estimate on fixed balls gives a uniform $C^{2,\beta}$ bound on smaller balls, without using any prior uniform higher derivative bound. [given, F1, F2, F3, F4, A1, step 1.1]

2.2 If $n=1$, work instead on compactly contained intervals in the annulus. The chain rule gives $w^{\prime\prime}=Q(y,w^\prime)$, where $Q(y,p)=-P_y(y,p)/P_p(y,p)$ and $P_p\ge\lambda>0$. The joint derivatives of $Q$ through order two have common bounds using only joint derivatives of $P$ through order three and powers of $\lambda^{-1}$: this follows by the product and chain rules and the directly differentiated identity $a(1/a)=1$. Hence $w^{\prime\prime}$ is bounded, then $w^{\prime\prime\prime}=Q_y+Q_p w^{\prime\prime}$ is bounded, and finally $w^{(4)}=Q_{yy}+2Q_{yp}w^{\prime\prime}+Q_{pp}(w^{\prime\prime})^2+Q_p w^{\prime\prime\prime}$ is bounded, with each $Q$ derivative evaluated at $(y,w^\prime(y))$. Together with the given height and slope bounds, this supplies all derivative suprema through order four. This is all that the remaining argument needs; no use of the dimension-restricted Schauder theorem is made in this case. [given, F4, step 1.1, algebra]

3.1 Still for $n\ge2$, the chain and product rules with the $C^{2,\beta}$ bound give uniform $C^{1,\beta}$ bounds for $A$ and $s(y,Dw)$ on a smaller ball. Apply F20 with $k=1$ and $\gamma=\beta$ after rescaling that ball to obtain uniform $C^{3,\beta}$ bounds for $w$ on its half ball. The same chain and product rules now bound $A$ and $s(y,Dw)$ in $C^{2,\beta}$; F20 with $k=2$ gives a uniform $C^{4,\beta}$ bound on a further smaller ball. Smoothness on neighborhoods of the compact closures supplies the finite $C^{k+2,\beta}$ membership required by each a priori application before it is used; its unknown preliminary norm never enters the right side. All radii and their ratios are fixed, and these preliminary bounds may depend on $M_0$ without being linear in it. [step 2.1, step 1.1, F2, F4, F20, given]

4.1 In either dimension case the suprema of derivatives of $w$ through order four are now uniformly bounded. F7 and F4 along segments show that $Dw,D^2w,D^3w$ are uniformly Lipschitz on smaller balls. Put $\Phi_t(y)=(y,tDw(y))$ for $0\le t\le1$, $G(y,p)=P_p(y,p)$ and $H_j(y,p)=s_{p_j}(y,p)$. The maps $\Phi_t,D\Phi_t,D^2\Phi_t$ are uniformly bounded and Lipschitz, uniformly in $t$. For either $J=G$ or $J=H_j$, twice applying F4 gives $D^2(J\circ\Phi_t)=D^2J(\Phi_t)[D\Phi_t,D\Phi_t]+DJ(\Phi_t)D^2\Phi_t$. The joint derivatives of $G$ through order two use derivatives of $P$ through order three, and those of $H_j$ through order two use derivatives of $P$ through order four. Their common $\alpha$-Hölder bounds follow from the given joint $C^{4,\alpha}$ bound (lower derivatives use F7 locally). Thus step 1.1 bounds $G\circ\Phi_1=A$ in $C^{2,\alpha}$ and bounds $h_j(y,t):=H_j(\Phi_t(y))$ and its first two $y$ derivatives in the same norms uniformly in $t$. No fifth derivative of $P$ is used. [step 3.1, step 2.2, step 1.1, F2, F4, F7, given]

5.1 On every closed coordinate box inside a controlled ball, $h_j$ and its first two spatial derivatives are continuous jointly with $t\in[0,1]$; smoothness on a neighborhood of the slope ball ensures this also when $tDw$ is on its boundary. Apply F5 along each coordinate interval, and again to each first derivative, to obtain $D_y^\nu b^j(y)=\int_0^1D_y^\nu h_j(y,t)\,dt$ for $|\nu|\le2$. F6 applied with one integrand zero bounds these derivative suprema. Applied to the second derivatives at two spatial points, it bounds their $\alpha$-Hölder differences by the common bounds of step 4.1. Finally choose a fixed finite interior cover of the desired smaller annulus by controlled balls whose concentric half balls still cover it. For pairs closer than half the least covering radius, the ball for the first point contains both points; separated pairs use the derivative sup bounds divided by that fixed separation to the power $\alpha$. The resulting $C^{2,\alpha}$ bounds for $A$ and $b$ depend only on the structural data, $M_0$ and the fixed annuli, without dependence on initially unknown derivative norms of $w$. [step 4.1, F2, F5, F6, given] ∎

### External input

[F20] Imported established input (Corollary 2.21): For $k\ge1$, $0<\gamma<1$, and $z\in C^{k+2,\gamma}(B_1)$ solving $a^{ij}D_{ij}z=f$, if $\lambda I\le a\le\Lambda I$ and $a,f\in C^{k,\gamma}(B_1)$, then $\|z\|_{C^{k+2,\gamma}(B_{1/2})}\le C(\|z\|_\infty+\|f\|_{C^{k,\gamma}(B_1)})$, with $C=C(n,k,\gamma,\lambda,\Lambda,\|a\|_{C^{k,\gamma}})$. The higher-order estimate is an a priori estimate and requires the displayed regularity of $z$ before use. Applied here only for $n\ge2$ and $k=1,2$ on rescaled compactly contained balls; smoothness gives this membership, and the preceding stage supplies uniform coefficient and forcing norms. The $k=0$ first stage uses the declared library theorem instead. Dimension one is handled locally. Reading limits: Read the complete extracted statements and hypotheses of Theorem 2.20 and Corollary 2.21 on printed pp. 46–47 (PDF pp. 52–53) in the author-hosted PDF during this assignment. Their proofs were not read or reconstructed; only the stated a priori estimates are imported.


## Coordinate and weak forms of the geometric Schrödinger equation

[Open item](item-lem-author-58255dfd955f-coordinate-schrodinger-form) · level 1


### Statement

Let $(\Sigma,h)$ be the smooth exterior, with real smooth $V$ and real $u\in C^2_{\mathrm{loc}}(\Sigma^\circ)$, where $\Sigma^\circ=\Sigma\setminus\partial\Sigma$. In any relatively compact coordinate chart $U$, including a boundary chart, put $U^\circ=U\cap\Sigma^\circ$, $m=\sqrt{\det(h_{ij})}$, $A^{ij}=mh^{ij}$ and $q=mV$. On $U^\circ$, the classical equation $(\Delta_h-V)u=0$ is equivalent to $-\partial_i(A^{ij}\partial_j u)+qu=0$. For such a $C^2$ function these equations are also equivalent to the weak identity $\int_{U^\circ}(A^{ij}\partial_j u\partial_i\varphi+qu\varphi)\,dx=0$ for every real $\varphi\in C_c^\infty(U^\circ)$, so every test has support compactly contained in the interior, away from the manifold boundary. Here $dx$ and the test functions are understood in chart coordinates. The matrix $A$ is symmetric uniformly positive definite on compact chart subsets, including those meeting $\partial\Sigma$. In nondivergence form the operator is $h^{ij}\partial_{ij}+b^j\partial_j-V$, where $b^j=m^{-1}\partial_i(mh^{ij})$. If $u$ is $C^2$ up to a portion of $U\cap\partial\Sigma$, the pointwise operator formulas and classical equation extend there by continuity.

### Facts & Assumptions

**Given:** The exterior, its smooth metric, boundary-chart conventions and sign convention are those of [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data). Use the regularity and notation in the Statement; repeated indices are summed. At finite regularity, the gradient is the metric dual of the differential, divergence is the trace of the Levi-Civita covariant derivative of a $C^1$ vector field, and the Laplacian is the metric trace of the Hessian of a $C^2$ function. Step 1.1 justifies the smooth supplier formulas at this regularity. A weak solution here means the displayed identity for interior-supported tests, with $u$ and its first derivatives locally square integrable on $U^\circ$; every $C^2$ function has that local integrability.

[F1] For smooth functions the gradient has components $h^{ij}\partial_j u$ by [math:def-riemannian-gradient](https://alphabetamath.cc/item/def-riemannian-gradient). For smooth vector fields the divergence has density formula $m^{-1}\partial_i(mX^i)$ by [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence). For smooth functions the metric trace of the Hessian equals divergence of gradient by [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian). These are smooth-input supplier statements; the needed extension is proved locally below.

[F2] For a real $C^1$ function $g$ on an open interval containing $[a,b]$, $\int_a^b g'(t)\,dt=g(b)-g(a)$, including oriented endpoints, by [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts).

[F3] A continuous real function on a nondegenerate closed rectangle in $\mathbb R^n$, $n\ge1$, has repeated Riemann integrals in every coordinate order, all equal to its multiple integral, by [math:cor-repeated-riemann-integrals-on-rectangles](https://alphabetamath.cc/item/cor-repeated-riemann-integrals-on-rectangles). We use this continuous-input result on enclosing rectangles for the compactly supported coordinate integrands below; no measurable-section or exceptional-section assertion is needed.

[F4] For $n\ge1$, [math:lem-schwartz-cutoffs-from-the-standard-smooth-step](https://alphabetamath.cc/item/lem-schwartz-cutoffs-from-the-standard-smooth-step) supplies $\chi\in C_c^\infty(\mathbb R^n)$ with $0\le\chi\le1$, $\chi=1$ on $|x|\le1$ and $\chi=0$ on $|x|\ge2$, together with smooth rescalings $\chi_R(x)=\chi(x/R)$ for $R>0$. We use $n=3$ and translate a rescaling inside the interior chart image.

### Proof

**Given:** The hypotheses and data in the Statement and Facts & Assumptions.

**Goal:** Establish the coordinate, ellipticity and interior weak-form conclusions of the Statement.

**Proof technique:** direct.

1.1 Fix an interior point $p$ with coordinates $x_0$. The smooth polynomial $P(x)=u(p)+\partial_i u(p)(x^i-x_0^i)+\tfrac12\partial_{ij}u(p)(x^i-x_0^i)(x^j-x_0^j)$ has the same derivatives through order two as $u$ at $p$. Metric duality gives $(\operatorname{grad}_h u)^i=h^{ij}\partial_j u$ directly, and differentiation gives $\partial_k(\operatorname{grad}_h u)^i=(\partial_kh^{ij})\partial_j u+h^{ij}\partial_{kj}u$. Thus $\operatorname{grad}_h u$ and $\operatorname{grad}_h P$ have equal values and first derivatives at $p$, so their covariant derivatives and traces agree there. More generally, the trace of $\nabla X$ for $C^1$ $X$ depends only on $X(p)$ and its first coordinate derivatives: replacing its coefficients by affine polynomials with those same data reduces the divergence density formula to its smooth case in [F1]. Applying [F1] to $P$ therefore proves $\Delta_hu(p)=m^{-1}\partial_i(mh^{ij}\partial_j u)(p)$, since the right side also uses only these derivatives through order two. This proves the required $C^2$ and $C^1$ extensions without assuming extra regularity. [F1, given, algebra]

2.1 Multiply the formula in step 1.1 by $m>0$ and change the sign to obtain the divergence equation. Expanding its derivative gives $\Delta_hu=h^{ij}\partial_{ij}u+m^{-1}\partial_i(mh^{ij})\partial_j u$, proving the nondivergence expression. If $u$ is $C^2$ up to the chart boundary, continuity of all these expressions extends the identities and any classical equation to that boundary. The inverse metric is symmetric positive definite and $m>0$. On any nonempty compact chart subset $K$, the continuous positive function $A^{ij}(x)\xi_i\xi_j$ on $K\times\{\xi\in\mathbb R^3:|\xi|=1\}$ has positive minimum and finite maximum. These are the asserted uniform ellipticity bounds, also when $K$ meets the boundary. [step 1.1, given, algebra]

3.1 Let $\varphi\in C_c^\infty(U^\circ)$ be real. For each $i$, put $G^i=A^{ij}\partial_j u\,\varphi$ on the interior chart image $\Omega$. This is $C^1$ and its support is compactly contained in $\Omega$. Its zero extension $\widehat G^i$ is $C^1$ on $\mathbb R^3$: near every point outside that compact support it is identically zero. Choose a nondegenerate closed rectangle $Q=\prod_{k=1}^3[a_k,b_k]$ with this support in its interior. The derivative $\partial_i\widehat G^i$ is continuous on $Q$, so [F3] computes its multiple integral by integrating first in $x^i$. For every fixed choice of the other coordinates, $t\mapsto\widehat G^i(x^1,\ldots,t,\ldots,x^3)$ is $C^1$ on $\mathbb R$ and vanishes at $a_i,b_i$. Thus [F2] makes its derivative's integral on $[a_i,b_i]$ zero, and [F3] gives $\int_Q\partial_i\widehat G^i\,dx=0$. All coordinate integrands are continuous with compact support, so their integrals are computed on such enclosing rectangles. Summing in $i$, applying the product rule and rearranging yields $\int_{U^\circ}(-\partial_i(A^{ij}\partial_j u)+qu)\varphi\,dx=\int_{U^\circ}(A^{ij}\partial_j u\partial_i\varphi+qu\varphi)\,dx$. If the classical equation holds, step 2.1 makes the left side zero, proving the weak identity. This integration-by-parts identity itself used only the regularity of $u$ and $\varphi$, and the support restriction excludes a manifold-boundary contribution even when $U$ is a boundary chart. [F2, F3, step 2.1, given, algebra]

4.1 Conversely, for the assumed $C^2$ function the residual $f=-\partial_i(A^{ij}\partial_j u)+qu$ is continuous on $U^\circ$. The same integration by parts turns the weak identity into $\int f\varphi\,dx=0$ for every such test. If $f(p)\ne0$, continuity gives $\delta>0$ such that the closed coordinate ball $\overline B_\delta(x_0)$ about the coordinates $x_0$ of $p$ is contained in the interior chart image and $f$ has the sign of $f(p)$ with $|f|\ge |f(p)|/2$ throughout this ball. Use [F4] with $n=3$ and set $\varphi(x)=\chi(2(x-x_0)/\delta)$. Translation of the smooth rescaling with $R=\delta/2$ is smooth; moreover $0\le\varphi\le1$, $\varphi=1$ on $\overline B_{\delta/2}(x_0)$ and $\operatorname{supp}\varphi\subseteq\overline B_\delta(x_0)$. Thus $\varphi\in C_c^\infty(U^\circ)$ is an admissible test, and $f\varphi$ has one sign everywhere and absolute value at least $|f(p)|/2$ on the smaller ball. Its integral is nonzero, contradicting the weak identity. This proves $f=0$, and step 2.1 recovers the classical geometric equation. Thus the weak and classical equations are equivalent at the stated regularity. [F4, step 2.1, step 3.1, given, algebra] ∎


## Multiplicative interior Harnack for geometric Schrödinger solutions

[Open item](item-lem-author-58255dfd955f-local-potential-harnack) · level 1


### Statement

Work in ZFC. Let $n\ge1$ be an integer, let $(\mathcal N,h)$ be a smooth $n$-dimensional Riemannian manifold, and identify an open coordinate neighborhood with the Euclidean ball $B_r(x_0)\subset\mathbb R^n$, where $r>0$. All balls and coefficient norms below are in these coordinates. The Laplace–Beltrami operator has sign convention $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$, equivalently the metric trace of the Levi-Civita Hessian, using the same pointwise expression for $C^2$ functions. Let $V:B_r(x_0)\to[0,\infty)$ be bounded, with no measurability assumption, and let $u\in C^2(B_r(x_0);\mathbb R)$ be nonnegative and satisfy $(\Delta_h-V)u=0$ pointwise. Put $m=\sqrt{\det(h_{ij})}$, $A=(mh^{ij})$ and $q=mV$. Suppose $\lambda>0$, $M<\infty$ and $Q\ge0$ satisfy $\xi^TA(x)\xi\ge\lambda|\xi|^2$, $\|A(x)\|_{\mathrm{op}}\le M$ and $q(x)\le Q$ at every point, for all $\xi\in\mathbb R^n$. Then

$$\sup_{B_{r/2}(x_0)}u\le C\inf_{B_{r/2}(x_0)}u,$$

where $C\ge1$ depends only on $n$, $M/\lambda$ and $r^2Q/\lambda$. This includes $n=1$ and the identically zero solution.

### Facts & Assumptions

**Given:** The pointwise data and bounds in the Statement. Work in ZFC, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice), as required by the analytic supplier and its formulation inputs; no additional choice is used by the local coordinate calculation.

[F1] The Riemannian metric is as in [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold). The smooth-function gradient formula is [math:def-riemannian-gradient](https://alphabetamath.cc/item/def-riemannian-gradient), the smooth-vector-field divergence density formula is [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence), and the trace-of-Hessian Laplacian with the stated sign is [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian). Their extension to the $C^2$ function in this item is justified in step 1.1; no exterior topology or smoothness of $V$ is assumed.

[F2] Use the affine-map case of [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) to differentiate $T_s(y)=x_0+sy$ and its compositions, where $0<s<r$ and $DT_s=sI$. The rescaling is calculated pointwise below, so it does not require a substitution theorem for a nonmeasurable integrand.

[F3] Measurability means the Borel/Lebesgue convention of [math:def-borel-and-lebesgue-measurable-function-on-rn](https://alphabetamath.cc/item/def-borel-and-lebesgue-measurable-function-on-rn), with coefficients extended by zero outside their open balls. Use the real Sobolev space from [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm). For $d\ge2$, [math:thm-divergence-theorem-for-bounded-c-one-euclidean-domains](https://alphabetamath.cc/item/thm-divergence-theorem-for-bounded-c-one-euclidean-domains) applies to $C^1$ vector fields on a neighborhood of a closed Euclidean ball. In particular a field vanishing near its boundary has zero integrated divergence. This will supply both the weak derivative identities and the weak equation in step 5.1.

[F4] [thm-author-58255dfd955f-bounded-potential-harnack-input](item-thm-author-58255dfd955f-bounded-potential-harnack-input) supplies the homogeneous unit-ball Harnack theorem in dimension $d\ge2$: a real measurable symmetric matrix $H\ge I$ with $\sum_{i,j}|H^{ij}|\le\Lambda$ and a measurable potential $0\le b\le K$ give $\operatorname{ess\,sup}_{B_{1/2}}w\le C_H(d,\Lambda,K)\operatorname{ess\,inf}_{B_{1/2}}w$ for every nonnegative real $W^{1,2}(B_1)$ weak solution of $-\operatorname{div}(H\nabla w)+bw=0$. Its weak identity is against all real $C_c^\infty(B_1)$ tests with Lebesgue integrals. The supplier records the independent Simon source, its exact coefficient specialization and reading limits; the underlying iteration theorem is imported, not reproved here.

### Proof

**Given:** The data of the Statement and [F1]–[F4].

**Goal:** The stated multiplicative comparison with only the displayed parameter dependence.

**Proof technique:** direct.

1.1 At any coordinate point $p$, replace $u$ by the quadratic polynomial having its value, first derivatives and second derivatives at $p$. The metric trace of the Levi-Civita Hessian uses only these data: in coordinates its Hessian entries are $\partial_{ij}u-\Gamma^k_{ij}\partial_k u$. Apply the smooth formulas in [F1] to this polynomial. The coordinate expression $m^{-1}\partial_i(mh^{ij}\partial_j u)$ also uses only these same derivatives through order two, so the polynomial and $u$ give equal values on both sides at $p$. Thus $\Delta_hu=m^{-1}\partial_i(A^{ij}\partial_j u)$ throughout the ball at the stated $C^2$ regularity. Multiplying the pointwise equation by $m$ gives $\partial_i(A^{ij}\partial_j u)=qu$, with repeated indices summed. Here $A$ is smooth and symmetric. [given, F1, algebra]

2.1 Set $D=\{x:u(x)>0\}$, an open set, and define $q_*(x)=m(x)\Delta_hu(x)/u(x)$ on $D$ and $q_*(x)=0$ off $D$. On $D$ this coefficient is continuous and equals $q$ by the given equation; hence $0\le q_*\le Q$ everywhere. Its zero extension is Borel: on the open set $D$ it is continuous, and on the complementary closed set it is constant, so preimages of open subsets of $\mathbb R$ are Borel. At points where $u=0$, the pointwise equation gives $\Delta_hu=Vu=0$. Consequently $q_*u=qu=m\Delta_hu$ everywhere, including those points, and $-\operatorname{div}(A\nabla u)+q_*u=0$ pointwise. In particular $q_*u$ is continuous even though $q_*$ need not be continuous. This construction includes $u\equiv0$ and makes no assertion that the originally given $V$ is measurable. [given, F3, step 1.1, algebra]

3.1 Fix $0<s<r$ and set $v(y)=u(T_s(y))$, $\widetilde A(y)=A(T_s(y))/\lambda$ and $\widetilde b(y)=s^2q_*(T_s(y))/\lambda$ on $B_1\subset\mathbb R^n$. The chain rule gives $\partial_{y_j}v=s(\partial_{x_j}u)\circ T_s$ and $\operatorname{div}_y(\widetilde A\nabla_yv)=(s^2/\lambda)(\operatorname{div}_x(A\nabla_xu))\circ T_s$. Thus $-\operatorname{div}_y(\widetilde A\nabla_yv)+\widetilde b v=0$ pointwise. The matrix $\widetilde A$ is smooth, symmetric and at least $I$, and $|\widetilde A^{ij}|\le M/\lambda$. The potential is Borel and satisfies $0\le\widetilde b\le K:=r^2Q/\lambda$, with this fixed bound independent of $s$. Because $\overline{B_s(x_0)}$ is compactly contained in $B_r(x_0)$, $v$ and $\widetilde A$ are respectively $C^2$ and smooth on a neighborhood of $\overline{B_1}$. [F2, F3, step 2.1, given, algebra]

4.1 If $n\ge2$, put $d=n$, $w=v$, $H=\widetilde A$ and $b=\widetilde b$. If $n=1$, put $d=2$ and, on the two-dimensional unit disk, set $w(z_1,z_2)=v(z_1)$, $H(z_1,z_2)=\operatorname{diag}(\widetilde A(z_1),1)$ and $b(z_1,z_2)=\widetilde b(z_1)$. In this latter case $\partial_2w=0$ and the equation of step 3.1 gives $-\partial_1(\widetilde A(z_1)v'(z_1))+b(z_1,z_2)w(z_1,z_2)=0$, exactly $-\operatorname{div}(H\nabla w)+bw=0$ on the disk. In either case $d\ge2$, $w\ge0$, $w$ is $C^2$ near the closed disk or ball, $H$ is smooth symmetric with $H\ge I$, and $b$ is Borel with $0\le b\le K$. Since $M/\lambda\ge1$, the entrywise bound $\sum_{i,j}|H^{ij}|\le d^2M/\lambda$ holds in both cases; for the lifted matrix its sum is at most $M/\lambda+1$. No one-dimensional version of the imported theorem is assumed. [step 3.1, given, algebra]

5.1 The function $w$ and its classical first derivatives are bounded on $B_1\subset\mathbb R^d$ and therefore square integrable. For every real $\varphi\in C_c^\infty(B_1)$, the field $\varphi w e_i$ is $C^1$ and vanishes near the boundary. Applying [F3] to its divergence gives $\int w\partial_i\varphi=-\int(\partial_iw)\varphi$, so these classical derivatives are weak derivatives and $w\in W^{1,2}(B_1)$. Likewise the field $\varphi H\nabla w$ is $C^1$ and vanishes near the boundary. Its divergence integrates to zero; the pointwise equation in step 4.1 and the product rule give $\int_{B_1}(H\nabla w\cdot\nabla\varphi+bw\varphi)=0$. The products are measurable and integrable; indeed $bw=\operatorname{div}(H\nabla w)$ is continuous. These are precisely the weak-solution hypotheses of [F4]. Therefore [F4] gives the comparison on $B_{1/2}\subset\mathbb R^d$ with the same constant $C_H(d,d^2M/\lambda,K)$ for every $s$. [F3, F4, step 4.1, algebra]

6.1 Since $w$ is continuous, its essential supremum and infimum on the open half-ball equal its ordinary supremum and infimum: any strict pointwise violation of an essential bound persists on a nonempty open ball, which has positive Lebesgue measure. For $n\ge2$ this directly gives $v(y)\le Cv(y')$ for all $y,y'\in B_{1/2}$. For $n=1$, restrict the resulting pointwise comparison to the pairs $(y,0),(y',0)$ in the half-disk; these range over all $y,y'\in(-1/2,1/2)$. Thus in all cases $u(x)\le Cu(x')$ for $x,x'\in B_{s/2}(x_0)$, where $C=\max\{1,C_H(d,d^2M/\lambda,r^2Q/\lambda)\}$ depends only on the asserted parameters. Every pair in $B_{r/2}(x_0)$ lies in some such smaller half-ball, so the same pairwise comparison holds throughout $B_{r/2}(x_0)$. Taking the supremum in $x$ and then the infimum in $x'$ proves the Statement. [step 5.1, step 4.1, given, algebra] ∎


## Compact-domain scalar Poisson solvability and fourth-order estimates

[Open item](item-lem-author-86990d62062f-compact-domain-poisson) · level 1


### Statement

Fix $0<\alpha<1$. Let $M$ be a compact smooth Riemannian three-manifold with smooth boundary, every connected component meeting the boundary. For $f\in C^{2,\alpha}(M)$ there is a unique $u\in C^{4,\alpha}(M)$ with $\Delta_hu=f$ and $u|_{\partial M}=0$. On a fixed smaller interior or boundary chart the fourth-order norm is bounded by the $C^{2,\alpha}$ norm of $f$ on a larger chart and the supremum of $u$ there. The constants depend on $\alpha$, the fixed smooth metric and charts, and the separation from artificial chart edges. Here $C^{k,\alpha}$ means derivatives through order $k$ continuous to the boundary and order-$k$ derivatives $\alpha$-Hölder. No orientability of $M$ is assumed. Work in ZFC, supplying the choice assumptions of the analytic inputs.

### Statement references

[def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### Facts & Assumptions

**Given:** the Statement hypotheses and $0<\alpha<1$; work in ZFC.

[F1] Smooth boundary charts and finite smooth partitions of unity are available. The exterior-data definition fixes the Riemannian metric, coordinate Hölder conventions and Laplacian sign; it is not used as a topology reduction of $M$ to a Euclidean domain. [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary) [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F2] The Riemannian density and its associated measure are independent of orientation; measurable integration is the partition-weighted coordinate integral. For boundary charts the boundary hyperplane has three-dimensional Lebesgue measure zero. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density) [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)

[F3] Euclidean weak Sobolev spaces are complete, smooth bounded domains admit bounded Sobolev extensions, Rellich gives $W^{1,2}$ compactness into $L^2$ in dimension three, the trace is bounded and agrees with continuous boundary restriction, and zero weak gradient implies componentwise constancy. A complete inner-product space is Hilbert. [math:def-sobolev-space-wkp-and-its-norm](https://alphabetamath.cc/item/def-sobolev-space-wkp-and-its-norm) [math:thm-sobolev-spaces-are-banach-spaces](https://alphabetamath.cc/item/thm-sobolev-spaces-are-banach-spaces) [Sobolev extension on smooth domains](https://alphabetamath.cc/item/thm-extension-theorem-for-bounded-smooth-domains) [math:thm-rellich-kondrachov-for-p-less-than-n](https://alphabetamath.cc/item/thm-rellich-kondrachov-for-p-less-than-n) [math:thm-lp-trace-operator-on-a-bounded-c-one-domain](https://alphabetamath.cc/item/thm-lp-trace-operator-on-a-bounded-c-one-domain) [math:thm-zero-weak-gradient-implies-componentwise-constancy](https://alphabetamath.cc/item/thm-zero-weak-gradient-implies-componentwise-constancy) [math:def-hilbert-space](https://alphabetamath.cc/item/def-hilbert-space)

[F4] Lax–Milgram applies to a bounded coercive bilinear form on a real Hilbert space. Weak boundary regularity gives a two-derivative gain on smooth bounded Dirichlet domains, and the separately declared nested-domain lemma supplies the interior gain. For weak solutions with locally square-integrable data, aligned boundary charts preserve the weak equation and, after localization, zero Dirichlet data. Smooth cutoff products have the stated weak-derivative bounds. The pullback of arbitrary Sobolev functions is supplied separately in [F6] and step 1.1. In dimension three, $H^4$ embeds into $C^{2,\gamma}$ for $0<\gamma<1/2$ on smooth bounded patches. [math:thm-lax-milgram](https://alphabetamath.cc/item/thm-lax-milgram) [math:thm-higher-order-boundary-regularity-for-dirichlet-problems](https://alphabetamath.cc/item/thm-higher-order-boundary-regularity-for-dirichlet-problems) [math:lem-nested-domain-induction-for-interior-elliptic-derivatives](https://alphabetamath.cc/item/lem-nested-domain-induction-for-interior-elliptic-derivatives) [math:lem-weak-divergence-form-equations-are-invariant-under-c-two-boundary-charts](https://alphabetamath.cc/item/lem-weak-divergence-form-equations-are-invariant-under-c-two-boundary-charts) [math:lem-cutoff-difference-quotient-commutator-estimate](https://alphabetamath.cc/item/lem-cutoff-difference-quotient-commutator-estimate) [math:thm-higher-order-sobolev-embedding](https://alphabetamath.cc/item/thm-higher-order-sobolev-embedding)

[F5] Classical second-order interior and global Dirichlet Schauder regularity and estimates are supplied by the library. The distinct imported higher-order regularity and local boundary estimate are specified in External input. [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations) [math:thm-boundary-schauder-estimate-for-the-dirichlet-problem](https://alphabetamath.cc/item/thm-boundary-schauder-estimate-for-the-dirichlet-problem)

[F6] For an integer $m\ge1$, let $T:U\to V$ be a $C^m$ diffeomorphism of open subsets of $\mathbb R^3$. Let $U_0\Subset U$ and $V_0\Subset V$ be open with $T(U_0)\subseteq V_0$, and assume bounded derivatives through order $m$ of $T$ on $\overline{U_0}$ and of $T^{-1}$ on $\overline{V_0}$. Then every $z\in W^{m,2}(V_0)$ has $z\circ T\in W^{m,2}(U_0)$, with a norm bound depending only on the dimension, $m$ and these chart bounds, and its weak derivatives satisfy the iterated chain rule. There is no differential-equation hypothesis. The supplier is initially applied only on patches compactly contained in the open coordinate interiors; step 1.1 extends the estimate to the boundary half-patches used here. [Sobolev boundary flattening](https://alphabetamath.cc/item/lem-c-k-boundary-flattening-preserves-wkp-locally)

### External input

The Schikorra reference supplies only the second-order global Dirichlet regularity statement under its stated admissibility hypotheses; smooth bounded domains are admissible. The corresponding library interface is [F5].

The Gilbarg–Trudinger reference supplies higher-order classical regularity (Theorems 6.17 and 6.19, with its local-boundary-portion conclusion) and the second-order local boundary estimate (Lemma 6.4 and Corollary 6.7). For the former, $C^{k,\alpha}$ coefficients and forcing give $C^{k+2,\alpha}$ regularity of a given classical solution, locally up to a $C^{k+2,\alpha}$ boundary portion carrying such Dirichlet values. For the latter, a given $C^{2,\alpha}$ solution has its smaller-patch norm bounded by the larger-patch forcing norm, Dirichlet-data norm and solution supremum, with positive separation from artificial edges. Uniform ellipticity, the coefficient bounds and $0<\alpha<1$ are required. These are imported Euclidean facts, not a claim to have reconstructed their proofs. No manifold existence result or fourth-order estimate is imported.

### Proof

**Given:** the Statement hypotheses; $0<\alpha<1$; ZFC. **Goal:** construct the solution and prove its fourth-order local estimate.

**Proof technique:** direct, combining a local Hilbert-space construction with the declared weak and classical regularity inputs.

1.1 First establish pullback bounds independently of any equation or manifold Sobolev construction. Let $T$ be a smooth coordinate transition between interior patches or between the open interiors of matched boundary half-patches. Restrict to patches with compact closure inside the ambient chart neighbourhoods, allowing that closure to meet the physical boundary. Boundary-chart compatibility in [F1] gives local ambient smooth extensions of the transition and its inverse. After finite subdivision, their derivatives through any fixed integer order $m\ge1$ are bounded and their Jacobians are bounded away from zero on these closures. For arbitrary $z\in H^m$ on the target patch, apply [F6] on compactly contained open interior subpatches: $D^\nu(z\circ T)$ is the sum of $(D^\beta z)\circ T$ times the prescribed bounded polynomials in derivatives of $T$, including order zero. These weak identities agree on overlapping interior subpatches. Exhaust the source open patch by such subpatches, choosing larger target interior subpatches containing their images. The norm estimates in [F6] have one common constant, since they depend only on $m$, dimension and the stated uniform chart and inverse bounds. Their right sides are bounded by the norm on the whole target patch. Taking the increasing integrals of the nonnegative squared derivative fields proves $\|z\circ T\|_{H^m}\le C\|z\|_{H^m}$ on the whole source half-patch, with the same weak identities. Every test function has compact support in that open half-patch, so these are its global weak derivatives. The inverse transition has the analogous bound. In particular $m=1$ applies to arbitrary functions and Cauchy sequences, without assuming that they are weak solutions; $m\le4$ also supplies the higher-order pullbacks used below. [F1, F6]

2.1 Let $d\mu_h$ be the measure of [F2], whose chart density is $\sqrt{\det h}\,dx$. Choose finitely many relatively compact coordinate patches and smooth cutoffs $\chi_i$ with $\sum_i\chi_i=1$. Each cutoff is supported away from artificial chart edges. In a boundary chart use a bounded smooth auxiliary domain in $\{x_3>0\}$ with a flat boundary portion covering that support; round its other boundary away from the support. Define $H^1(M)$ to consist of $L^2(d\mu_h)$ classes with local weak first derivatives and finite norm $\|v\|_{H^1_h}^2=\int_M(v^2+|dv|_h^2)\,d\mu_h$. On the compact supports, smooth metric positivity and bounded chart Jacobians make this norm equivalent to the square root of the sum of the squared Euclidean $W^{1,2}$ norms of $\chi_i v$, extended by zero only past artificial edges. The product formula bounds these local norms by the intrinsic norm; conversely $v=\sum_i\chi_i v$ and $dv=\sum_i d(\chi_i v)$ give the reverse bound. For arbitrary functions, coordinate changes obey the weak chain rule and bounded pullback estimates of step 1.1. Thus different such finite atlases give the same space and equivalent norms. All integrals are intrinsic density integrals, including on a nonorientable $M$. [F1, F2, F3, F4, step 1.1]

3.1 If $v_j$ is Cauchy in this norm, each $\chi_i v_j$ converges in Euclidean $W^{1,2}$ by completeness. The local limits agree as pieces of one function: on overlaps the identities $\chi_l(\chi_i v_j)=\chi_i(\chi_l v_j)$ pass to the $L^2$ limits using bounded coordinate pullbacks. Sum the finitely many pieces to obtain $v$; then $\chi_i v$ is the corresponding local limit. Testing against compactly supported smooth functions shows that its derivative limits are the weak derivatives of $v$. The norm equivalence proves $v_j\to v$ in $H^1_h$. The displayed norm comes from the positive-definite inner product $\int_M(vw+\langle dv,dw\rangle_h)\,d\mu_h$, so $H^1(M)$ is a real Hilbert space. Its closed subspace $H^1_0(M)$, defined as the closure of $C_c^\infty(M\setminus\partial M)$ in this norm, is Hilbert: a Cauchy sequence converges in $H^1(M)$ and its limit lies in that closure. [F2, F3, step 1.1, step 2.1]

4.1 The inclusion $H^1(M)\to L^2(M)$ is compact by applying Rellich with $p=q=2$, $n=3$, on the finitely many smooth auxiliary domains and taking finitely many successive subsequences; the extension theorem verifies the domain hypothesis. The local bounded trace operators give zero trace for every member of $H^1_0(M)$ by its defining closure. If Poincaré failed, choose $v_j\in H^1_0(M)$ with $\|v_j\|_2=1$ and $\|dv_j\|_2\to0$. Compactness gives an $L^2$ limit $v$. In charts, distributional testing gives $dv=0$; moreover $v_j\to v$ in $H^1_h$, so $v\in H^1_0(M)$. Zero-gradient constancy in connected coordinate interiors, and agreement on overlaps, give one constant on each component of $M$; the interior of each connected boundary manifold is connected, since a path may be pushed off the boundary in finitely many half-charts. Each component has a boundary chart, whose flat open boundary piece has positive surface measure. Its constant has zero trace there, hence is zero. This contradicts $\|v\|_2=1$. Thus $\|v\|_2\le C\|dv\|_2$ on $H^1_0(M)$. Choice is used only as permitted in the analytic suppliers and the subsequence argument. [F1, F2, F3, step 3.1]

5.1 On this Hilbert space the form $a(v,w)=\int_M\langle dv,dw\rangle_h\,d\mu_h$ is bounded and coercive by Poincaré. The functional $w\mapsto-\int_Mfw\,d\mu_h$ is bounded by Cauchy–Schwarz, since $f$ is continuous and the compact manifold has finite volume. Lax–Milgram gives one weak solution $u\in H^1_0(M)$, and it is unique there. In a chart its equation is $\partial_i(A^{ij}\partial_j u)=mf$, where $m=\sqrt{\det h}$ and $A^{ij}=mh^{ij}$. The smooth matrix $A$ is uniformly positive on every fixed compact patch. To match the positive-principal-part convention for $-\partial_i(A^{ij}\partial_j)$ in the weak regularity supplier, take forcing $-mf$. On overlapping aligned boundary charts the weak-equation invariance input applies to this solution with locally $L^2$ forcing and smooth uniformly elliptic coefficients. After a cutoff, its zero-Dirichlet assertion applies by the defining compactly supported smooth approximations to $u$. These solution-specific assertions are used only here; the arbitrary-function construction used step 1.1. [F2, F4, step 1.1, step 3.1, step 4.1]

6.1 In interior patches apply the declared nested-domain interior regularity lemma with $k=2$; $mf\in H^2$ and all coefficient bounds hold. At a boundary, localize with nested smooth cutoffs on smooth auxiliary domains of step 2.1. The localized function has zero Dirichlet data on the flat portion by the defining smooth approximations to $u$, and vanishes near every artificial boundary. The cutoff commutator contains only smooth multiples of $u$ and $Du$. Initially it is $L^2$, so the boundary theorem with $k=0$ gives local $H^2$. On a smaller patch the new commutator is now $H^1$ and $mf\in H^1$; use $k=1$ for $H^3$. On one further smaller patch it is $H^2$ and $mf\in H^2$; use $k=2$ for $H^4$. The arbitrary-function pullback bounds of step 1.1 and the multiplier bounds of [F4] justify each localization. Thus no undeclared interior counterpart or premature differentiation is needed. Smooth auxiliary domains satisfy the Sobolev extension hypothesis, so $H^4\hookrightarrow C^{2,\gamma}$ for any fixed $0<\gamma<1/2$. The weak equation is therefore classical and its zero trace is its continuous boundary value. [F1, F3, F4, step 1.1, step 2.1, step 5.1]

7.1 Write the classical coordinate equation as $Lu=h^{ij}u_{ij}+b^j u_j=f$, with smooth $b^j=m^{-1}\partial_i(mh^{ij})$ and zero reaction coefficient. The interior second-order Schauder interface gives $C^{2,\alpha}$ on smaller interior patches. On a boundary auxiliary domain apply the global boundary interface to $\eta u$: its forcing is $\eta f+[L,\eta]u$, and its entire boundary value is zero. Here $u\in C^{2,\gamma}$ already, so $[L,\eta]u$ has bounded first derivatives on the fixed compact patch and is $C^{0,\alpha}$ for every $0<\alpha<1$. Hence this application gives $C^{2,\alpha}$ up to the boundary as well. Now the imported higher-order regularity theorem applies with $k=2$ to each classical chart solution: the coefficients are smooth, $f\in C^{2,\alpha}$, the physical boundary is smooth and the data there are zero. Its local-boundary-portion version ignores artificial chart edges. It gives $u\in C^{4,\alpha}$ on smaller patches, hence on $M$ by a finite cover. This use is of the imported regularity theorem, not an assertion that second-order estimates alone license differentiating a merely $H^4$ solution. [F1, F5, step 6.1]

8.1 It remains to obtain the stated estimate with only the larger-chart data and supremum. Fix enough nested subpatches between the specified smaller and larger patches. Let $E_j(V)=\|u\|_{C^{j,\alpha}(V)}$ and $G_j(V)=\|f\|_{C^{j,\alpha}(V)}$. The interior second-order estimate or the imported local boundary estimate gives $E_2(V')\le C(G_0(V)+\|u\|_{0;V})$. All subsequent differentiations are legitimate by step 7.1. In the interior, $L(D_lu)=D_lf-(D_lh^{ij})u_{ij}-(D_lb^j)u_j$; the second-order estimate on nested patches gives $E_3(V')\le C(G_1(V)+E_2(V))$. Differentiate twice and apply it again to obtain $E_4(V')\le C(G_2(V)+E_3(V))$. At a flattened boundary, apply the local second-order estimate first to $D_tu$ and then to $D_sD_tu$, with $s,t$ tangential. Their boundary values are zero, and the differentiated forcing uses coefficient derivatives through order two and solution derivatives of strictly lower order. For order three these estimates control derivatives with at least one tangential factor; the equation solved for $u_{nn}$, divided by $h^{nn}\ge\lambda>0$, recovers $u_{nnn}$. For order four the two-tangential estimates control all derivatives with at most two normal factors. Apply $D_tD_n$ to the same identity to recover those with three normal factors, then $D_n^2$ to recover $u_{nnnn}$; all other highest-order terms have fewer normal factors, and coefficient-derivative terms use derivatives of $u$ of order at most three. This proves the same two recurrences at the boundary. Composing them on the nested patches gives $\|u\|_{4,\alpha;U'}\le C(\|f\|_{2,\alpha;U}+\|u\|_{0;U})$. Constants use only the ellipticity, coefficient $C^{2,\alpha}$ bounds and fixed chart separations; in particular this argument does not require a global topology restriction on $U$. [F1, F5, step 7.1]

9.1 Any classical solution with zero boundary values belongs to $H^1_0(M)$: cut it off in boundary charts at distance $\varepsilon$ from the flat face. Since it is $C^1$ and vanishes there, $u=O(x_n)$, so the cutoff error and its gradient tend to zero in $L^2$ on the shrinking boundary layer; finite partitions and interior smoothing give the defining compactly supported smooth approximations. The homogeneous weak energy identity may therefore be tested with the difference of two solutions, giving $\int_M|du|_h^2\,d\mu_h=0$. Poincaré gives $u=0$. Together with the constructed solution and step 8.1, this proves the Statement. [F1, F2, step 4.1, step 5.1, step 7.1, step 8.1] ∎


## Compact multiplication by a faster-decaying potential

[Open item](item-lem-author-86990d62062f-compact-potential) · level 1


### Statement

Work in ZFC. Let $\Sigma$ be the smooth three-dimensional exterior with compact smooth boundary $S$ and fixed weighted norms, let $0<\alpha<1$ and $\beta\in\mathbb R$, and put $X_\beta=\{u\in C^{4,\alpha}_\beta:u|_S=0\}$ and $Y_\beta=C^{2,\alpha}_{\beta-2}$. For every real $V\in C^{2,\alpha}_{-4}$, multiplication $u\mapsto Vu$ is a bounded compact linear map from $X_\beta$ to $Y_\beta$.

The same assertion holds with finitely many compact extra components, with the following precise conventions. Let $M_1,\ldots,M_m$ be compact smooth three-manifolds, each with possibly empty smooth boundary, where $m\ge0$. On each $M_j$ fix finitely many coordinate balls or boundary half-balls whose closures lie in larger charts and whose relative interiors cover $M_j$. Define $C^{k,\alpha}(M_j)$ by $C^k$ regularity up to the boundary and finite ordinary $C^{k,\alpha}$ norm on these closed patches, and use the sum of their coordinate derivative suprema through order $k$ and order-$k$ Hölder seminorms as its norm. Put $X_j=\{u_j\in C^{4,\alpha}(M_j):u_j|_{\partial M_j}=0\}$, with no boundary restriction when $\partial M_j=\varnothing$, and $Y_j=C^{2,\alpha}(M_j)$. Given real $V_j\in C^{2,\alpha}(M_j)$, componentwise multiplication by $(V,V_1,\ldots,V_m)$ is compact from $X_\beta\oplus\bigoplus_{j=1}^m X_j$ to $Y_\beta\oplus\bigoplus_{j=1}^m Y_j$, with the sum norm on each finite direct sum.

### Facts & Assumptions

**Given:** the hypotheses and norm conventions in the Statement; work in ZFC.

**Goal:** prove both compactness assertions.

[F1] The exterior, weighted annular norms and Dirichlet spaces are those of the weighted exterior definition. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F2] For real normed spaces, a linear map is compact exactly when the image of every bounded set has compact closure in the target norm metric. [math:def-compact-linear-operator](https://alphabetamath.cc/item/def-compact-linear-operator)

[F3] On a compact metric space, an equicontinuous pointwise bounded family of real continuous functions has compact closure in the supremum metric, assuming Countable Choice and Dependent Choice. [math:thm-arzela-ascoli-for-real-ck](https://alphabetamath.cc/item/thm-arzela-ascoli-for-real-ck)

[F4] On every bounded nonempty Euclidean open set, the finite-norm boundary-extension class $C^{2,\alpha}(\overline\Omega;\mathbb R)$ is Banach under Countable Choice. This includes balls, half-balls and annuli; no smoothness of the boundary is needed for this closure-class assertion. [math:thm-holder-spaces-on-bounded-domains-are-banach-spaces](https://alphabetamath.cc/item/thm-holder-spaces-on-bounded-domains-are-banach-spaces)

[F5] Ordinary Hölder norms, scaled derivative norms and boundary-extension classes use the declared Euclidean conventions. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F6] ZFC includes the Axiom of Choice, hence supplies the Countable Choice and Dependent Choice used in local completeness, subsequence extraction and metric compactness. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F7] For metric spaces, sequential compactness and compactness are equivalent under Countable Choice and Dependent Choice. [math:thm-metric-compactness-equivalences](https://alphabetamath.cc/item/thm-metric-compactness-equivalences)

[F8] For components with empty boundary use the smooth-manifold convention; for those with nonempty boundary use smooth boundary atlases with transitions smooth in the local-extension sense. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

### Proof

**Given:** the hypotheses and norm conventions in the Statement; work in ZFC.

**Goal:** prove both compactness assertions.

[F1] The exterior, weighted annular norms and Dirichlet spaces are those of the weighted exterior definition. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F2] For real normed spaces, a linear map is compact exactly when the image of every bounded set has compact closure in the target norm metric. [math:def-compact-linear-operator](https://alphabetamath.cc/item/def-compact-linear-operator)

[F3] On a compact metric space, an equicontinuous pointwise bounded family of real continuous functions has compact closure in the supremum metric, assuming Countable Choice and Dependent Choice. [math:thm-arzela-ascoli-for-real-ck](https://alphabetamath.cc/item/thm-arzela-ascoli-for-real-ck)

[F4] On every bounded nonempty Euclidean open set, the finite-norm boundary-extension class $C^{2,\alpha}(\overline\Omega;\mathbb R)$ is Banach under Countable Choice. This includes balls, half-balls and annuli; no smoothness of the boundary is needed for this closure-class assertion. [math:thm-holder-spaces-on-bounded-domains-are-banach-spaces](https://alphabetamath.cc/item/thm-holder-spaces-on-bounded-domains-are-banach-spaces)

[F5] Ordinary Hölder norms, scaled derivative norms and boundary-extension classes use the declared Euclidean conventions. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F6] ZFC includes the Axiom of Choice, hence supplies the Countable Choice and Dependent Choice used in local completeness, subsequence extraction and metric compactness. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F7] For metric spaces, sequential compactness and compactness are equivalent under Countable Choice and Dependent Choice. [math:thm-metric-compactness-equivalences](https://alphabetamath.cc/item/thm-metric-compactness-equivalences)

**Proof technique:** direct.

1.1 Write $\|\cdot\|^*_{k,\alpha;A_R}$ for the parenthesized scaled annular quantity in the weighted norm. Leibniz' rule and $[ab]_\alpha\le\|a\|_\infty[b]_\alpha+\|b\|_\infty[a]_\alpha$ give the ordinary $C^{2,\alpha}$ product bound. Lower-derivative Hölder seminorms are controlled by suprema of the next derivatives on balls and half-balls; a finite cover and the bound for pairs separated by a fixed positive distance give the same estimates on the unit annulus. Rescaling $x=Rz$ therefore gives $\|Vu\|^*_{2,\alpha;A_R}\le C\|V\|^*_{2,\alpha;A_R}\|u\|^*_{4,\alpha;A_R}$ and hence $R^{-(\beta-2)}\|Vu\|^*_{2,\alpha;A_R}\le CR^{-2}\|V\|_{C^{2,\alpha}_{-4}}\|u\|_{C^{4,\alpha}_\beta}$ for all $R\ge r_0$, with $C$ independent of $R$ and $u$. The finite compact-core norms satisfy the same unweighted product bound. On each $M_j$ the fixed chart norms likewise give $\|V_ju_j\|_{C^{2,\alpha}(M_j)}\le C_j\|V_j\|_{C^{2,\alpha}(M_j)}\|u_j\|_{C^{4,\alpha}(M_j)}$. These bounds prove that the componentwise linear map is bounded and well-defined. [F1, F5, F8, given, algebra]

2.1 Take any sequence bounded in the stated domain. The weighted bounds control all coordinate derivatives through order four on compact chart patches: use the finite core cover, finitely many annuli on any bounded end region, and bounded smooth chart-transition derivatives on compact overlaps. On compact extra components this follows directly from their fixed norms. For each patch use smaller closed balls or half-balls inside larger charts. Bounds through order four make the derivatives through order three equicontinuous and bounded, so Ascoli and a diagonal extraction give a subsequence for which these derivatives converge uniformly on a countable exhaustion. Include the bounded end-coordinate annuli $\{r_0<r<T\}$ for an increasing sequence of $T\to\infty$ in this extraction: finitely many overlapping $A_R$ control each such annulus, and derivative bounds give continuous extensions to its closure. This also controls pairs approaching its artificial inner sphere $r=r_0$. For a difference $w$ of two terms, the near-pair mean-value estimate and the far-pair supremum estimate on a convex patch give $[D^2w]_\alpha\le C\|D^2w\|_\infty^{1-\alpha}\|D^3w\|_\infty^\alpha$; a finite patch cover handles each annulus. Thus the subsequence is Cauchy in the ordinary $C^{2,\alpha}$ norm on every such patch and bounded end annulus. Local completeness supplies genuine $C^{2,\alpha}$ limits. Their function values agree on overlaps by uniform convergence, so they glue on $\Sigma$ and each $M_j$. Multiplication by the fixed potentials is continuous in these local norms by step 1.1, giving glued local limits $v$ of $Vu_n$ and $v_j$ of $V_ju_{j,n}$. [F1, F3, F4, F5, F6, F8, step 1.1]

3.1 Let $M$ bound the exterior input norms along this subsequence and set $B=C\|V\|_{C^{2,\alpha}_{-4}}M$. For every fixed $R\ge r_0$, pass to the limit in each derivative-value bound and each two-point Hölder bound from step 1.1. Taking the same suprema, maxima and finite sums gives $R^{-(\beta-2)}\|v\|^*_{2,\alpha;A_R}\le BR^{-2}$. The compact-core norm of $v$ is finite by its local $C^{2,\alpha}$ regularity. Consequently $v\in Y_\beta$, and the same finite-chart argument gives $v_j\in Y_j$. This constructs limits inside the specified targets without assuming completeness of a weighted space. [F1, F5, step 1.1, step 2.1]

4.1 For $R\ge T$, the two bounds for $Vu_n$ and $v$ give $R^{-(\beta-2)}\|Vu_n-v\|^*_{2,\alpha;A_R}\le2BT^{-2}$. For $r_0\le R<T$, all the annuli lie in the bounded end-coordinate region $\{r_0<r<2T\}$, and the powers of $R$ in their scaled norms are uniformly bounded because $R\in[r_0,T]$. Step 2.1 therefore makes the supremum of these remaining annular terms tend to zero. The compact-core norm tends to zero as well: a finite smaller-chart cover handles near pairs in each fixed core subset, and uniform convergence handles pairs a fixed distance apart. Choose $T$ first to make $2BT^{-2}$ small, and then choose $n$ to make the bounded-region terms small. This proves $Vu_n\to v$ in the full $Y_\beta$ norm. On the finitely many $M_j$ the local convergence from step 2.1 gives convergence in each full $Y_j$ norm, hence convergence in the finite direct-sum target norm. [F1, F5, step 1.1, step 2.1, step 3.1]

5.1 Every sequence in the image of a bounded domain set now has a subsequence converging in the target. The closure of that image is sequentially compact: for a sequence $z_n$ in the closure choose image points $y_n$ with target distance less than $1/n$ from $z_n$; a convergent subsequence of $y_n$ gives a subsequence of $z_n$ with the same limit, which lies in the closure. The metric compactness equivalence makes this closure compact. This is the required compactness, both for the exterior alone and for the finite direct sum. [F2, F6, F7, step 4.1] ∎


## Zero null optics supplies the missing null Ricci condition

[Open item](item-lem-author-6413ea293c6d-zero-optics-curvature) · level 1


### Statement

Let a smooth affinely parametrized null hypersurface congruence, before its first focal instant, satisfy the screen hypotheses of [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data) and [physics:prop-gr-fx-null-raychaudhuri](https://alphabetamath.cc/physics/item/prop-gr-fx-null-raychaudhuri). If its null second fundamental form vanishes identically on an open congruence neighborhood of a section, then $\operatorname{Ric}(\ell,\ell)=0$ there. At that section the same conclusion holds for every smooth nonzero rescaling $L=f\ell$. No conclusion from vanishing at a single isolated section alone is asserted.

### Facts & Assumptions

[F1] The screen definitions give the regular section metric, the screen Jacobi map $A$, the optical endomorphism $B=A' A^{-1}$, its expansion $\theta=\operatorname{tr}B$ and shear $\sigma=B-\frac12\theta\,\mathrm{id}$, and identify the initial optical data with the null second fundamental form of the initial section. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F2] The null Raychaudhuri supplier gives $\theta'=-\theta^2/2-|\sigma|^2-\operatorname{Ric}(\ell,\ell)$ under the stated smooth affine null hypersurface congruence hypotheses. Only this identity is used; neither a Ricci inequality nor a negative initial expansion is assumed. [physics:prop-gr-fx-null-raychaudhuri](https://alphabetamath.cc/physics/item/prop-gr-fx-null-raychaudhuri)

[F3] The Ricci tensor is a smooth covariant two-tensor, defined by the metric contraction of curvature, and is therefore pointwise bilinear. [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)

### Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Establish its identities with the indicated normalizations.

1.1 Fix any regular parameter $\lambda_0$ and work locally on its spacelike section $S_{\lambda_0}$, restricting to an embedded section patch if necessary. Rebase the same congruence at that section by using $s=\lambda-\lambda_0$ and relabeling each generator by its point on $S_{\lambda_0}$. Its tangent is still $\ell$, its parameter is still affine, and its section directions are still orthogonal to $\ell$. Under the identification of $T S_{\lambda_0}$ with the screen at $\lambda_0$, its screen Jacobi map is $\widetilde A_s=A_{\lambda_0+s}A_{\lambda_0}^{-1}$. Since the right factor is fixed in $s$, $\widetilde B_s=\widetilde A_s'\widetilde A_s^{-1}=B_{\lambda_0+s}$. Apply the initial-section identification of [F1] to this rebased congruence: at $s=0$, its optical expansion and shear correspond to the trace and trace-free part of $\chi_\ell$ on $S_{\lambda_0}$. These vanish by the assumed zero second fundamental form. As the regular point and section were arbitrary, $\theta=0$ and $\sigma=0$ throughout the open congruence neighborhood, with all constructions taken on the chosen parameter-domain branch. [given, F1, construct, algebra]

2.1 The smooth function $\theta$ vanishes on this open neighborhood, so its affine derivative also vanishes there. Substitution of $\theta=0$, $\sigma=0$ and $\theta'=0$ into the identity in [F2] gives $\operatorname{Ric}(\ell,\ell)=0$ throughout that neighborhood. The open-neighborhood hypothesis is what justifies taking the derivative of the identically zero expansion; vanishing at one isolated section would not suffice. [step 1.1, F2, algebra]

3.1 At the specified section, pointwise bilinearity of the covariant two-tensor in [F3] gives $\operatorname{Ric}(f\ell,f\ell)=f^2\operatorname{Ric}(\ell,\ell)=0$ for every smooth nonzero rescaling $L=f\ell$. This pointwise rescaling needs no affine extension of $L$. [step 2.1, F3, algebra] ∎


## Smooth approximation of compactly supported interior heights

[Open item](item-lem-author-423fe0348a31-finite-atlas-smoothing) · level 1


### Statement

Work in ZFC. Let $(R,k)$ be a compact smooth Riemannian region (a manifold with boundary) of dimension $n\ge0$, and let $v:R\to\mathbb R$ be Lipschitz with support compactly contained in its interior. There exist $v_j\in C_c^\infty(R^\circ)$, all supported in one fixed compact interior set, such that $\|v_j-v\|_\infty+\int_R(|v_j-v|+|dv_j-dv|_k)\,dV_k\to0$. Here $dv$ is the almost-everywhere weak differential, $|\cdot|_k$ is the dual metric norm and $dV_k$ is the Riemannian volume density; for $n=0$, differentials vanish and each point has volume one.

Lipschitz means that there is a single finite $L\ge0$ such that $|v(p)-v(q)|\le Ld_k(p,q)$ for every pair in the same connected component of $R$, with the usual distance on $\mathbb R$. Here $d_k$ is the infimum of the lengths $L_k(\gamma)=\int|\dot\gamma|_k$ of piecewise $C^1$ curves in $R$ joining the two points; distinct components have extended distance $+\infty$ and impose no cross-component inequality.

### Facts & Assumptions

[F1] Finite smooth interior cutoffs form a partition equal to one near the compact support. [lem-author-423fe0348a31-finite-relative-cutoffs](item-lem-author-423fe0348a31-finite-relative-cutoffs)

[F2] Chart and metric first-Sobolev norms are uniformly comparable on each chosen compact chart; locally Lipschitz functions have coordinate-independent weak differentials, with the smooth-cutoff product rule. The supplier also fixes the dimension-zero conventions. [lem-author-423fe0348a31-chart-sobolev-comparison](item-lem-author-423fe0348a31-chart-sobolev-comparison)

[F3] For every dimension $n\ge1$, a compactly supported Lipschitz coordinate function admits mollification converging uniformly and in $W^{1,1}$, with fixed compact support inside its coordinate domain; an admissible kernel exists. [lem-author-423fe0348a31-compact-chart-mollification](item-lem-author-423fe0348a31-compact-chart-mollification)

[F4] The metric is the smooth positive-definite tensor $k$ on $R$. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[F5] Lipschitz continuity is the finite-constant metric inequality, applied on each connected component with one common bound. Intrinsic Riemannian distance is the infimum of piecewise $C^1$ curve lengths; the extended distance is $+\infty$ between distinct components. Length is the integral of metric speed. [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction) [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold) [math:def-extended-riemannian-distance-on-a-disconnected-manifold](https://alphabetamath.cc/item/def-extended-riemannian-distance-on-a-disconnected-manifold) [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)

[F6] On a compact set contained in a coordinate chart, the Riemannian quadratic form has uniform positive lower and finite upper bounds relative to the Euclidean quadratic form. In particular $k_p(\xi,\xi)\le C|\xi|^2$ there for some finite $C>0$. [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

[F7] Write $R^\circ=\operatorname{Int}R$ for the manifold interior: in positive dimension its points have positive last boundary-chart coordinate; in dimension zero every point is interior and the boundary is empty. [math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)

[A1] Work in ZFC, carrying the mollification supplier's ZFC hypothesis and the chart-comparison supplier's Countable Choice hypothesis. Choice is inherited through these analytic suppliers, not through the finite partition or the explicit sequence of radii. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### Proof

**Given:**The hypotheses in the Statement.

**Goal:** Establish the stated construction or identity.

1.1 If $v=0$, take $v_j=0$ with empty support. If $n=0$, every point is interior by [F7], and every chart is a singleton, so $v$ is smooth; take $v_j=v$, whose compact interior support is fixed. The zero-dimensional conventions in [F2] make both errors zero. Henceforth take $n\ge1$ and nonempty support. Cover the support by finitely many interior coordinate balls $x_a:U_a\to B_a$, each with closure contained in a larger interior chart, and choose the cutoffs of [F1]. The identity $v=\sum_a\chi_av$ holds globally, since $v$ vanishes outside its support. By [F6], on $\overline{U_a}$ the coordinate quadratic form satisfies $k_p(\xi,\xi)\le C_a^{\mathrm{met}}|\xi|^2$ for a finite $C_a^{\mathrm{met}}>0$. For $p,q\in U_a$, the inverse-coordinate straight segment stays in $U_a$ and has length at most $\sqrt{C_a^{\mathrm{met}}}|x_a(p)-x_a(q)|$ by [F5]. Thus $d_k(p,q)$ is at most this bound, and the hypothesis gives $|v(p)-v(q)|\le L\sqrt{C_a^{\mathrm{met}}}|x_a(p)-x_a(q)|$. In particular $v$ is locally Lipschitz in smooth coordinates, as required by [F2]. Its coordinate expression is also bounded on the bounded ball $B_a$. Each coordinate cutoff is smooth with compact support in $B_a$, so its derivative is bounded there and the coordinate straight-segment estimate makes it Lipschitz. The product inequality therefore shows that $f_a=(\chi_av)\circ x_a^{-1}$ is Lipschitz and compactly supported in $B_a$. Apply [F3] in dimension $n$, using [A1], and fix for each chart a radius $r_a>0$ such that every mollified support for radius at most $r_a$ stays in one fixed compact subset $K_a$ of that chart. Use the explicit radii $r_a/(j+1)$. [given, F1, F2, F3, F5, F6, F7, A1, construct]

2.1 Pull the finitely many smooth coordinate approximants back to their charts, extend by zero, and sum them to obtain $v_j$. The zero extensions are smooth because their supports stay away from the chart sides, and all sums are supported in the fixed compact interior union $\bigcup_a K_a$. The supremum error is at most the sum of the finitely many coordinate supremum errors. Apply [F2] to each coordinate difference $f_{a,j}-f_a$, with the same fixed compact support set $K_a$ for all $j$; linearity and the cutoff product rule identify the resulting summed weak differential with $dv_j-dv$. The integral error is therefore at most $\sum_a C_a\|f_{a,j}-f_a\|_{W^{1,1}}$, with constants $C_a$ independent of $j$, and tends to zero by [F3]. Both stated convergences follow. [F2, F3, A1, step 1.1, algebra] ∎


## Positive right and adjoint eigenfunctions have the same eigenvalue

[Open item](item-lem-author-1a44964f66ee-positive-adjoint-pairing) · level 1


### Statement

For the closed-manifold operator $L$ of the formal-adjoint lemma, assume $S$ is nonempty and suppose smooth functions $\phi>0$ and $\chi>0$ satisfy $L\phi=\lambda\phi$ and $L^\dagger\chi=\lambda^\dagger\chi$, with real constants $\lambda,\lambda^\dagger$. Then $\lambda=\lambda^\dagger$. Positivity and compactness also give $\min_S\phi>0$ and $\min_S\chi>0$, so division by either is smooth and bounded.

### Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The integration-by-parts identity holds for the smooth real functions in question. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)

[F2] A continuous real-valued function on a nonempty compact space attains a maximum and a minimum. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

[F3] Smooth real-valued maps on smooth manifolds are continuous. [math:prop-smooth-maps-are-continuous](https://alphabetamath.cc/item/prop-smooth-maps-are-continuous)

[F4] The composite of two smooth maps between smooth manifolds is smooth. [math:prop-identity-maps-and-composites-of-smooth-maps-are-smooth](https://alphabetamath.cc/item/prop-identity-maps-and-composites-of-smooth-maps-are-smooth)

[F5] The smooth Riemannian metric $h$ and its smooth Levi–Civita connection are those of the formal-adjoint setting. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)

[F6] The dual connection on $T^*S$ and finite product connections on $(T^*S)^{\otimes j}$ are well-defined smooth connections, obey the tensor Leibniz rule, and are function-linear in their vector-field argument. [math:def-dual-connection](https://alphabetamath.cc/item/def-dual-connection) [math:def-product-connection-on-tensor-and-hom-bundles](https://alphabetamath.cc/item/def-product-connection-on-tensor-and-hom-bundles)

[F7] Assuming countable choice, integration of compactly supported smooth densities is linear and strictly positive on a nonzero nonnegative density. [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation)

[F8] The existing ZFC assumption includes the Axiom of Choice; applying it to countable families supplies the countable choice required by F7. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The integration-by-parts identity holds for the smooth real functions in question. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)

[F2] A continuous real-valued function on a nonempty compact space attains a maximum and a minimum. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

[F3] Smooth real-valued maps on smooth manifolds are continuous. [math:prop-smooth-maps-are-continuous](https://alphabetamath.cc/item/prop-smooth-maps-are-continuous)

[F4] The composite of two smooth maps between smooth manifolds is smooth. [math:prop-identity-maps-and-composites-of-smooth-maps-are-smooth](https://alphabetamath.cc/item/prop-identity-maps-and-composites-of-smooth-maps-are-smooth)

[F5] The smooth Riemannian metric $h$ and its smooth Levi–Civita connection are those of the formal-adjoint setting. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)

[F6] The dual connection on $T^*S$ and finite product connections on $(T^*S)^{\otimes j}$ are well-defined smooth connections, obey the tensor Leibniz rule, and are function-linear in their vector-field argument. [math:def-dual-connection](https://alphabetamath.cc/item/def-dual-connection) [math:def-product-connection-on-tensor-and-hom-bundles](https://alphabetamath.cc/item/def-product-connection-on-tensor-and-hom-bundles)

[F7] Assuming countable choice, integration of compactly supported smooth densities is linear and strictly positive on a nonzero nonnegative density. [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation)

[F8] The existing ZFC assumption includes the Axiom of Choice; applying it to countable families supplies the countable choice required by F7. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

**Proof technique:** direct.

1.1 Use the adjoint identity with $f=\chi$ and $g=\phi$. Substituting the eigenvalue equations and using linearity in F7 gives $(\lambda-\lambda^\dagger)\int_S\chi\phi\,d\mu_h=0$. Since $S$ is nonempty, $\chi\phi\,d\mu_h$ is a nonzero positive smooth density. Its support is all of compact $S$, so F7 applies, with countable choice supplied by F8, and gives $\int_S\chi\phi\,d\mu_h>0$. Hence the eigenvalues agree. [F1, F7, F8]

2.1 By F3 the smooth real functions $\phi$ and $\chi$ are continuous. Apply F2 to them on the nonempty compact manifold $S$. Each attains its minimum at a point where its value is positive, giving $\min_S\phi>0$ and $\min_S\chi>0$. The map $r:(0,\infty)\to\mathbb R$, $r(s)=1/s$, is smooth: its derivative of order $j\ge0$ is $(-1)^j j!s^{-j-1}$. Since $\phi$ and $\chi$ take values in this open interval, F4 makes $1/\phi=r\circ\phi$ and $1/\chi=r\circ\chi$ smooth. They satisfy $1/\phi\le(\min_S\phi)^{-1}$ and $1/\chi\le(\min_S\chi)^{-1}$. For $u\in\{1/\phi,1/\chi\}$ define $\nabla^0u=u$ and $\nabla^{j+1}u=\nabla(\nabla^ju)$ using F5 and F6. Function-linearity in the differentiating vector field makes $\nabla^{j+1}u$ a covariant $(j+1)$-tensor; the smooth dual and product connections show inductively that all these tensors have smooth local components. For every fixed derivative order, the squared Riemannian norm of the corresponding covariant derivative of either smooth reciprocal is a smooth real function: in coordinates it is a finite contraction of smooth tensor components with the smooth inverse metric. It is continuous by F3 and bounded by F2, so its nonnegative square root, the Riemannian norm itself, is continuous and bounded as well. This proves all assertions. [F2, F3, F4, F5, F6, step 1.1] ∎


## Imported positive eigenpairs for a smooth closed elliptic operator

[Open item](item-thm-author-1a44964f66ee-closed-principal-pair-external) · level 1


### Statement

Let $L=-\Delta_h+2t\cdot\nabla+c$ have the closed connected smooth Riemannian and real smooth coefficient hypotheses of the formal-adjoint lemma. There exist a real eigenvalue $\lambda$, a smooth real $\phi>0$ with $L\phi=\lambda\phi$, and a smooth real $\chi>0$ with $L^\dagger\chi=\lambda\chi$. This is an established external existence input, not a locally reconstructed resolvent or Krein–Rutman proof.

### Facts & Assumptions

[F1] The formal-adjoint lemma fixes the exact operator, metric density and adjoint conventions. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)

[A1] Work in ZFC, including Choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### External input

Andersson–Mars–Simon §4 Lemma 4.1 applies to the smooth real elliptic operator on the connected compact boundaryless manifold. Apply part (i) also to its formal adjoint, whose coefficients and ellipticity are supplied by the formal-adjoint lemma; part (ii) identifies the principal eigenvalues. We import the resulting positive right and adjoint eigenpairs. No local compact-resolvent construction or proof of Krein–Rutman is claimed.


## Normal deformation families and an outgoing null gauge

[Open item](item-lem-author-97780c2fed82-normal-deformation-families) · level 1


### Statement

Assume Countable Choice. For a surface and null pair as in the general surface interface and a smooth normal field $X$ along it, there is an $\epsilon>0$ and a smooth family of spacelike embeddings $\Phi_t:S\to M$, $|t|<\epsilon$, with $\Phi_0=i$ and $\partial_t\Phi_t|_0=X$. One choice is $\Phi_t(p)=\exp^\nabla_{i(p)}(tX_p)$, where $\exp^\nabla$ is the exponential map of the supplied metric-compatible affine connection $\nabla$; torsion freedom is not required. Smooth outgoing null normal pairs on these surfaces can be chosen with $g(\ell_t,k_t)=-1$ and $(\ell_0,k_0)=(\ell,k)$. Neither a spacelike slice nor a null hypersurface containing the variation is assumed.

### Statement references

[def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data)

[math:thm-the-exponential-domain-is-open-and-the-exponential-map-is-smooth](https://alphabetamath.cc/item/thm-the-exponential-domain-is-open-and-the-exponential-map-is-smooth)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

[math:prop-exponential-map-scales-geodesic-time](https://alphabetamath.cc/item/prop-exponential-map-scales-geodesic-time)

[math:def-domain-and-exponential-map-of-a-connection](https://alphabetamath.cc/item/def-domain-and-exponential-map-of-a-connection)

[math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

### Facts & Assumptions

[F1] The initial surface is compact, spacelike, oriented and has the supplied smooth null pair. [def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data)

[F2] For the supplied affine connection $\nabla$, write $\mathcal E^\nabla$ for its exponential domain and $\exp^\nabla(v)=\gamma_{p,v}(1)$ for $v\in T_pM$ in that domain. Under Countable Choice, $\mathcal E^\nabla$ is open and contains the zero section, and $\exp^\nabla$ is smooth. No torsion restriction is needed. [math:def-domain-and-exponential-map-of-a-connection](https://alphabetamath.cc/item/def-domain-and-exponential-map-of-a-connection) [math:thm-the-exponential-domain-is-open-and-the-exponential-map-is-smooth](https://alphabetamath.cc/item/thm-the-exponential-domain-is-open-and-the-exponential-map-is-smooth) [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F3] An invertible differential admits a smooth local inverse. [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

[F4] Under Countable Choice, for any affine connection, $tv$ lies in the exponential domain exactly when $t$ lies in the maximal interval of the geodesic with initial point $p$ and velocity $v$; on this domain $\exp_p(tv)=\gamma_{p,v}(t)$. [math:prop-exponential-map-scales-geodesic-time](https://alphabetamath.cc/item/prop-exponential-map-scales-geodesic-time) [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F5] A smooth embedding is an injective smooth immersion that is a homeomorphism onto its image with the subspace topology. [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

[F6] A continuous real-valued function on a nonempty compact space attains its minimum and maximum. A continuous bijection from a compact space to a Hausdorff space is a homeomorphism. Neither assertion requires a choice principle. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

### Proof

**Given:**The objects and hypotheses in the Statement.

**Goal:** Establish the assertions and well-definedness stated there.

1.1 Openness of the exponential domain and compactness of $S$ give one interval on which $tX_p$ lies in that domain for all $p$. The smooth exponential map gives a smooth family. By [F4], $\Phi_t(p)=\gamma_{i(p),X_p}(t)$ on that interval, so $\Phi_0(p)=i(p)$ and $\left.\partial_t\Phi_t(p)\right|_{t=0}=X_p$ by the initial data of this geodesic. Choose finitely many coordinate neighborhoods $V_j$ covering $S$ whose closures $K_j=\overline{V_j}$ are compact and contained in larger coordinate neighborhoods $W_j$. To obtain these, take around each point a coordinate ball with closed ball contained in the chart image, pull back a smaller concentric ball, and take a finite subcover by compactness. In the coordinates on $W_j$, put $q_{t,AB}=g(\partial_A\Phi_t,\partial_B\Phi_t)$. On each $K_j$, both $q_{0,11}$ and $\det(q_{0,AB})$ are positive continuous functions and hence have positive minima by [F6]. Continuity on these compact sets, and finiteness of the cover, give a common smaller parameter interval on which $q_{t,11}>0$ and $\det(q_{t,AB})>0$ throughout every $K_j$. These two principal-minor inequalities make the symmetric two-by-two Gram matrix positive definite, so the differential is injective and each deformed surface is spacelike. [F1, F2, F4, F6]

2.1 To check global injectivity, suppose there are $t_j\to0$ and distinct $p_j,q_j$ with $\Phi_{t_j}(p_j)=\Phi_{t_j}(q_j)$. Compactness gives convergent subsequences, and injectivity of $i$ makes their limits a common point $p$. Choose a coordinate projection of an ambient chart to two tangent coordinates whose differential on $di(T_pS)$ is invertible. The map $(t,y)\mapsto(t,\pi\Phi_t(y))$ has invertible differential at $(0,p)$; its local inverse contradicts equality for these pairs once they lie in that neighborhood. Thus $\Phi_t$ is injective for small $t$. By [F6], the continuous bijection $S\to\Phi_t(S)$ is a homeomorphism, since $S$ is compact and $\Phi_t(S)$ is a Hausdorff subspace of $M$; together with the rank condition, this makes $\Phi_t$ an embedding by [F5]. [F1, F3, F5, F6, step 1.1]

3.1 On each deformed surface, subtract from the ambient time-orientation vector $N$ its tangential projection: $U=N-q_t^{AB}g(N,E_A)E_B$, where $E_A=\partial_A\Phi_t$. The tangent term is spacelike and orthogonal to $U$, so $g(U,U)=g(N,N)-|N^\top|^2<0$, and $g(U,N)=g(U,U)<0$. Therefore $n_t=U/\sqrt{-g(U,U)}$ is a smooth future unit normal. The normal plane is Lorentzian. Its orientation from the orientations of $M$ and $S$, together with $n_t$, selects a smooth unit spacelike normal $\nu_t$; its sign is chosen to match the outgoing null ray at $t=0$. This can be computed by ordinary two-vector orthogonalization in each normal-plane chart; uniqueness of the oriented unit vector glues these formulas. Put $\widehat\ell_t=n_t+\nu_t$, $\widehat k_t=(n_t-\nu_t)/2$. [F1, step 1.1, step 2.1]

4.1 The initial outgoing ray agrees with that of $\ell$, so $\ell=a\widehat\ell_0$ for a positive smooth function $a$ on $S$. The normalization then gives $k=a^{-1}\widehat k_0$. Setting $\ell_t=a\widehat\ell_t$ and $k_t=a^{-1}\widehat k_t$, with $a$ constant in the variation parameter, supplies the required pair. All denominators are nonzero, and compactness permits the uniform shrinkings already used. Countable Choice is inherited from the exponential-map interface; no stronger choice is used in this construction. [F1, F2, step 3.1] ∎


## Uniform annular Schauder bootstrap for spacelike graph equations

[Open item](item-lem-annular-quasilinear-bootstrap-input) · level 2


### Statement

Work in ZFC. Let $n\ge2$ be a fixed integer, $A=\{y\in\mathbb R^n:1/2<|y|<4\}$ and $A'=\{y\in\mathbb R^n:1<|y|<2\}$, and let $u_R$ be a family of smooth scalar graph heights on $RA$, for $R\ge R_0\ge1$. Indices $i,j$ range from $1$ to $n$, and repeated indices are summed. Set $v_R(y)=u_R(Ry)$ and $w_R=v_R/R$. Fix $0<\alpha<1$. The norms below are ordinary fixed-domain Hölder norms.

The general realized-coefficient version is as follows: if $a_R^{ij}(y)(v_R)_{ij}+b_R^j(y)(v_R)_j+c_R(y)v_R=f_R(y)$, the symmetric matrices $a_R$ have common positive ellipticity bounds, $a_R,b_R,c_R$ have common $C^{2,\alpha}$ bounds on $A$, and $\|f_R\|_{C^{2,\alpha}(A)}\le K/R$, then
$$\sum_{j=0}^4R^j\sup_{RA'}|D_x^ju_R|\le C(\sup_{RA}|u_R|+R^{-1}).$$

For a stationary spacelike maximal graph, with flux $P_R$ taking values in $\mathbb R^n$, the following explicit operator hypotheses supply those realized coefficient bounds, rather than assuming them from smoothness: $\operatorname{div}_yP_R(y,Dw_R)=0$, with no dependence on height; $|Dw_R|\le p_0$, $\|w_R\|_\infty\le M_0$; on the whole slope ball $|p|\le p_0$, $P_{R,p}$ is symmetric with $\lambda I\le P_{R,p}\le\Lambda I$ and $P_R$ has common joint $C^{4,\alpha}$ bounds on slightly larger slope neighborhoods. Write $s_R(y,p)=\sum_i\partial_{y_i}P_R^i(y,p)$, with partial derivatives at fixed $p$, and assume $\|s_R(\cdot,0)\|_{C^{2,\alpha}(A)}\le K/R^2$. Then the same estimate follows. Uniformity over additional parameters means common constants on the specified parameter set; no claim of uniformity at a degenerate parameter endpoint is made. The stationary Lorentzian four-manifold application uses $n=3$; its metric flux and sufficient background hypotheses are explicit in the flux lemma. Every application must verify these hypotheses, not only pointwise decay of the evaluated principal coefficients.

### Facts & Assumptions

[F1] The fixed-annulus rescaling and finite-cover identities hold. [lem-author-db87cb8e0bab-annular-scaling](item-lem-author-db87cb8e0bab-annular-scaling)

[F2] The explicit stationary Lorentzian flux has symmetric elliptic gradient derivative under its stated metric and spacelike-cone hypotheses. [lem-author-db87cb8e0bab-stationary-flux-ellipticity](item-lem-author-db87cb8e0bab-stationary-flux-ellipticity)

[F3] For a smooth flux under the gradient lemma's ellipticity, slope and flux-position-derivative hypotheses, the differentiated flux equation gives an initial gradient Hölder estimate before any Schauder application. [lem-author-db87cb8e0bab-divergence-gradient-holder](item-lem-author-db87cb8e0bab-divergence-gradient-holder)

[F4] Under its inherited smooth-flux hypotheses, the preliminary bootstrap gives common realized coefficient bounds using only structural data and a height bound for the normalized graph. [lem-author-db87cb8e0bab-coefficient-regularity](item-lem-author-db87cb8e0bab-coefficient-regularity)

[F5] The linear fourth-order estimate is linear in the height and the forcing once realized coefficient bounds are known. [lem-author-db87cb8e0bab-linear-fourth-derivative-estimate](item-lem-author-db87cb8e0bab-linear-fourth-derivative-estimate)

[F6] Uniform asymptotic estimates require a common chart, radius and constants. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F7] The graph type, maximality convention and admissible spacelike image require explicit hypotheses. [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[F8] Use ordinary Euclidean Hölder norms on the fixed annuli. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F9] In dimension $n\ge2$ and under Countable Choice, the interior Schauder estimate takes a bounded classical $C^2$ solution of a uniformly elliptic equation with controlled $C^{0,\gamma}$ coefficients and forcing to an interior $C^{2,\gamma}$ bound. Here $0<\gamma<1$; lower-order coefficients can be zero. [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations)

[F10] Work in ZFC, carrying the analytic suppliers' choice assumptions. Full Choice supplies Countable Choice: for a sequence of nonempty sets, choose on its family of values and compose the choice function with that sequence. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F11] For totally differentiable maps between open Euclidean sets, $D(G\circ\Phi)=DG(\Phi)D\Phi$. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F12] Under Countable Choice, a continuous Banach-valued curve on $[a,b]$ whose interior derivative extends continuously to $[a,b]$ satisfies $\varphi(b)-\varphi(a)=\int_a^b\varphi'(t)\,dt$. Use the real scalar case $X=\mathbb R$ and $[a,b]=[0,1]$. [math:lem-fundamental-theorem-of-calculus-for-banach-valued-continuous-curves](https://alphabetamath.cc/item/lem-fundamental-theorem-of-calculus-for-banach-valued-continuous-curves)

[F13] Under Countable Choice, $H^1=W^{1,2}$ consists of square-integrable almost-everywhere classes with square-integrable first weak derivatives. For a bounded measurable uniformly elliptic real matrix $B$, the homogeneous local weak equation means $z\in H^1(U)$ and $\int_U(BDz)\cdot D\varphi=0$ for every $\varphi\in C_c^\infty(U)$. Use the real scalar convention with zero lower-order coefficients and datum. [math:def-hk-and-hk-zero-notation](https://alphabetamath.cc/item/def-hk-and-hk-zero-notation) [math:def-local-weak-solution-for-a-divergence-form-operator](https://alphabetamath.cc/item/def-local-weak-solution-for-a-divergence-form-operator)

[F14] A continuous real integrand on a compact rectangle with a continuous parameter derivative may be differentiated through its Riemann integral. Apply twice, componentwise, with other spatial coordinates fixed. A uniform difference bound $\eta$ between integrable functions on $[0,1]$ bounds the difference of their integrals by $\eta$. [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle) [math:lem-uniform-integral-error-bound](https://alphabetamath.cc/item/lem-uniform-integral-error-bound)

[F15] The real mean value theorem applies to continuous functions on a closed interval differentiable in its interior. Along line segments, a bound on a derivative therefore bounds increments by the length times that bound. [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

[F16] Under Countable Choice, for a bounded $C^1$ domain $U\subset\mathbb R^d$, $d\ge2$, and a vector field $V\in C^1(\overline U;\mathbb R^d)$, the divergence theorem gives $\int_U\operatorname{div}V=\int_{\partial U}V\cdot\nu$. In particular the integral is zero when $V$ vanishes near the boundary. [math:thm-divergence-theorem-for-bounded-c-one-euclidean-domains](https://alphabetamath.cc/item/thm-divergence-theorem-for-bounded-c-one-euclidean-domains)

[F20] Use the homogeneous De Giorgi–Nash estimate recorded in External input, only after verifying the lifted weak equation in dimension $n+1$.

### Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the asserted estimate with the stated uniform dependence.

1.1 In the general realized-coefficient case apply [F5] to $v_R$ on $A$ with target annulus $A'$. It yields $\|v_R\|_{C^{4,\alpha}(A')}\le C(\|v_R\|_\infty+K/R)$. Rescale derivatives using [F1]. Thus the full original annular estimate follows whenever the stated coefficient hypothesis means actual $C^{2,\alpha}$ bounds as functions of position. [given, F1, F5, F8, F9, F10]

1.2 If $P_R$ is smooth, [F3] and [F4] give the preliminary coefficient bounds under the stated structural hypotheses. For a general jointly $C^{4,\alpha}$ flux, their smooth-flux interfaces are not invoked. Instead the following local argument extends the gradient and coefficient bootstrap to that finite regularity while keeping $w_R$ smooth, as already assumed. Choose a fixed finite sequence of nested annuli strictly between $A'$ and $A$, with room for all the successive interior estimates below. Work on balls with compact closures in the larger annuli, then cover the smaller ones using [F1]. All radii, separations and finite covering constants are fixed independently of $R$. Suppress $R$ in the local calculation. [given, F1, F3, F4, F8, F10]

1.3 On a convex ball, subtracting products gives $[fg]_{0,\gamma}\le\|f\|_\infty[g]_{0,\gamma}+\|g\|_\infty[f]_{0,\gamma}$ for $0<\gamma<1$; iterate for finite products. The identity $\Delta(fg)=f\Delta g+g\Delta f+\Delta f\Delta g$, divided by the increment and passed to the limit, gives the product derivative rule. By [F11] and [F15] on line segments, an outer map with bounded first derivatives is Lipschitz on the ball times the slope ball. Hence $[G\circ\Psi]_{0,\gamma}\le\operatorname{Lip}(G)[\Psi]_{0,\gamma}$. If $G$ is merely $\gamma$-Hölder and $\Psi$ is Lipschitz, instead use $[G\circ\Psi]_{0,\gamma}\le[G]_{0,\gamma}\operatorname{Lip}(\Psi)^\gamma$. These inequalities give the product and composition bounds used below. [F8, F11, F15, algebra]

1.4 For each coordinate $k$, put $z=w_k$, $a(y)=P_p(y,Dw(y))$ and $F(y)=-P_{y_k}(y,Dw(y))$, with the partial derivative at fixed slope. Differentiating the given flux equation gives $\operatorname{div}(aDz)=\operatorname{div}F$. This differentiation uses only two joint derivatives of $P$ and the assumed smoothness of $w$. In particular, $a$ is symmetric with $\lambda I\le a\le\Lambda I$, $|z|\le p_0$, and $|F|$ is bounded by the common structural bound. No uniform bound on $D^2w$ has been used. [given, F11, algebra]

2.1 On the chosen ball let $M=\|z\|_\infty+\|F\|_\infty$. If $M=0$, the gradient component is zero and needs no estimate. Otherwise define $Z(y,t)=z(y)/M+t$, $H(y)=F(y)/M$, and on the ball times $(-1,1)$ set $B=\begin{pmatrix}a&-H\\-H^T&1+2/\lambda\end{pmatrix}$. Since $|H|\le1$, its quadratic form is at least $(\lambda/2)|\xi|^2+|\tau|^2$, using $2|\tau H\cdot\xi|\le(\lambda/2)|\xi|^2+(2/\lambda)\tau^2$; an upper bound depends only on $\lambda,\Lambda$. Independence of $t$ gives $\operatorname{div}_{y,t}(BDZ)=\operatorname{div}_y(aDz/M-H)=0$. The entries are $C^1$ locally, so this identity is classical. On every ball $U$ with compact closure in the cylinder, $Z$ and its first derivatives are bounded on $\overline U$ and are square-integrable because $U$ is bounded. To check the weak identities, let $\varphi\in C_c^\infty(U)$ and $1\le\ell\le n+1$. The ball is a bounded $C^1$ domain in dimension $n+1\ge2$. Both $Z\varphi e_\ell$ and $\varphi BDZ$ are $C^1$ on a neighborhood of $\overline U$ and vanish near $\partial U$, since the coefficients are $C^1$ there and $\varphi$ has compact support in $U$. With Countable Choice supplied by [F10], [F16] and the product rule give $0=\int_U\operatorname{div}(Z\varphi e_\ell)=\int_U(Z\partial_\ell\varphi+\varphi\partial_\ell Z)$. These identities identify the classical derivatives as weak derivatives, so $Z\in H^1(U)$ by [F13]. Applying [F16] to the second field gives $0=\int_U\operatorname{div}(\varphi BDZ)=\int_U(BDZ)\cdot D\varphi+\int_U\varphi\operatorname{div}(BDZ)=\int_U(BDZ)\cdot D\varphi$. Thus [F13] verifies exactly the weak-solution hypotheses of [F20]. [step 1.4, F10, F13, F16, F20, algebra]

3.1 Apply [F20] after translation and dilation of the $(n+1)$-dimensional interior balls to unit balls. On the fixed cylinder $|Z|\le2$, so its $L^2$ norm on each such ball is uniformly bounded. Restrict the resulting estimate to $t=0$, multiply by the uniformly bounded $M$, and cover a smaller $y$ ball by finitely many such patches. Performing this for all $k$ gives a uniform $C^{0,\beta}$ bound for $Dw$. Decrease the exponent if necessary to ensure $0<\beta\le\alpha$ and $\beta<1$; on fixed bounded sets this costs only a diameter factor. The exponent and constants depend only on the structural data and fixed separations. [step 2.1, F1, F8, F10, F20, given]

4.1 Put $S(y)=s(y,Dw(y))$. The chain rule gives $a^{ij}w_{ij}=-S$. From step 3.1, the joint derivative bounds on $P$ and step 1.3, $a$ and $S$ have common $C^{0,\beta}$ bounds on interior balls. The matrix has the inherited ellipticity bounds, $w$ is smooth and bounded by $M_0$, both lower-order coefficients are zero, and [F10] supplies Countable Choice. Applying [F9] with exponent $\beta$ gives a uniform $C^{2,\beta}$ bound for $w$ on smaller balls. [step 1.3, step 3.1, F8, F9, F10, F11, given]

5.1 The chain and product rules with step 4.1 now give uniform $C^{1,\beta}$ bounds for $a$ and $S$. Differentiating the equation once yields $a^{ij}(w_k)_{ij}=-D_kS-(D_ka^{ij})w_{ij}$. Its right-hand side has a uniform $C^{0,\beta}$ bound by step 1.3, while $w_k$ is smooth and has a bounded supremum. Apply [F9] to each $w_k$ on smaller balls. This gives a uniform $C^{3,\beta}$ bound for $w$, without an assumed uniform bound on its third derivatives. [step 1.3, step 4.1, F8, F9, F10, F11, given, algebra]

6.1 Now $a$ and $S$ have uniform $C^{2,\beta}$ bounds, using joint derivatives of $P$ through order three and step 5.1. Twice differentiating the equation gives $a^{ij}(w_{k\ell})_{ij}=-D_{k\ell}S-(D_{k\ell}a^{ij})w_{ij}-(D_ka^{ij})w_{ij\ell}-(D_\ell a^{ij})w_{ijk}$. Every term on the right has a uniform $C^{0,\beta}$ bound; $w_{k\ell}$ is smooth with bounded supremum. Apply [F9] once more to obtain a uniform $C^{4,\beta}$ bound for $w$ on further smaller balls. The differentiated equations use only the existing finite derivatives of $P$; the classical $C^2$ membership needed in these applications comes from the given smoothness of $w$. All preliminary bounds may depend on $M_0$, without being linear in it. [step 1.3, step 5.1, F8, F9, F10, F11, given, algebra]

7.1 In particular all derivative suprema of $w$ through order four are uniformly bounded. By [F15], $Dw,D^2w,D^3w$ are uniformly Lipschitz on convex interior balls. For $0\le t\le1$ set $\Phi_t(y)=(y,tDw(y))$, $G(y,p)=P_p(y,p)$ and $H_j(y,p)=s_{p_j}(y,p)$. The maps $\Phi_t,D\Phi_t,D^2\Phi_t$ are uniformly bounded and Lipschitz. For either $J=G$ or $J=H_j$, [F11] twice gives $D^2(J\circ\Phi_t)=D^2J(\Phi_t)[D\Phi_t,D\Phi_t]+DJ(\Phi_t)D^2\Phi_t$. For $G$, joint derivatives through order two use derivatives of $P$ through order three; for $H_j$ they use derivatives of $P$ through order four. Their $\alpha$-Hölder bounds follow from the joint $C^{4,\alpha}$ hypothesis, using [F15] for lower derivatives. Thus step 1.3 gives a common $C^{2,\alpha}$ bound for $a=G\circ\Phi_1$ and for $h_j(y,t)=H_j(\Phi_t(y))$ uniformly in $t$. No fifth derivative of $P$ is used. [step 1.3, step 6.1, F8, F11, F15, given]

8.1 On closed coordinate boxes inside these balls, $h_j$ and its first two spatial derivatives are continuous jointly with $t\in[0,1]$, including at the boundary of the slope ball because $P$ is defined on a slightly larger slope neighborhood. By [F14], twice passing spatial derivatives through the integral gives $D_y^\nu b^j(y)=\int_0^1D_y^\nu h_j(y,t)\,dt$ for $|\nu|\le2$, where $b^j=\int_0^1h_j\,dt$. The uniform integral error bound in [F14] bounds the derivative suprema and the second-derivative $\alpha$-Hölder differences by the bounds of step 7.1. Finite interior covers assemble common $C^{2,\alpha}$ bounds for $a$ and $b$ on a fixed intermediate annulus: close pairs lie in a controlled ball, and separated pairs use twice the supremum divided by the fixed separation to the power $\alpha$, as in [F1]. This completes the finite-regularity coefficient bootstrap. [step 7.1, F1, F8, F14, given]

9.1 Apply [F11] to the composition $y\mapsto P_R(y,Dw_R(y))$ to expand the flux equation as $A_R:D^2w_R+s_R(y,Dw_R)=0$. For each fixed $y$, the curve $\varphi_y(t)=s_R(y,tDw_R(y))$ is continuous on $[0,1]$, and [F11] gives $\varphi_y'(t)=\sum_j(s_R)_{p_j}(y,tDw_R(y))(w_R)_j(y)$. This derivative extends continuously to both endpoints: the whole segment lies in the slope ball, and the assumed joint regularity holds on a neighborhood of it. Thus [F12], with Countable Choice supplied by [F10], gives $s_R(y,Dw_R)=s_R(y,0)+b_R\cdot Dw_R$. Multiplying by $R$ gives $A_R:D^2v_R+b_R\cdot Dv_R=-R s_R(y,0)$. The forcing has $C^{2,\alpha}$ norm at most $K/R$. On the intermediate annulus of step 8.1 the realized coefficients have common $C^{2,\alpha}$ bounds, so apply [F5] there with target $A'$ exactly as in step 1.1, and use [F1] to rescale back. The supremum on that intermediate annulus is bounded by $\sup_A|v_R|$. This proves the asserted linear height estimate. [step 1.1, step 8.1, F1, F5, F10, F11, F12, given, algebra]

10.1 For stationary metric applications, [F2] identifies the sufficient flux and zero-slope forcing assumptions; [F7] fixes what stationary flow graph and maximality mean, while [F6] states exactly what parameter uniformity requires. These interfaces do not establish that a particular spacetime satisfies the quantitative bounds: the consumer must check differentiated background estimates, the common spacelike slope neighborhood, stationarity and the zero-slope forcing. The estimate just proved applies whenever these checks hold. [F2, F6, F7, step 9.1] ∎

### External input

In dimension $d$, a scalar $z\in H^1(B_1)$ weakly satisfying $\operatorname{div}(B Dz)=0$, with measurable symmetric $\lambda_* I\le B\le\Lambda_* I$, obeys $\|z\|_{C^{0,\theta}(B_{1/2})}\le C\|z\|_{L^2(B_1)}$ for some $\theta>0$, with $C,\theta$ depending only on $d,\lambda_*,\Lambda_*$. This is the symmetric real scalar case of Theorem 3.17 in [Fernández-Real and Ros-Oton, Regularity Theory for Elliptic PDE](https://www.ub.edu/pde/xros/Llibre-ellipticPDE.pdf), printed p. 93 (current PDF page 99). Only this homogeneous estimate is imported as [F20]; its proof is not reconstructed. The differentiated equation, lifting and restriction steps supply the local application under finite flux regularity.

### Remarks

The original realized-coefficient estimate is retained. The added stationary-flux route supplies precise sufficient hypotheses for the intended graph application and separates preliminary nonlinear control from the final linear estimate. The original article is not cited as a prerequisite source. No claim about an error in that article is made.


## A variable-coefficient annular barrier and inward boundary derivative

[Open item](item-lem-author-58255dfd955f-annular-hopf-barrier) · level 2


### Statement

Let $L=\Delta_h-V=a^{ij}\partial_{ij}+b^i\partial_i-V$ be the geometric operator on a relatively compact smooth metric chart, with symmetric uniformly elliptic $a$, bounded $a,b,V$, and $V\ge0$. Let $B_R(z)$ be an interior tangent Euclidean ball at $p$, with its closure in the chart. Suppose $u>0$ in the ball, $u\ge0$ on its closure, $u(p)=0$, $Lu\le0$, and $u$ is $C^2$ inside and $C^1$ at $p$. Then the derivative in direction $(z-p)/R$ at $p$ is strictly positive. This applies to the geometric operator from the coordinate-form lemma.

### Facts & Assumptions

[F1] The smooth metric $h$ is Riemannian in the sense of [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold). The symbol $\Delta_h$ uses the positive-divergence, metric-trace-of-Hessian convention of [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian). For the general metric-chart argument, use the differential expression $\Delta_h=a^{ij}\partial_{ij}+b^i\partial_i$ and coefficient bounds assumed in the Statement. For the smooth-exterior application, [lem-author-58255dfd955f-coordinate-schrodinger-form](item-lem-author-58255dfd955f-coordinate-schrodinger-form) supplies this differential expression for its smooth metric. Subtracting a bounded potential is a pointwise zeroth-order operation; no smoothness of the original $V$ is used below. For this application use the smooth metric on the closed ball, so the stated coefficient bounds and ellipticity hold. Fix $\lambda>0$ with $a^{ij}\xi_i\xi_j\ge\lambda|\xi|^2$, and bounds $\operatorname{tr}a\le T$, $|b|\le B$ and $0\le V\le Q$, where $Q\ge0$ is a constant.

[F2] The supplier [lem-author-58255dfd955f-compact-comparison](item-lem-author-58255dfd955f-compact-comparison) gives comparison for $\Delta_h-W$ on relatively compact smooth domains when $W\ge0$ is smooth and bounded and the difference belongs to $C^2(D)\cap C^1(\overline D)$, with each component closure meeting the boundary. In its stated ZFC setting, $(\Delta_h-W)w\ge0$ and $w\le0$ on the boundary imply $w\le0$ inside. We use this supplier only with the smooth constant $W=Q$ and annuli whose closed outer spheres lie strictly inside $B_R(z)$.

[F3] For every integer $n\ge1$, [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn), part 2, says that a subset of Euclidean $\mathbb R^n$ is compact if and only if it is closed and bounded. We use the Euclidean subspace metric on coordinate spheres and closed annuli. A compact coordinate set is also compact in the manifold: a manifold open cover pulls back under the inverse chart to an open cover of that coordinate set, and a finite subcover transfers back.

[F4] By [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric), a continuous real function on a nonempty compact metric space attains a minimum and a maximum. If it is strictly positive everywhere, its attained minimum is strictly positive.

[F5] Use the half-space chart and smooth-transition conventions of [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary). By [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary), an embedded smooth submanifold with boundary is a subset with a manifold-with-boundary smooth structure for which inclusion is a smooth embedding. Step 1.2 constructs these charts and the embedding for the closed annulus; no smooth-domain assertion is imported from the comparison theorem.

### Proof

**Given:** The hypotheses in the Statement and the suppliers and bounds in [F1]–[F5].

**Goal:** Prove that the inward derivative at $p$ is strictly positive.

**Proof technique:** direct.

1.1 Put $L_Q=\Delta_h-Q$. Positivity of $u$ inside the ball gives $L_Qu=Lu-(Q-V)u\le0$. Choose $\alpha>0$ so large that $\alpha^2\lambda R^2-2\alpha T-2\alpha BR-Q\ge0$; this is possible because $\lambda R^2>0$. This choice is independent of the truncated outer radius used below. [F1, given, algebra, choose]

1.2 For $R/2<s<R$, let $r=|x-z|$ and $D_s=\{R/2<r<s\}$. Write $n$ for the chart dimension. Since $|p-z|=R>0$, $n\ge1$. The sets $S_{R/2}=\{|x-z|=R/2\}$ and $N_s=\{R/2\le|x-z|\le s\}$ are closed and bounded in $\mathbb R^n$, hence compact by [F3], and lie inside $B_R(z)$. The sphere is nonempty, containing $z+(R/2)e_1$, where $e_1$ is the first coordinate unit vector. The radial inequalities show that $N_s=\overline{D_s}$ and $N_s\setminus D_s$ consists exactly of the spheres of radii $R/2$ and $s$. Here is an explicit smooth boundary chart near a point $y$ of either sphere. Write its radius as $r_0$ and choose $j$ with $y_j-z_j\ne0$. Set $\sigma=\operatorname{sign}(y_j-z_j)$ and use coordinates $(\widehat x_j,t)$, where $\widehat x_j$ lists all coordinates other than $x_j$, with $t=r-r_0$ on the inner sphere and $t=r_0-r$ on the outer sphere. With $\eta=1$ in the inner case and $\eta=-1$ in the outer case, the inverse is $x_j=z_j+\sigma\sqrt{(r_0+\eta t)^2-\sum_{i\ne j}(x_i-z_i)^2}$, retaining the other coordinates. Near $y$ the radicand is positive and the other radial inequality is strict, so these maps are mutually inverse smooth extensions on open Euclidean neighborhoods, and $N_s$ corresponds exactly to $t\ge0$. Along with ordinary charts in $D_s$, they form compatible half-space charts as in [F5]. The inclusion has the subspace topology and in each chart extends to a local Euclidean diffeomorphism, hence is a smooth embedding. Thus $N_s$ is a compact smooth full-dimensional closure with intrinsic boundary exactly those two spheres. Finally, for any $x$ in a component $C$ of $D_s$, the radial path $z+\tau(x-z)/|x-z|$, $|x-z|\le\tau<s$, lies in $D_s$ and in the same component as $x$; its limit at $\tau=s$ lies in $\overline C\cap\partial D_s$. This also covers $n=1$, when the annulus has two interval components and the boundary-chart list $\widehat x_j$ is empty. All these sets lie in the chart interior, so the same smooth-domain and component-boundary assertions hold on the manifold. [F3, F5, given, construct, algebra]

2.1 For any $R/2<s<R$, on $D_s=\{R/2<r=|x-z|<s\}$ set $\psi_s=e^{-\alpha r^2}-e^{-\alpha s^2}$. Direct differentiation in the coordinates from [F1] gives $L_Q\psi_s=e^{-\alpha r^2}(4\alpha^2a^{ij}(x-z)_i(x-z)_j-2\alpha\operatorname{tr}a-2\alpha b\cdot(x-z)-Q)+Qe^{-\alpha s^2}$. Since $r\ge R/2$ and $r\le R$, the parenthesis is at least $\alpha^2\lambda R^2-2\alpha T-2\alpha BR-Q$. Thus $L_Q\psi_s\ge0$ for every such $s$. [F1, step 1.1, algebra]

3.1 By step 1.2 the sphere $r=R/2$ is nonempty and compactly contained in the ball. The $C^2$ regularity of $u$ there gives continuity, so [F4] and strict positivity give an attained minimum $\mu=\min_{r=R/2}u>0$. Put $M=e^{-\alpha R^2/4}>0$ and fix $\epsilon=\mu/(2M)>0$, independently of $s$. On the inner sphere $0\le\psi_s\le M$, hence $\epsilon\psi_s\le u$; on the outer sphere $r=s$, $\psi_s=0<u$. The closed annulus lies inside the open ball, where $u$ is $C^2$, so $w_s=\epsilon\psi_s-u$ belongs to $C^2(D_s)\cap C^1(\overline D_s)$. Step 1.2 supplies its smooth relatively compact closure and proves that every component closure meets its boundary. Moreover $L_Qw_s\ge0$ by steps 1.1 and 2.1. Apply [F2] with constant potential $Q$ to conclude $u\ge\epsilon\psi_s$ throughout $D_s$. This application uses neither regularity on $r=R$ nor smoothness of $V$. [F2, F4, step 1.1, step 2.1, step 1.2, given, algebra, choose]

4.1 Fix $x$ with $R/2<|x-z|<R$. The comparison in step 3.1 holds for every $s\in(|x-z|,R)$, so taking $s\uparrow R$ yields $u(x)\ge\epsilon\psi_R(x)$, where $\psi_R(x)=e^{-\alpha|x-z|^2}-e^{-\alpha R^2}$. Let $v=(z-p)/R$. For $0<t<R/2$, the point $p+tv$ has radius $R-t$ and lies in this annulus. Since $u(p)=\psi_R(p)=0$, division by $t$ gives $(u(p+tv)-u(p))/t\ge\epsilon(e^{-\alpha(R-t)^2}-e^{-\alpha R^2})/t$. The assumed $C^1$ regularity at $p$ gives the left-hand limit $\partial_vu(p)$, and the right-hand limit is $2\epsilon\alpha R e^{-\alpha R^2}>0$. This proves the asserted inward derivative bound with exactly the stated regularity. [step 3.1, given, algebra] ∎


## Rescaling a geometric Schrödinger equation without treating its potential as forcing

[Open item](item-lem-author-58255dfd955f-unit-ball-rescaling) · level 2


### Statement

In a coordinate ball $B_r(x_0)$ let $-\operatorname{div}(A\nabla u)+qu=0$, with $A$ symmetric and $A\ge\lambda I$ for some $\lambda>0$. Define $v(y)=u(x_0+ry)$ on $B_1$. Then $-\operatorname{div}_y(\widetilde A\nabla_yv)+\widetilde qv=0$, where $\widetilde A(y)=A(x_0+ry)/\lambda$ and $\widetilde q(y)=r^2q(x_0+ry)/\lambda$. Thus $\widetilde A\ge I$, $\|\widetilde A\|\le\|A\|/\lambda$ and $\|\widetilde q\|_\infty\le r^2\|q\|_\infty/\lambda$.

### Facts & Assumptions

**Given:** The divergence and weak forms, matrix $A$ and potential coefficient $q$ are those of [lem-author-58255dfd955f-coordinate-schrodinger-form](item-lem-author-58255dfd955f-coordinate-schrodinger-form). Here $\|A\|$ is its operator-norm supremum. This is a homogeneous equation for an operator that includes the potential; $qu$ is not taken as an independently controlled forcing.

[F1] The coordinate supplier gives $u\in C^2_{\mathrm{loc}}$ and smooth $A,q$, with the weak identity for every real smooth test compactly supported in the interior coordinate ball. In this regularity all test integrands are continuous and compactly supported; the chart integrals in the calculation below may be evaluated as compactly supported Riemann integrals.

[F2] The total-derivative chain rule [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) applies to the affine maps $T(y)=x_0+ry$ and $T^{-1}(x)=(x-x_0)/r$, and to the differentiable functions composed with them. Here $r>0$, $DT=rI$ and $DT^{-1}=r^{-1}I$; these affine derivatives follow directly from their exact linear increments.

[F3] The compact-support substitution formula [math:cor-change-of-variables-for-compactly-supported-functions](https://alphabetamath.cc/item/cor-change-of-variables-for-compactly-supported-functions) applies to an injective $C^1$ map with invertible derivative and a compactly supported Riemann integrable function whose support lies in its image. Here $T:B_1\to B_r(x_0)$ is a smooth diffeomorphism, $|\det DT|=r^n$, and the integrands, extended by zero, are continuous and compactly supported in $B_r(x_0)$. Their restrictions to any nondegenerate bounding rectangle are Riemann integrable by [math:thm-continuous-on-a-rectangle-is-riemann-integrable](https://alphabetamath.cc/item/thm-continuous-on-a-rectangle-is-riemann-integrable). This uses the compact-support Riemann formula, not a change-of-variables assertion for arbitrary $L^1$ data.

### Proof

**Given:** The hypotheses and data in the Statement and Facts & Assumptions.

**Goal:** Establish the conclusions of the Statement.

**Proof technique:** direct.

1.1 Fix a real $\eta\in C_c^\infty(B_1)$ and set $\varphi=\eta\circ T^{-1}$. Its support is $T(\operatorname{supp}\eta)$, a compact subset of $B_r(x_0)$, so it is an admissible test in the coordinate weak identity. The chain rule gives $\nabla_yv=r(\nabla_xu)\circ T$ and $(\nabla_x\varphi)\circ T=r^{-1}\nabla_y\eta$. The functions $A\nabla u\cdot\nabla\varphi$ and $qu\varphi$, extended by zero outside the ball, are continuous compactly supported Riemann integrands. Apply compact-support substitution separately to these functions using $|\det DT|=r^n$ to obtain $r^{n-2}\int_{B_1} A(T(y))\nabla_yv\cdot\nabla_y\eta\,dy+r^n\int_{B_1}q(T(y))v\eta\,dy=0$. Dividing by $\lambda r^{n-2}>0$ proves the claimed homogeneous weak equation for every such $\eta$. The transformed coefficients are smooth and $v$ is $C^2$, so the weak identity has the classical interpretation as well, by the same interior integration-by-parts and continuous-residual argument supplied by the coordinate lemma. [F1, F2, F3, given, algebra]

2.1 For every vector $\xi$, $\xi^T\widetilde A(y)\xi=\lambda^{-1}\xi^TA(T(y))\xi\ge|\xi|^2$. Since $T$ maps $B_1$ bijectively onto $B_r(x_0)$, composition preserves the coefficient suprema. Thus $\|\widetilde A\|\le\|A\|/\lambda$ and $\|\widetilde q\|_\infty\le r^2\|q\|_\infty/\lambda$. These statements do not estimate $qu$ by an additive source norm. [step 1.1, given, algebra] ∎


## Finite Harnack chains on fixed compact connected interior sets

[Open item](item-lem-author-58255dfd955f-compact-harnack-chain) · level 2


### Statement

Let $(\Sigma,h)$ be a smooth three-dimensional Riemannian exterior and let $K\subset\Sigma^\circ$ be a nonempty compact connected subset, with compactness and connectedness taken in its subspace topology. There are finitely many interior coordinate balls $U_i$, $1\le i\le N$, with compact closures in their chart domains, whose concentric half-balls $H_i$ cover $K$. Each $H_i$ meets $K$, and the graph with vertices $1,\ldots,N$ and an edge between distinct $i,j$ exactly when $H_i\cap H_j\cap K\ne\varnothing$ is connected, meaning any two vertices can be joined by a finite sequence of edges. All balls are Euclidean in their respective coordinates. For any positive real function $u$ on $\bigcup_i U_i$, if $C_*\ge1$ and $u(x)\le C_*u(y)$ for every $x,y\in H_i$ and every $i$, then $\sup_Ku\le C_*^N\inf_Ku$. Thus the conditional comparison applies to every positive solution of $(\Delta_h-V)u=0$ for which these local comparisons hold.

In particular, work in ZFC for the following analytic consequence. Fix such a finite chart cover. Consider smooth Riemannian metrics $h$, potentials $V:\bigcup_i U_i\to[0,\infty)$ bounded on each $U_i$, and positive real $C^2$ functions $u$ solving $(\Delta_h-V)u=0$ pointwise there, where $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. Write $r_i$ for the coordinate radius of $U_i$ and, in its coordinates, put $m_i=\sqrt{\det(h_{ab})}$, $A_i=(m_i h^{ab})$ and $q_i=m_iV$. Suppose fixed constants $\lambda_i>0$, $M_i<\infty$ and $Q_i\ge0$, independent of the family member, satisfy $\xi^TA_i(x)\xi\ge\lambda_i|\xi|^2$, $\|A_i(x)\|_{\mathrm{op}}\le M_i$ and $q_i(x)\le Q_i$ on $U_i$ for every $\xi\in\mathbb R^3$. Then the comparison is uniform over the family: $C_*$ can be chosen using only the finitely many parameters $3$, $M_i/\lambda_i$ and $r_i^2Q_i/\lambda_i$. No measurability or smoothness of $V$ beyond these hypotheses is required. The preceding conditional chain comparison does not impose a sign condition on $V$ when the local comparisons are supplied independently.

### Facts & Assumptions

[F1] Compact subsets are compact in their subspace topology by [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space): every relatively open cover has a finite subcover. Connected subsets admit no partition into two disjoint nonempty relatively open sets by [math:def-connected-space](https://alphabetamath.cc/item/def-connected-space).

[F2] The smooth exterior, its interior charts, the Riemannian metric and the Laplacian convention are those of [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data). The letter $K$ here denotes the subset in the Statement, not necessarily the compact core of that definition. The sets $U_i,H_i$ and their graph are defined in the Statement; they are not required to be metric balls.

[F3] [lem-author-58255dfd955f-local-potential-harnack](item-lem-author-58255dfd955f-local-potential-harnack) applies to a nonnegative real $C^2$ pointwise solution on a coordinate ball for a smooth metric and a bounded nonnegative potential, with the displayed bounds on $A_i,q_i$. It gives a half-ball comparison constant at least one depending only on dimension, $M_i/\lambda_i$ and $r_i^2Q_i/\lambda_i$. The analytic consequence inherits its ZFC assumption, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice); that imported assumption is used precisely when this supplier is invoked in step 3.1. The finite-cover and finite-chain arguments themselves require no arbitrary-index choice.

### Proof

**Given:** The data and hypotheses in the Statement and [F1]–[F3].

**Goal:** The finite connected cover, conditional chain comparison and stated uniform analytic consequence.

**Proof technique:** direct.

1.1 Consider all interior chart balls centered at points of $K$ with compact closures inside their chart domains, together with their concentric half-balls. Such balls exist around every point by shrinking an interior coordinate neighborhood. The traces of these half-balls on $K$ are a relatively open cover of $K$, so [F1] supplies a finite subcover; retain the associated balls and discard any empty traces. Write $U_i,H_i$, $1\le i\le N$, for the resulting balls and half-balls. If their graph were disconnected, fix a vertex and let $I$ consist of the vertices reachable from it by finite edge sequences. Then $I$ and its complement are both nonempty, and there is no edge between them. The unions of $H_i\cap K$ over these two index sets are nonempty, relatively open, disjoint, and cover $K$. This contradicts connectedness in [F1], proving the geometric assertion. [given, F1, F2]

2.1 For $x,y\in K$, choose half-balls containing them. By step 1.1 their vertices are joined by a finite edge sequence; deleting segments between repeated vertices gives a path of $s\le N$ distinct vertices. At each edge take a point in the corresponding intersection with $K$. The resulting sequence starts at $x$, ends at $y$, and each consecutive pair lies in one of the $s$ half-balls. Applying the assumed local comparisons and multiplying gives $u(x)\le C_*^s u(y)\le C_*^N u(y)$, also when $s=1$. Taking the supremum in $x$ and then the infimum in $y$ proves the conditional bound. These extrema are finite and positive as bounded by any fixed value through the pairwise inequalities; continuity is not needed for this conditional argument. [given, step 1.1, algebra]

3.1 For the analytic family, on each fixed $U_i$ the metric is smooth, $V$ is bounded and nonnegative, $u$ is positive and $C^2$, and the pointwise equation and all three coefficient bounds are exactly those of [F3], with dimension three. Thus [F3] supplies a constant $C_i\ge1$ using only $3$, $M_i/\lambda_i$ and $r_i^2Q_i/\lambda_i$, common to all family members. Take $C_*=\max_{1\le i\le N}C_i$ and apply step 2.1. Both $N$ and these coefficient parameters are fixed, so the resulting comparison is uniform as asserted. [given, F2, F3, step 2.1] ∎


## A positive global supersolution with the exact exterior decay

[Open item](item-lem-author-86990d62062f-global-decaying-barrier) · level 2


### Statement

On the component containing the Euclidean end, with the smooth exterior data and Laplacian convention of the weighted exterior definition, assume $h-\delta\in C^{3,\alpha}_{-1}$ and $-1<\beta<0$. There is a positive continuous function $B$, smooth on either side of one large coordinate sphere $S_R=\{r=R\}$ up to each side's boundary, with $B=r^\beta$ outside that sphere, $B\asymp1$ on the compact core and $-\Delta_h B\ge c\rho^{\beta-2}$ away from the sphere, for some $c>0$. Here $\rho$ is any positive smooth function equal to $r$ far out. With $\nu$ the $h$-unit normal from the core into the end, define $J_\nu w=(\partial_\nu w)_{\mathrm{ext}}-(\partial_\nu w)_{\mathrm{int}}$, using the same normal on both sides. Across the sphere $J_\nu B<0$.

The precise maximum comparison is as follows. Suppose $v$ is continuous on this component including its original boundary, is $C^2$ off $S_R$ with one-sided $C^1$ regularity at $S_R$, and satisfies $\Delta_hv\ge0$ off $S_R$, $J_\nu v\ge0$, $v\le0$ on the original boundary and $\limsup_{r\to\infty}v\le0$. The last condition means that for every $a>0$, $v\le a$ outside some compact set. Then $v\le0$ everywhere. On a compact truncation $M_T$ with $T>R$, the same comparison holds with $v\le0$ on its entire boundary, including $\{r=T\}$, and no condition at infinity.

### Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] Weighted coefficients, the smooth Riemannian exterior, compact core, Laplacian sign and end derivative conventions are fixed. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] Compact smooth cores with a boundary admit a zero-boundary torsion solution of class $C^{4,\alpha}$. [lem-author-86990d62062f-compact-domain-poisson](item-lem-author-86990d62062f-compact-domain-poisson)

[F3] Higher classical elliptic regularity, including regularity at a smooth boundary portion with smooth Dirichlet values, is the imported Euclidean input specified below (Gilbarg–Trudinger, Theorems 6.17 and 6.19).

### External input

The cited regularity theorems apply to an already classical solution, with the coefficient, forcing and boundary regularity recorded in the source contract. Only their regularity conclusions are imported. Smoothness of the manifold torsion solution is deduced in step 3.1 by applying them in charts; no manifold existence theorem is imported.

### Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] Weighted coefficients, the smooth Riemannian exterior, compact core, Laplacian sign and end derivative conventions are fixed. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] Compact smooth cores with a boundary admit a zero-boundary torsion solution of class $C^{4,\alpha}$. [lem-author-86990d62062f-compact-domain-poisson](item-lem-author-86990d62062f-compact-domain-poisson)

[F3] Higher classical elliptic regularity, including regularity at a smooth boundary portion with smooth Dirichlet values, is the imported Euclidean input specified below (Gilbarg–Trudinger, Theorems 6.17 and 6.19).

**Proof technique:** direct.

1.1 Write $\Delta_h=h^{ij}\partial_i\partial_j+b^i\partial_i$. The stated decay gives $h^{ij}=\delta^{ij}+O(r^{-1})$ and $b^i=O(r^{-2})$. Direct radial differentiation gives $\Delta_hr^\beta=\beta(\beta+1)r^{\beta-2}+O(r^{\beta-3})$. Since $\beta(\beta+1)<0$, choose a large $R$ so $-\Delta_hr^\beta\ge c_0r^{\beta-2}$ on $r\ge R$. [F1]

2.1 Let $M_R$ be the end component truncated at $r=R$. It is compact with smooth boundary. It is connected: any excursion of a path into $r>R$ can be retracted radially onto $S_R$, which is connected. In particular it meets its boundary $S_R$, so the compact Poisson supplier applies. Solve $-\Delta_ht=1$, $t=0$ on its entire boundary, including any original boundary, obtaining $t\in C^{4,\alpha}(M_R)$. If $t$ had a negative minimum, it would be interior, where its vanishing gradient and nonnegative Hessian imply $\Delta_ht\ge0$, contradicting $\Delta_ht=-1$. Thus $t\ge0$. [F1, F2, step 1.1]

3.1 In each relatively compact interior or boundary chart the equation for $t$ is a strictly elliptic scalar equation with smooth coefficients and forcing $-1$. Positivity of the smooth metric gives uniform ellipticity on the smaller compact patch. The solution is already classical by step 2.1. Theorem 6.17 applies in interior charts. At a boundary chart, Theorem 6.19's local-boundary-portion conclusion applies to the smooth physical boundary with zero data; no regularity of values on artificial chart edges is required. For each integer $k\ge0$ these inputs give $C^{k+2,\alpha}$ regularity on smaller patches. A finite chart cover proves $t\in C^\infty(M_R)$ up to its entire boundary, including $S_R$. This is a local application of the imported theorems, not a reduction of the compact core to one Euclidean domain. [F1, F3, step 2.1]

4.1 Set $B=R^\beta+\epsilon t$ on $M_R$ and $B=r^\beta$ outside. Both traces on the seam are $R^\beta$. There $\nu=\nabla_hr/|\nabla_hr|_h$, so $\nu(r)=|\nabla_hr|_h>0$ and the exterior derivative $\beta R^{\beta-1}\nu(r)$ is strictly negative. [math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function) Compactness of $S_R$ bounds it uniformly away from zero and bounds $\partial_\nu t$. Choose $\epsilon>0$ small enough that $J_\nu B=\beta R^{\beta-1}\nu(r)-\epsilon\partial_\nu t<0$ on the whole sphere. Inside, $-\Delta_hB=\epsilon$; outside use step 1.1. The positive smooth $\rho$ has finite maximum and positive minimum on compact sets and equals $r$ far out, so decreasing $c>0$ if necessary gives $-\Delta_hB\ge c\rho^{\beta-2}$ on both pieces. The barrier is positive; on the core it lies between $R^\beta$ and $R^\beta+\epsilon\max t$, proving $B\asymp1$ there. Its asserted piecewise smoothness follows from step 3.1 and smoothness of $r^\beta$ on the end. [F1, step 1.1, step 2.1, step 3.1]

5.1 First consider a function $w$ with the stated continuity and one-sided regularity, with $\Delta_hw>0$ on each piece, $J_\nu w>0$, negative original boundary values and $\limsup_{r\to\infty}w\le0$. If $w(p)>0$ anywhere, choose $0<a<w(p)$. Outside a compact set $w\le a$, so $w$ attains a positive global maximum on a compact truncation, away from both its outer boundary and its original boundary. At an interior maximum off the seam, the gradient vanishes and the Hessian is negative semidefinite, giving $\Delta_hw\le0$, a contradiction. At a seam maximum, the interior derivative in direction $\nu$ is nonnegative and the exterior derivative in the same direction is nonpositive. Hence $J_\nu w\le0$, again a contradiction. Thus $w\le0$. On compact $M_T$ the same argument uses compactness and negative entire boundary values directly. [F1, step 4.1]

6.1 For $v$ satisfying the weak comparison hypotheses set $w=v-\eta B$ for any $\eta>0$. Then $\Delta_hw=\Delta_hv-\eta\Delta_hB>0$ off the seam, $J_\nu w=J_\nu v-\eta J_\nu B>0$, and $w<0$ on every boundary where $v\le0$. Since $B=r^\beta\to0$, the condition $\limsup_{r\to\infty}v\le0$ also gives $\limsup_{r\to\infty}w\le0$. Step 5.1 yields $v\le\eta B$; let $\eta\downarrow0$ at each point to obtain $v\le0$. For compact truncations the same perturbation has negative values on the entire boundary, so the compact version of step 5.1 applies. This proves the comparison and completes the Statement. [F1, step 4.1, step 5.1] ∎


## Compact extra components contribute index zero

[Open item](item-lem-author-86990d62062f-closed-component-index) · level 2


### Statement

If the exterior definition permits extra compact components, there are only finitely many. A compact component with nonempty boundary contributes an invertible Dirichlet block. On a connected closed component the scalar Laplacian $C^{4,\alpha}\to C^{2,\alpha}$ has constants as kernel and the mean-zero functions as range, hence index zero. Consequently allowing these components does not change the index-zero conclusion on the full exterior.

### Facts & Assumptions

**Given:** the hypotheses in the Statement, $0<\alpha<1$, and the exterior conventions; work in ZFC.

[A1] Work in ZFC; full Choice supplies the DC and Countable Choice required by the analytic and integration inputs. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F1] The exterior has a compact core and exactly one specified noncompact end. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F2] Compact components with nonempty boundary have the Dirichlet inverse. [lem-author-86990d62062f-compact-domain-poisson](item-lem-author-86990d62062f-compact-domain-poisson)

[F3] The compact boundaryless scalar Laplace-type Green operator has range orthogonal to its smooth kernel. [math:thm-sobolev-compactness-and-elliptic-estimates-give-fredholm-hodge-decomposition](https://alphabetamath.cc/item/thm-sobolev-compactness-and-elliptic-estimates-give-fredholm-hodge-decomposition)

[F4] The interior Schauder estimate gives $C^{2,\alpha}$ regularity and a smaller-ball estimate for bounded classical $C^2$ solutions with $C^{0,\alpha}$ forcing. Its boundary counterpart supplies the second-order Dirichlet estimate used in the compact-domain construction. [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations) [math:thm-boundary-schauder-estimate-for-the-dirichlet-problem](https://alphabetamath.cc/item/thm-boundary-schauder-estimate-for-the-dirichlet-problem)

[F5] For the compact boundaryless operators under consideration, $H^k$ is defined by finite smooth localization, and $H^k\hookrightarrow C^r$ continuously if $k>r+3/2$. In particular $H^4\hookrightarrow C^2$ and $H^2\hookrightarrow C^0$. [math:thm-elliptic-differential-operators-on-compact-vector-bundles-have-parametrices-and-regularity](https://alphabetamath.cc/item/thm-elliptic-differential-operators-on-compact-vector-bundles-have-parametrices-and-regularity)

[F6] The Riemannian density is $d\mu_h=\sqrt{\det h}\,|dx^1dx^2dx^3|$. Its integral is the partition-weighted coordinate integral, without an orientation; smooth subordinate partitions of unity exist. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration) [math:thm-smooth-partitions-of-unity-exist-on-manifolds](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds)

[F7] For $m=\sqrt{\det h}$, the coordinate divergence is $m^{-1}\partial_i(mX^i)$, also on nonorientable manifolds. A compactly supported $C^1$ vector field on $\mathbb R^3$ has integrable field and divergence and zero divergence integral. [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence) [math:lem-integral-of-a-divergence-of-an-l-one-c-one-field-vanishes](https://alphabetamath.cc/item/lem-integral-of-a-divergence-of-an-l-one-c-one-field-vanishes)

[F8] The finite-norm Euclidean closure Hölder spaces are Banach. A bounded linear bijection between Banach spaces has bounded inverse under DC. Fredholm index is kernel dimension minus cokernel dimension, with closed range required. [math:thm-holder-spaces-on-bounded-domains-are-banach-spaces](https://alphabetamath.cc/item/thm-holder-spaces-on-bounded-domains-are-banach-spaces) [math:thm-bounded-inverse-theorem](https://alphabetamath.cc/item/thm-bounded-inverse-theorem) [def-fredholm-continuation-data](item-def-fredholm-continuation-data)

[F9] Higher interior regularity for a classical solution is imported in External input.

### External input

Theorem 6.17 in the cited book supplies the higher interior regularity in [F9], with $k=2$. Only precompact Euclidean charts are used; the Hölder inverse estimate below is derived locally.

[Gilbarg–Trudinger, Theorem 6.17](https://djvu.online/file/jxRRleAzbYjsl).

### Proof

**Given:** the hypotheses in the Statement, $0<\alpha<1$, and the exterior conventions; work in ZFC.

**Goal:** prove the Statement.

**Proof technique:** direct.

1.1 Manifold components are open, since each point has a connected ball or half-ball neighborhood. Their intersections with the compact core $K$ form an open cover of $K$, so only finitely many components meet $K$. The connected tail $\{r>2r_0\}$ lies in one component. Every other component lies in $K$, is closed in the manifold, and hence is compact. Thus there are finitely many extra components. [F1]

1.2 Let $M$ be a connected closed component. For a $C^1$ vector field $X$, choose a finite smooth partition $(\chi_a)$ supported compactly inside precompact coordinate charts. In chart $a$ put $m_a=\sqrt{\det h}$ and extend the vector field with coefficients $m_a\chi_a X^i$ by zero to $\mathbb R^3$. This is $C^1$ and compactly supported, so [F7] gives zero integral of its Euclidean divergence. By [F6] and the coordinate formula, this is $\int_M\operatorname{div}_h(\chi_aX)\,d\mu_h=0$. Summing over $a$, the product rule and $\sum_a\chi_a=1$ give $\int_M\operatorname{div}_hX\,d\mu_h=0$. For real $C^2$ functions $u,v$, take $X=u\operatorname{grad}_h v$; expanding the same coordinate formula gives $\int_M u\Delta_hv\,d\mu_h=-\int_M h^{ij}(\partial_i u)(\partial_jv)\,d\mu_h$. Taking $u=1$ gives $\int_M\Delta_hv\,d\mu_h=0$. This proof uses densities throughout and needs no orientation. [A1, F1, F6, F7]

2.1 On any fixed compact component, use finitely many precompact coordinate balls or boundary half-balls and the usual closure Hölder norms, for $k=2,4$. A Cauchy sequence converges in each chart by [F8]; its local function and derivative limits agree on overlaps by their uniform convergence and the coordinate chain rule. They therefore define a global $C^{k,\alpha}$ limit, with convergence in the finite chart norm. This proves the needed Banach property. The zero-boundary subspace is closed because the norm controls the continuous boundary values. The coordinate formula for $\Delta_h$ has smooth coefficients on these compact patches, so it is a bounded linear map from that Dirichlet $C^{4,\alpha}$ space to $C^{2,\alpha}$. For a component with nonempty boundary, [F2] gives bijectivity; [F8] then gives a bounded inverse. The boundary estimate in [F4] is used only in that supplied compact-domain construction, not as an estimate on a closed component. [A1, F1, F2, F4, F8, step 1.1]

2.2 Use $P=-\Delta_h$ on the trivial real line bundle over $M$ with the positive density $d\mu_h$. Its smooth principal symbol is $h^{ij}\xi_i\xi_j>0$ for $\xi\ne0$, and step 1.2 makes it formally symmetric. These are precisely the compact, boundaryless, positive scalar-symbol hypotheses of [F3] and [F5]. The Green theorem makes the $H^2$ kernel smooth. For a member $v$ of that kernel, step 1.2 with $u=v$ gives $\int_M|dv|_h^2\,d\mu_h=0$. The integrand is continuous and nonnegative, and the density is positive in every chart, so $dv=0$ everywhere. A connected manifold is path connected, because its path components are open in connected coordinate neighborhoods; thus $v$ is constant. Conversely constants are in the kernel. Consequently [F3] gives a bounded Green map $G:H^k\to H^{k+2}$ on mean-zero data, for every integer $k\ge0$. [A1, F3, F5, F6, step 1.2]

3.1 If $f\in C^{2,\alpha}(M)$ and $\int_M f\,d\mu_h=0$, set $u=-Gf$. Finite smooth localization on compact charts puts $f$ in $H^2$, with $\|f\|_{H^2}\le C\|f\|_{C^{2,\alpha}}$: each localized derivative through order two is bounded on a bounded chart support. The Green bounds give $u\in H^4$, $\Delta_hu=f$, and $\int_Mu\,d\mu_h=0$. By [F5], $H^4\hookrightarrow C^2$ in dimension three, so this distributional equation is classical: its two sides are continuous and agree as distributions. Moreover $\|u\|_{C^0}\le C\|u\|_{H^2}\le C\|f\|_{L^2}\le C\|f\|_{C^0}$, by the $H^2\hookrightarrow C^0$ embedding and the $k=0$ Green bound. The hypotheses of [F9] now hold in each precompact chart: $L=\Delta_h=h^{ij}\partial_i\partial_j+b^j\partial_j$ is uniformly elliptic there with smooth coefficients, $f\in C^{2,\alpha}$, and $u\in C^2$. Theorem 6.17 with $k=2$ gives $u\in C^{4,\alpha}$ locally. A finite smaller-chart cover gives this regularity on $M$. [A1, F1, F3, F5, F6, F9, step 2.2]

4.1 To prove the Hölder inverse bound, fix nested coordinate balls $B_R\supset B_{R/2}\supset B_{R/4}\supset B_{R/8}$ with the closure of $B_R$ inside a chart. Write $a^{ij}=h^{ij}$ and $Lu=a^{ij}u_{ij}+b^ju_j=f$. By [F4], $\|u\|_{C^{2,\alpha}(B_{R/2})}\le C(\|f\|_{C^{0,\alpha}(B_R)}+\|u\|_{C^0(B_R)})$. All subsequent differentiations are legitimate by step 3.1. For a coordinate index $\ell$, $L(\partial_\ell u)=\partial_\ell f-(\partial_\ell a^{ij})u_{ij}-(\partial_\ell b^j)u_j$. Apply [F4] to this classical solution on $B_{R/2}$ and estimate products by $[pq]_\alpha\le\|p\|_\infty[q]_\alpha+[p]_\alpha\|q\|_\infty$. This gives $\|u\|_{C^{3,\alpha}(B_{R/4})}\le C(\|f\|_{C^{1,\alpha}(B_R)}+\|u\|_{C^0(B_R)})$. For $|\gamma|=2$, $L(D^\gamma u)=D^\gamma f-[D^\gamma,L]u$, where the commutator $[D^\gamma,L]=D^\gamma L-LD^\gamma$ has coefficients involving derivatives of $a,b$ through order two and applies derivatives of order at most three to $u$. Its $C^{0,\alpha}$ norm is bounded by $C\|u\|_{C^{3,\alpha}(B_{R/4})}$. One more application of [F4] on $B_{R/4}$ yields $\|u\|_{C^{4,\alpha}(B_{R/8})}\le C(\|f\|_{C^{2,\alpha}(B_R)}+\|u\|_{C^0(B_R)})$. Choose finitely many such inner balls covering $M$. Smooth coordinate transitions on their compact overlaps compare the finite chart norms by the chain rule and the same product inequality. Summation and the $C^0$ bound of step 3.1 give $\|u\|_{C^{4,\alpha}(M)}\le C_M\|f\|_{C^{2,\alpha}(M)}$. [F1, F4, F5, step 3.1]

5.1 The integral functional $f\mapsto\int_M f\,d\mu_h$ is continuous on $C^{2,\alpha}(M)$, since its absolute value is at most $\mu_h(M)\|f\|_{C^0}$. It is nonzero on constants because $0<\mu_h(M)<\infty$. Its kernel is therefore a closed codimension-one subspace: explicitly, every $f$ decomposes as its mean constant plus a mean-zero function. Step 1.2 shows the Laplacian range is contained in this kernel; step 3.1 proves equality. The $C^{4,\alpha}$ kernel is exactly the constants by step 1.2, and step 4.1 supplies the bounded inverse between the mean-zero subspaces. Thus the closed block is Fredholm with one-dimensional kernel and cokernel, hence index zero. [F1, F6, F8, step 2.1, step 1.2, step 3.1, step 4.1]

6.1 Only finitely many compact blocks occur by step 1.1. Their finite direct sum has closed range, kernel the direct sum of their kernels, and cokernel the direct sum of their cokernels. Indeed, in finitely many coordinates convergence is coordinatewise, so a product of closed ranges is closed, and quotienting the product range is the product of the coordinate quotients. Each nonempty-boundary block has index zero by step 2.1; each closed connected block has index zero by step 5.1. Hence their kernel and cokernel dimensions are equal and finite. Adding these blocks to the end-component operator adds equal amounts to the kernel and cokernel dimensions and preserves closedness of the range. Consequently, whenever the end-component operator has index zero, so does the full operator. This proves every assertion of the Statement. [F1, F8, step 1.1, step 2.1, step 5.1] ∎



## A compact chronological target supplies a causal endpoint

[Open item](item-lem-author-2632702918ef-compact-target-causal-endpoint) · level 2


### Statement

Let $(E,g,N)$ be globally hyperbolic in the causal-exterior interface, and let $C\subset E$ be a compact spacelike two-surface in the null-screen interface. Let $\tau$ be a temporal function and suppose $p\in\partial_E I_E^-(C)$ with $\tau(p)<\min_C\tau$. Then some $c\in C$ satisfies $p\le_Ec$ and $p\ne c$, whereas $p\notin I_E^-(C)$. No acausality of $C$ is assumed.

### Facts & Assumptions

[A1] Work in ZFC; the axiom of choice includes the countable and dependent choice assumptions of the causal suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] All chronological and causal relations, boundaries, temporal functions and global hyperbolicity are relative to $E$. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F2] A spacelike two-surface is a nonempty smooth embedded two-manifold without boundary with positive-definite induced metric. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F3] In a globally hyperbolic spacetime, $J^-(C)$ is closed for compact $C$. [physics:lem-gr-globally-hyperbolic-causal-structure](https://alphabetamath.cc/physics/item/lem-gr-globally-hyperbolic-causal-structure)

[F4] The chronological past of each point is open. [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[F5] Arbitrary unions of open sets are open, by topology axiom (T2). [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)

[F6] A continuous real-valued function on a nonempty compact space attains its minimum, by the extreme-value clause (2). The restriction of a continuous function to a subspace is continuous. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the asserted conclusion.

1.1 The set $I_E^-(C)=\bigcup_{c\in C}I_E^-(c)$ is open by [F4] and [F5], so its boundary is disjoint from it. Every point of that set lies in $J_E^-(C)$; its closure also lies there by [F3]. Thus $p\in J_E^-(C)\setminus I_E^-(C)$. [A1, F1, F2, F3, F4, F5, given]

2.1 The temporal function $\tau$ is continuous by [F1], so $\tau|_C$ is continuous by [F6]. The space $C$ is nonempty by [F2] and compact by hypothesis; clause (2) of [F6] therefore makes $\min_C\tau$ well defined. By the definition of $J_E^-(C)$ there is a $c\in C$ with $p\le_Ec$. If $p\in C$, minimality would give $\min_C\tau\le\tau(p)$, contrary to the strict temporal inequality. Thus $p\notin C$ and $p\ne c$. Together with step 1.1 this proves the assertion without any condition on causal relations among different points of $C$. [step 1.1, F1, F2, F6, given] ∎


## A temporal covector has uniform compact negativity and orientation margins

[Open item](item-lem-author-89004136b63c-temporal-compact-margins) · level 2


### Statement

Let $O$ be an open subset of a smooth four-manifold, $g$ a $C^2$ Lorentz metric of signature $(-,+,+,+)$ on $O$, $N$ a continuous timelike orientation field on $O$, and $\alpha$ a continuous covector field on $O$. Let $K\subset O$ be nonempty and compact. At each point, the raised vector $\alpha^\sharp$ is characterized by $g(\alpha^\sharp,w)=\alpha(w)$ for every tangent vector $w$, and $g^{-1}(\alpha,\beta)=g(\alpha^\sharp,\beta^\sharp)$. The future timelike cone is the component of the timelike set containing $N$; the other component is past timelike. These pointwise constructions are justified below at the stated regularity.

Suppose $g^{-1}(\alpha,\alpha)<0$, $\alpha(N)>0$ and $g(N,N)<0$ on $K$. Then there are constants $m,a,b>0$ such that $g^{-1}(\alpha,\alpha)\le-m$, $\alpha(N)\ge a$, and $g(N,N)\le-b$ throughout $K$. For any fixed finite compact chart cover consisting of compact sets $K_j\subset O\cap U_j$, where $U_j$ is a smooth chart domain and $K\subset\bigcup_j K_j$, the components of $\alpha$ and $N$ in that chart are bounded on each $K_j$. Such covers exist, and may be chosen with every $K_j\subset K$. At any point, call $\alpha$ temporal when $g^{-1}(\alpha,\alpha)<0$ and $\alpha(N)>0$; its raised vector is past timelike there.

### Statement references

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)

[math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

[lem-author-89004136b63c-compact-neighborhood-localization](item-lem-author-89004136b63c-compact-neighborhood-localization)

[physics:def-lorentz-form-and-inertia](https://alphabetamath.cc/physics/item/def-lorentz-form-and-inertia)

[physics:def-causal-classification-of-lorentz-vectors](https://alphabetamath.cc/physics/item/def-causal-classification-of-lorentz-vectors)

[physics:def-time-orientation-and-future-causal-sets](https://alphabetamath.cc/physics/item/def-time-orientation-and-future-causal-sets)

[physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components)

[math:thm-cauchy-schwarz-finite](https://alphabetamath.cc/item/thm-cauchy-schwarz-finite)

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:thm-tensor-transition-laws-define-a-smooth-vector-bundle](https://alphabetamath.cc/item/thm-tensor-transition-laws-define-a-smooth-vector-bundle)

[math:thm-coordinate-differentials-form-the-dual-cotangent-basis](https://alphabetamath.cc/item/thm-coordinate-differentials-form-the-dual-cotangent-basis)

[math:def-vector-bundle-chart-and-transition-function](https://alphabetamath.cc/item/def-vector-bundle-chart-and-transition-function)

[math:def-c-r-and-smooth-maps-between-smooth-manifolds](https://alphabetamath.cc/item/def-c-r-and-smooth-maps-between-smooth-manifolds)

[math:thm-ck-euclidean-maps-closed-under-algebra-and-composition](https://alphabetamath.cc/item/thm-ck-euclidean-maps-closed-under-algebra-and-composition)

### Facts & Assumptions

[F1] For smooth data, the musical convention characterizes raising by $g(\alpha^\sharp,w)=\alpha(w)$, and the temporal-function convention uses past-timelike gradients. These suppliers fix the conventions only; their smooth hypotheses are not asserted for the present data. The pointwise construction and orientation test for the present $C^2$ metric and continuous fields are established in steps 2.1 and 3.1. [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F2] A Lorentz form on a four-dimensional real vector space is nondegenerate and has signature $(-,+,+,+)$, with an orthonormal basis in which its quadratic form is $-(v^0)^2+|\mathbf v|^2$. Timelike means negative quadratic form. The timelike set has exactly two components, described in such a basis by $v^0>|\mathbf v|$ and $v^0<-|\mathbf v|$; a time orientation chooses one component as future. All these are pointwise vector-space statements, with no differentiability hypothesis. [physics:def-lorentz-form-and-inertia](https://alphabetamath.cc/physics/item/def-lorentz-form-and-inertia) [physics:def-causal-classification-of-lorentz-vectors](https://alphabetamath.cc/physics/item/def-causal-classification-of-lorentz-vectors) [physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components) [physics:def-time-orientation-and-future-causal-sets](https://alphabetamath.cc/physics/item/def-time-orientation-and-future-causal-sets)

[F3] An invertible matrix with $C^2$ entries on an open coordinate domain has $C^2$ inverse entries. We apply this with $4\times4$ metric matrices and nonvanishing determinant. [math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)

[F4] Compactness gives finite open subcovers, also for ambient open covers. Applying compact-neighborhood localization inside the specified open set $O$ gives finite compact chart pieces covering $K$; its construction can take the pieces to be subsets of $K$, hence of $O$. [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space) [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient) [lem-author-89004136b63c-compact-neighborhood-localization](item-lem-author-89004136b63c-compact-neighborhood-localization)

[F5] For two lists of three real numbers, $|\sum_{i=1}^3 x_i y_i|\le(\sum_{i=1}^3 x_i^2)^{1/2}(\sum_{i=1}^3 y_i^2)^{1/2}$. This is the finite Cauchy-Schwarz inequality with three entries. [math:thm-cauchy-schwarz-finite](https://alphabetamath.cc/item/thm-cauchy-schwarz-finite)

[F6] A smooth manifold has a maximal smooth atlas. Tensor-coordinate trivializations give smooth vector bundles for types $(1,0)$, $(0,1)$ and $(0,2)$, with fibres respectively tangent vectors, covectors and bilinear forms. The coordinate tangent vectors and coordinate differentials are dual bases. Bundle-chart changes are smooth and fibrewise linear. The $C^2$ class of a map is tested in smooth coordinates, and finite $C^2$ sums, products and compositions are $C^2$. These structural interfaces are used in step 1.1 to justify the component criteria for the present continuous and $C^2$ sections, without assuming that those sections are smooth. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:thm-tensor-transition-laws-define-a-smooth-vector-bundle](https://alphabetamath.cc/item/thm-tensor-transition-laws-define-a-smooth-vector-bundle) [math:thm-coordinate-differentials-form-the-dual-cotangent-basis](https://alphabetamath.cc/item/thm-coordinate-differentials-form-the-dual-cotangent-basis) [math:def-vector-bundle-chart-and-transition-function](https://alphabetamath.cc/item/def-vector-bundle-chart-and-transition-function) [math:def-c-r-and-smooth-maps-between-smooth-manifolds](https://alphabetamath.cc/item/def-c-r-and-smooth-maps-between-smooth-manifolds) [math:thm-ck-euclidean-maps-closed-under-algebra-and-composition](https://alphabetamath.cc/item/thm-ck-euclidean-maps-closed-under-algebra-and-composition)

### Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the compact margins, the component bounds on the specified chart pieces, and the pointwise past-timelike conclusion.

1.1 Use the smooth charts and the tensor-coordinate trivializations from F6. In a chart $(U,x)$ restricted to $O$, write $e_a=\partial/\partial x^a$ and let $dx^a$ be its dual basis. Then $N=\sum_a N^a e_a$, $\alpha=\sum_a\alpha_a dx^a$ and $g=\sum_{a,b}g_{ab}\,dx^a\otimes dx^b$, with $N^a=dx^a(N)$, $\alpha_a=\alpha(e_a)$ and $g_{ab}=g(e_a,e_b)$. For any of these bundles, a section $s$ has trivialization coordinates $p\mapsto(p,c(p))$, where $c$ is precisely its finite list of field components. A trivialization and its inverse are continuous, so $s$ is continuous on the chart domain exactly when $c$ is continuous: the forward direction projects the continuous map $(p,c(p))$ to its fibre coordinates, and the reverse direction composes this product map with the inverse trivialization. In total-space smooth coordinates the same representative is $x(p)\mapsto(x(p),c(p))$, so F6's coordinate definition of $C^2$ gives the corresponding equivalence for $C^2$ sections. Changing a bundle chart replaces $c$ by a smooth matrix times $c$ and changes the base coordinates smoothly; hence continuity and $C^2$ regularity are preserved, the latter by F6's algebra and composition rule. Consequently $N^a$ and $\alpha_a$ are continuous and $g_{ab}$ is $C^2$ in every smooth chart on $O$, at exactly the regularities stated. [given, F6, algebra]

2.1 At $p\in O$, let $G=(g_{ab}(p))$ in a smooth coordinate chart. Nondegeneracy gives an inverse matrix $(g^{ab}(p))$. Define $v^a=\sum_b g^{ab}(p)\alpha_b(p)$. Matrix multiplication gives $g_p(v,w)=\alpha_p(w)$ for every $w\in T_pO$. This vector is unique, since a difference of two candidates pairs to zero with every $w$ and $g_p$ is nondegenerate. Thus the coordinate construction is independent of the chart and defines $\alpha^\sharp$. The same construction for any covector $\beta$ defines $g^{-1}(\alpha,\beta)$ with coefficients $g^{ab}$ and gives $g(\alpha^\sharp,\alpha^\sharp)=g^{-1}(\alpha,\alpha)$ and $g(\alpha^\sharp,N)=\alpha(N)$. By step 1.1 the metric coefficients are $C^2$, so F3 makes the inverse coefficients $C^2$; finite sums and products of them with the continuous field components show that $g^{-1}(\alpha,\alpha)$, $\alpha(N)$ and $g(N,N)$ are continuous. This constructs the convention of F1 without imposing smoothness on $g,N$ or $\alpha$. [given, F1, F2, F3, step 1.1, algebra]

3.1 Fix $p\in O$ and a $g_p$-orthonormal basis from F2, and write a timelike vector $v$ and $N_p$ as $(v^0,\mathbf v)$ and $(n^0,\mathbf n)$. Their timelikeness gives $|\mathbf v|<|v^0|$ and $|\mathbf n|<|n^0|$, so F5 yields $|\mathbf v\cdot\mathbf n|\le|\mathbf v|\,|\mathbf n|<|v^0n^0|$. Consequently $g_p(v,N_p)=-v^0n^0+\mathbf v\cdot\mathbf n$ is negative exactly when $v^0,n^0$ have the same sign, and positive exactly when their signs differ. F2 identifies these alternatives with the same and opposite timelike components. Therefore, relative to the component selected by $N_p$, a timelike $v$ is past directed exactly when $g_p(v,N_p)>0$. This is a pointwise test and requires no smooth orientation field or smoothly varying orthonormal basis. Applied to $v=\alpha^\sharp$, step 2.1 proves the asserted temporal-covector convention, including the past-timelike conclusion wherever the two defining inequalities hold. [F1, F2, F5, step 2.1, algebra]

3.2 Put $h=-g^{-1}(\alpha,\alpha)$, $u=\alpha(N)$ and $z=-g(N,N)$. These functions are continuous on $O$ and positive on $K$. For each $p\in K$, define $W_p$ to be the set of $q\in O$ satisfying $h(q)>h(p)/2$, $u(q)>u(p)/2$ and $z(q)>z(p)/2$. This is an open neighborhood of $p$. The indexed family $(W_p)_{p\in K}$ covers $K$; F4 gives finitely many centers $p_1,\ldots,p_r$ whose neighborhoods cover $K$. Set $m=\min_i h(p_i)/2$, $a=\min_i u(p_i)/2$ and $b=\min_i z(p_i)/2$. The finite list is nonempty and all its entries are positive. These constants give the three required uniform inequalities throughout $K$. [given, F4, step 2.1]

4.1 F4 supplies a finite compact chart cover inside $O$, with pieces in $K$ if desired. Now fix any cover allowed in the Statement, not necessarily that particular one. Each component function $f$ of either field is defined and continuous on $O\cap U_j$, which contains $K_j$. If $K_j$ is nonempty, cover it by the open neighborhoods on which $|f(q)|<|f(p)|+1$ for centers $p\in K_j$. A finite subcover from F4 bounds $|f|$ on $K_j$ by the maximum of the finitely many numbers $|f(p)|+1$. For empty pieces the bound is vacuous. Repeating this for the finitely many components in the finitely many specified charts proves the component conclusion. Step 3.1 proves the past-timelike conclusion on $K$, and step 3.2 proves the uniform margins, completing all the claims. [given, F4, step 1.1, step 3.1, step 3.2] ∎


## ADM section time and causal spatial speed

[Open item](item-lem-author-eb8e266b8b92-adm-time-speed) · level 2


### Statement

Assume the Axiom of Choice. Equip $E=\mathbb R_v\times S$, where $S$ is a connected smooth three-manifold, with the canonical product smooth structure. Let $h$ be a smooth Riemannian metric on $S$, $N>0$ a smooth function on $S$, and $X$ a smooth vector field on $S$, extended independently of $v$ using the product splitting. Give $g=-N^2dv^2+h(dx+Xdv,dx+Xdv)$ the time orientation of $n=N^{-1}(\partial_v-X)$. This is a smooth Lorentzian metric of signature $(-,+,+,+)$, and $n$ is its smooth unit timelike normal to the $v$-slices, declared future-directed. A causal curve means a locally absolutely continuous curve with nonzero causal velocity almost everywhere. Every future causal curve has strictly increasing $v$ and can be written as $(v,x(v))$ on its $v$-image. This representation is locally Lipschitz in charts, is future causal, and satisfies $|x'+X|_h\le N$ almost everywhere. In particular $|x'|_h\le N+|X|_h$ and $|(f\circ x)'|\le N|df|_h+|X(f)|$ for every smooth real $f$ on $S$. Here $|Y|_h=\sqrt{h(Y,Y)}$, $|df|_h:=|\operatorname{grad}_h f|_h$, where $h(\operatorname{grad}_h f,Y)=df(Y)$, and $X(f)=df(X)$ is the action of $X$ on $f$. Inextendibility as absence of an endpoint is preserved by this change of parameter.

### Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)

[math:thm-c1-lipschitz-ac-bv-hierarchy](https://alphabetamath.cc/item/thm-c1-lipschitz-ac-bv-hierarchy)

[math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function)

[math:def-pointwise-norm-and-angle-from-a-riemannian-metric](https://alphabetamath.cc/item/def-pointwise-norm-and-angle-from-a-riemannian-metric)

[math:def-action-of-a-vector-field-on-smooth-functions](https://alphabetamath.cc/item/def-action-of-a-vector-field-on-smooth-functions)

[math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)

[math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

### Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice implies Dependent Choice and Countable Choice, supplying the hypotheses of the causal-curve calculus and absolutely-continuous fundamental theorem used below. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F2] Causal curves are locally absolutely continuous, have nonzero future causal velocity almost everywhere, and inextendibility means absence of a limit at a parameter end. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F3] A lapse and shift decompose the stationary vector as $\partial_v=Nn+X$ with $g(n,n)=-1$ and $X$ tangent to the spacelike slice. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F4] Smooth composition of a locally absolutely continuous curve is locally absolutely continuous and satisfies the chain rule almost everywhere; strictly increasing continuous changes of parameter preserve the endpoint criterion. [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[F5] An absolutely continuous real function is the integral of its almost-everywhere derivative; Lipschitz functions are absolutely continuous. [math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions) [math:thm-c1-lipschitz-ac-bv-hierarchy](https://alphabetamath.cc/item/thm-c1-lipschitz-ac-bv-hierarchy)

[F6] On a compact coordinate ball, a smooth positive-definite metric bounds the Euclidean norm from below and above. [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

[F7] The canonical product charts give $E=\mathbb R\times S$ its smooth four-manifold structure and the splitting $T_{(v,p)}E=\mathbb R\partial_v\oplus T_pS$. [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[F8] The pointwise norm is $|Y|_h=\sqrt{h(Y,Y)}$, the gradient satisfies $df(Y)=h(\operatorname{grad}_h f,Y)$, and the vector-field action is $X(f)=df(X)$. Cauchy–Schwarz in the inner product $h_p$ gives $|df(Y)|\le|df|_h|Y|_h$ with the norm convention in the Statement. [math:def-pointwise-norm-and-angle-from-a-riemannian-metric](https://alphabetamath.cc/item/def-pointwise-norm-and-angle-from-a-riemannian-metric) [math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function) [math:def-action-of-a-vector-field-on-smooth-functions](https://alphabetamath.cc/item/def-action-of-a-vector-field-on-smooth-functions) [math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)

[F9] A Riemannian metric is a smooth symmetric covariant two-tensor that is positive definite on each tangent space. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[F10] A Lorentzian metric in four dimensions is a smooth symmetric nondegenerate covariant two-tensor of signature $(-,+,+,+)$. A time orientation is a smooth timelike vector field $n$; a nonzero causal vector $Y$ is future-directed exactly when $g(Y,n)<0$. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

### Proof

1.1 In the product splitting, the map $(a,W)\mapsto(a,W+aX)$ is invertible and carries the quadratic form of $g$ to $-N^2a^2+h(W,W)$. Smoothness, $N>0$ and positive definiteness of $h$ therefore make $g$ smooth and Lorentzian of the asserted signature. Direct substitution gives $g(n,n)=-1$ and $g(n,W)=0$ for spatial $W$, while the restriction to each slice is $h$; hence $n$ is the asserted smooth unit normal. For a nonzero future causal vector $Y=a\partial_v+W$, its pairing with $n$ is $-Na<0$, so $a>0$. The metric identity gives $|W+aX|_h\le Na$. Applied almost everywhere to the original curve parameter $s$, these identities give $v_s>0$ and the coordinate estimate $|x_s|_{\mathrm e}\le Bv_s$ on any relatively compact coordinate neighborhood, for some finite $B$. The bound follows from smoothness of $N,X,h$ and the metric comparison. [F2, F3, F6, F7, F9, F10, algebra]

2.1 Integrating $v_s>0$ on any nondegenerate compact parameter interval shows that $v$ is strictly increasing. It therefore has a continuous inverse on its image interval. To justify the required vector estimate using scalar integration, let $z:[a,b]\to\mathbb R^3$ have absolutely continuous coordinates, let $w:[a,b]\to\mathbb R$ be absolutely continuous with $w_s\ge0$ almost everywhere, and suppose $|z_s|_H\le Cw_s$ almost everywhere for a fixed inner product $H$ and constant $C\ge0$. Put $D=z(b)-z(a)$. If $D\ne0$, fix $e=D/|D|_H$ and the real function $\phi(s)=H(e,z(s))$. This fixed linear combination of coordinates is absolutely continuous, and $\phi_s=H(e,z_s)$ almost everywhere. The scalar fundamental theorem makes $\phi_s,w_s$ integrable; Cauchy–Schwarz gives $\phi_s\le Cw_s$. Consequently $|D|_H=\phi(b)-\phi(a)=\int_a^b\phi_s\,ds\le C\int_a^b w_s\,ds=C(w(b)-w(a))$. If $D=0$, the same bound follows from $w(b)\ge w(a)$. On each compact chart subarc apply this estimate with $z=x$, $w=v$, $H$ the Euclidean inner product and $C=B$, obtaining $|x(s_2)-x(s_1)|_{\mathrm e}\le B(v(s_2)-v(s_1))$. Thus $x$ as a function of $v$ is locally Lipschitz; each coordinate is therefore locally absolutely continuous. This argument does not assume absolute continuity of the inverse of $v$. [F1, F4, F5, F8, step 1.1, algebra]

3.1 At an interior differentiability point $v_0$ of $x(v)$, put $p=x(v_0)$ and, in a spatial chart, freeze $H=h_p$, $N_0=N(p)$ and $c=X(p)$, identifying coordinate tangent vectors with $\mathbb R^3$. On a sufficiently short subarc about $p$, continuity of the coefficients and the coordinate speed bound imply $|x_s+v_sc|_H\le(N_0+\epsilon)v_s$ almost everywhere, where $\epsilon\to0$ as the subarc shrinks. On each compact subarc the coordinates of $z(s)=x(s)+v(s)c$ are absolutely continuous, since they are fixed linear combinations of the original absolutely continuous coordinates. Their derivatives and $v_s$ are integrable by the scalar fundamental theorem. Apply the scalar-projection estimate proved in step 2.1 with this $z$, $w=v$, the fixed inner product $H$ and $C=N_0+\epsilon$; it yields $|x(s_2)-x(s_1)+(v(s_2)-v(s_1))c|_H\le(N_0+\epsilon)(v(s_2)-v(s_1))$. Take one endpoint at $v_0$, divide by the positive increase of $v$, and shrink the subarc to $v_0$. The differentiability of $x(v)$ gives $|x_v(v_0)+X(p)|_{h_p}\le N(p)$. By local Lipschitz continuity and the scalar fundamental theorem applied to the three coordinates, such differentiability points have full measure in the $v$-interval. Hence $|x_v+X|_h\le N$ almost everywhere. Its time component is one, so the reparametrized velocity is nonzero future causal. This proves the reparametrized causal inequality. [F1, F4, F5, F6, F8, step 1.1, step 2.1, algebra]

4.1 The triangle inequality gives $|x_v|_h\le N+|X|_h$. For a smooth real $f$, the smooth-composition chain rule gives $(f\circ x)'=df(x_v)=df(x_v+X)-X(f)$ almost everywhere. Applying the gradient identity and Cauchy–Schwarz of [F8] to $x_v+X$ yields $|(f\circ x)'|\le|df|_h|x_v+X|_h+|X(f)|\le N|df|_h+|X(f)|$. Finally the increasing homeomorphism of parameter intervals preserves all endpoint limits in either direction, proving the inextendibility assertion. [F4, F8, step 2.1, step 3.1, algebra] ∎


## Temporal normal angle and compact positive-height portions

[Open item](item-def-author-fd2999663761-temporal-angle-data) · level 2


### Definition

Work in ZFC on a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$. Let $g$ be its metric and $\Sigma$ a smooth embedded spacelike maximal hypersurface, smooth up to its actual boundary $\partial\Sigma$, with future unit normal $n$. Maximal means its induced mean curvature vanishes.

Fix a compact ambient set $Q$, allowed to be empty, and let $\tau$ be a smooth real function on an open neighborhood of $\Sigma\cup Q$. A compact positive-height portion is the entire set $P=\Sigma\cap\{\tau\ge0\}$, assumed compact and contained in $Q$; it is not a clipping of $\Sigma$ by $Q$. Require the metric gradient of $\tau$ to be past-directed timelike on an open neighborhood of $P$. On that temporal neighborhood put $\alpha=\sqrt{-g^{-1}(d\tau,d\tau)}>0$ and $V=-\alpha^{-1}\operatorname{grad}_g\tau$, where $\operatorname{grad}_g\tau$ is characterized by $g(\operatorname{grad}_g\tau,Y)=d\tau(Y)$ for every ambient tangent vector $Y$. Along the hypersurface in that neighborhood put $v=-g(n,V)$. Thus $V$ is future unit timelike and $v$ is the temporal normal angle.

Write $h=g|_{T\Sigma}$. For a real function $f$ smooth on an open subset of $\Sigma$, smooth up to any actual boundary there, write $\nabla_\Sigma f=\operatorname{grad}_h f$ and $\Delta_\Sigma f=\operatorname{div}_h(\nabla_\Sigma f)$ for the positive-trace Laplacian. If $f$ is an ambient function, these operators act on its restriction to $\Sigma$. At actual boundary points use the smooth one-sided extensions of these local operators.

Fix an arbitrary real exponent $\mu>0$. For nonempty $Q$ set $T=\max_{q\in Q}\max\{\tau(q),0\}$, and for empty $Q$ set $T=0$. Set $B=\sup_{\partial\Sigma\cap\{\tau>0\}}\tau^\mu v$, with the supremum zero for an empty set. At positive height only the actual hypersurface boundary contributes a boundary term.

### Definition references

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function)

[math:def-riemannian-divergence](https://alphabetamath.cc/item/def-riemannian-divergence)

[math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)

[math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

### Justification

The normal and induced metric are those of the spacelike hypersurface interface; the temporal orientation is that of the causal interface. The inverse metric and metric dual of $d\tau$ have the musical-isomorphism convention. Dividing a past timelike gradient by its positive Lorentzian norm and reversing its sign gives a future unit timelike $V$. In a Lorentz-orthonormal frame with time axis $V$, the unit equation for the future $n$ gives $v=\sqrt{1+|n^{\mathrm{space}}|^2}\ge1$.

The Riemannian gradient and divergence suppliers define the two intrinsic operators. The Laplace–Beltrami supplier identifies their composition with the positive metric trace of the Hessian and supplies the stated one-sided boundary convention. The gradient's inverse-metric formula also extends smoothly in boundary half-charts, since $h$ stays positive definite and $f$ is smooth up to the boundary; its values there are determined by its values in the interior.

For nonempty $Q$, the continuous function $q\mapsto\max\{\tau(q),0\}$ attains a finite maximum by the compactness supplier's extreme-value assertion. If $Q$ is empty, so is $P$, and the explicit convention defines $T$. On nonempty compact $P$, smoothness up to the actual boundary makes $v$ continuous and bounded for each individual hypersurface, again by that extreme-value assertion. Since $\mu>0$, the weight $\tau^\mu$ is continuous on $P$, with value zero at zero height, and $0\le\tau\le T$ there. Thus the actual boundary supremum is finite, and its empty-set convention covers empty $P$ as well. No uniform bound along a sequence is assumed.


## Ground-state identity, spectral ordering and eigenspace uniqueness

[Open item](item-lem-author-1a44964f66ee-ground-state-identity) · level 2


### Statement

For $L$ on $(S,h)$ as in the formal-adjoint lemma, suppose $L\phi=\lambda\phi$ and $L^\dagger\chi=\lambda\chi$ with $\lambda\in\mathbb C$ and smooth positive real $\phi,\chi$. Define $P w=\phi^{-1}(L-\lambda)(\phi w)$ and $m=\phi\chi$. Then $P=-\Delta_h+2(t-\nabla\log\phi)\cdot\nabla$, $\int_Sm Pw\,d\mu_h=0$, and $P|w|^2=2\operatorname{Re}(\overline w Pw)-2|\nabla w|^2$ for complex smooth $w$. If $S$ is nonempty, then $\lambda$ is necessarily real and every smooth eigenpair $L\psi=\mu\psi$, $\psi\not\equiv0$, satisfies $\operatorname{Re}\mu\ge\lambda$. On such nonempty $S$, the eigenspace at $\lambda$ is exactly the complex span of $\phi$; in particular the positive real eigenfunction is unique up to a positive constant. If $S=\varnothing$, the displayed differential and integral identities hold trivially, the eigenspace at $\lambda$ and the complex span of $\phi$ both equal $\{0\}$, and there is no nonzero eigenfunction; $\lambda$ need not be real.

### Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The formal-adjoint lemma fixes the real-coefficient operator, positive density integral and adjoint identity. On nonempty $S$ with real eigenvalues, the positive-adjoint-pairing lemma identifies the eigenvalues of a positive right eigenfunction and a positive adjoint eigenfunction, and supplies smooth bounded reciprocals of both. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint) [lem-author-1a44964f66ee-positive-adjoint-pairing](item-lem-author-1a44964f66ee-positive-adjoint-pairing)

[F2] A smooth real-valued function with zero differential is constant on each connected component of its smooth manifold. [math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component](https://alphabetamath.cc/item/prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component)

[F3] For the complex vector space $V=C^\infty(S;\mathbb C)$ and the complex-linear endomorphism $L:V\to V$, the eigenspace at any scalar $\lambda$ is $E_\lambda(L)=\ker(L-\lambda I_V)=\{u\in V:Lu=\lambda u\}$. This definition also applies to the zero vector space. [math:def-eigenvalue-eigenvector-eigenspace-and-spectrum](https://alphabetamath.cc/item/def-eigenvalue-eigenvector-eigenspace-and-spectrum)

[F4] Work in ZFC, including the Axiom of Choice. Choice supplies the countable-choice hypotheses for density integration and the chart-subordinate partitions of unity used by the formal-adjoint lemma. Its adjoint integral identity and strict positivity of the density integral are invoked here under those same assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)

### Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The formal-adjoint lemma fixes the real-coefficient operator, positive density integral and adjoint identity. On nonempty $S$ with real eigenvalues, the positive-adjoint-pairing lemma identifies the eigenvalues of a positive right eigenfunction and a positive adjoint eigenfunction, and supplies smooth bounded reciprocals of both. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint) [lem-author-1a44964f66ee-positive-adjoint-pairing](item-lem-author-1a44964f66ee-positive-adjoint-pairing)

[F2] A smooth real-valued function with zero differential is constant on each connected component of its smooth manifold. [math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component](https://alphabetamath.cc/item/prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component)

[F3] For the complex vector space $V=C^\infty(S;\mathbb C)$ and the complex-linear endomorphism $L:V\to V$, the eigenspace at any scalar $\lambda$ is $E_\lambda(L)=\ker(L-\lambda I_V)=\{u\in V:Lu=\lambda u\}$. This definition also applies to the zero vector space. [math:def-eigenvalue-eigenvector-eigenspace-and-spectrum](https://alphabetamath.cc/item/def-eigenvalue-eigenvector-eigenspace-and-spectrum)

[F4] Work in ZFC, including the Axiom of Choice. Choice supplies the countable-choice hypotheses for density integration and the chart-subordinate partitions of unity used by the formal-adjoint lemma. Its adjoint integral identity and strict positivity of the density integral are invoked here under those same assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)



**Proof technique:** direct.

1.1 If $S=\varnothing$, then $C^\infty(S;\mathbb C)=\{0\}$: every smooth function is the unique empty function. The differential operators, products and integrals in the Statement are zero, so the identities and eigenspace description hold, with no nonzero eigenfunction and no restriction on $\lambda$. This settles the empty case. Henceforth assume $S$ is nonempty. Since $L$ has real coefficients and $\phi$ is real, $L\phi$ is real valued. At any $p\in S$, the eigenvalue equation and $\phi(p)>0$ give $\lambda=(L\phi)(p)/\phi(p)\in\mathbb R$. Both eigenvalue parameters in the positive-adjoint-pairing lemma are therefore this same real $\lambda$, and all its nonempty closed-manifold and positive-function hypotheses hold. Its reciprocal conclusion makes division by $\phi$ smooth and bounded. [given, F1, F3]

2.1 Expand $\Delta_h(\phi w)=\phi\Delta_hw+2\nabla\phi\cdot\nabla w+w\Delta_h\phi$. The zeroth-order terms cancel by $L\phi=\lambda\phi$, giving the displayed $P$ with $\nabla\log\phi=\phi^{-1}\nabla\phi$. For any smooth complex $w$, integration by parts gives $\int_Sm Pw=\int_S\chi(L-\lambda)(\phi w)=\int_S(L^\dagger-\lambda)\chi\,\phi w=0$. All these operations are valid for complex functions by applying the real identity to their real and imaginary parts. [F1, F4, step 1.1]

3.1 The product rule gives $P|w|^2=2\operatorname{Re}(\overline w Pw)-2|\nabla w|^2$. For $w=\psi/\phi$, the eigenvalue equation becomes $Pw=(\mu-\lambda)w$. Integrating this product identity against $m>0$ and using step 2.1 yields $(\operatorname{Re}\mu-\lambda)\int_Sm|w|^2=\int_Sm|\nabla w|^2\ge0$. The denominator is positive, proving the spectral ordering. If $\mu=\lambda$, the last integral is zero, so every component of $\nabla w$ vanishes everywhere. Applying F2 separately to the smooth real functions $\operatorname{Re}w$ and $\operatorname{Im}w$, whose differentials vanish, shows that both are constant on connected $S$; hence $w$ is constant. Conversely every constant multiple of $\phi$, including zero, satisfies $L\psi=\lambda\psi$ and belongs to the eigenspace; its nonzero multiples are eigenfunctions. Thus the eigenspace at $\lambda$ is exactly the complex span of $\phi$. [F1, F2, F3, F4, step 1.1, step 2.1]

4.1 Let $u$ be any smooth everywhere positive real eigenfunction with $Lu=\nu u$, initially allowing $\nu\in\mathbb C$. On the nonempty $S$ now under consideration, evaluate at any $p\in S$: real coefficients and $u(p)>0$ give $\nu=(Lu)(p)/u(p)\in\mathbb R$. Apply the positive-adjoint-pairing lemma to the right eigenfunction $u$ at $\nu$ and the adjoint eigenfunction $\chi$ at the real eigenvalue $\lambda$ from step 1.1. The same nonempty closed manifold and operator are used, both functions are smooth and positive, and both eigenvalues are real; hence $\nu=\lambda$. Step 3.1 gives $u=a\phi$ for a complex constant $a$, and evaluating at $p$ gives $a=u(p)/\phi(p)>0$. This proves uniqueness among all positive real eigenfunctions, even when their eigenvalues were initially allowed to differ, and completes the Statement without a selfadjointness assumption on $L$. [F1, F3, step 1.1, step 3.1] ∎


## Nonnegative supersolutions detect the principal spectral sign

[Open item](item-lem-author-1a44964f66ee-spectral-sign-test) · level 2


### Statement

Let $(S,h)$ be a nonempty connected compact smooth Riemannian manifold without boundary, of positive dimension. Let $t$ be a smooth real vector field and $c$ a smooth real function on $S$. Put $Lu=-\Delta_hu+2\langle t,\nabla u\rangle_h+cu$, where $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. Use the positive Riemannian density $d\mu_h$ and the formal adjoint $L^\dagger u=-\Delta_hu-2\langle t,\nabla u\rangle_h+(c-2\operatorname{div}_ht)u$ for the pairing $\langle f,g\rangle=\int_S\overline f g\,d\mu_h$.

Assume smooth real functions $\phi>0$ and $\chi>0$ satisfy $L\phi=\lambda\phi$ and $L^\dagger\chi=\lambda\chi$ for a real constant $\lambda$. Then $\lambda\ge0$ if and only if there is a smooth real $\psi\ge0$, $\psi\not\equiv0$, with $L\psi\ge0$ pointwise. The strict variant $\lambda>0$ is equivalent to existence of such a $\psi$ with $L\psi$ additionally positive somewhere. Thus a nonnegative test function suffices; it is not necessary to assume the test is everywhere positive.

### Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] For the operator, manifold and density in the Statement, the formal-adjoint identity is $\int_S f Lg\,d\mu_h=\int_S(L^\dagger f)g\,d\mu_h$ for smooth real $f,g$. The operators have smooth real coefficients and map smooth real functions to smooth real functions. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)

[F2] Positive right and adjoint eigenfunctions at real eigenvalues have the same eigenvalue; the Statement denotes this common value by $\lambda$. [lem-author-1a44964f66ee-positive-adjoint-pairing](item-lem-author-1a44964f66ee-positive-adjoint-pairing)

[F3] Compactly supported smooth density integration is linear, nonnegative on nonnegative densities and strictly positive on any nonzero nonnegative density, without an orientation assumption. Every smooth density on compact $S$ has compact support, so this applies to the density products below. The stated ZFC assumption includes AC; applying AC to countable families gives the countable-choice hypothesis $\mathrm{AC}_\omega$ required for this integration theorem. [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F4] Smooth real-valued maps on smooth manifolds are continuous; apply this to $\psi$ and the smooth function $L\psi$. [math:prop-smooth-maps-are-continuous](https://alphabetamath.cc/item/prop-smooth-maps-are-continuous)

### Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] For the operator, manifold and density in the Statement, the formal-adjoint identity is $\int_S f Lg\,d\mu_h=\int_S(L^\dagger f)g\,d\mu_h$ for smooth real $f,g$. The operators have smooth real coefficients and map smooth real functions to smooth real functions. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint)

[F2] Positive right and adjoint eigenfunctions at real eigenvalues have the same eigenvalue; the Statement denotes this common value by $\lambda$. [lem-author-1a44964f66ee-positive-adjoint-pairing](item-lem-author-1a44964f66ee-positive-adjoint-pairing)

[F3] Compactly supported smooth density integration is linear, nonnegative on nonnegative densities and strictly positive on any nonzero nonnegative density, without an orientation assumption. Every smooth density on compact $S$ has compact support, so this applies to the density products below. The stated ZFC assumption includes AC; applying AC to countable families gives the countable-choice hypothesis $\mathrm{AC}_\omega$ required for this integration theorem. [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F4] Smooth real-valued maps on smooth manifolds are continuous; apply this to $\psi$ and the smooth function $L\psi$. [math:prop-smooth-maps-are-continuous](https://alphabetamath.cc/item/prop-smooth-maps-are-continuous)

**Proof technique:** direct.

1.1 If $\lambda\ge0$, take $\psi=\phi$. Then $\psi$ is smooth, everywhere positive and nonzero because $S$ is nonempty, and $L\psi=\lambda\phi\ge0$. If $\lambda>0$, this is positive everywhere. This proves both forward implications. [given]

2.1 Conversely, let $\psi$ be a smooth real nonzero nonnegative function with $L\psi\ge0$. Adjoint integration gives $\int_S\chi L\psi\,d\mu_h=\int_S(L^\dagger\chi)\psi\,d\mu_h=\lambda\int_S\chi\psi\,d\mu_h$. The last integral is strictly positive: continuity and nonzero nonnegativity of $\psi$ give a nonempty open set where $\psi>0$, and $\chi$ is everywhere positive, so $\chi\psi\,d\mu_h$ is a nonzero nonnegative smooth density. The left side is nonnegative, hence $\lambda\ge0$. If $L\psi$ is positive at one point, its smoothness makes it positive on a nonempty open set. Then $\chi L\psi\,d\mu_h$ is also a nonzero nonnegative smooth density, so the left side is strictly positive and $\lambda>0$. Together with step 1.1 this proves both equivalences. [given, F1, F2, F3, F4, step 1.1] ∎


## Outgoing expansion variation at a general MOTS

[Open item](item-lem-author-97780c2fed82-mots-variation-second-jet) · level 2


### Statement

Assume Countable Choice $\mathrm{AC}_\omega$. At a MOTS with the general spacelike-surface data and fixed base outgoing normal $\ell$, for any smooth normal velocity $X$ define $\delta_X\theta_{(\ell)}=\left.\partial_t\right|_0\Phi_t^*(\theta_{(\ell_t)})$ using a smooth deformation and null gauge as in the normal-deformation lemma. This derivative is independent of the chosen deformation and of the parameter-dependent null gauge having this same base $\ell$ and outgoing ray. As a function of $X$ it is a real linear differential operator of order at most two. This states well-definedness, not its curvature-coefficient formula.

### Statement references

[def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data)

[lem-author-97780c2fed82-normal-deformation-families](item-lem-author-97780c2fed82-normal-deformation-families)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

### Facts & Assumptions

[A1] Countable Choice is assumed, as required by the general surface data and the deformation-existence supplier. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F1] The general surface data supply the smooth metric connection, ambient future timelike field $N$, ambient and surface orientations, and the smooth null pair. The expansion is the $q$-trace of $g(\nabla\ell,\cdot)$. Metric compatibility is assumed; torsion freedom is not. [def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data)

[F2] Under Countable Choice, every smooth normal velocity has an actual smooth family of spacelike embeddings and a smooth outgoing null gauge with the prescribed initial pair. Only this existence assertion is imported; the first-jet dependence needed below is proved locally. [lem-author-97780c2fed82-normal-deformation-families](item-lem-author-97780c2fed82-normal-deformation-families) [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

### Proof

**Given:** The objects and hypotheses in the Statement, including Countable Choice.

**Goal:** Establish the stated well-definedness and linear differential-operator conclusion.

1.1 Choose a deformation from [F2]. On a positive surface chart set $E_A=\partial_A\Phi_t$ and $q_{AB}=g(E_A,E_B)$. Define $U_t=N-q^{AB}g(N,E_A)E_B$, evaluating ambient fields at $\Phi_t(p)$. This is normal to the surface and satisfies $g(U_t,U_t)=g(N,N)-q^{AB}g(N,E_A)g(N,E_B)<0$ and $g(U_t,N)=g(U_t,U_t)<0$. Hence $n_t=U_t/\sqrt{-g(U_t,U_t)}$ is a future unit normal. The projection is independent of the surface coordinates, and its formula is smooth in $\Phi_t$ and its first surface derivatives. [A1, F1, F2]

2.1 Write the metric volume form in a positive spacetime chart as $\operatorname{vol}_g=\sqrt{-\det(g_{ab})}\,dx^0\wedge dx^1\wedge dx^2\wedge dx^3$. Define $w_t(v)=\operatorname{vol}_g(n_t,E_1,E_2,v)/\sqrt{\det(q_{AB})}$ and let $\widetilde\nu_t$ be the unique vector with $g(\widetilde\nu_t,v)=w_t(v)$ for every ambient tangent vector $v$. The covector $w_t$ annihilates $n_t,E_1,E_2$. In an orthonormal basis consisting of $n_t$, an oriented orthonormal tangent pair, and a unit vector in their spacelike orthogonal complement, $w_t$ evaluates to $1$ or $-1$ on the last vector. Thus $\widetilde\nu_t$ is a unit spacelike normal orthogonal to $n_t$. Under a positive surface-coordinate change both the numerator and $\sqrt{\det q}$ acquire the same positive Jacobian factor, so these formulas glue. Choose the locally constant sign $\sigma:S\to\{1,-1\}$ so that $n_0+\sigma\widetilde\nu_0$ has the ray of $\ell$, and put $\nu_t=\sigma\widetilde\nu_t$. Such a smooth sign exists because the supplied smooth outgoing ray selects one of the two distinct null rays in each normal plane. The formulas use only the embedding and its first surface derivatives, with nonzero denominators $\det q$, $\sqrt{-g(U_t,U_t)}$ and the nondegenerate metric matrix. [F1, step 1.1]

3.1 Put $a(p)=-g(\ell,n_0)>0$. Decomposing the initial null pair in the orthonormal normal basis $(n_0,\nu_0)$ gives $\ell=a(n_0+\nu_0)$ and $k=a^{-1}(n_0-\nu_0)/2$. Holding $a$ and $\sigma$ fixed in $t$, set $\ell_t=a(n_t+\nu_t)$ and $k_t=a^{-1}(n_t-\nu_t)/2$. This is a smooth future null pair with $g(\ell_t,k_t)=-1$ and the required initial values. Its outgoing branch is fixed by continuity from $t=0$, after shrinking the parameter interval if needed. Any two deformations with the same initial embedding and base pair use the same $a$ and $\sigma$. This proves locally the required smooth first-jet gauge construction, without strengthening the cited supplier's interface. [F1, step 1.1, step 2.1]

4.1 In spacetime coordinates let $E_A^a=\partial_A\Phi^a$ and write $\nabla_{\partial_c}\partial_d=\Gamma^b{}_{cd}\partial_b$. Metric compatibility and differentiation of $g(\ell_t,E_B)=0$ along $E_A$ give $\theta_{(\ell_t)}=-q^{AB}g_{ab}(\Phi)\ell_t^a(\partial_A\partial_B\Phi^b+\Gamma^b{}_{cd}(\Phi)E_A^cE_B^d)$. This identity does not use symmetry of $\Gamma^b{}_{cd}$. With the gauge just constructed it is a smooth function of $\Phi$, its first and second surface derivatives, and the fixed base functions $a,\sigma$. No extension of $\ell_t$ off the surface is used. [F1, step 3.1]

5.1 Differentiate that finite expression once in $t$ at zero. Smoothness permits interchange with each surface-coordinate derivative, so the differentiated embedding variables are $X$, $\partial_AX$ and $\partial_A\partial_BX$. The ordinary chain rule expresses the result as a linear combination of these jets; its coefficients depend only on the initial embedding, fixed background fields and fixed base gauge. Therefore it is independent of all higher parameter derivatives of the deformation, and two deformation families with the same velocity give the same result in this gauge. Since expansion and pullback are scalars, the coordinate formulas agree before differentiation and hence afterward. This establishes a globally defined real linear differential operator on smooth normal fields of order at most two for the constructed gauge. [F1, step 3.1, step 4.1]

6.1 On any fixed deformed surface, another smooth future null normal in the same outgoing ray is $h_t\ell_t$ for a smooth positive function $h_t$; the same base normal means $h_0=1$. The product rule for the connection and tangential orthogonality give $\theta_{(h_t\ell_t)}=h_t\theta_{(\ell_t)}$, because the derivative of $h_t$ multiplies $g(\ell_t,E_B)=0$. Differentiation at zero adds only $(\partial_th_t)|_0\theta_{(\ell)}=0$ at the MOTS. Thus each deformation's arbitrary allowed gauge gives the derivative of its constructed gauge, and step 5.1 then compares any two deformations. The well-definedness and linear second-order conclusion follow for all the gauges in the Statement. The zero-expansion hypothesis is essential to this last gauge assertion. [F1, step 5.1] ∎


## Strong minimum principle from the annular barrier

[Open item](item-lem-author-58255dfd955f-strong-minimum) · level 3


### Statement

On a connected smooth Riemannian interior, let $V\ge0$ be locally bounded and smooth. A nonnegative $C^2$ function satisfying $(\Delta_h-V)u\le0$ is either strictly positive everywhere or identically zero.

### Facts & Assumptions

[F1] The interior, denoted by $M$, has the smooth positive-definite metric of [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold). Work in interior charts; all closed coordinate balls used below are compactly contained in such a chart.

[F2] Use the positive-divergence sign convention and metric trace of the Hessian from [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian). For smooth functions the coordinate Hessian is $(\operatorname{Hess}f)_{ij}=\partial_{ij}f-\Gamma^k{}_{ij}\partial_kf$ by [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas). For $C^2$ functions use the same pointwise trace; step 1.1 justifies this extension and its coordinate expression. Repeated indices are summed.

[F3] A connected space has no nonempty proper clopen subset by [math:thm-connectedness-characterisations](https://alphabetamath.cc/item/thm-connectedness-characterisations), part 1(b). Continuity of $u$ makes $P=\{u>0\}$ open and $Z=\{u=0\}$ closed; nonnegativity gives $M=P\cup Z$.

[F4] The general metric-chart interface of [lem-author-58255dfd955f-annular-hopf-barrier](item-lem-author-58255dfd955f-annular-hopf-barrier) gives a strictly positive inward derivative at a zero on an interior tangent Euclidean ball when $u>0$ inside, $u\ge0$ on the closure, $Lu\le0$, and $u$ is $C^2$ inside and $C^1$ at the tangency point, for $L=\Delta_h-V$ with bounded coefficients and uniformly elliptic principal part on that chart and $V\ge0$.

[F5] For Euclidean dimension $m\ge1$, [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn), part 2, identifies compact subsets of $\mathbb R^m$ with closed bounded subsets. We apply it in dimensions $n$ and $2n$ only after disposing of dimension zero.

[F6] By [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric), a continuous real-valued function on a nonempty compact metric space is bounded and attains its minimum and maximum. In particular, a strictly positive continuous function on such a space has a strictly positive attained minimum.

### Proof

**Given:** The hypotheses in the Statement and the mathematical inputs [F1]–[F6].

**Goal:** Establish the stated alternative without restricting the Riemannian interior to an exterior.

**Proof technique:** direct.

1.1 If $M$ is empty the alternative is vacuous. If $n=\dim M=0$, each chart is a singleton open set because $\mathbb R^0$ is a singleton; hence $M$ is discrete. Every singleton is then clopen, so connectedness and [F3] force a nonempty $M$ to be a singleton. The alternative follows from nonnegativity at its sole point. In the remaining argument $n\ge1$. At any point $x_0$ of an interior chart, replace $u$ by its quadratic Taylor polynomial with the same value, first derivatives and second derivatives at $x_0$. The smooth Hessian formula in [F2] uses only these data and the metric connection coefficients at $x_0$. Under a smooth change of coordinates, the chain rule transforms the derivatives through order two using only these same data, so the Hessian coefficients defined for $u$ transform as those of the polynomial, hence as a bilinear tensor at $x_0$. This proves that their metric trace is well-defined for $u\in C^2$ and gives $\Delta_hu=h^{ij}\partial_{ij}u-h^{ij}\Gamma^k{}_{ij}\partial_ku$. Thus $a^{ij}=h^{ij}$ and $b^k=-h^{ij}\Gamma^k{}_{ij}$ are smooth on the chart. For any nonempty compact chart subset $K$, its coordinate image is closed and bounded by [F5]. Thus $K\times\{\xi\in\mathbb R^n:|\xi|=1\}$, in coordinates, is a nonempty closed bounded subset of $\mathbb R^{2n}$ and is compact by [F5]. The continuous strictly positive function $(x,\xi)\mapsto h^{ij}(x)\xi_i\xi_j$ has a strictly positive attained minimum there by [F6]. Scaling $\xi$ gives uniform ellipticity on $K$. Applying [F6] on $K$ to the absolute values of each of the finitely many smooth coefficients and of $V$ gives finite coefficient and potential bounds. For empty $K$ these bounds are vacuous. These are exactly the metric-chart coefficient conditions in [F4]. [F1, F2, F3, F4, F5, F6, given, algebra]

1.2 Suppose $P$ and $Z$ are both nonempty. If $\overline P\cap Z$ were empty, then $\overline P\subseteq P$, so the open set $P$ would also be closed. It would be a nonempty proper clopen subset of the connected space $M$, contradicting [F3]. Consequently choose $q\in\overline P\cap Z$. [F3, given, choose]

2.1 Center coordinates at $q$ and choose $\rho>0$ such that the closed Euclidean ball $\overline B_{2\rho}(0)$ is contained in the chart image. Choose $z\in P$ with $|z|<\rho/4$, which is possible since $q\in\overline P$. The set $E=Z\cap\overline B_\rho(0)$ in these coordinates contains $0$ and is closed and bounded in $\mathbb R^n$: it is the zero set of the continuous coordinate function $u$ restricted to the closed ball, which lies in the chart. Thus $E$ is nonempty and compact by [F5]. The continuous function $x\mapsto|x-z|$ on $E$ attains its minimum $R$ at some $p\in E$ by [F6]. Since $p\in Z$ and $z\notin Z$, $R=|p-z|>0$; since $0\in E$, $R\le|z|<\rho/4$. Thus $\overline B_R(z)\subset B_{\rho/2}(0)$, and its open ball contains no point of $Z$, so it lies in $P$. Its closure lies in the interior chart and $p$ is a zero on its sphere. [F1, F3, F5, F6, step 1.2, choose]

3.1 On this ball, step 1.1 verifies the operator hypotheses of [F4]. All its function hypotheses hold because $u$ is nonnegative and $C^2$ throughout the interior, positive in the ball by step 2.1, zero at $p$, and satisfies $(\Delta_h-V)u\le0$. The barrier therefore gives $\partial_vu(p)>0$ for $v=(z-p)/R$. But $p$ is an interior minimum of $u$, so the differentiable function $g(t)=u(p+tv)$ has a minimum at $0$ for both signs of small $t$. For $t>0$ its difference quotient $(g(t)-g(0))/t$ is nonnegative, and for $t<0$ it is nonpositive. Both one-sided limits equal $g'(0)$ by differentiability, so $g'(0)\ge0$ and $g'(0)\le0$, hence $\partial_vu(p)=g'(0)=0$. The contradiction excludes simultaneous nonempty $P,Z$. If $P$ is empty then $u\equiv0$; if $Z$ is empty then $u>0$ everywhere. These alternatives also cover the empty interior. [F4, step 1.1, step 2.1, given] ∎


## Hopf positivity and uniform linear growth on a fixed compact collar

[Open item](item-lem-author-58255dfd955f-boundary-linear-growth) · level 3


### Statement

Let $S$ be a nonempty compact smooth boundary of a smooth Riemannian exterior. Suppose $u\in C^2(\Sigma^\circ)\cap C^1_{\mathrm{loc}}(\Sigma)$ is positive inside, vanishes on $S$, and satisfies $(\Delta_h-V)u\le0$ with smooth $V\ge0$. Then $\partial_{\nu_{\mathrm{in}}}u>0$ at every point of $S$, where $\nu_{\mathrm{in}}$ is the metric unit inward normal. On some fixed compact collar, $u\ge c_0\rho$ with $c_0>0$, for the collar coordinate $\rho$ or the metric distance to $S$.

### Facts & Assumptions

[F1] Smooth boundary, the Riemannian metric and the Laplacian convention are those of [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data). The inward unit normal is the vector orthogonal to $T_yS$, of $h$-norm one, pointing into $\Sigma$. The regularity $C^1_{\mathrm{loc}}(\Sigma)$ includes continuous first derivatives up to the boundary in boundary charts.

[F2] The tangent-ball derivative conclusion is supplied by [lem-author-58255dfd955f-annular-hopf-barrier](item-lem-author-58255dfd955f-annular-hopf-barrier). Smoothness of the metric and potential on a sufficiently small closed chart ball gives its coefficient bounds and uniform ellipticity.

[F3] Work in ZFC, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) and the choice assumptions inherited through the barrier supplier. In particular the Countable Choice hypothesis of [math:thm-collar-neighborhood-theorem](https://alphabetamath.cc/item/thm-collar-neighborhood-theorem) holds. Fix its smooth collar $F:S\times[0,\epsilon)\to\Sigma$, a smooth embedding onto a relatively open neighbourhood of $S$ with $F(y,0)=y$. Its coordinate is $\rho(F(y,t))=t$. The vector $\partial_tF(y,0)$ is strictly inward and transverse, since $F$ is a collar embedding.

[F4] A continuous real function on a nonempty compact space attains its minimum and maximum, and a continuous image of a compact space is compact, by [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps). The interval $[0,\delta]$ is compact for $\delta>0$ by [math:lem-closed-interval-compactness-from-completeness](https://alphabetamath.cc/item/lem-closed-interval-compactness-from-completeness), and its product with compact $S$ is compact by [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces). Compactness also means that every open cover has a finite subcover; the common collar width will be obtained by that property directly.

[F5] The closed-interval mean value theorem [math:lem-mean-value-theorem-on-closed-interval](https://alphabetamath.cc/item/lem-mean-value-theorem-on-closed-interval) applies to a real function continuous on $[a,b]$ and differentiable on $(a,b)$. The supplier [math:lem-continuous-functions-riemann-integrable](https://alphabetamath.cc/item/lem-continuous-functions-riemann-integrable) defines the Riemann integral of continuous real functions on compact intervals, proves its interval additivity, and gives $m(b-a)\le\int_a^b g(s)\,ds\le M(b-a)$ whenever $m\le g\le M$ and $a<b$. These are used over the real numbers with the complete ordered-field structure of [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field).

[F6] For the distance formulation, curves are continuous maps $\gamma:[a,b]\to\Sigma$ that are $C^1$ on each piece of a finite subdivision $a=t_0<\cdots<t_N=b$, up to the piece endpoints in interior or boundary charts; endpoint derivatives are one-sided. They are allowed to lie on or meet $S$. Define $L_h(\gamma)=\sum_{j=1}^N\int_{t_{j-1}}^{t_j}\sqrt{h_{\gamma(s)}(\dot\gamma(s),\dot\gamma(s))}\,ds$. Each speed is continuous on its closed piece, so [F5] makes the length finite and nonnegative. At a subdivision point each adjacent piece uses its own one-sided derivative. Interval additivity gives invariance under refinement, and a common refinement gives independence of subdivision. For $a=b$, set $L_h(\gamma)=0$. Define $d_h(x,S)$ to be the infimum of $L_h(\gamma)$ over all these curves starting at any point of $S$ and ending at $x$, with $\inf\varnothing=+\infty$. A nonempty family of lengths has an infimum in $[0,\infty)$ by the completeness axiom in [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field), applied to the negatives of the nonnegative lengths. Thus this distance-to-subset construction applies to manifolds with boundary and disconnected exteriors, including components not joined to $S$; finiteness on the collar will follow from its explicit curves.

### Proof

**Given:** The hypotheses in the Statement and the data and suppliers in [F1]–[F6].

**Goal:** Establish the conclusions of the Statement.

**Proof technique:** direct.

1.1 In a boundary chart flatten the smooth boundary to a coordinate plane. A sufficiently small Euclidean ball in the half-space is tangent at the chosen boundary point and has closure in the chart. Apply [F2] to obtain a positive inward transverse derivative. All tangential derivatives vanish because $u|_S=0$. Its differential is therefore a positive multiple of the inward conormal, proving the strict positivity for the metric unit inward normal as well as for every smooth strictly inward transverse vector. [F1, F2, given]

2.1 Put $B(y,t)=\partial_t(u\circ F)(y,t)$ and $a(y)=B(y,0)$. These functions are continuous up to $t=0$, and $a(y)>0$ by step 1.1 and [F3]. Since $S$ is nonempty and compact, [F4] gives $a_*:=\min_Sa>0$. Fix $0<b<\epsilon$. For each $y\in S$, continuity of $B$ gives an open neighbourhood $U_y\subset S$ and a width $0<\eta_y<b$ such that $B(z,t)>a_*/2$ for $z\in U_y$ and $0\le t<\eta_y$. A finite subcover $U_{y_1},\ldots,U_{y_m}$ of $S$ exists by compactness. Choose $0<\delta<\min_i\eta_{y_i}$. Every $z\in S$ then lies in one of these sets, so $B(z,t)\ge a_*/2$ for all $0\le t\le\delta$. This proves the common width directly. [F3, F4, step 1.1, given, choose]

3.1 By [F4], $S\times[0,\delta]$ is compact and its continuous image $K_\delta:=F(S\times[0,\delta])$ is a compact collar. The speed $q(y,t):=\sqrt{h_{F(y,t)}(\partial_tF(y,t),\partial_tF(y,t))}$ is continuous there by smoothness of $h$ and $F$. Its maximum exists by [F4]; put $C:=\max(1,\max_{S\times[0,\delta]}q)$. Thus $0\le q\le C$ and $C\ge1$. [F1, F3, F4, step 2.1, construct]

3.2 For fixed $y$ and $0<t\le\delta$, the function $s\mapsto u(F(y,s))$ is continuous on $[0,t]$ and differentiable on $(0,t)$ with derivative $B(y,s)$. By [F5] there is $\theta\in(0,t)$ with $u(F(y,t))-u(F(y,0))=tB(y,\theta)\ge a_*t/2$. Since $u(F(y,0))=0$, this proves $u(F(y,t))\ge a_*t/2$; the same inequality holds at $t=0$. The closed-interval hypotheses include the boundary endpoint, so this argument uses exactly the stated regularity. [F3, F5, step 2.1, given]

4.1 For $x=F(y,t)$, $0\le t\le\delta$, the curve $s\mapsto F(y,s)$ on $[0,t]$ starts at $y\in S$, ends at $x$, and stays in $\Sigma$. Its length, as defined in [F6], is $\int_0^t q(y,s)\,ds\le Ct$ by [F5] and step 3.1. Hence $0\le d_h(x,S)\le Ct<\infty$. Combining this with step 3.2 yields $u(x)\ge (a_*/2C)d_h(x,S)$. With $c_0=a_*/(2C)>0$, the same constant also gives $u(x)\ge c_0\rho(x)$, since $C\ge1$ and $\rho(x)=t$. The constants depend on the actual solution and collar; no uniform family bound follows solely from pointwise Hopf positivity. [F3, F5, F6, step 3.1, step 3.2, algebra] ∎



## Positive anchor values and the limits of uniform Harnack propagation

[Open item](item-lem-author-58255dfd955f-anchored-uniform-positivity) · level 3


### Statement

Let a family of positive Schrödinger solutions have a common finite chain cover joining a compact interior set $K$ to an anchor point $x_*$, with common comparison constant $H$. If $u(x_*)\ge a>0$ uniformly, then $\inf_Ku\ge a/H$. A common limit $u\to c>0$ on the end supplies such an anchor if the end threshold giving, for example, $u\ge c/2$ is uniform in the family, with the comparison controls extending to the chosen anchor. A uniform end threshold is sufficient, but is not necessary for a uniform anchor. Individual end limits alone guarantee neither a fixed point with a positive uniform anchor value, nor a uniform end threshold, nor a uniform compact lower bound, even on a fixed Euclidean three-dimensional exterior with smooth nonnegative potentials uniformly bounded everywhere.

### Facts & Assumptions

[F1] The finite-chain comparison is the conditional part of [lem-author-58255dfd955f-compact-harnack-chain](item-lem-author-58255dfd955f-compact-harnack-chain): common local pairwise comparisons on the half-balls of a common finite connected chain cover give a common comparison constant on the covered set. For a connected compact $K$ and an anchor outside $K$, include a fixed path from $K$ to $x_*$ and cover its compact image together with $K$; a connected smooth manifold is path connected because chart balls are path connected and its path components are open. More generally, the assumed common connected chain cover must contain all of $K$ and $x_*$. The coefficient and cover controls, when used to obtain the local comparisons, must hold on this enlarged compact region. Below, the examples' local comparisons are proved directly; the supplier's ZFC analytic consequence is not invoked.

[F2] The exterior and Laplacian conventions are [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data). For the examples take $\Sigma=\mathbb R^3$ with its Euclidean metric and empty compact boundary; outside the closed unit ball this is the prescribed exterior chart. Here $\Delta u=\sum_{i=1}^3\partial_i^2u$. For a smooth positive $u$, define $V=\Delta u/u$, so $(\Delta-V)u=0$ pointwise. No boundary condition is assumed in this lemma.

[F3] Coordinatewise sum, product, quotient and chain differentiation use [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules). All functions differentiated below have strictly positive square-root arguments and denominators. Their potentials, signs, bounds and local comparisons are computed locally rather than imported from an external result.

### Proof

**Given:** The hypotheses in the Statement and [F1]–[F3].

**Goal:** Prove the anchor estimate and both distinctions concerning end normalization.

**Proof technique:** direct.

1.1 By [F1], $u(x_*)\le H u(x)$ for every $x\in K$. Insert $u(x_*)\ge a$ and take the infimum to obtain $\inf_Ku\ge a/H$. A common end threshold permits a single fixed $x_*$ beyond it, with $a=c/2$, provided the same comparison controls hold to this point. This proves the anchor estimate and the sufficiency assertion. [F1, given, algebra]

1.2 For $0<b<1$, $\lambda>0$ and $z\in\mathbb R^3$, put $Q(x)=1+\lambda^2|x-z|^2$ and $f(x)=1-bQ(x)^{-1/2}$. This is smooth and $f\ge1-b>0$. For $t>0$, rationalizing gives $(\sqrt{t+h}-\sqrt t)/h=1/(\sqrt{t+h}+\sqrt t)$ for nonzero sufficiently small $h$; the quotient rule then gives $(t^{-1/2})'=-1/(2t^{3/2})$. Repeated differentiation on $t>0$ gives smoothness. Applying [F3] coordinatewise yields $\partial_i f=b\lambda^2(x_i-z_i)Q^{-3/2}$ and $\partial_i^2 f=b\lambda^2Q^{-3/2}-3b\lambda^4(x_i-z_i)^2Q^{-5/2}$. Summing in [F2] yields $\Delta f=3b\lambda^2Q^{-5/2}$, hence $0\le V_f:=\Delta f/f\le3b\lambda^2/(1-b)$. For fixed parameters, $f\to1$ uniformly as $|x|\to\infty$, since $|x-z|\ge|x|-|z|$. [F2, F3, algebra]

2.1 To show that a uniform threshold is not necessary, let $e_1=(1,0,0)$ and, for integers $n\ge1$, set $w_n(x)=1-\frac34(1+|x-2ne_1|^2)^{-1/2}$. Step 1.2 gives positive smooth Schrödinger solutions with $0\le V_{w_n}\le9$, and each has end limit $1$. At the fixed anchor $0$, $w_n(0)\ge1-3/(4\sqrt5)>1/2$. Nevertheless $w_n(2ne_1)=1/4$, so no radius works for the inequality $w_n\ge1/2$ for every $n$ beyond that radius. The bounds $1/4\le w_n\le1$ give $w_n(x)\le4w_n(y)$ for all $x,y$, directly supplying common local comparisons on every fixed chain cover in [F1]. The Euclidean metric and the displayed potential bounds also give uniform coefficient controls there. Thus a common anchor can exist without the indicated uniform end threshold. [step 1.2, F1, algebra]

3.1 For $0<\varepsilon\le1/2$ set $u_\varepsilon(x)=1-(1-\varepsilon)(1+\varepsilon^2|x|^2)^{-1/2}$. Step 1.2 gives $u_\varepsilon\ge\varepsilon>0$, $u_\varepsilon\to1$ at infinity for each $\varepsilon$, and $0\le V_\varepsilon\le3\varepsilon(1-\varepsilon)\le3/4$ everywhere. The Euclidean metric and these potential bounds give uniform coefficient controls on every fixed finite compact chain cover. To check the local comparisons directly, write $s=(1+\varepsilon^2|x|^2)^{1/2}\ge1$. Then $u_\varepsilon(x)=\varepsilon+(1-\varepsilon)\varepsilon^2|x|^2/[s(s+1)]$. On $|x|\le R$ this implies $\varepsilon\le u_\varepsilon(x)\le\varepsilon(1+R^2/4)$, using $s(s+1)\ge2$ and $\varepsilon\le1/2$. Thus for all $x,y$ in this ball, $u_\varepsilon(x)\le(1+R^2/4)u_\varepsilon(y)$, uniformly in $\varepsilon$, and every fixed finite chart cover with compact closures fits into such a ball. For the closed unit ball $K$, $\inf_Ku_\varepsilon=u_\varepsilon(0)=\varepsilon\to0$. Moreover the same bound gives $u_\varepsilon(x)\to0$ at every fixed $x$, so there is no fixed point with a positive uniform anchor value. For any proposed common end radius $R_0$, fix $x$ with $|x|>R_0$; then $u_\varepsilon(x)<1/2$ for sufficiently small $\varepsilon$. Hence the individual common end limits supply neither a uniform threshold nor a uniform compact lower bound, despite the common local comparison controls in [F1]. [step 1.2, F1, algebra] ∎


## Scalar exterior inverse from exhaustion and uniform annular estimates

[Open item](item-lem-author-86990d62062f-weighted-scalar-inverse) · level 3


### Statement

On the end component under $h-\delta\in C^{3,\alpha}_{-1}$, $-1<\beta<0$, the zero-Dirichlet scalar Laplacian is a bounded isomorphism $X_\beta\to Y_\beta$, with $\|u\|_{4,\alpha,\beta}\le C\|\Delta_hu\|_{2,\alpha,\beta-2}$. The spaces and sign are exactly those of the weighted exterior definition. No assumption that the compact core is diffeomorphic to a Euclidean obstacle is required.

### Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] The weighted norms and coefficient decay use the fixed atlas and end chart. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] Compact truncations are solvable and have local fourth-order estimates. [lem-author-86990d62062f-compact-domain-poisson](item-lem-author-86990d62062f-compact-domain-poisson)

[F3] A positive decaying barrier exists, including a controlled inner seam. [lem-author-86990d62062f-global-decaying-barrier](item-lem-author-86990d62062f-global-decaying-barrier)

[F4] Uniform local Schauder estimates and diagonal compactness can be applied on fixed charts. [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations) [math:thm-boundary-schauder-estimate-for-the-dirichlet-problem](https://alphabetamath.cc/item/thm-boundary-schauder-estimate-for-the-dirichlet-problem) [math:thm-arzela-ascoli-for-real-ck](https://alphabetamath.cc/item/thm-arzela-ascoli-for-real-ck)

### Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] The weighted norms and coefficient decay use the fixed atlas and end chart. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] Compact truncations are solvable and have local fourth-order estimates. [lem-author-86990d62062f-compact-domain-poisson](item-lem-author-86990d62062f-compact-domain-poisson)

[F3] A positive decaying barrier exists, including a controlled inner seam. [lem-author-86990d62062f-global-decaying-barrier](item-lem-author-86990d62062f-global-decaying-barrier)

[F4] Uniform local Schauder estimates and diagonal compactness can be applied on fixed charts. [math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations](https://alphabetamath.cc/item/thm-interior-schauder-estimate-for-uniformly-elliptic-equations) [math:thm-boundary-schauder-estimate-for-the-dirichlet-problem](https://alphabetamath.cc/item/thm-boundary-schauder-estimate-for-the-dirichlet-problem) [math:thm-arzela-ascoli-for-real-ck](https://alphabetamath.cc/item/thm-arzela-ascoli-for-real-ck)



**Proof technique:** direct.

1.1 For $f\in Y_\beta$ solve $\Delta_hu_T=f$ on the smooth truncation $M_T$, with zero values on both its original and outer boundary, using the compact-domain lemma. Let $F=\|f\|_{2,\alpha,\beta-2}$. The norm definition gives $|f|\le C_0F\rho^{\beta-2}$. Comparing $\pm u_T-C_1FB$ using the barrier, with $C_1$ large enough, gives $|u_T|\le C_1FB$ independently of $T$. The comparison works at its seam by the derivative-jump argument, and on both boundary parts the barrier is positive. [F1, F2, F3]

2.1 Cover any annulus $A_R$ by a fixed finite number of balls of radius proportional to $R$, using larger annuli $\{R/2<r<4R\}$ for the estimates. Under $x=Ry$ the equation becomes $(h^{ij}(Ry)\partial_{ij}+Rb^i(Ry)\partial_i)u_T(Ry)=R^2f(Ry)$. These coefficients have uniformly bounded $C^{2,\alpha}$ norms and uniform ellipticity for large $R$, since $h-\delta\in C^{3,\alpha}_{-1}$. The fourth-order estimate of the compact-domain lemma, here using its interior argument, therefore gives $\|u_T(R\cdot)\|_{4,\alpha;A_1}\le C R^\beta F$ when $4R<T$. A finite ball cover controls close pairs in the annular Hölder seminorm; separated pairs are controlled by the derivative supremum divided by their fixed rescaled separation. The larger annulus data norm is bounded by the given norm using finitely many overlapping annuli. On each fixed compact core the boundary estimate has constants independent of $T$. [F1, F2, F4, step 1.1]

3.1 Exhaust $T\to\infty$. On each fixed compact region the fourth-order estimates give, by Ascoli on derivatives and a diagonal subsequence, convergence in $C^4$ (and $C^{4,\gamma}$ for $\gamma<\alpha$) to a zero-Dirichlet solution $u$. Hölder difference quotients pass to the limit for each pair of points, preserving the full exponent $\alpha$ and all weighted bounds from step 2.1. Thus $u\in X_\beta$ and $\Delta_hu=f$. For uniqueness a homogeneous solution tends uniformly to zero at infinity because $\beta<0$. Apply the scalar maximum principle on truncations and let their outer boundary supremum tend to zero, to $u$ and $-u$. The maximum principle itself follows by perturbing by a strictly subharmonic local test or by the positive-part energy comparison; its zeroth-order term is zero. Hence $u=0$. [F2, F3, F4, step 2.1]

4.1 The spaces here are Banach: a norm-Cauchy sequence converges on every compact chart in the ordinary Hölder Banach space; the limits agree on overlaps, and passing each annular norm inequality to the limit preserves the global weighted norm and Cauchy convergence. The zero trace subspace is closed. Product differentiation in $\Delta_h=h^{ij}\partial_{ij}+b^i\partial_i$ shows boundedness from $X_\beta$ to $Y_\beta$. The bound from steps 1.1 and 2.1 passes to the limit and gives a bounded inverse. This proves the Statement. [F1, step 3.1] ∎


## A compact-target boundary point has a null geodesic segment

[Open item](item-lem-author-2632702918ef-compact-target-null-segment) · level 3


### Statement

Under the hypotheses of the compact-target causal-endpoint lemma, $p$ is joined to some $c\in C$ by a nonconstant future null geodesic segment. The segment may be affinely parametrized on $[0,1]$ and is smooth up to both endpoints.

### Facts & Assumptions

[A1] Work in ZFC; the axiom of choice includes the countable and dependent choice assumptions of the causal suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The smooth spacetime, global hyperbolicity and causal relations are those of [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data).

[F2] The target surface has the smooth embedded spacelike meaning of [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data).

[F3] There is a distinct $c\in C$ with $p\le_Ec$, and $p\notin I_E^-(C)$. [lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)

[F4] The External input is the Avez–Seifert theorem for two distinct causally related points in a globally hyperbolic spacetime, with the affine geodesic-segment convention of the source’s section 2.1.

[F5] A future null affine geodesic is a smooth nonconstant curve with nonzero future null tangent and $D_s\dot\gamma=0$; positive affine changes preserve its orientation. Only this definition, not any completeness assertion, is used. [physics:def-gr-fx-future-null-geodesic-completeness](https://alphabetamath.cc/physics/item/def-gr-fx-future-null-geodesic-completeness)

[F6] The metric-selected connection is smooth and metric-compatible: along a curve, $\frac{d}{ds}g(V,V)=2g(D_sV,V)$. It is the Levi–Civita connection used by the imported geodesic equation. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the asserted conclusion.

1.1 Apply [F4] in $(E,g)$ to the pair provided by [F3]. Global hyperbolicity holds, and the endpoints are distinct and causally related. In the source’s section 2.1 convention this gives a nonconstant future causal affine geodesic segment $\gamma:[a,b]\to E$, $a<b$, with $\gamma(a)=p$ and $\gamma(b)=c$; both endpoints are included in the segment. [F1, F2, F3, F4, F6, given]

2.1 By [F6] and the affine geodesic equation, $\frac{d}{ds}g(\dot\gamma,\dot\gamma)=2g(D_s\dot\gamma,\dot\gamma)=0$. Thus the squared speed is constant. If it were negative, the future causal geodesic would be timelike from $p$ to $c$, contrary to [F3]. Its tangent is therefore null everywhere, with the nonzero future tangent required in [F5]. [step 1.1, F1, F3, F5, F6, algebra]

3.1 Put $\eta(t)=\gamma(a+(b-a)t)$ for $0\le t\le1$. The chain rule gives $\eta\prime=(b-a)\dot\gamma$ and $D_t\eta\prime=(b-a)^2D_s\dot\gamma=0$, so this is the desired positive affine normalization. The imported segment has included endpoints, rather than merely an asymptotic endpoint. In endpoint charts its equation is $x^{\mu\prime\prime}=-\Gamma^\mu_{\alpha\beta}(x)x^{\alpha\prime}x^{\beta\prime}$, with smooth coefficients by [F6]; starting with its twice differentiable geodesic solution, this equation successively gives derivatives of every order, with one-sided derivatives at included endpoints. Hence $\gamma$ and its affine reparametrization are smooth up to both endpoints, as asserted. [step 1.1, step 2.1, F4, F5, F6, algebra] ∎

### External input

Import Theorem 4.123 for the distinct points $p\le_Ec$ in the smooth globally hyperbolic spacetime $E$, using section 2.1’s affine geodesic-segment convention. It supplies a causal geodesic; maximality of length is unused. The endpoint lemma supplies the causal pair and chronological exclusion. Nullness, normalization and smooth endpoint regularity are deduced above; boundary containment and orthogonality belong to separate local lemmas.


## A compact temporal covector persists under metric perturbation

[Open item](item-lem-author-89004136b63c-compact-temporal-persistence) · level 3


### Statement

Let $g$ be a $C^2$ Lorentz metric on an open subset of a smooth four-manifold, $N$ a continuous timelike orientation field, $K$ compact, and $\alpha$ a continuous covector field near $K$ with $g^{-1}(\alpha,\alpha)<0$ and $\alpha(N)>0$ on $K$. There is $\delta>0$ such that every Lorentz metric $\widetilde g$ whose coefficients differ from those of $g$ by less than $\delta$ on a fixed finite compact chart cover of $K$ satisfies $\widetilde g(N,N)<0$, $\widetilde g^{-1}(\alpha,\alpha)<0$ and $\alpha(N)>0$ on $K$. Orient $\widetilde g$ by $N$ on $K$. Thus if $\alpha=d\tau$ for a smooth real function $\tau$, the $\widetilde g$-gradient of $\tau$ is past timelike on $K$. This asserts persistence on the compact set; it asserts no causal property away from that set.

### Statement references

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[lem-author-89004136b63c-compact-neighborhood-localization](item-lem-author-89004136b63c-compact-neighborhood-localization)

[lem-author-89004136b63c-temporal-compact-margins](item-lem-author-89004136b63c-temporal-compact-margins)

[lem-author-89004136b63c-uniform-inverse-metric-continuity](item-lem-author-89004136b63c-uniform-inverse-metric-continuity)

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary)

[math:thm-compact-subset-of-a-hausdorff-space-is-closed](https://alphabetamath.cc/item/thm-compact-subset-of-a-hausdorff-space-is-closed)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

### Facts & Assumptions

[F1] Use a finite compact chart cover and the compact margins and component bounds for $\alpha,N$. [lem-author-89004136b63c-compact-neighborhood-localization](item-lem-author-89004136b63c-compact-neighborhood-localization) [lem-author-89004136b63c-temporal-compact-margins](item-lem-author-89004136b63c-temporal-compact-margins)

[F2] Uniformly small matrix perturbations make inverse coefficients uniformly close. [lem-author-89004136b63c-uniform-inverse-metric-continuity](item-lem-author-89004136b63c-uniform-inverse-metric-continuity)

[F3] The inverse metric raises covectors, and the past-timelike convention is fixed by pairing positively with $N$. [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F4] A smooth manifold has an underlying topological manifold, which is Hausdorff. Every compact subset of a Hausdorff space is closed. Closed sets in a subspace are traces of ambient closed sets, and a closed subspace of a compact space is compact. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:def-topological-manifold-without-boundary](https://alphabetamath.cc/item/def-topological-manifold-without-boundary) [math:thm-compact-subset-of-a-hausdorff-space-is-closed](https://alphabetamath.cc/item/thm-compact-subset-of-a-hausdorff-space-is-closed) [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top) [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

### Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the conclusions in the Statement.

1.1 If $K$ is empty the conclusion is vacuous. Otherwise write $C_j$ for the pieces of the fixed finite compact chart cover and set $K_j=C_j\cap K$. The ambient smooth manifold is Hausdorff by [F4]. Each compact $C_j$ is therefore closed in it, so $K_j=C_j\cap K$ is closed in the compact subspace $K$ and hence compact by [F4]. These compact pieces still cover $K$ and lie where $\alpha,N$ are defined. Choose $m,a,b>0$ from [F1], and a common bound $R\ge1$ for all components of $\alpha$ and $N$ on the restricted pieces $K_j$. For a coefficient perturbation less than $\delta$, the change in $g(N,N)$ has absolute value at most $16\delta R^2$. Choose $\delta<b/(32R^2)$ to retain $\widetilde g(N,N)<0$. [F1, F3, F4]

2.1 Apply [F2] on the restricted pieces $K_j$ with $\eta=m/(32R^2)$ and reduce $\delta$ to its resulting threshold. The change in $g^{-1}(\alpha,\alpha)$ then has absolute value at most $16\eta R^2=m/2$, so it remains negative. The pairing $\alpha(N)\ge a$ does not change with the metric. For $\alpha=d\tau$, [F3] identifies these inequalities with a past-timelike $\widetilde g$-gradient. [F1, F2, F3, step 1.1] ∎


## Collar barrier against finite section-time boundary arrival

[Open item](item-lem-author-eb8e266b8b92-collar-nonarrival) · level 3


### Statement

Assume the Axiom of Choice and the stationary ADM setting with causal curves of the section-time speed lemma. Let the spatial slice be the interior of a smooth manifold $\overline S$ with compact boundary $B$. A supplied collar is a diffeomorphism $[0,\epsilon)\times B$ onto a boundary neighborhood; its first coordinate is $\rho$, and $\rho=0$ exactly on $B$. Here diffeomorphism means a bijection that is smooth, with smooth inverse, in boundary charts. Suppose $h$ extends smoothly and positively to the boundary, and in the collar $N\le A\rho$, $|X(\rho)|\le A\rho$, and $|d\rho|_h\le A$, with $A<\infty$. Fix $0<a<\epsilon$ and define $b(x)=\min(\rho(x),a)$ in the collar and $b(x)=a$ outside it. For every causal section-time curve and every two times in its interval, $b(x(v))\ge b(x(v_0))e^{-C|v-v_0|}$, with $C=A^2+A$. Thus no finite section-time endpoint can lie on $B$, including for curves that leave and re-enter the collar.

### Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)

[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)

[math:thm-gronwall-integral-inequality](https://alphabetamath.cc/item/thm-gronwall-integral-inequality)

[math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)

[physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)

[math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)

### Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice implies Dependent Choice and Countable Choice, supplying the choice assumptions of the analytic and smooth-composition suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F2] Every causal curve can use section time; the resulting curve $\gamma(v)=(v,x(v))$ is locally Lipschitz in charts, is future causal, and obeys $|x\prime+X|_h\le N$ almost everywhere. The norms, gradient and vector-field action have the conventions in the ADM supplier. [lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)

[F3] Absolutely continuous scalar functions satisfy the fundamental theorem of calculus. [math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)

[F4] For a continuous nonnegative function satisfying either oriented integral inequality with constant coefficients, Gronwall gives $u(t)\le Ae^{C|t-t_0|}$. [math:thm-gronwall-integral-inequality](https://alphabetamath.cc/item/thm-gronwall-integral-inequality)

[F5] For a locally absolutely continuous future causal curve with nonzero velocity almost everywhere in a time-oriented smooth Lorentzian four-manifold, composition with a smooth map defined on an open set containing the curve image is locally absolutely continuous and satisfies the chain rule almost everywhere. Apply this statement to restrictions of the curve when the map is only locally defined. [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[F6] Cauchy–Schwarz for the inner product $h$ gives $|d\rho(Y)|=|h(\operatorname{grad}_h\rho,Y)|\le|d\rho|_h|Y|_h$ at each point where $\rho$ is defined. [math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)

[F7] Interior points and boundary points of a smooth manifold with boundary are specified by the positive and zero last coordinate, respectively, in a boundary chart; here $S=\operatorname{Int}\overline S$ and $B=\partial\overline S$. [math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)

[F8] Smooth structures with boundary are maximal compatible atlases of boundary charts; maps are smooth when their boundary-chart representatives are smooth in the local-extension sense. The collar and its inverse use these conventions. [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)

### Proof

1.1 Let $U$ be the collar intersected with $S$, an open subset of $S$. The inverse collar map is smooth in boundary charts; taking its first coordinate makes $\rho$ smooth on $U$, so the map $F(v,p)=\rho(p)$ below is smooth. On every section-time subarc whose spatial image lies in $U$, apply smooth composition to $F:\mathbb R\times U\to\mathbb R$, $F(v,p)=\rho(p)$, and the causal curve $\gamma(v)=(v,x(v))$. Then $r=\rho\circ x$ is locally absolutely continuous and $r'=d\rho(x')=d\rho(x'+X)-X(\rho)$ almost everywhere. The pointwise Cauchy–Schwarz inequality and the ADM vector-speed bound therefore give $|r'|\le|d\rho|_h|x'+X|_h+|X(\rho)|\le N|d\rho|_h+|X(\rho)|$. This uses no global extension of $\rho$. [F1, F2, F5, F6, F8, algebra]

2.1 Within a connected time interval on which $\rho<a$, the speed estimate gives $|\rho\prime|\le C\rho$ almost everywhere. On any compact subinterval $[s,t]$ of it, the fundamental theorem gives $\rho(u)\le\rho(t)+C\int_u^t\rho(w)\,dw$ for $s\le u\le t$. The reflected Gronwall inequality yields $\rho(s)\le\rho(t)e^{C(t-s)}$, or $\rho(t)\ge\rho(s)e^{-C(t-s)}$. Applying the forward version gives the same lower bound in the reverse orientation. [F3, F4, step 1.1, given, algebra]

3.1 For $v\ge v_0$, if $\rho(x(v))\ge a$ or $x(v)$ is outside the collar, the asserted bound is immediate since $b(x(v))=a\ge b(x(v_0))$. Otherwise use the connected component of $\{u:\rho(x(u))<a\}$ containing $v$. If the component does not contain $v_0$, its left endpoint $\ell$ satisfies $v_0\le\ell<v$, including the case $\ell=v_0$. Continuity gives $\rho(x(\ell))=a$; pass to that endpoint in the previous lower bound. If the component contains $v_0$, use the value $\rho(x(v_0))$ instead. Both cases give the stated estimate with elapsed time at most $v-v_0$. Reversing the time interval proves the other orientation. The positive resulting lower bound for bounded elapsed time excludes all boundary approaches, even with repeated collar entries. [F2, step 2.1, algebra] ∎


## Proper end radius and exclusion of finite-time spatial infinity

[Open item](item-lem-author-eb8e266b8b92-proper-radius-control) · level 3


### Statement

Assume the Axiom of Choice and the stationary ADM setting of the section-time speed lemma. Let $\overline S$ be a connected smooth three-manifold with compact boundary, with $S=\operatorname{int}\overline S$, and a smooth positive-definite extension of $h$. Smoothness on $\overline S$ is understood in boundary charts by local smooth extension; the metric and differential norms use the section-time speed lemma's conventions, extended to the boundary using the inverse metric. Suppose $N$ and $X$ extend smoothly to $\overline S$, and supply a smooth function $R:\overline S\to[0,\infty)$ such that every sublevel $\{R\le m\}$ is compact. This is the proper-radius hypothesis. Suppose outside a compact set $K_0\subset\overline S$ one has $|dR|_h(N+|X|_h)\le C_0$. Then there is a finite constant $C_R$ such that every causal section-time curve satisfies $|R(x(v))-R(x(v_0))|\le C_R|v-v_0|$. In particular its spatial image for bounded section time stays in a compact subset of $\overline S$, although that subset can meet the boundary. One sufficient end realization of this hypothesis is a compact core with finitely many product ends $[r_0,\infty)\times F_j$, each $F_j$ compact, and a smooth $R$ equal to their unbounded first coordinate outside a larger compact core, with the displayed estimate for that coordinate.

### Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)

[physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)

[math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)

[math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

[math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r)

[math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)

[math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

### Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice implies Dependent Choice and Countable Choice, which discharge the choice hypotheses of the causal-curve calculus and the absolutely-continuous fundamental theorem. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F2] The section-time speed lemma makes $\gamma(v)=(v,x(v))$ a causal, locally Lipschitz curve on the smooth time-oriented Lorentzian four-manifold $E=\mathbb R_v\times S$ and gives $|(R\circ x)\prime|\le N|dR|_h+|X(R)|$ almost everywhere. Apply clause (b) of the causal-curve calculus to the smooth scalar $F:E\to\mathbb R$, $F(v,p)=R(p)$: its composite $F\circ\gamma=R\circ x$ is locally absolutely continuous. The required Countable Choice and Dependent Choice follow from F1. [lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed) [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

[F3] Absolutely continuous scalar functions are recovered by integrating their almost-everywhere derivatives. [math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)

[F4] Boundary charts use the local-extension notion of smoothness, smooth maps are continuous, and a Riemannian metric is a smooth positive-definite symmetric tensor, with smoothness up to the boundary where stated. [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary) [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[F5] Cauchy–Schwarz holds in each real inner product space. [math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)

[F6] A continuous real-valued function on a nonempty compact space attains its maximum; continuous images of compact spaces are compact. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

[F7] Every closed bounded real interval is compact, and a finite product of compact spaces is compact in the product topology. [math:thm-heine-borel-r](https://alphabetamath.cc/item/thm-heine-borel-r) [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)

[F8] A closed subspace of a compact space is compact, and a finite union of compact subspaces is compact, including the empty union. [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

### Proof

1.1 In a boundary chart write $h=(h_{ij})$. Positive definiteness makes $\det(h_{ij})$ nonzero, so the cofactor formula shows that the inverse matrix $(h^{ij})$ is smooth up to the boundary. The identities $|dR|_h^2=\sum_{i,j}h^{ij}(\partial_iR)(\partial_jR)$ and $|X|_h^2=\sum_{i,j}h_{ij}X^iX^j$ therefore give continuous nonnegative norms, including at boundary points. The vector with components $Y^i=\sum_j h^{ij}\partial_jR$ satisfies $h(Y,X)=dR(X)$ and $|Y|_h=|dR|_h$, so Cauchy–Schwarz gives $|X(R)|\le|dR|_h|X|_h$. Thus $q=N|dR|_h+|X(R)|$ is continuous on $\overline S$. [given, F2, F4, F5, algebra]

2.1 If $K_0$ is nonempty, let $M_0$ be the maximum of $q$ on $K_0$; if $K_0$ is empty, set $M_0=0$, with no extreme-value assertion needed there. On $S\setminus K_0$, step 1.1 and the given estimate imply $q\le|dR|_h(N+|X|_h)\le C_0$. Hence $C_R=\max\{0,C_0,M_0\}$ bounds $q$ along every spatial curve in $S$. The section-time speed lemma gives $|(R\circ x)\prime|\le C_R$ almost everywhere. On the compact interval between any two section times $v,v_0$ in the domain of the curve, F2 makes the scalar composition absolutely continuous; the fundamental theorem, with its choice hypotheses supplied by F1, gives $|R(x(v))-R(x(v_0))|\le C_R|v-v_0|$. [given, F1, F2, F3, F6, step 1.1, algebra]

3.1 If $|v-v_0|\le T$, step 2.1 places the image in $\{R\le R(x(v_0))+C_RT\}$, which is compact in $\overline S$ by the supplied proper-radius hypothesis. This proves confinement in the manifold with boundary; it does not exclude boundary accumulation. [given, step 2.1, algebra]

4.1 For the sufficient end realization, let $C$ be the larger compact core containing the transition region so that every point outside $C$ lies in a stated product end where $R=r$. For any real $m$, put $L=\max\{r_0,m\}$. The interval $[r_0,L]$ is compact, so each $[r_0,L]\times F_j$ is compact; its image under the end identification is compact by continuity. The union $P$ of those finitely many images with $C$ is compact. If $R(p)\le m$, either $p\in C$ or its end coordinate satisfies $r=R(p)\le m\le L$, so $p\in P$. Continuity of $R$ makes $\{R\le m\}$ closed in $\overline S$, hence closed in $P$ and compact. This includes the case $m<r_0$, where any points of the sublevel already lie in $C$. A bounded or nonproper reparameterization of an end coordinate alone supplies no such conclusion. [given, F4, F6, F7, F8] ∎


## An interior compact causal trajectory has a finite-time endpoint

[Open item](item-lem-author-eb8e266b8b92-compact-causal-endpoint) · level 3


### Statement

Assume the Axiom of Choice and the stationary ADM causal conventions of the section-time speed lemma. If a causal curve $(v,x(v))$, $v\in[v_0,v_*)$, with $v_*<\infty$, has spatial image in a compact interior subset $K\subset S$, then it converges to a point $(v_*,p)\in E$. The corresponding conclusion holds at a finite lower endpoint. Consequently neither end of a causal curve that is inextendible in $E$ can have finite section time while its spatial projection stays in an interior compact set.

### Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)

[math:thm-the-riemannian-distance-topology-is-the-manifold-topology](https://alphabetamath.cc/item/thm-the-riemannian-distance-topology-is-the-manifold-topology)

[math:thm-metric-compactness-equivalences](https://alphabetamath.cc/item/thm-metric-compactness-equivalences)

[math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)

### Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice supplies inherited countable and dependent choice assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F2] A causal curve in section time is locally Lipschitz and has $|x\prime|_h\le N+|X|_h$; inextendibility is absence of an endpoint. [lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)

[F3] The Riemannian distance gives the manifold topology, and a compact metric space is sequentially compact under the inherited choice assumptions. [math:thm-the-riemannian-distance-topology-is-the-manifold-topology](https://alphabetamath.cc/item/thm-the-riemannian-distance-topology-is-the-manifold-topology) [math:thm-metric-compactness-equivalences](https://alphabetamath.cc/item/thm-metric-compactness-equivalences)

[F4] A positive-definite smooth metric uniformly bounds the Euclidean norm on a compact coordinate ball. [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

[F5] For absolutely continuous coordinate functions the integral of the derivative gives their endpoint difference. [math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions](https://alphabetamath.cc/item/thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions)

[F6] A continuous real-valued function on a nonempty compact metric space is bounded. [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)

### Proof

1.1 The smooth ADM data make $N+|X|_h$ continuous on $K$. Since $x(v_0)\in K$, this compact set is nonempty. The extreme-value theorem therefore bounds $N+|X|_h$ on $K$, say by $B$. Choose times $v_j\uparrow v_*$; compactness gives a subsequence for which $x(v_j)\to p\in K$. Take an interior coordinate ball centered at $p$, with coordinate radius $r>0$ and compact closure in its chart. Metric comparison on its closure gives $h(Y,Y)\ge c|Y|_{\mathrm e}^2$ for $c>0$. Thus while the curve remains in the ball, $|x\prime|_{\mathrm e}\le B/\sqrt c=:D$ almost everywhere. [F1, F2, F3, F4, F6, choose]

2.1 Choose a subsequence time $v_j$ so late that its coordinate distance from the center is less than $r/4$ and $D(v_*-v_j)<r/4$; for $D=0$ only the first condition is needed. Were there a subsequent exit from the coordinate ball, continuity would give a first exit, but integration of the coordinate speed up to that exit would give total displacement less than $r/4$, contradicting the required displacement of more than $3r/4$. Hence the whole remaining tail stays in that chart. Its coordinates are $D$-Lipschitz and are Cauchy as $v\uparrow v_*$. They converge to the coordinate of $p$, since the chosen subsequence does. Thus $(v,x(v))\to(v_*,p)\in E$. The argument with reversed parameter direction treats a finite lower endpoint. Such a limit contradicts precisely the endpoint definition of inextendibility. [F1, F2, F5, step 1.1, algebra] ∎


## Temporal angle and tangential height gradient identity

[Open item](item-lem-author-fd2999663761-temporal-tangent-gradient) · level 3


### Statement

For the temporal angle data, the tangential projection of $V$ is $W=V-vn$ and satisfies $|W|_h^2=v^2-1$. Consequently $\nabla_\Sigma\tau=-\alpha W$ and $|\nabla_\Sigma\tau|_h^2=\alpha^2(v^2-1)$. If $\alpha\ge a_0>0$, this gives $|\nabla_\Sigma\tau|_h^2\ge a_0^2(v^2-1)$.

### Facts & Assumptions

[F1] The temporal angle data have $g(n,n)=g(V,V)=-1$, $g(n,V)=-v$ and $\operatorname{grad}_g\tau=-\alpha V$. [def-author-fd2999663761-temporal-angle-data](item-def-author-fd2999663761-temporal-angle-data)

### Proof

**Given:** The data in [F1]. **Goal:** Establish the projections and norm identity.

1.1 The vector $W=V-vn$ is tangent because $g(W,n)=-v+v=0$. Expansion gives $g(W,W)=-1+2v^2-v^2=v^2-1$. [F1, algebra]

2.1 For every tangent $Y$, $d\tau(Y)=-\alpha g(V,Y)=-\alpha h(W,Y)$. The defining property of the induced gradient gives $\nabla_\Sigma\tau=-\alpha W$. Squaring and using step 1.1 gives the identity and its lower-bound consequence. [F1, step 1.1, algebra] ∎


## From hyperbolic angle to logarithmic angle inequalities

[Open item](item-lem-author-fd2999663761-logarithmic-angle-conversion) · level 3


### Statement

On a Riemannian hypersurface let $v>2$ be smooth, put $\eta=\operatorname{arcosh}v=\log(v+\sqrt{v^2-1})$, and suppose $\Delta\eta\ge\coth\eta\,(\tfrac14|\nabla\eta|^2-Cv^2)$ for some $C\ge0$. Then $f=\log v$ satisfies $\Delta f\ge\tfrac14|\nabla f|^2-Cv^2$. The convention for gradient and Laplacian is that of the temporal angle data.

### Facts & Assumptions

[F1] Use the positive-trace scalar Laplacian and its gradient from [def-author-fd2999663761-temporal-angle-data](item-def-author-fd2999663761-temporal-angle-data). The differential inequality in the Statement is an explicit hypothesis of this algebraic lemma, not a geometric conclusion proved here.

[F2] The hypersurface carries a smooth positive-definite metric $h$ in the general sense of [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold), allowing an actual boundary and smoothness up to it. The metric-dual gradient, the coordinate Hessian formula $(\operatorname{Hess}_h u)_{ij}=\partial_i\partial_j u-\Gamma^k{}_{ij}\partial_k u$, and the divergence connection formula are supplied by [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas). The identity $\Delta_h u=\operatorname{tr}_h\operatorname{Hess}_h u=\operatorname{div}_h\operatorname{grad}_h u$ and its smooth one-sided boundary convention are [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian). Only the intrinsic operator convention is borrowed from the temporal angle data; no ambient Lorentzian or maximality assumption is used here.

[F3] The scalar sum, product, quotient and chain rules are [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules), applied to each coordinate derivative.

[F4] The inverse identity for $\operatorname{arcosh}$ on $[1,\infty)$ is [math:thm-inverse-hyperbolic-logarithm-formulas](https://alphabetamath.cc/item/thm-inverse-hyperbolic-logarithm-formulas). The hyperbolic identities, quotient definitions and derivatives, including $(\cosh s)^{\prime}=\sinh s$, $(\tanh s)^{\prime}=\operatorname{sech}^2s$ and $0<\tanh s<1$ for $s>0$, are [math:thm-hyperbolic-identities-and-derivatives](https://alphabetamath.cc/item/thm-hyperbolic-identities-and-derivatives). The formula $(\log x)^{\prime}=1/x$ for $x>0$ is [math:thm-logarithm-derivative-and-integral](https://alphabetamath.cc/item/thm-logarithm-derivative-and-integral); positive-base powers and their derivative formula, used for the square root on $(0,\infty)$, are [math:thm-real-power-continuity-and-derivatives](https://alphabetamath.cc/item/thm-real-power-continuity-and-derivatives). Iterating these derivative formulas with [F3] gives smoothness on the indicated open domains.

### Proof

**Given:** The smooth function and differential inequality in the Statement. **Goal:** Derive the logarithmic inequality.

1.1 Since $v>2$, [F4] makes $\eta=\operatorname{arcosh}v$ smooth and positive, with $v=\cosh\eta$. Set $H(s)=\log\cosh s$, so $f=H(\eta)$. The scalar rules and the logarithm and hyperbolic derivatives give $H^{\prime}(s)=\sinh s/\cosh s=\tanh s$ and $H^{\prime\prime}(s)=\operatorname{sech}^2s$. [F3, F4, given, algebra]

2.1 In an arbitrary interior coordinate chart, the scalar chain and product rules give $\partial_i(H(\eta))=H^{\prime}(\eta)\partial_i\eta$ and $\partial_i\partial_j(H(\eta))=H^{\prime\prime}(\eta)\partial_i\eta\,\partial_j\eta+H^{\prime}(\eta)\partial_i\partial_j\eta$. Substitution in the coordinate Hessian formula yields $\operatorname{Hess}_h(H(\eta))=H^{\prime\prime}(\eta)d\eta\otimes d\eta+H^{\prime}(\eta)\operatorname{Hess}_h\eta$. Taking the metric trace and using the metric-dual characterization of the gradient gives $\nabla f=\tanh\eta\,\nabla\eta$ and $\Delta f=\tanh\eta\,\Delta\eta+\operatorname{sech}^2\eta\,|\nabla\eta|^2$. At any actual boundary point these identities follow by continuity from the interior in a boundary half-chart: the metric, inverse metric, function derivatives and operator coefficients are smooth up to that point, and the operators there have the one-sided convention in [F1] and [F2]. [F1, F2, F3, step 1.1, algebra]

3.1 Multiply the assumed lower bound for $\Delta\eta$ by $\tanh\eta>0$. Since $\tanh\eta\coth\eta=1$, step 2.1 gives $\Delta f\ge(\tfrac14+\operatorname{sech}^2\eta)|\nabla\eta|^2-Cv^2\ge\tfrac14|\nabla f|^2-Cv^2$, where the last step uses $|\tanh\eta|\le1$ and the nonnegativity of the squared norm. This also holds at actual boundary points under the stated smooth one-sided convention. [F1, F2, F4, step 2.1, given, algebra] ∎



## Compact weighted maximum and the actual boundary term

[Open item](item-lem-author-fd2999663761-compact-weighted-maximum) · level 3


### Statement

For a compact positive-height portion $P$ of the temporal angle data, let $\mu>0$. Use the real-power convention $0^\mu=0$. A local maximum of $w$ at $p\in S=\Sigma\cap\{\tau>0\}$ means that there is an open neighborhood $U\subseteq S$ of $p$ in $\Sigma$ with $w(q)\le w(p)$ for every $q\in U$. Suppose $w=\tau^\mu v$ has no local maximum at any interior point of $\Sigma$ with $\tau>0$ and $v>2$. Then $\sup_{\Sigma\cap\{\tau>0\}}\tau^\mu v\le\max\{2T^\mu,B\}$. The supremum on the left is defined to be zero if $\Sigma\cap\{\tau>0\}=\varnothing$. No regularity of the zero level $\{\tau=0\}\cap\Sigma$ is required.

### Statement references

[def-author-fd2999663761-temporal-angle-data](item-def-author-fd2999663761-temporal-angle-data)

[math:def-real-power](https://alphabetamath.cc/item/def-real-power)

### Facts & Assumptions

[F1] The entire portion $P=\Sigma\cap\{\tau\ge0\}$ is compact, $v$ is continuous and bounded on it, $0\le\tau\le T$, and $B$ uses only $\partial\Sigma\cap\{\tau>0\}$. [def-author-fd2999663761-temporal-angle-data](item-def-author-fd2999663761-temporal-angle-data)

[F2] A continuous real-valued function on a nonempty compact space attains a maximum and a minimum (Statement, assertion 2). [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

[F3] For $r>0$, $0^r=0$ and $t\mapsto t^r$ is strictly increasing on $[0,\infty)$; in particular $t^r>0$ when $t>0$. Use the real-power definition and the monotonicity assertion of the measurability lemma; no measurable-space hypothesis is needed for that assertion. [math:def-real-power](https://alphabetamath.cc/item/def-real-power) [math:lem-real-power-preserves-measurability](https://alphabetamath.cc/item/lem-real-power-preserves-measurability)

[F4] For every real $r$, $t\mapsto t^r$ is continuous for $t>0$. For $a>0$ and real $r,s$, $(a^r)^s=a^{rs}$, and $a^1=a$ by agreement with rational powers. [math:thm-real-power-continuity-and-derivatives](https://alphabetamath.cc/item/thm-real-power-continuity-and-derivatives) [math:thm-real-power-laws](https://alphabetamath.cc/item/thm-real-power-laws) [math:thm-real-power-agrees-with-rational-exponent](https://alphabetamath.cc/item/thm-real-power-agrees-with-rational-exponent)

[F5] Restrictions of continuous maps to subspaces are continuous, and a continuous map whose range lies in a subspace is continuous into that subspace, with its subspace topology. Composites of continuous maps between arbitrary topological spaces are continuous (Statement, assertion 1). Products of continuous real-valued maps on any topological space are continuous. [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top) [math:lem-continuity-is-local-and-pastes](https://alphabetamath.cc/item/lem-continuity-is-local-and-pastes) [math:lem-algebra-of-continuous-real-maps-on-a-space](https://alphabetamath.cc/item/lem-algebra-of-continuous-real-maps-on-a-space)

### Proof

**Given:** [F1] and the no-interior-maximum hypothesis, with $\mu>0$. **Goal:** Bound the weighted supremum.

1.1 For the fixed $\mu>0$, the power function is continuous at every positive argument by [F4]. To check continuity at zero, let $\varepsilon>0$ and put $\delta=\varepsilon^{1/\mu}>0$ by [F3] with exponent $1/\mu>0$. The iterated-power law and normalization in [F4] give $\delta^\mu=\varepsilon$. If $0\le t<\delta$, [F3] gives $0\le t^\mu<\delta^\mu=\varepsilon$. Since $0^\mu=0$, this proves continuity at zero relative to $[0,\infty)$. The same monotonicity gives $0\le\tau^\mu\le T^\mu$ on $P$. [F1, F3, F4, given, algebra]

2.1 Put $S=\Sigma\cap\{\tau>0\}$. If $S$ is empty, its stipulated supremum is zero and the right-hand side is nonnegative by $T\ge0$ and [F3], so the estimate holds, even when $P$ consists only of zero-height points. Otherwise $P$ is nonempty. Applying [F2] to the continuous $v$ on compact $P$ gives finite extrema; taking $M$ to be the larger of their absolute values and $1$ yields $|v|\le M$ on $P$. Extend $w$ by zero at zero height. By the restriction and subspace assertions of [F5], the continuous $\tau$ restricts to a continuous map $\tau|_P:P\to[0,\infty)$, since its values are nonnegative by [F1]. Composing this map with the continuous power map $t\mapsto t^\mu$ from step 1.1 gives continuity of $\tau^\mu:P\to\mathbb R$ by [F5]. The product assertion of [F5], applied on the topological space $P$ to $\tau^\mu$ and $v$, makes the extended $w$ continuous on all of $P$. At a zero-height point, $|w|\le M\tau^\mu$ tends to zero by step 1.1 and continuity of $\tau$, proving continuity there too. [F1, F2, F3, F5, step 1.1, given]

3.1 In the remaining case $P$ is nonempty and compact, and the extended $w:P\to\mathbb{R}$ is continuous. Applying [F2] with domain $P$ gives a point at which $w$ attains its maximum on $P$. [F1, F2, step 2.1]

4.1 At a maximum point with $\tau=0$ the value is zero. At a positive-height point on $\partial\Sigma$ it is at most $B$. If the maximum point $p$ is interior to $\Sigma$ and has positive height, then $U=S\cap(\Sigma\setminus\partial\Sigma)$ is an open neighborhood of $p$ in $\Sigma$ by continuity of $\tau$. Since $U\subseteq P$, the maximum on $P$ gives $w(q)\le w(p)$ for every $q\in U$, exactly the local-maximum condition in the Statement. The hypothesis therefore gives $v(p)\le2$, so $w(p)\le2\tau(p)^\mu\le2T^\mu$ by step 1.1. These exhaustive cases bound the maximum on $P$ by $\max\{2T^\mu,B\}$ and hence bound the supremum on $S\subseteq P$, with no regularity required of the zero level. [F1, F3, step 1.1, step 3.1, given] ∎


## MOTS boosts preserve the spacetime stability sign

[Open item](item-lem-author-97780c2fed82-mots-boost-variation) · level 3


### Statement

For a MOTS with null pair $(\ell,k)$ normalized by $g(\ell,k)=-1$, let $h:S\to(0,\infty)$ be smooth and set $\ell'=h\ell$, $k'=h^{-1}k$. For the same normal velocity $X$, the variation satisfies $\delta_X\theta_{(\ell')}=h\delta_X\theta_{(\ell)}$. Consequently if $X=\gamma\ell-\psi k$ with $\gamma\ge0$ and $\psi>0$, then $X=\gamma'\ell'-\psi'k'$ with $\gamma'=\gamma/h\ge0$, $\psi'=h\psi>0$, and the inequality $\delta_X\theta\ge0$ is unchanged by the boost.

### Statement references

[def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data)

[lem-author-97780c2fed82-mots-variation-second-jet](item-lem-author-97780c2fed82-mots-variation-second-jet)

### Facts & Assumptions

[F1] The null pairing and tangential expansion use the general surface convention. [def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data)

[F2] The variation at a MOTS is well defined and independent of extensions of its base null gauge. [lem-author-97780c2fed82-mots-variation-second-jet](item-lem-author-97780c2fed82-mots-variation-second-jet)

### Proof

**Given:**The objects and hypotheses in the Statement.

**Goal:** Establish the assertions and well-definedness stated there.

1.1 Choose any actual deformation realizing $X$ and extend $h$ smoothly along its parameter with its prescribed initial value. Orthogonality of $\ell_t$ to the tangent surface gives $\theta_{(h_t\ell_t)}=h_t\theta_{(\ell_t)}$. Differentiating at zero gives $\delta_X\theta_{(\ell')}=h\delta_X\theta_{(\ell)}+(\partial_th_t)|_0\theta_{(\ell)}=h\delta_X\theta_{(\ell)}$. Its sign is unchanged since $h>0$. [F1, F2]

2.1 Substitution of $\ell=\ell'/h$ and $k=hk'$ into $X$ gives the stated new coefficients and signs. Moreover $g(X,X)=2\gamma\psi\ge0$, so these are outgoing non-timelike normal directions, including the past null direction $-k$ when $\gamma=0$. This is a pointwise identity and does not assume that $X$ is tangent to a spacelike slice. [F1, step 1.1] ∎



## Exterior Dirichlet parametrix and compact decaying potentials

[Open item](item-lem-exterior-parametrix-and-compact-potential) · level 4


### Statement

Let $(\Sigma,h)$ be the smooth three-dimensional exterior with compact smooth boundary of the weighted exterior definition, $0<\alpha<1$, $h-\delta\in C^{3,\alpha}_{-1}$ and $-1<\beta<0$. The scalar Dirichlet Laplacian $\Delta_h:X_\beta\to Y_\beta$ is Fredholm of index zero. Multiplication by any real $V\in C^{2,\alpha}_{-4}$ is compact from $X_\beta$ to $Y_\beta$. Hence $\Delta_h-V$ is Fredholm of index zero. No sign assumption on $V$ is required for this index assertion. The smooth compact inner boundary is included in the construction; no restriction on its number of components or on the topology of the compact core is imposed.

### Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] The exact weighted spaces and end falloff conventions are fixed. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] Fredholm means finite-dimensional kernel and cokernel and closed range between Banach spaces. [def-fredholm-continuation-data](item-def-fredholm-continuation-data)

[F3] The scalar Laplacian on the end component has a bounded inverse obtained by compact-boundary exhaustion; Proof 4.1 of this supplier proves completeness of its end-component spaces. [lem-author-86990d62062f-weighted-scalar-inverse](item-lem-author-86990d62062f-weighted-scalar-inverse)

[F4] There are finitely many extra compact components. Proof 2.1 of this supplier proves their Hölder spaces are Banach and their nonempty-boundary Dirichlet inverses are bounded; Proof 4.1 gives the bounded mean-zero Green inverse on each closed component, and Proof 5.1 identifies its kernel and range. [lem-author-86990d62062f-closed-component-index](item-lem-author-86990d62062f-closed-component-index)

[F5] Potential multiplication is compact at the stated orders and weights. [lem-author-86990d62062f-compact-potential](item-lem-author-86990d62062f-compact-potential)

[F6] A compact perturbation preserves Fredholmness and index. [math:thm-fredholm-index-is-stable-under-compact-perturbations](https://alphabetamath.cc/item/thm-fredholm-index-is-stable-under-compact-perturbations)

### Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** prove the Statement.

[F1] The exact weighted spaces and end falloff conventions are fixed. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] Fredholm means finite-dimensional kernel and cokernel and closed range between Banach spaces. [def-fredholm-continuation-data](item-def-fredholm-continuation-data)

[F3] The scalar Laplacian on the end component has a bounded inverse obtained by compact-boundary exhaustion; Proof 4.1 of this supplier proves completeness of its end-component spaces. [lem-author-86990d62062f-weighted-scalar-inverse](item-lem-author-86990d62062f-weighted-scalar-inverse)

[F4] There are finitely many extra compact components. Proof 2.1 of this supplier proves their Hölder spaces are Banach and their nonempty-boundary Dirichlet inverses are bounded; Proof 4.1 gives the bounded mean-zero Green inverse on each closed component, and Proof 5.1 identifies its kernel and range. [lem-author-86990d62062f-closed-component-index](item-lem-author-86990d62062f-closed-component-index)

[F5] Potential multiplication is compact at the stated orders and weights. [lem-author-86990d62062f-compact-potential](item-lem-author-86990d62062f-compact-potential)

[F6] A compact perturbation preserves Fredholmness and index. [math:thm-fredholm-index-is-stable-under-compact-perturbations](https://alphabetamath.cc/item/thm-fredholm-index-is-stable-under-compact-perturbations)



**Proof technique:** direct.

1.1 Write $\Sigma_0$ for the end component and $M_1,\ldots,M_m$ for the finitely many compact components supplied by [F4]. The spaces $X_0,Y_0$ on $\Sigma_0$ are Banach by [F3], Proof 4.1, and the compact-component spaces $X_j,Y_j$ are Banach by [F4], Proof 2.1, at orders four and two respectively. Here $X_j$ has zero trace when $\partial M_j\ne\varnothing$. Restriction identifies $X_\beta$ and $Y_\beta$ with these finite direct sums, with equivalent norms: the annular term involves only $\Sigma_0$, and the compact terms are finite chart norms. Smooth coordinate transitions compare these compact norms by the chain and product rules. Restriction decreases each chart supremum and seminorm; conversely, pairs lying in different components of a fixed compact chart subset have positive Euclidean separation, so their Hölder quotients are bounded by derivative suprema. Thus the full norm and the sum of the component norms bound each other by fixed constants. A Cauchy sequence in either full space is therefore Cauchy in each component space, has component limits there, and converges in the finite sum norm and hence in the original norm. The component limits glue across the disjoint open-and-closed components and preserve the zero boundary values. This proves completeness of both full-exterior spaces. [F1, F3, F4]

2.1 Let $H_j$ denote the mean-zero inverse of $\Delta_h$ on a closed component $M_j$. The estimate $\|H_j f\|_{C^{4,\alpha}(M_j)}\le C_j\|f\|_{C^{2,\alpha}(M_j)}$ for mean-zero $f$ is proved in [F4], Proof 4.1; it is not inferred merely from a kernel-and-range assertion. Put $P_j f=\mu_h(M_j)^{-1}\int_{M_j}f\,d\mu_h$, viewed as a constant function. Since $|P_j f|\le\|f\|_{C^0(M_j)}$, this is a bounded projection at both relevant Hölder orders. Use $H_j(I-P_j)$ as the closed-component block of $G$, the bounded compact Dirichlet inverse on each nonempty-boundary compact component, and the bounded end inverse on $\Sigma_0$. The finite sum and step 1.1 make $G:Y_\beta\to X_\beta$ bounded. The same componentwise reasoning makes $\Delta_h:X_\beta\to Y_\beta$ bounded. The inverse identities on each component give $\Delta_hG=I_{Y_\beta}-\Pi_Y$ and $G\Delta_h=I_{X_\beta}-\Pi_X$, where $\Pi_X,\Pi_Y$ apply $P_j$ on closed components and vanish elsewhere. They are bounded finite-rank projections. [F1, F3, F4, step 1.1]

3.1 Let $q$ be the number of closed compact components. Their constants are in the Laplacian kernel, and $G\Delta_h=I-\Pi_X$ implies that these are the entire kernel. The closed-component range assertion in [F4] gives $\Pi_Y\Delta_h=0$, while $\Delta_hG=I-\Pi_Y$ shows every element of $\ker\Pi_Y$ lies in the range. Hence $\operatorname{ran}\Delta_h=\ker\Pi_Y$, a closed subspace. The kernel and cokernel both have dimension $q$, since $\Pi_X$ and $\Pi_Y$ project onto the $q$ independent closed-component constants. Together with boundedness and the Banach property this proves Fredholmness and index zero, with all inner-boundary conditions retained. [F2, F4, step 1.1, step 2.1]

4.1 Multiplication by $V$ is a compact bounded linear map by [F5]. Step 1.1 establishes the Banach hypotheses on the full exterior, including its compact components, and step 3.1 establishes Fredholmness of the bounded Dirichlet Laplacian. Apply [F6] to this operator and the compact map $-M_V$, where $M_Vu=Vu$. The operator $\Delta_h-V$ is Fredholm with the same index zero. No sign assumption on $V$ was used. This proves all assertions. [F5, F6, step 1.1, step 3.1] ∎

### Source notes

The proof composes the existing scalar exhaustion inverse with the compact-block construction. In the latter, Proof 2.1 proves compact Hölder completeness and the bounded Dirichlet inverse, and Proof 4.1 proves the mean-zero Green estimate used here. The finite-component argument above completes the full-exterior Banach-space check. No weighted vector-operator theorem is used.


## Compact timelike-length bounds and local temporal functions

[Open item](item-thm-compact-temporal-function-input) · level 4


### Statement

Assume countable choice for the usual Lebesgue-measure convention. Let $B$ be an open subset of a smooth four-manifold without boundary, $g$ a $C^2$ time-oriented Lorentz metric, and $N$ a continuous timelike orientation field. Suppose every compact $C\subset B$ admits a finite $L_C$ bounding $L_g(c)=\int_a^b\sqrt{-g(\dot c,\dot c)}\,dt$ for every future Lipschitz curve $c:[a,b]\to C$ with $g(\dot c,\dot c)\le-\epsilon_c<0$ almost everywhere for some curve-dependent $\epsilon_c>0$. The curves, length and quantifiers have exactly the compact-length convention below. Then every compact $Q\subset B$ has an open neighborhood $O\subset B$ and a smooth real function $\tau$ on $O$ whose $g$-gradient is past timelike. For every compact $K\subset O$, the same $d\tau$ remains past-timelike after raising with any sufficiently small $C^0$ perturbation of $g$ on $K$, oriented by $N$. Here smallness means uniform coefficient closeness in a finite compact chart cover; no property of a deformed metric away from $K$ is inferred. The length hypothesis must hold for every compact subset of the open domain, not merely one selected family of curves.

### Statement references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[lem-author-89004136b63c-compact-neighborhood-localization](item-lem-author-89004136b63c-compact-neighborhood-localization)

[lem-author-89004136b63c-compact-length-restriction](item-lem-author-89004136b63c-compact-length-restriction)

[lem-author-89004136b63c-temporal-compact-margins](item-lem-author-89004136b63c-temporal-compact-margins)

[lem-author-89004136b63c-uniform-inverse-metric-continuity](item-lem-author-89004136b63c-uniform-inverse-metric-continuity)

[lem-author-89004136b63c-compact-temporal-persistence](item-lem-author-89004136b63c-compact-temporal-persistence)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

### Facts & Assumptions

[A1] Countable choice is assumed for the standard Lebesgue measure in the compact-length convention used in [F2] and step 1.1. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F1] The Lorentzian-object interface supplies its pointwise conventions: $g_p$ is symmetric and nondegenerate of signature $(-,+,+,+)$, timelike means $g_p(v,v)<0$, and $N_p$ selects the future timelike cone by $g_p(v,N_p)<0$; the opposite cone is past. The causal and inverse-metric interfaces supply the temporal-gradient and index-raising conventions. Only these pointwise definitions are used for the stated $C^2$ metric and continuous orientation field; the suppliers' smooth-field hypotheses and any stationarity requirement are not imposed. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[F2] Compact sets admit nested relatively compact neighborhoods, and the exact compact-length hypothesis restricts to open subdomains. [lem-author-89004136b63c-compact-neighborhood-localization](item-lem-author-89004136b63c-compact-neighborhood-localization) [lem-author-89004136b63c-compact-length-restriction](item-lem-author-89004136b63c-compact-length-restriction)

[F3] Compact margins, uniform inverse-metric continuity and temporal-covector persistence hold as locally proved in the three prerequisite helpers. [lem-author-89004136b63c-temporal-compact-margins](item-lem-author-89004136b63c-temporal-compact-margins) [lem-author-89004136b63c-uniform-inverse-metric-continuity](item-lem-author-89004136b63c-uniform-inverse-metric-continuity) [lem-author-89004136b63c-compact-temporal-persistence](item-lem-author-89004136b63c-compact-temporal-persistence)

[F4] Radu Lemma B.2 is an imported existence input under exactly the stated $C^2$, time-orientation and all-compact length hypotheses; the External input section gives its scope.

### External input

Radu, Lemma B.2 and (B.2), supplies the following external existence input: a $C^2$ time-oriented Lorentz metric on an open domain, with a uniform length bound on all uniformly timelike future Lipschitz curves in every compact subset (allowing a curve-dependent positive timelikeness constant), admits a smooth function with past timelike gradient on a neighborhood of each compact subset. This is imported as a source statement. No proof of this existence theorem is claimed locally.

### Proof

**Given:** The hypotheses in the Statement.

**Goal:** Establish the conclusions in the Statement.

1.1 Choose $Q\subset V\Subset W\Subset B$ using [F2]. Under [A1], the length hypothesis restricts to $W$ with exactly the same curve and compact-set quantifiers. Apply the precise external existence input [F4] on $W$ to the compact set $Q$. It supplies an open neighborhood $O$ of $Q$, restricted to $W$ if necessary, and a smooth $\tau$ whose $g$-gradient is past timelike. [A1, F1, F2, F4]

2.1 On any compact $K\subset O$, set $\alpha=d\tau$. Then $g^{-1}(\alpha,\alpha)<0$ and $\alpha(N)>0$. The three compact-control helpers in [F3] yield a coefficient threshold preserving these inequalities for the perturbed inverse metric and preserving that $N$ is timelike. Raising $d\tau$ with that metric gives the asserted past-timelike gradient on $K$. This proves both conclusions, with existence supplied externally and perturbation stability proved locally. [F1, F3, step 1.1] ∎


## Exterior exhaustion bounds for normalized Schrödinger solutions

[Open item](item-lem-author-58255dfd955f-exterior-exhaustion) · level 4


### Statement

On a connected exterior as in the exterior-data definition, let $V\ge0$ be smooth and let $u\in C^2(\Sigma^\circ)\cap C^1_{\mathrm{loc}}(\Sigma)$ solve $(\Delta_h-V)u=0$, vanish on $S$, and tend uniformly to $c>0$ as $r\to\infty$. Then $0<u\le c$ in the interior. If $S$ is nonempty, then $u<c$ there.

### Facts & Assumptions

**Given:** The end chart and compact core are those of [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data). The limit means that for every $\epsilon>0$, $|u-c|<\epsilon$ beyond a sufficiently large end sphere. Use compact comparison [lem-author-58255dfd955f-compact-comparison](item-lem-author-58255dfd955f-compact-comparison) and the strong minimum alternative [lem-author-58255dfd955f-strong-minimum](item-lem-author-58255dfd955f-strong-minimum).

### Proof

**Given:** The hypotheses and data in the Statement and Facts & Assumptions.

**Goal:** Establish the conclusions of the Statement.

**Proof technique:** direct.

1.1 Truncate the exterior at $r=R$. For $R$ sufficiently large, $u\ge c/2>0$ on the outer sphere and $u=0$ on $S$. Comparison applied to $-u$ gives $u\ge0$ on the truncation. Applied to $u-(c+\epsilon)$, whose image under $\Delta_h-V$ is $V(c+\epsilon)\ge0$, it gives $u\le c+\epsilon$ when the outer sphere satisfies that bound. Every fixed point belongs to all sufficiently large truncations. Taking $R$ large and then $\epsilon\downarrow0$ proves $0\le u\le c$. Components of a truncation meet its boundary; otherwise such a component would be a compact component of the connected exterior separated from its end. [given]

2.1 The end limit excludes $u\equiv0$, so the strong minimum alternative makes $u>0$. The nonnegative function $c-u$ satisfies $(\Delta_h-V)(c-u)=-Vc\le0$. If it vanished inside, the same alternative would make $u\equiv c$. This contradicts $u|_S=0$ when $S\ne\varnothing$. Thus the stated strict upper bound also holds. [step 1.1, given, algebra] ∎


## The entire target segment stays on the chronological boundary

[Open item](item-lem-author-2632702918ef-target-segment-boundary-containment) · level 4


### Statement

Under the same compact-target hypotheses, let $\gamma:[0,1]\to E$ be any future causal segment from $p$ to a point $c\in C$. Then $\gamma([0,1])\subset\partial_E I_E^-(C)$. In particular this holds for the null geodesic supplied by the compact-target null-segment lemma.

### Facts & Assumptions

[A1] Work in ZFC; the axiom of choice includes the countable and dependent choice assumptions of the causal suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The relations and metric-selected connection have the meanings in [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data).

[F2] The target is the surface defined in [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data).

[F3] The initial point does not belong to $I_E^-(C)$. [lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)

[F4] A future null geodesic segment from $p$ to some $c\in C$ exists under these hypotheses. [lem-author-2632702918ef-compact-target-null-segment](item-lem-author-2632702918ef-compact-target-null-segment)

[F5] Push-up gives $x\le y\ll z\Rightarrow x\ll z$ and $x\ll y\le z\Rightarrow x\ll z$. [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[F6] Chronological pasts are open. [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[F7] Sufficiently short geodesics with prescribed past timelike initial tangent exist smoothly. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F8] Every piecewise $C^1$ curve with future timelike tangents is a future timelike curve in the stipulated locally absolutely continuous class. [Curve calculus, clause (c)](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the asserted conclusion.

1.1 For $r=\gamma(s)$, causal restriction gives $p\le_Er\le_Ec$. If $r\in I_E^-(C)$, choose $c^{\prime}\in C$ with $r\ll_Ec^{\prime}$; push-up would imply $p\ll_Ec^{\prime}$, contradicting [F3]. Hence every such $r$ is outside $I_E^-(C)$. [F1, F2, F3, F5, given]

2.1 Fix $r=\gamma(s)$ and use [F7] in $E$ to choose a smooth geodesic $\eta$ with $\eta(0)=r$ and $\dot\eta(0)=-N_r$. At $0$ one has $g(\dot\eta,\dot\eta)<0$ and $g(\dot\eta,N)>0$. Smoothness of $g$, $N$ and $\eta$ makes these scalar functions continuous, so both strict inequalities persist on some $[0,\delta]$ within its domain. Thus $\dot\eta$ is past timelike there. For $0<\varepsilon<\delta$, put $r_\varepsilon=\eta(\varepsilon)$. The reversed segment $t\mapsto\eta(\varepsilon-t)$, $0\le t\le\varepsilon$, is smooth with future timelike tangent; [F8] makes it a future timelike curve in the stipulated class, so $r_\varepsilon\ll_Er$, and continuity gives $r_\varepsilon\to r$. Push-up and $r\le_Ec$ imply $r_\varepsilon\ll_Ec$, including when $r=c$. Thus $r$ is in the closure of $I_E^-(C)$ and outside this open set, which places it in its boundary. This argument applies to each $s$, and [F4] supplies the particular null segment. [step 1.1, F1, F4, F5, F6, F7, F8, A1] ∎


## Endpoint orthogonality without an acausal target assumption

[Open item](item-lem-author-2632702918ef-target-endpoint-orthogonality) · level 4


### Statement

Under the same compact-target hypotheses, let $\gamma:[0,1]\to E$ be a smooth nonconstant future null affine geodesic with $\gamma(0)=p$ and $\gamma(1)=c\in C$. Then $g(\dot\gamma(1),Y)=0$ for every $Y\in T_cC$. It suffices that $C$ be smooth and without boundary near $c$; no global acausality assumption on $C$ is needed.

### Facts & Assumptions

[A1] Work in ZFC; the axiom of choice implies the countable and dependent choice assumptions of the causal suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F1] The smooth metric, connection, causal relations and time orientation are those of [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data).

[F2] The target is a smooth embedded spacelike two-manifold without boundary. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F3] The initial point satisfies $p\notin I_E^-(C)$. [lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)

[F4] Such a smooth null affine segment exists under these hypotheses. [lem-author-2632702918ef-compact-target-null-segment](item-lem-author-2632702918ef-compact-target-null-segment)

[F5] Every point has arbitrarily small convex normal neighborhoods. [physics:thm-gr-convex-normal-neighborhoods](https://alphabetamath.cc/physics/item/thm-gr-convex-normal-neighborhoods)

[F6] On a convex normal neighborhood, $h(q)=g_r(\exp_r^{-1}(q),\exp_r^{-1}(q))$ is smooth and $dh_q(Y)=2g_q(P(r,q),Y)$, where $P(r,q)$ is the final tangent of the radial geodesic on $[0,1]$. [physics:lem-gr-position-vector-differential](https://alphabetamath.cc/physics/item/lem-gr-position-vector-differential)

[F7] A future timelike radial inverse vector in a convex normal neighborhood gives a future timelike geodesic. [physics:thm-gr-normal-neighborhood-causal-cone](https://alphabetamath.cc/physics/item/thm-gr-normal-neighborhood-causal-cone)

[F8] Causal then timelike reachability implies timelike reachability. [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[F9] At a point with future unit observer $n$, every nonzero future causal vector $w$ satisfies $g(n,w)<0$. A unit timelike vector $w$ is future-directed if and only if $g(n,w)<0$. These are clauses (1) and (3) of [physics:lem-gr-observer-pairing-with-future-causal-vectors](https://alphabetamath.cc/physics/item/lem-gr-observer-pairing-with-future-causal-vectors).

[F10] Every tangent vector to a smooth manifold is the velocity of a smooth curve through that point. Applied to the manifold $C$ without boundary, the curve is defined on an open interval about zero. [math:cor-every-tangent-vector-is-the-velocity-of-a-smooth-curve](https://alphabetamath.cc/item/cor-every-tangent-vector-is-the-velocity-of-a-smooth-curve)

[F11] A real function differentiable at an interior point of its domain has derivative zero there if it has a local extremum there. [math:thm-fermat-interior-extremum](https://alphabetamath.cc/item/thm-fermat-interior-extremum)

[F12] For a smooth real function $f$, $df_x(V)=V([f])$; the velocity derivation of a smooth curve $\eta$ acts by $\dot\eta(0)([f])=(f\circ\eta)'(0)$. Thus $df_{\eta(0)}(\dot\eta(0))=(f\circ\eta)'(0)$. [math:def-differential-of-a-smooth-real-valued-function](https://alphabetamath.cc/item/def-differential-of-a-smooth-real-valued-function) [math:def-velocity-derivation-of-a-smooth-curve](https://alphabetamath.cc/item/def-velocity-derivation-of-a-smooth-curve)

[F13] A future null affine geodesic is a smooth nonconstant curve whose tangent is nonzero, future-directed and null and satisfies $D_s\dot\gamma=0$ at every interior parameter. Only the geodesic definition is used; no completeness condition is imposed. [physics:def-gr-fx-future-null-geodesic-completeness](https://alphabetamath.cc/physics/item/def-gr-fx-future-null-geodesic-completeness)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the asserted conclusion.

1.1 Choose by [F5] a strictly convex normal neighborhood $B\subset E$ of $c$ and $s_0\in(0,1)$ sufficiently close to $1$ that the tail of $\gamma$ from $r=\gamma(s_0)$ to $c$ lies in $B$. Use the inverse domains selected by $B$ and put $v(q)=\exp_r^{-1}(q)$ and $h(q)=g_r(v(q),v(q))$ for $q\in B$. By the affine geodesic definition in [F13] and uniqueness of the joining geodesic in [F5], its radial segment to $c$ is $t\mapsto\gamma(s_0+(1-s_0)t)$, so $v(c)=(1-s_0)\dot\gamma(s_0)$ is nonzero future null and $h(c)=0$. Normalize $n_r=N_r/\sqrt{-g_r(N_r,N_r)}$, so $g_r(n_r,n_r)=-1$ and $g_r(n_r,N_r)<0$; this is a future unit observer. Clause (1) of [F9] gives $g_r(v(c),n_r)<0$. By continuity, restrict to a neighborhood $V\subset B$ of $c$ where $g_r(v(q),n_r)<0$. If $q\in V\cap C$ had $h(q)<0$, then $w=v(q)/\sqrt{-h(q)}$ would be unit timelike with $g_r(w,n_r)<0$. Clause (3) of [F9] makes $w$, and hence its positive multiple $v(q)$, future-directed. By [F7] the radial geodesic in $B\subset E$ gives $r\ll_E q$. The initial segment of $\gamma$ gives $p\le_E r$, so [F8] gives $p\ll_E q$, contradicting [F3]. Consequently $h|_{V\cap C}\ge0$ and $h(c)=0$. The causal suppliers are used with the choice assumptions in [A1]. [A1, F1, F2, F3, F5, F6, F7, F8, F9, F13, given, algebra]

2.1 Fix $Y\in T_cC$. By [F10], since $C$ is smooth without boundary, there is a smooth curve $\eta:(-\varepsilon,\varepsilon)\to C$ with $\eta(0)=c$ and $\dot\eta(0)=Y$. Shrink $\varepsilon>0$ so that $\eta$ lies in $V\cap C$. The smooth real function $f=h\circ\eta$ has a local minimum at the interior parameter $0$ by step 1.1, so [F11] gives $f'(0)=0$. Regard $Y$ as its ambient tangent under the embedded inclusion; [F12] identifies $f'(0)=dh_c(Y)$. By [F6], $0=dh_c(Y)=2g_c(P(r,c),Y)$. The radial segment identified in step 1.1 has terminal tangent $P(r,c)=(1-s_0)\dot\gamma(1)$. Dividing by $2(1-s_0)>0$ proves $g_c(\dot\gamma(1),Y)=0$ for every $Y$. Only endpoints near $c$ were varied, so no global acausality of $C$ is required; [F4] supplies the existence of a segment under the compact-target hypotheses. [step 1.1, F1, F2, F4, F6, F10, F11, F12, algebra] ∎


## Combining the collar and end barriers into interior compact confinement

[Open item](item-lem-author-eb8e266b8b92-interior-compact-confinement) · level 4


### Statement

Assume the Axiom of Choice. Let $\overline S$ have the stationary ADM, smooth-boundary and compact-boundary collar data of the collar-barrier lemma, and the proper radius and smooth extensions of the proper-radius lemma. Assume both lemmas' stated estimates. Every causal curve on a bounded section-time interval containing $v_0$ has its spatial image in a compact subset of the interior $S$. More precisely, if $|v-v_0|\le T$, choose $\eta=\tfrac12 b(x(v_0))e^{-CT}>0$ and $m=R(x(v_0))+C_RT$ with the constants and the truncated collar coordinate $b$ of those lemmas. The set $K=\{R\le m\}\setminus\{\rho<\eta\}$ contains the image and is compact in $S$; the removed set denotes the collar neighborhood including the boundary.

### Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[lem-author-eb8e266b8b92-collar-nonarrival](item-lem-author-eb8e266b8b92-collar-nonarrival)

[lem-author-eb8e266b8b92-proper-radius-control](item-lem-author-eb8e266b8b92-proper-radius-control)

[math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

[math:thm-the-interior-is-an-open-smooth-n-manifold](https://alphabetamath.cc/item/thm-the-interior-is-an-open-smooth-n-manifold)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

### Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice is assumed for the inherited interfaces. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F2] The collar barrier gives $b(x(v))\ge b(x(v_0))e^{-C|v-v_0|}$, with $b=\rho$ close to the boundary and constant farther away. [lem-author-eb8e266b8b92-collar-nonarrival](item-lem-author-eb8e266b8b92-collar-nonarrival)

[F3] Proper-radius control gives $R(x(v))\le R(x(v_0))+C_R|v-v_0|$, and every sublevel of $R$ is compact in the manifold with boundary. [lem-author-eb8e266b8b92-proper-radius-control](item-lem-author-eb8e266b8b92-proper-radius-control)

[F4] A closed subspace of a compact topological space is compact; no metric hypothesis is required. [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

[F5] The interior $S=\operatorname{Int}\overline S$ is open in $\overline S$ and carries the smooth structure of restricted charts. Its topology is the subspace topology: open sets are traces of ambient open sets, and because $S$ is open these traces are also open in $\overline S$. [math:thm-the-interior-is-an-open-smooth-n-manifold](https://alphabetamath.cc/item/thm-the-interior-is-an-open-smooth-n-manifold) [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[F6] For a subset of any topological space with the subspace topology, compactness is equivalent to the finite-subcover property for families of ambient open sets covering that subset, including the empty-subset case. [math:lem-compactness-of-a-subspace-is-ambient](https://alphabetamath.cc/item/lem-compactness-of-a-subspace-is-ambient)

### Proof

1.1 The radius estimate places the entire image in $\{R\le m\}$. The collar estimate places it outside $\{\rho<\eta\}$, since within that neighborhood $b=\rho<\eta$ contradicts $b(x(v))\ge2\eta$. The chosen $\eta$ is less than the truncation threshold, so the removed collar neighborhood is unambiguously defined. [F2, F3, algebra]

2.1 Let $C_m=\{R\le m\}$ and let $U_\eta=\{\rho<\eta\}$ denote the stated collar neighborhood. Under the supplied collar diffeomorphism, $U_\eta$ is the image of $[0,\eta)\times B$, open relative to $[0,\epsilon)\times B$; hence it is open in $\overline S$ and contains the entire boundary $B$. Thus $K=C_m\setminus U_\eta$ is closed in the compact space $C_m$ and lies in $S$. The closed-subspace theorem makes $K$ compact with the topology induced from $C_m$. [given, F2, F3, F4, step 1.1]

3.1 The restricted charts identify the topology of $S$ with its open subspace topology in $\overline S$. Consequently, if $V$ is open in $S$, it is open in $\overline S$, and $V\cap C_m$ is open in $C_m$. For any family of open subsets of $S$ covering $K$, their traces on $C_m$ cover $K$. Compactness from step 2.1 and the ambient-cover criterion in $C_m$ give finitely many of those traces covering $K$, so the corresponding original sets also cover $K$. The same ambient-cover criterion in $S$ now proves that $K$ is compact in $S$. Together with step 1.1 this proves interior compact confinement. [F5, F6, step 1.1, step 2.1] ∎



## Differential exclusion of a large interior weighted angle maximum

[Open item](item-lem-author-fd2999663761-cutoff-interior-maximum-exclusion) · level 4


### Statement

For the temporal angle data, suppose $\alpha\ge a_0>0$. On $\{\tau>0,v>2\}$ assume $\Delta_\Sigma\log v\ge\tfrac14|\nabla_\Sigma\log v|^2-Cv^2$ and $|\Delta_\Sigma\tau|\le Cv^2$ with $C\ge1$. If $T>0$, choose $\mu>4$ so that $(\mu^2/4-\mu)a_0^2\ge2C(T^2+\mu T)$. Then $\tau^\mu v$ has no local maximum in the interior positive-height region where $v>2$. The logarithmic inequality may be obtained from the hyperbolic-angle inequality by the conversion lemma.

### Facts & Assumptions

[F1] The tangential gradient identity gives $|\nabla_\Sigma\tau|^2\ge a_0^2(v^2-1)$. [lem-author-fd2999663761-temporal-tangent-gradient](item-lem-author-fd2999663761-temporal-tangent-gradient)

[F2] The operators and height bound $\tau\le T$ are those in [def-author-fd2999663761-temporal-angle-data](item-def-author-fd2999663761-temporal-angle-data); the conversion from $\eta=\operatorname{arcosh}v$ to $\log v$ is [lem-author-fd2999663761-logarithmic-angle-conversion](item-lem-author-fd2999663761-logarithmic-angle-conversion). The two differential inequalities are assumptions of this lemma.

[F3] In an open Euclidean coordinate domain, a $C^2$ function at an interior local maximum has zero differential and a negative semidefinite matrix of second partial derivatives. [math:lem-negative-semidefinite-hessian-at-an-interior-local-maximum](https://alphabetamath.cc/item/lem-negative-semidefinite-hessian-at-an-interior-local-maximum) The metric-dual gradient and coordinate identity $(\operatorname{Hess}_h f)_{ij}=\partial_i\partial_j f-\Gamma^k{}_{ij}\partial_k f$ are [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas). The positive-trace convention is $\Delta_\Sigma f=\operatorname{tr}_h\operatorname{Hess}_h f$. [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)

[F4] Apply the scalar sum, product, quotient and chain rules in each coordinate. [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules) For $s>0$, $(\log s)^{\prime}=1/s$ and $\log s=\int_1^s dt/t$, so the logarithm is smooth and strictly increasing there. [math:thm-logarithm-derivative-and-integral](https://alphabetamath.cc/item/thm-logarithm-derivative-and-integral)

[F5] For $a>0$ and $r\in\mathbb R$, define $a^r=\exp(r\log a)$ as in [math:def-real-power](https://alphabetamath.cc/item/def-real-power). The exponential maps $\mathbb R$ into $(0,\infty)$ and $\log(\exp s)=s$ for every real $s$, as recorded in [math:def-natural-logarithm](https://alphabetamath.cc/item/def-natural-logarithm); hence $a^r>0$ and $\log(a^r)=r\log a$. For $x,y>0$, $\log(xy)=\log x+\log y$ by [math:thm-natural-logarithm-laws](https://alphabetamath.cc/item/thm-natural-logarithm-laws).

### Proof

**Given:** The displayed bounds and choice of $\mu$. **Goal:** Exclude an interior local maximum with $v>2$.

1.1 Suppose $p$ is an interior local maximum of $\tau^\mu v$ with $\tau(p)>0$ and $v(p)>2$. In a neighborhood with these strict inequalities put $f=\log v+\mu\log\tau$. By [F5], $\tau^\mu>0$ and $f=\log(\tau^\mu v)$ there. By [F4], $f$ is smooth and has a local maximum at $p$. Apply the Euclidean extremum test in [F3] to its coordinate representation in an interior chart: $df(p)=0$ and the matrix $(\partial_i\partial_j f)(p)$ is negative semidefinite. The connection term in the coordinate Hessian formula vanishes because $df(p)=0$. Thus $\operatorname{Hess}_h f(p)$ is negative semidefinite, $\nabla_\Sigma f(p)=0$, and $\Delta_\Sigma f(p)=\sum_{a=1}^3\operatorname{Hess}_h f(e_a,e_a)\le0$ for an $h_p$-orthonormal basis $(e_a)$. [F2, F3, F4, F5, given, algebra]

2.1 By the coordinate scalar rules and the Hessian and trace formulas in [F3] and [F4], $\nabla_\Sigma\log\tau=\nabla_\Sigma\tau/\tau$ and $\Delta_\Sigma\log\tau=\Delta_\Sigma\tau/\tau-|\nabla_\Sigma\tau|^2/\tau^2$. At $p$, step 1.1 therefore gives $\nabla_\Sigma\log v=-\mu\nabla_\Sigma\tau/\tau$. Substituting this into the assumed inequalities gives $0\ge\Delta_\Sigma f\ge(\mu^2/4-\mu)|\nabla_\Sigma\tau|^2/\tau^2-Cv^2(1+\mu/\tau)$. [F2, F3, F4, step 1.1, given, algebra]

3.1 Multiply by $\tau^2>0$ and use [F1]. Put $A=T^2+\mu T>0$. The lower bound from step 2.1 is at least $2CA(v^2-1)-C(\tau^2+\mu\tau)v^2\ge CA(v^2-2)>0$, since $0<\tau\le T$ and $v>2$. This contradicts $\Delta f\le0$. Such a $\mu$ exists because the left side of its required inequality is quadratic in $\mu$ and the right side is affine. [F1, F2, step 1.1, step 2.1, algebra] ∎



## Boundary-constant-preserving smooth approximation

[Open item](item-lem-author-423fe0348a31-fixed-boundary-approximation) · level 4


### Statement

Work in ZFC. Let $(R,k)$ be a compact smooth Riemannian region (a manifold with boundary) of dimension $n\ge0$ whose boundary is $B_-\sqcup B_+$, with both parts closed and disjoint. Let $u:R\to\mathbb R$ be Lipschitz, equal to constants $c_-$ and $c_+$ respectively on open neighborhoods of these parts. There exist smooth $u_j$ on $R$, all equal to those same constants on fixed smaller boundary neighborhoods, with $u_j\to u$ uniformly and in metric $W^{1,1}(R)$. Here smoothness includes smooth local extension in boundary charts. Lipschitz means a single finite bound with respect to intrinsic Riemannian distance within each connected component; the distance between distinct components is $+\infty$. Metric first-Sobolev convergence here means
$$\int_R\bigl(|u_j-u|+|du_j-du|_k\bigr)\,dV_k\longrightarrow0,$$
where $du$ is the almost-everywhere coordinate weak differential, $|\cdot|_k$ is the dual metric norm, and $dV_k$ is the Riemannian volume density. In dimension zero differentials vanish and each point has volume one; for empty $R$ the supremum error and integral are zero.

### Facts & Assumptions

[F1] Smooth relative cutoffs may equal one near a compact boundary set and have support inside its prescribed open neighborhood. Support is the closure in $R$ of the nonzero locus. [lem-author-423fe0348a31-finite-relative-cutoffs](item-lem-author-423fe0348a31-finite-relative-cutoffs)

[F2] A compactly supported interior Lipschitz function has simultaneous uniform and metric first-Sobolev smooth approximation with all supports in one fixed compact interior set, in every dimension $n\ge0$, under ZFC. Its integral convergence is exactly the one displayed in the Statement. [lem-author-423fe0348a31-finite-atlas-smoothing](item-lem-author-423fe0348a31-finite-atlas-smoothing)

[F3] In dimension three, metric weak gradients and normalized cut areas retain the fixed Riemannian conventions; no cut-area input is needed for the approximation construction. [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[F4] Locally Lipschitz functions have coordinate-independent weak differentials on the interior. The metric Sobolev integral uses the dual norm and Riemannian volume density; dimension zero has zero differentials and unit point volumes. These conventions and coordinate norm comparisons are supplied by [lem-author-423fe0348a31-chart-sobolev-comparison](item-lem-author-423fe0348a31-chart-sobolev-comparison).

[F5] The boundary smooth structure uses compatible half-space charts and smooth local Euclidean extensions; $k$ is a smooth positive-definite tensor. Intrinsic distance is the infimum of piecewise $C^1$ curve lengths, with cross-component value $+\infty$; length is the integral of metric speed. [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold) [math:def-extended-riemannian-distance-on-a-disconnected-manifold](https://alphabetamath.cc/item/def-extended-riemannian-distance-on-a-disconnected-manifold) [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)

[F6] The induced dual metric is smooth, so the squared dual norm of a smooth differential is continuous. Continuous real-valued functions on a nonempty compact space attain finite bounds (claim 2). The half-space chain rule holds for local smooth extensions, and the scalar fundamental theorem evaluates a $C^1$ function increment by the integral of its derivative, including one-sided endpoint derivatives. [math:prop-riemannian-metrics-induce-metrics-on-dual-tensor-and-exterior-bundles](https://alphabetamath.cc/item/prop-riemannian-metrics-induce-metrics-on-dual-tensor-and-exterior-bundles) [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps) [math:prop-chain-rule-for-smooth-half-space-maps](https://alphabetamath.cc/item/prop-chain-rule-for-smooth-half-space-maps) [math:thm-ftc-second-part](https://alphabetamath.cc/item/thm-ftc-second-part)

[A1] Work in ZFC, including the Axiom of Choice inherited from the smoothing supplier and sufficient for the chart supplier's Countable Choice assumption. Its use is the approximation in step 3.1 and the weak-differential calculus there. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### Proof

**Given:** The hypotheses and conventions in the Statement.

**Goal:** Construct the smooth approximants with exact fixed boundary values and both stated convergences.

1.1 Write $O_-$ and $O_+$ for the open neighborhoods where $u$ has the two prescribed constant values. The set $V=O_+\setminus B_-$ is open and contains the compact set $B_+$. By [F1], take a smooth $\chi_+:R\to[0,1]$ supported in $V$ and equal to one on an open neighborhood $U_+$ of $B_+$, shrinking $U_+$ inside $O_+$. Put $U_-=O_-\setminus\operatorname{supp}\chi_+$; this is an open neighborhood of $B_-$. Set $h=c_-+(c_+-c_-)\chi_+$. Then $h$ is smooth up to the boundary, equals $c_-$ on $U_-$ and $c_+$ on $U_+$, and $v=u-h$ vanishes on $U_-\cup U_+$. [given, F1, F5, construct]

2.1 The smooth dual metric and compactness give a finite $M\ge1$ with $|dh|_k\le M$ on $R$; for empty $R$ take $M=1$. For any piecewise $C^1$ curve $\gamma$ joining $p$ to $q$, refine into finitely many chart pieces. The half-space chain rule, using smooth local extensions also when a piece touches the boundary, gives $|(h\circ\gamma)'|=|dh(\dot\gamma)|\le M|\dot\gamma|_k$. The scalar fundamental theorem on each piece and the triangle inequality therefore give $|h(p)-h(q)|\le M L_k(\gamma)$. Taking the infimum over curves gives $|h(p)-h(q)|\le M d_k(p,q)$ on each component. Distinct components impose no finite-distance constraint. Thus $h$ is Lipschitz under the convention in the Statement, and if $u$ has Lipschitz bound $L$, then $v=u-h$ has bound $L+M$. Its support is closed in compact $R$ and disjoint from the open neighborhood $U_-\cup U_+$ of all of $\partial R$, hence is compactly contained in $R^\circ$. [given, F1, F5, F6, step 1.1, algebra]

3.1 Apply [F2], under [A1], to the Lipschitz $v$ from step 2.1, obtaining smooth $v_j$ supported in a single compact $K\subset R^\circ$, with uniform error tending to zero and $\int_R(|v_j-v|+|dv_j-dv|_k)\,dV_k\to0$. Define $u_j=h+v_j$. On the fixed open neighborhoods $U_-\setminus K$ and $U_+\setminus K$ of the respective boundary parts, every $u_j$ has the exact prescribed constant. Weak differentiation is linear: the coordinate test identities add, so $du_j-du=dv_j-dv$ almost everywhere, while $u_j-u=v_j-v$ pointwise. Thus the uniform errors and the displayed Sobolev errors are exactly those of $v_j-v$ and tend to zero. The sum is smooth up to the boundary because $h$ is, and $v_j$ vanishes near it. The conventions of [F4] include dimension zero and the empty case, completing all assertions. [F2, F4, F5, A1, step 1.1, step 2.1, algebra] ∎



## Scalar metric Jacobian and weak-gradient identification

[Open item](item-lem-author-423fe0348a31-scalar-metric-jacobian) · level 4


### Statement

Work in ZFC. For a real-valued Lipschitz function $u$ on a smooth Riemannian three-region $(R,k)$, at every differentiability point the scalar coarea Jacobian of $du:T_xR\to\mathbb R$ is $J_1u=|du|_k=|\nabla_k u|$. At points with $du=0$ the value is zero. This is the one-dimensional-target (rank at most one) Jacobian, not an endpoint-map two-dimensional area Jacobian.

Precisely, for a linear functional $\ell:T_xR\to\mathbb R$, let $\ell^\sharp$ be the unique vector satisfying $k_x(\ell^\sharp,v)=\ell(v)$ for every $v\in T_xR$, and put $|\ell|_k=\sqrt{k_x(\ell^\sharp,\ell^\sharp)}$. Its adjoint $\ell^*:\mathbb R\to T_xR$ is characterized by $k_x(\ell^*t,v)=t\ell(v)$, with the usual Euclidean inner product on $\mathbb R$. Define the scalar metric coarea Jacobian by $J_1(\ell):=\sqrt{\det(\ell\ell^*)}$, where the determinant is on the one-dimensional target, and set $J_1u(x)=J_1(du_x)$ at differentiability points. There $\nabla_k u=(du_x)^\sharp$; almost everywhere this agrees with the metric weak gradient.

### Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice. This supplies the countable choice required by the Lipschitz differentiability and weak-derivative input used in step 2.1; the finite-dimensional calculation in step 1.1 needs no choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The metric is positive definite, so its matrix is invertible and defines the metric dual vector, dual norm and gradient used above. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[F2] Under the choice setting in [A1], the Lipschitz height has almost-everywhere chart derivatives equal to its weak derivatives; areas have the normalized metric Hausdorff convention. [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

### Proof

**Given:** The hypotheses and definitions in the Statement.

**Goal:** Prove the scalar Jacobian identity and its almost-everywhere weak-gradient interpretation.

1.1 For a linear functional $\ell$ on a finite-dimensional real inner-product space, the inverse metric gives a unique $\ell^\sharp$ with $k(\ell^\sharp,v)=\ell(v)$. The vector $t\ell^\sharp$ satisfies $k(t\ell^\sharp,v)=t\ell(v)$, hence $\ell^*t=t\ell^\sharp$. Thus $(\ell\ell^*)t=t\ell(\ell^\sharp)=t k(\ell^\sharp,\ell^\sharp)$, and the defining determinant on $\mathbb R$ gives $J_1(\ell)=\sqrt{k(\ell^\sharp,\ell^\sharp)}=|\ell|_k$. This also gives zero when $\ell=0$. [F1, given, algebra]

2.1 At each differentiability point take $\ell=du_x$ with the inner product $k_x$. The definitions and step 1.1 give $J_1u(x)=|du_x|_k=|\nabla_k u(x)|$. Under [A1], the weak and classical differential agree almost everywhere by [F2], so this is also the weak-gradient norm almost everywhere and identifies the scalar coarea integrand. No multiplicity or endpoint-map hypothesis is part of this calculation. [A1, F1, F2, step 1.1, algebra] ∎


## Exterior Schrödinger maximum principles, Hopf growth and Harnack

[Open item](item-lem-exterior-lapse-maximum-and-boundary-control) · level 5


### Statement

On a connected smooth Riemannian exterior $(\Sigma,h)$ with compact smooth boundary $S$, let $V\ge0$ be smooth and let $u\in C^2(\Sigma^\circ)\cap C^1_{\mathrm{loc}}(\Sigma)$ satisfy $(\Delta_h-V)u=0$, $u|_S=0$, and $u\to c>0$ uniformly at infinity. Then $0<u\le c$ in the interior; when $S\ne\varnothing$, $u<c$ there. The metric inward unit normal derivative is strictly positive at $S$. On a sufficiently small fixed compact boundary collar, $u\ge c_0\rho$ for $c_0>0$, where $\rho$ is the collar coordinate or the metric distance to $S$.

Positive solutions admit multiplicative interior Harnack comparison on fixed compact connected interior subsets. The constants are uniform for families with a common finite chart cover and uniform metric ellipticity, metric coefficient and bounded-potential controls there. A uniform absolute lower bound additionally requires a positive uniform anchor value. No uniformity is asserted when the metric degenerates, the cover loses control, or the only normalization is an individual end limit.

### Facts & Assumptions

**Given:** Work in ZFC, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) and the choice uses inherited through the declared suppliers. The exterior, end limit and Laplacian convention are those of [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data). The normal is the unit vector orthogonal to $S$ pointing into $\Sigma$; the gradient formulation fixes this notion. A collar coordinate and its distance version are specified in [lem-author-58255dfd955f-boundary-linear-growth](item-lem-author-58255dfd955f-boundary-linear-growth).

[F1] Exterior bounds and strict interior positivity are [lem-author-58255dfd955f-exterior-exhaustion](item-lem-author-58255dfd955f-exterior-exhaustion). Boundary normal positivity and fixed-collar linear growth are [lem-author-58255dfd955f-boundary-linear-growth](item-lem-author-58255dfd955f-boundary-linear-growth).

[F2] Bounded-potential multiplicative Harnack is [lem-author-58255dfd955f-local-potential-harnack](item-lem-author-58255dfd955f-local-potential-harnack), with its actual coefficient contract. Finite propagation is [lem-author-58255dfd955f-compact-harnack-chain](item-lem-author-58255dfd955f-compact-harnack-chain), and absolute uniform positivity from an anchor is [lem-author-58255dfd955f-anchored-uniform-positivity](item-lem-author-58255dfd955f-anchored-uniform-positivity).

### Proof

**Given:** The hypotheses and data in the Statement and Facts & Assumptions.

**Goal:** Establish the conclusions of the Statement.

**Proof technique:** direct.

1.1 Apply [F1] with the given boundary values and the uniform end limit. Its exhaustion argument first supplies nonnegativity and the upper bound; the strong minimum argument excludes an interior zero. Its strict upper clause applies when the boundary is nonempty. This proves all asserted interior bounds. [given, F1]

2.1 If $S$ is empty, the boundary assertions are vacuous. Otherwise apply the boundary result in [F1] to this positive solution. Smoothness of the boundary gives tangent balls in boundary charts, and the variable-coefficient barrier uses the actual nonpositive zeroth-order coefficient $-V$. It yields the strict inward normal derivative and, by compactness and $C^1$ continuity, a positive linear bound on one small collar. [step 1.1, F1]

3.1 In each of the finitely many interior chart balls use [F2]. In particular the potential belongs to the operator, not to an additive uncontrolled forcing term. The finite chain compares arbitrary values on the compact connected set. Its constants depend only on the chosen cover and the displayed coefficient controls; the anchor result identifies precisely the extra normalization needed for absolute positivity in a family. This proves the remaining statements and qualifications. [F2, given] ∎

### Source notes

The prior Laplacian-only Hopf supplier and additive-forcing Harnack supplier are not used outside their interfaces. The boundary and maximum arguments are supplied locally in the explicit helper chain. The outstanding bounded-potential Harnack theorem is an honestly labeled independent external input in the Harnack chain; its underlying iteration proof is not claimed as locally reconstructed. This resolution concerns a generated prerequisite draft, and asserts no defect in the original article or its literature.


## Temporal cutoff estimate for normals to maximal hypersurfaces

[Open item](item-thm-maximal-normal-angle-estimate-input) · level 5


### Statement

Let $g_j$ be smooth time-oriented Lorentz metrics of signature $(-,+,+,+)$ on a common smooth four-manifold, converging in $C^2$ to a Lorentz metric near a fixed compact set $Q$. Use a common time orientation and a fixed finite coordinate cover near $Q$, with uniformly bounded metric $C^2$ and inverse-metric $C^0$ norms. Let $\tau$ be a fixed smooth function, with past-directed timelike $g_j$-gradient and $\alpha_j^2=-g_j^{-1}(d\tau,d\tau)\ge a_0^2>0$ on $Q\cap\{\tau\ge0\}$. Let $\Sigma_j$ be smooth spacelike maximal hypersurfaces, smooth up to their actual boundaries, with future unit normals $n_j$, such that the entire portions $\Sigma_j\cap\{\tau\ge0\}$ are compact and contained in $Q$. Set $V_j=-\alpha_j^{-1}\operatorname{grad}_{g_j}\tau$, $v_j=-g_j(n_j,V_j)$ and $\tau_{\max}=\max_Q\max(\tau,0)$ when $Q$ is nonempty, and $\tau_{\max}=0$ when $Q=\varnothing$. There is $\mu>4$, depending only on $a_0$, the uniform metric and inverse bounds and $\|\tau\|_{C^3(Q)}$ in that cover, such that $\sup_{\Sigma_j\cap\{\tau>0\}}\tau^\mu v_j\le2\max\{2\tau_{\max}^{\mu},\ \sup_{\partial\Sigma_j\cap\{\tau>0\}}\tau^\mu v_j\}$. A supremum over an empty set is zero. In particular the boundary supremum is retained unless it is empty or separately bounded. No uniform bound on the normals is assumed in advance.

### Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The meanings of spacelike, future normal and maximality are [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data); past timelike gradient and temporal function have the convention of [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data). The temporal angle, operator and compact-portion conventions are [def-author-fd2999663761-temporal-angle-data](item-def-author-fd2999663761-temporal-angle-data).

[F2] The temporal gradient identity is [lem-author-fd2999663761-temporal-tangent-gradient](item-lem-author-fd2999663761-temporal-tangent-gradient); the conversion of a hyperbolic-angle differential inequality to the logarithmic one on $\{v>2\}$ is [lem-author-fd2999663761-logarithmic-angle-conversion](item-lem-author-fd2999663761-logarithmic-angle-conversion).

[F3] The compact weighted maximum and interior exclusion lemmas are [lem-author-fd2999663761-compact-weighted-maximum](item-lem-author-fd2999663761-compact-weighted-maximum) and [lem-author-fd2999663761-cutoff-interior-maximum-exclusion](item-lem-author-fd2999663761-cutoff-interior-maximum-exclusion).

[F4] Use the exact external differential estimate in the following External input section, under the complete geometric hypotheses of the Statement.

[F5] Positive-base real powers are $a^r=\exp(r\log a)$ for $a>0$ and real $r$; the supplementary convention is $0^r=0$ for $r>0$. [math:def-real-power](https://alphabetamath.cc/item/def-real-power)

### External input

Import (B.11) of Radu, Appendix B: with the geometric hypotheses of the Statement and $\eta_j=\operatorname{arcosh}v_j$, there is a uniform $C\ge1$ such that on $\{v_j>2\}$, $\Delta_{\Sigma_j}\eta_j\ge\coth\eta_j(\tfrac14|\nabla_{\Sigma_j}\eta_j|^2-Cv_j^2)$ and $|\Delta_{\Sigma_j}\tau|\le Cv_j^2$. Its constant depends only on $a_0$, the stated uniform coordinate metric/inverse bounds and the $C^3$ norm of $\tau$. This is an external geometric differential estimate, not a local reconstruction. The source derives it from (B.8)–(B.10) using Gauss–Codazzi, maximality and the trace-free eigenvalue bound in three tangent dimensions; the present proof imports that step with all its hypotheses.

### Proof

**Given:** The sequence, compact portions and temporal function in the Statement, with imported differential estimate [F4].

**Goal:** Prove the stated uniform weighted angle bound.

1.1 The temporal data are well defined by [F1]. If $\tau_{\max}=0$, including when $Q=\varnothing$, containment of the entire nonnegative-height portions in $Q$ implies that the positive-height sets are empty, so the conclusion holds for any fixed $\mu>4$ by the zero-supremum convention. Otherwise put $T=\tau_{\max}>0$. By [F4] choose a common $C\ge1$ for both differential estimates. By [F2] its hyperbolic-angle inequality gives $\Delta\log v_j\ge\tfrac14|\nabla\log v_j|^2-Cv_j^2$ on $\{v_j>2\}$, and $|\nabla\tau|^2\ge a_0^2(v_j^2-1)$. [F1, F2, F4, F5, given]

2.1 Choose a common $\mu>4$ so that $(\mu^2/4-\mu)a_0^2\ge2C(T^2+\mu T)$. The exclusion lemma [F3] rules out a local interior maximum of $\tau^\mu v_j$ at positive height with $v_j>2$. The compact maximum lemma [F3] then gives $\sup\tau^\mu v_j\le\max\{2T^\mu,B_j\}\le2\max\{2T^\mu,B_j\}$, where $B_j$ is exactly the actual boundary supremum in the Statement. The choice of $\mu$ uses only the uniform geometric constant, $a_0$ and $T$, itself bounded by the specified $C^3$ norm. This proves the stated bound for every $j$ with all boundary terms intact. [F2, F3, F5, step 1.1, algebra] ∎

### Source notes

The scalar argument follows the maximum-principle method of Radu, Appendix B, (B.11)–(B.12), using the explicitly proved conversion to log v and retaining the source’s conservative stated constant. The independent source is not the article under study. No graph existence, temporal-function existence, boundary-angle estimate or tensor-identity reconstruction is asserted. The compact sets must contain the entire nonnegative-height portions; replacing them by intersections with an arbitrary compact Q would introduce extra boundary terms.


## Stationary ADM speed bounds and Cauchy sections

[Open item](item-lem-stationary-adm-causal-completeness-input) · level 5


### Statement

Assume the Axiom of Choice. Let $\overline\Sigma$ be a connected smooth three-manifold with compact boundary $B$ and interior $\Sigma^\circ$. Let $h$ extend to a smooth positive-definite metric on $\overline\Sigma$, complete up to its compact boundary, meaning that its intrinsic metric with the boundary included is complete. Let $N:\overline\Sigma\to\mathbb R$ be a smooth real-valued function and $X$ a smooth tangent vector field on $\overline\Sigma$, with $N>0$ in the interior. On $E=\mathbb R_v\times\Sigma^\circ$ put $g=-N^2dv^2+h_{ij}(dx^i+X^idv)(dx^j+X^jdv)$, oriented by $n=N^{-1}(\partial_v-X)$; all coefficients are independent of $v$.

Supply a collar $[0,\epsilon)\times B$ with coordinate $\rho$, and constants with $N\le A\rho$, $|X(\rho)|\le A\rho$, and $|d\rho|_h\le A$ there. Supply a smooth nonnegative proper exhaustion $R$ of $\overline\Sigma$: each $\{R\le m\}$ is compact. Outside a compact core require $|dR|_h(N+|X|_h)\le C$. A sufficient end-coordinate realization is to provide a compact core with finitely many ends $[r_0,\infty)\times F_j$, compact $F_j$, let $R$ equal their unbounded radial coordinates sufficiently far out, and impose this estimate there. A bounded function of radius is insufficient. If $B$ is empty, omit the collar conditions.

Then each inextendible causal curve, with locally absolutely continuous nonzero causal velocity almost everywhere, has $v$-image all of $\mathbb R$. Consequently every $v$-level is a spacelike Cauchy hypersurface, and $(E,g,n)$ is globally hyperbolic. This is completeness of causal section time, not completeness of geodesic affine parameters. The smoothness and proper-exhaustion conditions explicitly specify all escape mechanisms; spatial metric completeness alone does not replace the proper-radius estimate.

### Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)

[lem-author-eb8e266b8b92-interior-compact-confinement](item-lem-author-eb8e266b8b92-interior-compact-confinement)

[lem-author-eb8e266b8b92-compact-causal-endpoint](item-lem-author-eb8e266b8b92-compact-causal-endpoint)

[physics:thm-gr-cauchy-surface-implies-globally-hyperbolic](https://alphabetamath.cc/physics/item/thm-gr-cauchy-surface-implies-globally-hyperbolic)

[lem-author-eb8e266b8b92-proper-radius-control](item-lem-author-eb8e266b8b92-proper-radius-control)

### Facts & Assumptions

**Given:** The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

[F1] The Axiom of Choice implies Dependent Choice and Countable Choice, supplying the inherited choice assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F2] Causal curves, absence of endpoints, Cauchy hypersurfaces and global hyperbolicity are interpreted relative to $E$. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F3] Lapse and shift use the unit-normal decomposition; completeness up to compact boundary concerns the intrinsic spatial distance with that boundary included. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F4] The ADM section-time lemma gives strict monotonicity, a causal locally Lipschitz reparametrization and spatial speed $|x\prime|_h\le N+|X|_h$. [lem-author-eb8e266b8b92-adm-time-speed](item-lem-author-eb8e266b8b92-adm-time-speed)

[F5] Under the stated collar and proper-radius assumptions, both barriers put a bounded section-time spatial trajectory in a compact subset of the interior. [lem-author-eb8e266b8b92-interior-compact-confinement](item-lem-author-eb8e266b8b92-interior-compact-confinement)

[F6] A causal section-time trajectory in an interior compact set has a limit in $E$ at each finite section-time endpoint. [lem-author-eb8e266b8b92-compact-causal-endpoint](item-lem-author-eb8e266b8b92-compact-causal-endpoint)

[F7] On a time-oriented smooth Lorentzian four-manifold, existence of a Cauchy set implies strong causality and compact causal diamonds, assuming countable and dependent choice. [physics:thm-gr-cauchy-surface-implies-globally-hyperbolic](https://alphabetamath.cc/physics/item/thm-gr-cauchy-surface-implies-globally-hyperbolic)

[F8] When the boundary is empty, the proper-radius control alone confines bounded section-time trajectories to compact interior sets. [lem-author-eb8e266b8b92-proper-radius-control](item-lem-author-eb8e266b8b92-proper-radius-control)

### Proof

**Given:**The data and hypotheses in the Statement.

**Goal:** The conclusions stated there.

1.1 The displayed ADM metric has Lorentzian signature, and its unit future normal is $n$ as specified. Each $v$-level is an embedded copy of $\Sigma^\circ$ with induced positive metric $h$. For an inextendible future causal curve, the section-time lemma makes $v$ strictly increasing and gives its locally Lipschitz section-time representation on an interval $I$. This change of parameter preserves the absence of endpoints. [F2, F3, F4, algebra]

2.1 If $\sup I=v_*<\infty$, fix $v_0\in I$. The barrier hypotheses give interior compact confinement of the spatial trajectory for $v_0\le v<v_*$. The compact endpoint lemma then gives a limit $(v_*,p)\in E$, contradicting inextendibility. When $B$ is empty, the proper-radius estimate alone gives the required interior compact set, since all spatial points are interior. The identical argument at $\inf I$ excludes a finite lower endpoint. Therefore $I=\mathbb R$. [F5, F6, F8, step 1.1, algebra]

3.1 For every real $a$, the continuous strictly increasing section time on each inextendible causal curve takes the value $a$ exactly once. Thus $\{v=a\}$ is a Cauchy set in $E$ and, by its already established positive induced metric, a Cauchy hypersurface. The Cauchy-set implication applies to the smooth Lorentzian four-manifold $(E,g,n)$; its Countable Choice and Dependent Choice hypotheses follow from the assumed Axiom of Choice by F1. Hence $E$ is strongly causal with compact causal diamonds, which is global hyperbolicity. [F1, F2, F7, step 1.1, step 2.1] ∎

### Remarks

The proper-exhaustion version is the general contract; the finite product-end version is a sufficient way to supply it, rather than a consequence of an arbitrary radial notation. The theorem does not construct a stationary product from a stationary flow, and does not assert existence of a maximal section. Applications to a transformed geometry must separately supply the global product, the smooth boundary/collar data and the actual proper end radius for each fixed parameter. No uniform estimate as a deformation parameter tends to zero is asserted. The spatial completeness hypothesis is retained from the scaffold, although the compact-exhaustion proof does not need it once the explicit escape controls are supplied.


## Boundary membership excludes interior focal points from the target

[Open item](item-lem-author-2632702918ef-target-interior-focal-exclusion) · level 5


### Statement

For the null segment $\gamma$ in the compact-target hypotheses, reverse its direction and regard it as a past null normal geodesic issued from $c\in C$. There is no focal point to $C$ strictly between $c$ and $p$. Focal points here are rank loss of the normal screen Jacobi map, with the direction and affine parameter reversed from the future convention in the null-screen definition.

### Statement references

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)

[lem-author-2632702918ef-compact-target-null-segment](item-lem-author-2632702918ef-compact-target-null-segment)

### Facts & Assumptions

[A1] Work in ZFC. The axiom of choice implies dependent choice and countable choice, supplying the choice assumptions of the geometric and causal suppliers used below. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F1] The causal relations, boundary, global hyperbolicity and temporal function are relative to $E$ as in the causal-exterior interface. The metric-selected connection is torsion-free and metric-compatible, so differentiation of metric pairings obeys the product rule. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F2] The target surface, null normal congruence, positive screen quotient, normal screen Jacobi map and rank-loss definition of focality have the meanings in the null-screen interface. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F3] The entire causal segment from $p$ to $c$ lies in $\partial_E I_E^-(C)$ under the compact-target hypotheses specified in [F7]. [lem-author-2632702918ef-target-segment-boundary-containment](item-lem-author-2632702918ef-target-segment-boundary-containment)

[F4] The final tangent of a smooth nonconstant future null affine segment from $p$ to $c\in C$ is orthogonal to $T_cC$ under those hypotheses; global acausality of $C$ is not required. [lem-author-2632702918ef-target-endpoint-orthogonality](item-lem-author-2632702918ef-target-endpoint-orthogonality)

[F5] For a smooth null normal geodesic from a smooth spacelike surface without boundary, a normal screen Jacobi field with nonzero initial tangent vector and zero screen value at a positive instant puts points sufficiently shortly afterward in $I^+(C)$. Its equation is $\mathcal D_u^2J+\mathcal R J=0$, where $\mathcal R[Z]=[R(Z,L)L]$; its initial data are $J(0)=[X]$ and $\mathcal D_uJ(0)=B_0X$, with $g(B_0X,Y)=\chi_\ell(X,Y)$ for $X,Y\in T_cC$. Apply this mathematical theorem in $(E,g,-N)$ when reversing time orientation. [physics:lem-gr-fx-null-focal-boundary-exclusion](https://alphabetamath.cc/physics/item/lem-gr-fx-null-focal-boundary-exclusion)

[F6] The geodesic initial-value problem has a unique smooth maximal solution on an open interval, and its evaluation is smooth on an open time-and-initial-data domain. An included smooth finite endpoint extends by this same initial-value theorem. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[F7] The compact-target hypotheses mean that $(E,g,N)$ is a smooth globally hyperbolic time-oriented Lorentzian four-manifold, $C\subset E$ is a nonempty compact smooth embedded spacelike two-surface without boundary, $\tau$ is temporal, and $p\in\partial_E I_E^-(C)$ satisfies $\tau(p)<\min_C\tau$. Under these hypotheses some $c\in C$ satisfies $p\le_Ec$, $p\ne c$, and $p\notin I_E^-(C)$. [lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)

[F8] Under [F7], there is a nonconstant future null affine segment $\gamma:[0,1]\to E$ from $p$ to some $c\in C$, smooth up to both endpoints and with nonzero tangent. The argument below applies to every such segment. [lem-author-2632702918ef-compact-target-null-segment](item-lem-author-2632702918ef-compact-target-null-segment)

[F9] Around every point of a smooth embedded spacelike two-surface there is a smooth normalized pair of future null normals. The normal plane is Lorentzian with exactly two future null rays; selecting a ray and positive rescaling gives a prescribed nonzero vector on that ray. The positive screen metric, screen derivative and symmetric form $\chi_\ell(X,Y)=g(\nabla_X\ell,Y)$ are well-defined. [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen)

[F10] For a smooth variation through affinely parametrized geodesics with tangent $L$ and variation field $V$, $D_uV=D_rL$ and $D_u^2V=R(L,V)L$. These are the geodesic-deviation identities, with the same curvature convention as [F5]. [physics:thm-gr-jacobi-equation-and-geodesic-deviation](https://alphabetamath.cc/physics/item/thm-gr-jacobi-equation-and-geodesic-deviation)

[F11] Each chronological past $I_E^-(c)$ is open. Arbitrary unions of open sets are open by topology axiom (T2). [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness) [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)

[F12] Each $X\in T_cC$ is the velocity at zero of a smooth curve in $C$ through $c$, defined on an open interval about zero. [math:cor-every-tangent-vector-is-the-velocity-of-a-smooth-curve](https://alphabetamath.cc/item/cor-every-tangent-vector-is-the-velocity-of-a-smooth-curve)

[F13] Closed bounded real intervals are compact: every open cover has a finite subcover. [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)

### Proof

**Given:** The data and hypotheses in the Statement, with the compact-target hypotheses and segment made explicit in [F7] and [F8].

**Goal:** Exclude rank loss of the reversed normal screen Jacobi map at every $u\in(0,1)$.

1.1 Put $\delta(u)=\gamma(1-u)$ for $0\le u\le1$ and reverse the time orientation to $-N$. Then $\delta$ is a smooth nonconstant future null affine geodesic in $(E,g,-N)$ starting at $c$, with nonzero normal tangent by [F4] and [F8]. Apply [F9] with this reversed orientation. Interchange the two local null-normal labels if necessary so that $\delta\prime(0)=a\ell_c$ for $a>0$, and replace the local pair $(\ell,k)$ by $(a\ell,a^{-1}k)$. It remains normalized and now $\ell_c=\delta\prime(0)$. This uses only a local field near $c$, not a global normal pair. The choice assumptions of these suppliers follow from [A1]. [A1, F1, F2, F4, F7, F8, F9, given]

2.1 By [F6], extend $\delta$ slightly past both endpoints. The open smooth geodesic-evaluation domain contains its initial state at every time in the interval $[0,1]$, compact by [F13]; a finite subcover therefore gives a neighborhood $U$ of $c$ in $C$ and an open interval $J\supset[0,1]$ on which the geodesics with initial data $(x,\ell_x)$ define a smooth map $F:U\times J\to E$. Uniqueness gives $F(c,u)=\delta(u)$. Each parameter curve is null by metric compatibility and its null initial tangent, has nonzero tangent by uniqueness, and stays future-directed for $-N$ by continuity. For $X\in T_cC$, choose the curve $x(r)$ in [F12] with $x(0)=c$ and $x\prime(0)=X$, and set $V_X(u)=\partial_rF(x(r),u)|_{r=0}$. By [F10], $D_uV_X=D_rL$ and $D_u^2V_X=R(L,V_X)L$, where $L=\partial_uF$. Metric compatibility gives $\frac{d}{du}g(V_X,L)=g(D_rL,L)=\frac12\partial_r g(L,L)=0$. Its initial value is $g(X,\ell_c)=0$, so $V_X$ is orthogonal to $L$ throughout. The same calculation at every $x\in U$ verifies the orthogonality requirement in [F2], hence $F$ is an admissible local null-normal congruence even at rank loss. [step 1.1, F1, F2, F6, F10, F12, F13, construct, algebra]

3.1 Put $J_X=[V_X]=A_uX$ in the positive screen along $\delta$. Projecting the deviation equation from step 2.1 gives $\mathcal D_u^2J_X+\mathcal R J_X=0$ with the convention of [F5], since $R(L,V_X)L=-R(V_X,L)L$. At $u=0$, $J_X(0)=[X]$ and $\mathcal D_uJ_X(0)=[\nabla_X\ell]$. At $c$, normality gives $T_cC\subset\ell_c^\perp$. If $a\ell_c\in T_cC$, its squared norm is zero, so positivity of $g|_{T_cC}$ forces $a\ell_c=0$. Thus the quotient map $\iota:T_cC\to\ell_c^\perp/\mathbb R\ell_c$, $Y\mapsto[Y]$, is injective. Nondegeneracy of the ambient metric and $\ell_c\ne0$ give $\dim\ell_c^\perp=3$, so its quotient by $\mathbb R\ell_c$ has dimension two, equal to $\dim T_cC$; hence $\iota$ is onto. By the quotient metric in [F2], $\bar\gamma(\iota Y,\iota Z)=g(Y,Z)$, so $\iota$ is an isometry. Metric compatibility in [F1] gives $g(\nabla_X\ell,\ell_c)=\frac12X(g(\ell,\ell))=0$, making $[\nabla_X\ell]$ a screen vector. For every $Y\in T_cC$, $\bar\gamma([\nabla_X\ell],\iota Y)=g(\nabla_X\ell,Y)=\chi_\ell(X,Y)=g(B_0X,Y)=\bar\gamma(\iota(B_0X),\iota Y)$. Since $\iota$ is onto and the screen metric is positive definite, $[\nabla_X\ell]=\iota(B_0X)$, which is the identification used in [F5]. Thus $J_X$ has exactly the equation and initial data required in [F5]. In particular rank loss of $A_{u_0}$ supplies $X\ne0$ with $J_X(u_0)=0$, which is a focal instant in that theorem's sense. [step 2.1, F1, F2, F5, F9, F10, algebra]

4.1 Suppose $u_0\in(0,1)$ were such a rank-loss instant. Step 3.1 makes [F5] applicable in $(E,g,-N)$, so for some $u$ with $u_0<u<1$, sufficiently near $u_0$, one has $\delta(u)\in I^+_{E,-N}(C)=I^-_{E,N}(C)$. On the other hand [F3] puts $\delta(u)$ in $\partial_E I^-_{E,N}(C)$. The set $I^-_{E,N}(C)=\bigcup_{c\in C}I^-_{E,N}(c)$ is open by [F11], so by the boundary definition in [F1] it is disjoint from its boundary. This is a contradiction. Hence no focal point occurs strictly between $c$ and $p$. No exclusion of a focal point at $p$ is asserted. [A1, step 1.1, step 3.1, F1, F3, F5, F11] ∎



## Removing the boundary before applying scalar coarea

[Open item](item-lem-author-423fe0348a31-interior-coarea-boundary-treatment) · level 5


### Statement

Work in ZFC. Let $(R,k)$ be a compact smooth Riemannian three-manifold with boundary $\partial R=B_-\cup B_+$. Let $u:R\to\mathbb R$ be Lipschitz for the intrinsic length distance $d_R$, and constant on neighborhoods of the two boundary parts with respective values $c_-$ and $c_+$, where $c_-<t<c_+$ for every $t$ in an interval $I$. Then $\partial R$ has zero three-dimensional Riemannian volume, and every level $\{u=t\}$ with $t\in I$ is a compact subset of $R^\circ$. On each connected component $C$ of $R^\circ$, the restriction of $u$ is Lipschitz for the intrinsic distance $d_C$. The boundaryless Lipschitz coarea theorem therefore applies componentwise on $R^\circ$; for bands with levels in $I$, neither its volume integral nor its level-area integral acquires a boundary contribution.

Here $d_R$ is the infimum of lengths of finite piecewise $C^1$ curves in $R$, including curves meeting its boundary; $d_C$ uses curves confined to $C$. Distances between different components of $R$ are $+\infty$, and all Hausdorff measures on $R$ are interpreted componentwise. Volume is the measure of the density $\sqrt{\det(k_{ij})}\,|dx^1dx^2dx^3|$, also in boundary charts. Cut area is normalized $\mathcal H^2=(\pi/4)\mathcal H^2_{\rm unnormalized}$, formed from the stated length distance. The measures formed with $d_R$ and $d_C$ agree on Borel subsets of $C$.

### Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice. Countable choice is used for the density-measure and Hausdorff-measure suppliers and countable localization. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The scalar coarea Jacobian equals the metric weak-gradient norm almost everywhere. [lem-author-423fe0348a31-scalar-metric-jacobian](item-lem-author-423fe0348a31-scalar-metric-jacobian)

[F2] The metric is smooth and positive definite up to the boundary. Curve length is the integral of metric speed; connected-component distances are infima of those lengths, with $+\infty$ between different components. These distances induce the manifold topology, including at boundary points. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length) [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold) [math:def-extended-riemannian-distance-on-a-disconnected-manifold](https://alphabetamath.cc/item/def-extended-riemannian-distance-on-a-disconnected-manifold) [math:thm-the-riemannian-distance-topology-is-the-manifold-topology](https://alphabetamath.cc/item/thm-the-riemannian-distance-topology-is-the-manifold-topology)

[F3] Lipschitz heights and normalized Hausdorff areas are measured with the fixed metric. [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[F4] In a boundary chart the boundary is in the coordinate hyperplane. On a compact coordinate set there are $0<a\le b<\infty$ such that $a|v|\le |v|_k\le b|v|$. [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

[F5] The Riemannian volume density has coordinate coefficient $\sqrt{\det(k_{ij})}$. Its measure restricted to any Borel subset of any chart is the integral of that coefficient; the gluing theorem explicitly allows boundary charts and assumes countable choice. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing)

[F6] The plane $\mathbb R^2\times\{0\}$ is a positive-codimension smooth submanifold of $\mathbb R^3$, so it is Lebesgue null under countable choice. [math:cor-positive-codimension-immersed-submanifolds-are-null](https://alphabetamath.cc/item/cor-positive-codimension-immersed-submanifolds-are-null)

[F7] Hausdorff measure is obtained from countable diameter covers as their scale tends to zero. Under countable choice it measures every Borel set and is countably additive there. The library definitions are unnormalized; multiplication by $\pi/4$ gives the two-dimensional normalization used here and preserves these properties. [math:def-hausdorff-content-at-scale-delta](https://alphabetamath.cc/item/def-hausdorff-content-at-scale-delta) [math:def-hausdorff-measure](https://alphabetamath.cc/item/def-hausdorff-measure) [math:thm-hausdorff-measure-is-metric-and-borel-measurable](https://alphabetamath.cc/item/thm-hausdorff-measure-is-metric-and-borel-measurable)

[F8] Nonnegative integrals commute with countable nonnegative sums, including infinite values. [math:cor-beppo-levi-theorem](https://alphabetamath.cc/item/cor-beppo-levi-theorem)

[F9] The independent coarea input, with its exact scope, is recorded in External input below. It supplies a theorem on boundaryless manifolds, not a theorem on regions with boundary.

[F10] A closed subset of a compact space is compact. [math:thm-closed-subspace-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-closed-subspace-of-a-compact-space-is-compact)

### Proof

**Given:** The region, height, boundary constants, and interval in the Statement.

**Goal:** Justify boundary removal for coarea, including its metric and measure conventions.

1.1 The boundary is Borel: in the half-space charts its complement is open. Each boundary-chart image of $\partial R$ lies in a Lebesgue-null coordinate plane by [F4] and [F6]. Its volume is therefore zero by the chart formula [F5]; a finite chart cover of the compact region gives $V_k(\partial R)=0$. By [F2] the Lipschitz function $u$ is continuous in the manifold topology. Since the boundary constants lie outside $I$, the closed level $E_t=\{u=t\}$ misses the boundary for $t\in I$, and [F10] makes it compact. [given, A1, F2, F4, F5, F6, F10]

1.2 Let $C$ be any interior component. Every curve confined to $C$ is a curve in $R$, so $d_R(x,y)\le d_C(x,y)$ for $x,y\in C$. If $L$ is the given Lipschitz constant, then $|u(x)-u(y)|\le Ld_R(x,y)\le Ld_C(x,y)$. Thus $u|_C$ satisfies the global Lipschitz hypothesis of the boundaryless theorem; completeness of $C$ is not required by that theorem. [given, F2, F9]

2.1 Fix an interior point $p\in C$ and choose coordinates centered at $p$ with the closed Euclidean ball $\overline B_r$ inside the chart and inside $C$. Use [F4] on this compact set and choose $0<\varepsilon<r$ with $2b\varepsilon<a(r-\varepsilon)$. For any $y,z$ with coordinates in $B_\varepsilon$, the coordinate segment between them has metric length at most $2b\varepsilon$. Any curve in $R$ from $y$ to $z$ that leaves the coordinate ball $B_r$ has an initial segment reaching its sphere; its length is at least $a(r-\varepsilon)$, since Euclidean curve length bounds endpoint displacement. Hence such curves cannot lower the infimum below the segment bound, and $d_R(y,z)$ equals the infimum over curves confined to $B_r$. As these curves are also confined to $C$, step 1.2 yields $d_R(y,z)\le d_C(y,z)\le d_R(y,z)$. Thus the two distances agree on the neighborhood $B_\varepsilon$. This argument uses infima and does not assume existence of minimizing curves. [given, F2, F4, step 1.2, choose, algebra]

2.2 Fix a Borel interval $J\subset I$ and put $A=\{x\in R:u(x)\in J\}$. It is Borel by continuity, and step 1.1 gives $A\subset R^\circ$. For each interior component $C$, apply [F9] to $X=C$, $Y=\mathbb R$ with its Euclidean metric, $F=u|_C$, $n=2$, $k=1$, and the Borel set $A\cap C$. Its Lipschitz hypothesis is step 1.2. The source normalization identifies full-dimensional Hausdorff measure with $dV_k$ and target measure with $dt$. By [F1] and [F3] its Jacobian is $|\nabla_k u|$ almost everywhere. The resulting identity is $\int_{A\cap C}|\nabla_k u|\,dV_k=\int_J\mathcal H^2_{d_C}(C\cap E_t)\,dt$, with nonnegative extended integrals. [given, F1, F3, F9, step 1.1, step 1.2]

3.1 For a subset of one of the neighborhoods in step 2.1, intersect every Hausdorff covering set with that neighborhood and discard empty intersections. This does not increase diameters, so Hausdorff outer measure equals the one computed within the neighborhood. The restricted distances agree there; therefore the two normalized Hausdorff outer measures agree on every such subset. Second countability supplies a countable cover $(U_j)$ by these neighborhoods: take a countable basis refinement and choose a containing neighborhood for each selected basis element, using [A1]. Partition $C$ into the Borel sets $P_j=U_j\setminus\bigcup_{i<j}U_i$. For a Borel $E\subset C$, [F7] gives equality of the two measures of $E$ by summing their equal values on $E\cap P_j$. The Borel domains agree by [F2]. Interior components are open, because coordinate balls are connected; they are countably many, since disjoint nonempty open sets contain different members of a countable basis. Consequently the $d_R$-area of any Borel interior set is the sum of its $d_C$-areas over those components. [A1, F2, F7, step 2.1, construct]

4.1 Sum the identities in step 2.2 over the countably many interior components. The coarea input [F9] supplies measurable fiber-area functions, and [F8] interchanges their nonnegative sum with the $t$-integral. Step 3.1 identifies the sum of component areas with $\mathcal H^2_{d_R}(E_t)$ for $t\in J$. Thus $\int_A|\nabla_k u|\,dV_k=\int_J\mathcal H^2_{d_R}(E_t)\,dt$. On the volume side the density measure on the interior is the restriction of the measure on $R$ by [F5], and the removed boundary is null by step 1.1; on the level side $E_t\subset R^\circ$ and step 3.1 gives agreement of the Hausdorff areas. This proves the claimed absence of boundary contributions. [F5, F8, F9, step 1.1, step 3.1, step 2.2] ∎

### External input

Theorem 5.3 of Nicolaescu gives $\int_A JF\,d\mathcal H_X^{n+k}=\int_Y\mathcal H_X^n(A\cap F^{-1}(y))\,d\mathcal H_Y^k(y)$ for a Lipschitz map between boundaryless $C^1$ Riemannian manifolds of dimensions $n+k$ and $k$, and a measurable $A$. Section 3 defines the normalization $\omega_s/2^s$ for diameter covers; Example 3.1(a) identifies full-dimensional measure with Riemannian volume. The source supplies this established theorem; the local proof above checks its hypotheses and transfers the formula from interior components to the region. See the precise citation and reading limits in sources.references.


## Compact-target null generators and the required endpoint conditions

[Open item](item-lem-compact-target-achronal-generator-input) · level 6


### Statement

Let $(E,g,N)$ be a smooth globally hyperbolic time-oriented Lorentzian four-manifold and let $C\subset E$ be a compact spacelike two-surface, meaning a smooth embedded two-manifold without boundary with positive-definite induced metric. If $p\in\partial_E I_E^-(C)$ and some temporal function $\tau$ satisfies $\tau(p)<\min_C\tau$, then $p$ is joined to a point of $C$ by a future null geodesic whose entire segment lies in that boundary. Its final tangent is orthogonal to $C$, and there is no focal point to $C$ strictly between its endpoints, with focality measured from $C$ toward $p$. Achronal boundaries are locally Lipschitz. Choosing one of the two null normal directions, proving a closed endpoint domain, and controlling endpoint-map regularity require additional arguments specific to the chosen cylinder and cut.

### Facts & Assumptions

[A1] Work in ZFC; the axiom of choice includes the countable and dependent choice assumptions of the causal suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The chronological and causal relations, boundary, global hyperbolicity and temporal function are relative to $E$ as in [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data).

[F2] The surface and focal notions are those of [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data).

[F3] Compactness and boundary membership give a distinct causal endpoint $c\in C$, with $p\notin I_E^-(C)$. [lem-author-2632702918ef-compact-target-causal-endpoint](item-lem-author-2632702918ef-compact-target-causal-endpoint)

[F4] There is a future null geodesic segment from $p$ to such a target point. [lem-author-2632702918ef-compact-target-null-segment](item-lem-author-2632702918ef-compact-target-null-segment)

[F5] The whole segment is contained in the chronological boundary. [lem-author-2632702918ef-target-segment-boundary-containment](item-lem-author-2632702918ef-target-segment-boundary-containment)

[F6] Its target tangent is orthogonal to $C$ without assuming $C$ acausal. [lem-author-2632702918ef-target-endpoint-orthogonality](item-lem-author-2632702918ef-target-endpoint-orthogonality)

[F7] No focal point to $C$ occurs strictly inside the segment. [lem-author-2632702918ef-target-interior-focal-exclusion](item-lem-author-2632702918ef-target-interior-focal-exclusion)

[F8] The boundary of an open future set is locally a Lipschitz graph, and the time-reversed assertion holds for an open past set. [physics:lem-gr-achronal-boundaries-lipschitz-graphs](https://alphabetamath.cc/physics/item/lem-gr-achronal-boundaries-lipschitz-graphs)

[F9] Each chronological past $I_E^-(c)$ is open in $E$, by clause (a) of [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness).

[F10] Finite concatenation of future timelike curves and positive affine reparametrization preserve the future timelike curve class, by clauses (d) and (e) of [physics:lem-gr-causal-curve-calculus](https://alphabetamath.cc/physics/item/lem-gr-causal-curve-calculus).

[F11] Arbitrary unions of open sets are open, by topology axiom (T2) in [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space).

### Proof

**Given:**The data and hypotheses in the Statement.

**Goal:** Establish the asserted conclusion.

1.1 Apply [F3]–[F4] using the globally hyperbolic spacetime $E$, compact smooth target $C$, and the strict temporal separation in the Statement. These supply a nonconstant future null geodesic to a point of $C$. Apply [F5] to get containment of its whole closed segment in $\partial_E I_E^-(C)$; [F6] gives endpoint orthogonality and [F7] excludes interior focal points measured from that endpoint. Each use retains precisely the same domain and causal relations. [given, F1, F2, F3, F4, F5, F6, F7]

1.2 Put $P:=I_E^-(C)=\bigcup_{c\in C}I_E^-(c)$. Each set in this union is open by [F9], so $P$ is open by [F11]. If $x\in I_E^-(P)$, some $y\in P$ and $c\in C$ satisfy $x\ll_E y\ll_E c$. Positively affinely reparametrize the two joining timelike curves to adjoining compact intervals and concatenate them using [F10]. This gives $x\ll_E c$, hence $I_E^-(P)\subseteq P$. [F1, F9, F10, F11, A1]

2.1 Conversely, if $x\in P$, choose a future timelike curve $\gamma:[a,b]\to E$ from $x$ to some $c\in C$ and an interior parameter $s\in(a,b)$. Restriction to $[a,s]$ and $[s,b]$ preserves local absolute continuity and the nonzero future timelike velocity condition almost everywhere, directly from the curve definition in [F1]; thus $x\ll_E\gamma(s)\ll_E c$. It follows that $\gamma(s)\in P$ and $x\in I_E^-(P)$. Together with step 1.2 this gives $I_E^-(P)=P$. Therefore $P$ is an open past set in [F8]'s sense; reversing the time orientation makes it an open future set, with the same topological boundary. Apply [F8] to obtain the local Lipschitz property of $\partial_E P$. The argument does not choose a null-normal branch or assert regularity of an endpoint map; those remain the separate obligations in the Statement. [step 1.1, step 1.2, F1, F8, A1] ∎

### External input

Minguzzi's theorem gives the local Lipschitz property of achronal boundaries; the compact-target endpoint, orthogonality and focal conclusions above use the declared local suppliers.


## Outward unit variation in the normalized null basis

[Open item](item-lem-author-6413ea293c6d-null-variation-normalization) · level 6


### Statement

In the normal plane of the surface data [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data), let $l=L=n+\nu$, $k=2\underline L=n-\nu$ and $v=\nu$. Then $g(l,k)=-2$, $g(l,v)=1$, $v=-k/2+Vl$ with $V=1/2$, and the accompanying normal $u=k/2+Vl$ is $n$. The future normal $n$ is timelike unit and $\nu$ is spacelike unit, with $g(n,\nu)=0$.

### Facts & Assumptions

[F1] The supplied surface gauge fixes the orthonormal normal pair and its null combinations. [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)

### Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Establish its identities with the indicated normalizations.

1.1 Expand the pairings using $g(n,n)=-1$, $g(\nu,\nu)=1$ and $g(n,\nu)=0$; they give $g(n+\nu,n-\nu)=-2$ and $g(n+\nu,\nu)=1$. [given, F1, algebra]

2.1 The identity $-k/2+Vl=(-1/2+V)n+(1/2+V)\nu$ equals $\nu$ exactly for $V=1/2$. Substituting this value in $k/2+Vl$ gives $n$. [step 1.1, F1, algebra] ∎


## Electrovac contraction in the normalized normal plane

[Open item](item-lem-author-6413ea293c6d-electrovac-normal-contraction) · level 6


### Statement

Under the geometric electrovac equations of [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data) and the oriented surface gauge of [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data), one has $\operatorname{Scal}_g=0$, $G=\operatorname{Ric}$ and $\operatorname{Ric}(L,\underline L)=e^2+b^2$. Here $F|_{TS}=b\,d\mu_q$ and $(\star F)|_{TS}=e\,d\mu_q$ are the actual oriented flux densities. This identity needs no vanishing assumption on the tangential electromagnetic components.

### Facts & Assumptions

[F1] The geometric electrovac equations use $\operatorname{Ric}_{ab}=2(F_{ac}F_b{}^c-g_{ab}F_{cd}F^{cd}/4)$, and the Hodge and surface orientations are fixed. [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data) [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)

[F2] Scalar curvature and the Einstein tensor mean $\operatorname{Scal}_g=g^{ab}\operatorname{Ric}_{ab}$ and $G_{ab}=\operatorname{Ric}_{ab}-\tfrac12\operatorname{Scal}_g g_{ab}$, with the same curvature and Ricci contraction convention as in [F1]. [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors)

### Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Establish its identities with the indicated normalizations.

1.1 At a point choose an orthonormal frame $(n,\nu,E_1,E_2)$ with $(E_1,E_2)$ positively oriented on $S$. Put $a=F(n,\nu)$, $x_A=F(n,E_A)$, $y_A=F(\nu,E_A)$ and $c=F(E_1,E_2)$. Then $F_{ab}F^{ab}=2(-a^2-|x|^2+|y|^2+c^2)$. Direct substitution gives $\operatorname{Ric}(n,n)=a^2+|x|^2+|y|^2+c^2$ and $\operatorname{Ric}(\nu,\nu)=-a^2+|x|^2+|y|^2-c^2$. The trace of the defining electrovac equation is $\operatorname{Scal}_g=2(F_{ac}F^{ac}-4F_{cd}F^{cd}/4)=0$. [given, F1, F2, algebra]

2.1 Symmetry of Ric and $L=n+\nu$, $\underline L=(n-\nu)/2$ yield $\operatorname{Ric}(L,\underline L)=(\operatorname{Ric}(n,n)-\operatorname{Ric}(\nu,\nu))/2=a^2+c^2$. By the flux definitions $c=b$, while the Hodge definition in this orthonormal frame gives $e=\pm a$, with the sign fixed by the independently chosen spacetime orientation. Therefore $a^2+c^2=e^2+b^2$; the definition of $G$ and the zero scalar trace also give $G=\operatorname{Ric}$. [step 1.1, F1, F2, algebra] ∎


## Riemannian Lipschitz coarea on compact interior bands

[Open item](item-lem-author-423fe0348a31-riemannian-lipschitz-coarea) · level 6


### Statement

Let $(R,k)$ be a compact smooth Riemannian three-region with boundary, and let $u:R\to\mathbb R$ be Lipschitz for its intrinsic length distance. Suppose that $u$ is constant near each of two boundary parts whose union is $\partial R$, with the two constants outside an interval $I$ on opposite sides. For every Borel interval $J\subset I$,

$$\int_{\{x\in R:u(x)\in J\}}|\nabla_k u|\,dV_k=\int_J\mathcal H_k^2(\{x\in R:u(x)=t\})\,dt.$$

Here $dV_k$ is Riemannian volume, $\nabla_k u$ is the almost-everywhere weak gradient characterized by $k(\nabla_k u,\cdot)=du$, and $\mathcal H_k^2$ is normalized two-dimensional Hausdorff measure for the metric. A smooth $u$ satisfying the same boundary condition also satisfies the identity. More generally, for any nonnegative measurable $w$ on $R^\circ$,

$$\int_{R^\circ}w|\nabla_k u|\,dV_k=\int_{\mathbb R}\left(\int_{\{x\in R^\circ:u(x)=t\}}w\,d\mathcal H_k^2\right)dt.$$

Both sides are extended nonnegative integrals. Level area here is Hausdorff area; it is not defined to be BV perimeter.

### Statement references

[lem-author-423fe0348a31-interior-coarea-boundary-treatment](item-lem-author-423fe0348a31-interior-coarea-boundary-treatment)

[def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

### Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The metric supplies intrinsic curve length and Riemannian volume. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[F2] The Lipschitz height has almost-everywhere weak gradient and normalized Hausdorff cut-area conventions as stated above. [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[F3] At almost every point the scalar metric coarea Jacobian is $|\nabla_k u|$. [lem-author-423fe0348a31-scalar-metric-jacobian](item-lem-author-423fe0348a31-scalar-metric-jacobian)

[F4] The boundary has zero three-dimensional volume, levels in $I$ miss it, and the restriction of $u$ to each interior component is Lipschitz for that component's length distance. [lem-author-423fe0348a31-interior-coarea-boundary-treatment](item-lem-author-423fe0348a31-interior-coarea-boundary-treatment)

[F5] The Riemannian Lipschitz coarea formula and its nonnegative weighted form are the independent inputs recorded below.

### Proof

**Given:** The region, metric, height, boundary constants and interval in the Statement.

**Goal:** Prove the band and weighted identities, including the smooth-height case.

1.1 Apply the cited coarea formula to $u$ on each connected component of $R^\circ$, with target $\mathbb R$ and dimensions three and one. By the boundary-treatment result the restriction is Lipschitz for the component distance; the scalar Jacobian is $|\nabla_k u|$ almost everywhere. The source's full-dimensional Hausdorff measures are Riemannian volume and Lebesgue measure under its normalization. Summing over the countably many components gives the weighted identity, with nonnegative integrals interpreted in the extended sense. [given, A1, F1, F2, F3, F4, F5]

2.1 Take the weight to be the indicator of $\{u\in J\}$ on the interior. It is measurable because $u$ is continuous and $J$ is Borel. Its restriction to the fiber at $t$ is one when $t\in J$ and zero otherwise. For $t\in I$ the fiber has no boundary points, and the boundary has zero volume, so the resulting equality is exactly the displayed band identity on $R$. If $u$ is smooth on compact $R$, its gradient is bounded; integrating its derivative along curves shows that it is Lipschitz for the intrinsic length distance on each component, so the same application proves the smooth case. [given, F1, F4, step 1.1] ∎

### External input

The cited Riemannian coarea theorem applies to Lipschitz maps between $C^1$ Riemannian manifolds and expresses the integral of their metric Jacobian as the integral of normalized Hausdorff measures of fibers. Its weighted corollary gives the same identity for nonnegative measurable weights; its proof uses monotone convergence. The source input is used only on the boundaryless interior, while the boundary treatment and identification of the scalar Jacobian are supplied by the local dependencies.


## Outward graph stability has the negative-Laplacian principal symbol

[Open item](item-lem-author-1a44964f66ee-outward-elliptic-variation) · level 6


### Statement

Use the smooth Lorentzian and outward normal-graph data of the surface supplier on a closed surface $S$. Let $q$ be its induced metric, $n$ the future hypersurface unit normal and $\nu$ the supplied outward unit normal within the spacelike hypersurface. For $\Theta(u)=F_u^*\theta_{n+\nu_u}$ define $\mathcal L\psi=\left.\partial_\epsilon\right|_0\Theta(\epsilon\psi)$. Then $\mathcal L=-\Delta_q+b\cdot\nabla+c$ for a smooth real tangent vector field $b$ and smooth real scalar $c$. Equivalently, with $t=b/2$, $\mathcal L=-\Delta_q+2t\cdot\nabla+c$ is a real smooth elliptic operator. The normalization $l=n+\nu$, $k=n-\nu=2\underline L$ gives $g(l,k)=-2$, $g(l,\nu)=1$, $\nu=-k/2+l/2$ and $s_A=-g(k,\nabla_Al)/2=\zeta_A$. These identities use the outward sign fixed by the supplier.

### Facts & Assumptions

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The surface supplier fixes the expansion, intrinsic derivatives, outward graph tube and null normalization. [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data) [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)

[F2] The second-graph-data supplier states the exact expansion formula, its first-data remainder and its zero-graph second-partial coefficient; the linearization supplier gives the smooth linear, path-independent derivative. [lem-author-c50357f4fa9e-expansion-second-jet](item-lem-author-c50357f4fa9e-expansion-second-jet) [lem-author-c50357f4fa9e-linear-expansion-variation](item-lem-author-c50357f4fa9e-linear-expansion-variation)

[F3] The differential chain rule applies to the smooth coordinate changes and finite-dimensional coefficient functions used below. [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[F4] For a real scalar second-order principal symbol $p_2(x,\xi)=a^{ab}(x)\xi_a\xi_b$ with symmetric coefficients, ellipticity at $x$ means $p_2(x,\xi)\ne0$ for every nonzero covector $\xi$. [math:def-elliptic-hyperbolic-and-parabolic-principal-symbols](https://alphabetamath.cc/item/def-elliptic-hyperbolic-and-parabolic-principal-symbols)

### Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

[F1] The surface supplier fixes the expansion, intrinsic derivatives, outward graph tube and null normalization. [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data) [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)

[F2] The second-graph-data supplier states the exact expansion formula, its first-data remainder and its zero-graph second-partial coefficient; the linearization supplier gives the smooth linear, path-independent derivative. [lem-author-c50357f4fa9e-expansion-second-jet](item-lem-author-c50357f4fa9e-expansion-second-jet) [lem-author-c50357f4fa9e-linear-expansion-variation](item-lem-author-c50357f4fa9e-linear-expansion-variation)

[F3] The differential chain rule applies to the smooth coordinate changes and finite-dimensional coefficient functions used below. [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[F4] For a real scalar second-order principal symbol $p_2(x,\xi)=a^{ab}(x)\xi_a\xi_b$ with symmetric coefficients, ellipticity at $x$ means $p_2(x,\xi)\ne0$ for every nonzero covector $\xi$. [math:def-elliptic-hyperbolic-and-parabolic-principal-symbols](https://alphabetamath.cc/item/def-elliptic-hyperbolic-and-parabolic-principal-symbols)



**Proof technique:** direct.

1.1 By the exact decomposition in [F2], $\Theta(u)=-q_u^{ab}h(\nu_u,T_r)\partial_a\partial_bu+R(x,u,\partial u)$, with all coefficients and $R$ smooth and real. At the zero graph the same supplier gives $h(\nu_0,T_r)=1$ and $q_0=q$. Along $u=\epsilon\psi$, the derivative of the coefficient multiplying $\partial_a\partial_bu$ contributes zero at $\epsilon=0$, since the zero graph has zero second partials. The second-order part of $\mathcal L$ is consequently $-q^{ab}\partial_a\partial_b$, and the remaining terms are smooth real first- and zeroth-order terms by the supplied linearization. The intrinsic Laplacian from [F1] has second-order part $q^{ab}\partial_a\partial_b$, so $P=\mathcal L+\Delta_q$ has order at most one. Set $c=P(1)$. In coordinates $P-c$ has the form $b^a\partial_a$ with smooth real coefficients; coordinate independence of $P-c$ and the chain rule give the vector-field transformation law for these coefficients. They therefore define a global smooth real vector field $b$, and $\mathcal L=-\Delta_q+b\cdot\nabla+c=-\Delta_q+2t\cdot\nabla+c$ for $t=b/2$. In the quadratic-symbol convention of [F4], the principal symbol is $p_2(x,\xi)=-q^{ab}(x)\xi_a\xi_b$. For every nonzero covector $\xi$, positive definiteness of $q$ gives $q^{ab}\xi_a\xi_b>0$, so $p_2(x,\xi)<0$. Thus the principal symbol is nonzero on every nonzero covector at every point, and [F4] gives the asserted ellipticity. [F1, F2, F3, F4]

2.1 The null pairings follow from $g(n,n)=-1$, $g(\nu,\nu)=1$ and $g(n,\nu)=0$: $g(n+\nu,n-\nu)=-2$ and $g(n+\nu,\nu)=1$. Direct substitution yields $\nu=-k/2+l/2$. The supplier defines $\zeta_A=-g(\underline L,\nabla_Al)$; because $k=2\underline L$, the source convention $s_A=-g(k,\nabla_Al)/2$ is exactly $\zeta_A$. For each smooth test function the compact-surface tube supplies a common parameter interval for the graph path, and its velocity is $\psi\nu$. Thus $\delta_{\psi\nu}\theta_l=\mathcal L\psi$ in this same fixed outward direction. This proves all assertions, independently of any specialization of the zeroth-order curvature coefficient. [F1, F2, step 1.1] ∎


## Spacetime stably outermost condition and the slice bridge

[Open item](item-def-author-97780c2fed82-spacetime-stably-outermost-data) · level 6


### Definition

Assume Countable Choice $\mathrm{AC}_\omega$ for the supplied general-surface and spacetime-deformation constructions and, in the slice setting below, the normal-graph construction.

For a closed MOTS with supplied global future null pair $g(\ell,k)=-1$, say that it is spacetime stably outermost when there are smooth functions $\bar\gamma\ge0$ and $\psi>0$ such that, with $x=\bar\gamma\ell-k$ and $X=\psi x=\gamma\ell-\psi k$ where $\gamma=\psi\bar\gamma$, one has $\delta_X\theta_{(\ell)}\ge0$ pointwise. The derivative is the general spacetime deformation derivative, not a derivative restricted by definition to a spacelike slice. Stability with respect to a specified normal direction $v$ means the same condition with $X=\psi v$ for some positive $\psi$.

When $S$ is also in a spacelike hypersurface with future unit normal $n$ and outward unit normal $\nu$ within it, use $\ell=n+\nu$, $k=(n-\nu)/2$. Its normal-graph operator $\mathcal L$ is the derivative defined in the slice supplier. If a smooth positive function $f$ satisfies $\mathcal Lf\ge0$, then this supplies the spacetime-stability witness $X=f\nu=(f/2)\ell-fk$, namely $\psi=f$ and $\bar\gamma=1/2$. A principal-eigenvalue argument can supply such an $f$ only after its own positive-eigenfunction theorem and hypotheses have been supplied.

### Definition references

[def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data)

[lem-author-97780c2fed82-mots-variation-second-jet](item-lem-author-97780c2fed82-mots-variation-second-jet)

[lem-author-97780c2fed82-mots-boost-variation](item-lem-author-97780c2fed82-mots-boost-variation)

[def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

### Facts & Assumptions

[A1] Countable Choice is assumed as required by the general-surface, spacetime-deformation and slice normal-graph suppliers. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F1] Under [A1], general spacelike MOTS data and well-defined spacetime expansion variation are available. [def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data) [lem-author-97780c2fed82-mots-variation-second-jet](item-lem-author-97780c2fed82-mots-variation-second-jet)

[F2] Positivity of the variation condition is independent of boosts of the base null pair. [lem-author-97780c2fed82-mots-boost-variation](item-lem-author-97780c2fed82-mots-boost-variation)

[F3] Under [A1], in the slice setting, the graph gauge and its derivative $\mathcal Lf$ have the stated fixed base normal and actual admissible deformations. [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)

### Justification

**Given:** The objects and hypotheses in the Definition, including Countable Choice.

**Goal:** Establish the assertions and well-definedness stated there.

1.1 Under [A1], the quantified functions and the well-defined derivative of [F1] give an unambiguous predicate. The equivalence of the two displayed coefficient descriptions follows from $\gamma=\psi\bar\gamma$ and $\psi>0$. The normal velocity is spacelike or null by the calculation in [F2], while [F2] also makes the predicate independent of a positive rescaling of the chosen pair. [A1, F1, F2]

2.1 Under [A1], the slice supplier gives actual admissible normal-graph deformations. In the slice gauge, direct substitution gives $\ell/2-k=\nu$. The graph with initial velocity $f\nu$ is one of the spacetime deformation families in [F1], and its outgoing normal has precisely the same base $\ell=n+\nu$. Independence of the family and of its extension gauge at a MOTS in [F1] identifies its derivative with $\delta_{f\nu}\theta_{(\ell)}$. Thus $\mathcal Lf\ge0$ supplies exactly the stated witness. This proves the bridge from an actual positive supersolution; it makes no unsupported spectral-existence assertion. [A1, F1, F3, step 1.1] ∎


## Principal eigenfunctions and MOTS spectral stability

[Open item](item-thm-principal-eigenvalue-and-mots-stability-input) · level 7


### Statement

On a connected compact smooth Riemannian manifold $(S,h)$ without boundary, of positive dimension, let $L=-\Delta_h+2t\cdot\nabla+c$ have smooth real coefficients. There is a real principal eigenvalue $\lambda$, a smooth everywhere positive real eigenfunction $\phi$ unique up to multiplication by a positive constant, and a smooth positive adjoint eigenfunction $\chi$ at the same eigenvalue. Every other eigenvalue $\mu$ satisfies $\operatorname{Re}\mu\ge\lambda$.

For a connected closed smooth MOTS $S$ in the supplied smooth spacetime, fix smooth future-directed null normals $l,k$ with $g(l,k)=-2$ and outgoing expansion $\theta_l=0$. Here an admissible outward normal direction means a fixed smooth vector field $v$ normal to $S$, pointwise linearly independent of $l$, and normalized by $g(l,v)=1$. Its smooth elliptic stability operator $L_v\psi=\delta_{\psi v}\theta_l$ has $\lambda\ge0$ if and only if the MOTS is stably outermost in that direction. Here this means that some smooth $\psi\ge0$, $\psi\not\equiv0$, has $\delta_{\psi v}\theta_l\ge0$ everywhere. Strict stability means additionally that this variation is positive somewhere; it is equivalent to $\lambda>0$. For the outward graph in a spacelike hypersurface use $v=\nu$, $l=n+\nu$ and $k=n-\nu$. This spectral criterion by itself establishes no stability claim for a particular bifurcation sphere.

### Facts & Assumptions

[F1] Formal adjoint, smooth measure and real coefficients are fixed; the adjoint has the same elliptic leading symbol. [lem-author-1a44964f66ee-formal-adjoint](item-lem-author-1a44964f66ee-formal-adjoint) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F2] Positive right and adjoint eigenpairs exist by the explicitly imported closed-manifold theorem. [thm-author-1a44964f66ee-closed-principal-pair-external](item-thm-author-1a44964f66ee-closed-principal-pair-external)

[F3] Adjoint pairing identifies their eigenvalues, and the ground-state identity gives spectral ordering and uniqueness. [lem-author-1a44964f66ee-positive-adjoint-pairing](item-lem-author-1a44964f66ee-positive-adjoint-pairing) [lem-author-1a44964f66ee-ground-state-identity](item-lem-author-1a44964f66ee-ground-state-identity)

[F4] Nonnegative supersolutions characterize the common eigenvalue sign. [lem-author-1a44964f66ee-spectral-sign-test](item-lem-author-1a44964f66ee-spectral-sign-test)

[F5] The authored surface convention gives an elliptic outward graph operator and the exact null-pair normalization. [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data) [lem-author-1a44964f66ee-outward-elliptic-variation](item-lem-author-1a44964f66ee-outward-elliptic-variation)

[F6] For the fixed smooth null gauge $g(l,k)=-2$ and smooth normal field $v$ with $g(l,v)=1$, Andersson–Mars–Simon §3 equation (2), Definition 3.1 and Lemma 3.2 supply $\delta_{\psi v}\theta_l=L_v\psi$ and the smooth real negative-Laplacian form of $L_v$. Their Definition 5.1 supplies the directional stability and strict-stability conventions used here. [Andersson–Mars–Simon](https://arxiv.org/pdf/0704.2889).

### Proof

**Given:** the hypotheses in the Statement; work in ZFC.

**Goal:** establish the Statement.

**Proof technique:** direct.

1.1 Apply the imported positive-eigenpair theorem to $L$ and its adjoint; their exact smooth real closed-manifold hypotheses are those in the Statement and in the formal-adjoint lemma. The adjoint-pairing lemma gives a common real eigenvalue. The ground-state identity shows that every smooth complex eigenvalue has real part at least this one and that its eigenspace consists of constant multiples of $\phi$. Rescaling $\phi$ positively is exactly the ambiguity among everywhere positive real eigenfunctions. This proves the spectral assertions. [F1, F2, F3]

2.1 For the MOTS application keep the direction and null gauge fixed as in the Statement. In the hypersurface graph convention the geometric helper proves $\delta_{\psi\nu}\theta_l=\mathcal L\psi$, with $\mathcal L=-\Delta_q+2t\cdot\nabla+c$ having smooth real coefficients, so step 1.1 applies. Its null-pair normalization gives $g(l,k)=-2$ and $g(l,\nu)=1$. For every other admissible fixed direction, [F6] supplies $\delta_{\psi v}\theta_l=L_v\psi$ with $L_v$ of the same smooth real negative-Laplacian form, so step 1.1 applies to it as well. By the imported stability definition in [F6], stability is exactly existence of a nonzero smooth nonnegative $\psi$ with $L_v\psi\ge0$, and strict stability additionally requires positivity somewhere. Apply the spectral-sign lemma to obtain the equivalence with $\lambda\ge0$, and its strict version for $\lambda>0$. This is a criterion only; further geometry is required to verify either sign for any specific MOTS. This proves the Statement. [F2, F4, F5, F6, step 1.1] ∎

### External input

The imported MOTS stability convention is Andersson–Mars–Simon Definition 5.1: a fixed direction $v$, a nonzero smooth nonnegative test $\psi$, and the pointwise sign of $\delta_{\psi v}\theta_l$; strictness requires positivity somewhere. Fix smooth future-directed null normals $l,k$ with $g(l,k)=-2$ and a smooth normal field $v$, pointwise independent of $l$, with $g(l,v)=1$, as in their §3 equation (2). Their Definition 3.1 and Lemma 3.2 supply the smooth real negative-Laplacian operator $L_v$ and identify $\delta_{\psi v}\theta_l=L_v\psi$ for every such fixed direction. The hypersurface graph normalization and principal symbol are independently calculated in the geometric helper, and the sign equivalence is locally proved rather than assumed.

### Source notes

This mathematical prerequisite uses the independent Andersson–Mars–Simon source for the normal-direction convention, general-direction variation operator and stability definition. The imported eigenpair theorem remains an explicitly external input; the local helpers do not purport to reconstruct the compact-resolvent existence proof.


## Stable MOTS area–charge inequality

[Open item](item-pthm-stable-mots-area-charge-input) · level 7


### Statement

Assume Countable Choice $\mathrm{AC}_\omega$ for the surface, flux and deformation constructions below. In the smooth four-dimensional classical Einstein–Maxwell model, adopt geometric units and explicitly assume the field equation $G_{ab}+\Lambda g_{ab}=8\pi(T^{\rm EM}_{ab}+\tau_{ab})$, where $\Lambda\ge0$ and $T^{\rm EM}_{ab}=(4\pi)^{-1}(F_{ac}F_b{}^c-\tfrac14g_{ab}F_{cd}F^{cd})$. Here $G=\operatorname{Ric}-\tfrac12R g$, with the metric-selected (torsion-free, metric-compatible) connection $\nabla^g$, and the smooth non-electromagnetic stress tensor $\tau$ satisfies the dominant energy condition: $-\tau^a{}_bv^b$ is future causal or zero for each future timelike $v$. Charged matter is allowed; source-free Maxwell equations, axial symmetry and asymptotic flatness are not assumptions of this result.

Let $S$ be a nonempty connected closed orientable spacelike two-surface with supplied future null normals $\ell,k$, $g(\ell,k)=-1$, and outgoing expansion $\theta_{(\ell)}=0$, using the general spacelike-surface data with its connection fixed to the same $\nabla^g$ used for $G$. Use this connection for the outgoing expansion and for all deformations and expansion variations below. Suppose it is spacetime stably outermost in the exact sense of the spacetime-stably-outermost definition: some smooth $\gamma\ge0$, $\psi>0$ give $X=\gamma\ell-\psi k$ with $\delta_X\theta_{(\ell)}\ge0$. The derivative is the general spacetime derivative supplied by the expansion-variation lemma, with boost invariance supplied by the boost-variation lemma; no containing spacelike slice is required. Then, with $A$, $e,b$ and the flux normalization of the general spacelike-surface data,

$$A\ge4\pi\bigl(Q_E(S)^2+Q_M(S)^2\bigr).$$

The stronger source bound retained for applications is $\int_S(e^2+b^2)\,d\mu_q\le4\pi(1-g_S)\le4\pi$, where $g_S$ is the genus of the connected orientable surface (the number of handles). If this integral is positive, $g_S=0$. For a disconnected closed surface apply these assertions to each connected component satisfying the hypotheses; in particular $A_{\rm total}\ge4\pi\sum_j(Q_{E,j}^2+Q_{M,j}^2)$. This does not assert a bound by the square of the sum of component charges.

For a surface lying in a spacelike section, a supplied smooth positive supersolution $f$ of its outward graph operator, $\mathcal Lf\ge0$, verifies the spacetime-stability hypothesis by the slice bridge in the spacetime-stably-outermost definition: $\ell=n+\nu$, $k=(n-\nu)/2$ and $X=f\nu=(f/2)\ell-fk$. Nonnegativity of a principal eigenvalue suffices only together with an applicable theorem furnishing its smooth positive eigenfunction. No such spectral theorem is silently assumed here.

### Statement references

[def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data)

[lem-author-97780c2fed82-normal-deformation-families](item-lem-author-97780c2fed82-normal-deformation-families)

[lem-author-97780c2fed82-mots-variation-second-jet](item-lem-author-97780c2fed82-mots-variation-second-jet)

[lem-author-97780c2fed82-mots-boost-variation](item-lem-author-97780c2fed82-mots-boost-variation)

[def-author-97780c2fed82-spacetime-stably-outermost-data](item-def-author-97780c2fed82-spacetime-stably-outermost-data)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[physics:def-emg-pointwise-energy-conditions](https://alphabetamath.cc/physics/item/def-emg-pointwise-energy-conditions)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

### Facts & Assumptions

[A1] Countable Choice is assumed to meet the hypotheses of the general surface, flux, spacetime-deformation and slice-bridge suppliers. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F1] Under Countable Choice, general surface, flux and null-normal data use the explicit codimension-two interface; smooth deformations and their derivatives are supplied by the local helper chain. [def-author-97780c2fed82-general-spacelike-surface-data](item-def-author-97780c2fed82-general-spacelike-surface-data) [lem-author-97780c2fed82-normal-deformation-families](item-lem-author-97780c2fed82-normal-deformation-families) [lem-author-97780c2fed82-mots-variation-second-jet](item-lem-author-97780c2fed82-mots-variation-second-jet) [lem-author-97780c2fed82-mots-boost-variation](item-lem-author-97780c2fed82-mots-boost-variation)

[F2] Spacetime stably outermost means exactly the quantified outgoing variation condition; the same interface supplies the explicit slice supersolution bridge. [def-author-97780c2fed82-spacetime-stably-outermost-data](item-def-author-97780c2fed82-spacetime-stably-outermost-data)

[F3] The displayed Einstein equation with electromagnetic stress plus general non-electromagnetic matter is an explicit physical model assumption, in the geometric normalization of Dain–Jaramillo–Reiris equations (1)–(2). The source permits charged non-electromagnetic matter satisfying DEC.

[F4] The dominant energy condition is the stated algebraic condition on the non-electromagnetic stress tensor. [physics:def-emg-pointwise-energy-conditions](https://alphabetamath.cc/physics/item/def-emg-pointwise-energy-conditions)

[F5] Dain–Jaramillo–Reiris Theorem 2.1 supplies the area–charge conclusion, and its proof equation (31) supplies the retained squared-density bound, under these exact hypotheses.

[F6] The metric-selected connection is the unique torsion-free, metric-compatible connection of $g$. The general surface and deformation interfaces are used with this same $\nabla^g$ for expansion and variation, as required by the Levi–Civita convention at the start of Dain–Jaramillo–Reiris §3. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

### External input

The area–charge theorem and the stronger squared-density bound are imported from Dain–Jaramillo–Reiris Theorem 2.1 and equation (31), not claimed as locally reconstructed proofs. The surface expansion and its variation use the same Levi–Civita connection $\nabla^g$ as the curvature in the field equation, matching the opening convention of source §3. The source's null normals satisfy $g(\ell,k)=-1$, its MOTS condition is $\theta_{(\ell)}=0$, and its Definitions 3.1–3.2 require a positive stability weight in an outgoing non-timelike normal direction. The field equation has the sign $G+\Lambda g=8\pi(T^{\rm EM}+\tau)$ and the factor $1/(4\pi)$ in $T^{\rm EM}$. Under the explicitly assumed Countable Choice, the local helpers supply the general null variation and its exact relation to the slice graph derivative, so the import does not restrict the source's surface to a spacelike section. Connectedness is explicit for the genus and single-surface inequality; componentwise application preserves the valid disconnected scope. The field-law and energy hypotheses must be established in each application; this import neither establishes them nor proves spectral stability of a particular surface.


## Agreement of expansion and normal-connection conventions

[Open item](item-lem-author-6413ea293c6d-second-form-and-connection-signs) · level 7


### Statement

Use the smooth surface and null pair of [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data) and [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data). Define the vector second fundamental form $\mathbf K(X,Y)=-(\nabla_XY)^\perp$ and $H=\operatorname{tr}_q\mathbf K$, where projection is onto the Lorentzian normal plane. Then $g(\mathbf K(X,Y),l)=\chi_l(X,Y)$ and $g(H,l)=\theta_l$. With $k=2\underline L$ as in [lem-author-6413ea293c6d-null-variation-normalization](item-lem-author-6413ea293c6d-null-variation-normalization), the one-form $s(X)=-g(k,\nabla_Xl)/2$ equals $\zeta(X)=-g(\underline L,\nabla_XL)$.

### Facts & Assumptions

[F1] The surface expansion is the trace of the null second form and the null gauge specifies ζ. [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data) [lem-author-6413ea293c6d-null-variation-normalization](item-lem-author-6413ea293c6d-null-variation-normalization)

### Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Establish its identities with the indicated normalizations.

1.1 Since $g(Y,l)=0$ on the surface, metric compatibility gives $-g(\nabla_XY,l)=g(Y,\nabla_Xl)=\chi_l(X,Y)$. Projection of $\nabla_XY$ onto the normal plane leaves its pairing with the normal $l$ unchanged. [given, F1, algebra]

2.1 Taking the $q$-trace proves $g(H,l)=\theta_l$. Substituting $k=2\underline L$ and $l=L$ into the displayed definition of $s$ gives $s=\zeta$, including its sign. [step 1.1, F1, algebra] ∎


## Transferring area-controlled band energy through smooth approximation

[Open item](item-lem-author-423fe0348a31-band-energy-transfer) · level 7


### Statement

Work in ZFC. Let $(R,k)$ be a compact smooth Riemannian three-region with boundary $\partial R=B_-\sqcup B_+$, where the two boundary parts are closed and disjoint. Let $I\subset\mathbb R$ be an interval and let $c_-,c_+\in\mathbb R$ satisfy $c_-<t<c_+$ for every $t\in I$. Let $u:R\to\mathbb R$ be Lipschitz for the intrinsic Riemannian length distance within each connected component. Let $(u_j)$ be any sequence of real Lipschitz functions on $R$ for this distance. Assume that there are fixed open neighborhoods $U_-$ and $U_+$ of the boundary parts on which $u$ and every $u_j$ equal $c_-$ and $c_+$, respectively. The assertion also applies to smooth approximants, where smoothness includes smooth local extension in boundary charts.

Suppose $u_j\to u$ uniformly and in metric $W^{1,1}(R,k)$, meaning that $\int_R(|u_j-u|+|\nabla_k u_j-\nabla_k u|_k)\,dV_k\to0$. Here $dV_k$ is Riemannian volume, $k(\nabla_k v,\cdot)=dv$ defines the almost-everywhere weak gradient, and $\mathcal H_k^2$ is normalized metric two-dimensional Hausdorff measure. Suppose $\mathcal H_k^2(\{x\in R:u(x)=t\})\le A<\infty$ for almost every $t\in I$, with $A\ge0$.

Fix $J=(a,b)$ with $a<b$ and $[a,b]\subset\operatorname{int}I$. Put $e_j=\sup_{x\in R}|u_j(x)-u(x)|$ and $d_j=\int_R|\nabla_k u_j-\nabla_k u|_k\,dV_k$; for empty $R$ the supremum error is zero. For all sufficiently large $j$,
$$\int_J\mathcal H_k^2(\{x\in R:u_j(x)=t\})\,dt\le A(b-a+2e_j)+d_j.$$
In particular,
$$\limsup_{j\to\infty}\frac{1}{b-a}\int_J\mathcal H_k^2(\{x\in R:u_j(x)=t\})\,dt\le A.$$

### Facts & Assumptions

[F1] Boundary-preserving approximation on a compact smooth region uses the intrinsic Lipschitz and metric first-Sobolev conventions in the Statement and supplies smooth sequences with uniform and metric $W^{1,1}$ convergence and the exact constants on fixed boundary neighborhoods. The present estimate is conditional on the stated properties of the sequence and does not infer them for an arbitrary sequence from this existence result. [lem-author-423fe0348a31-fixed-boundary-approximation](item-lem-author-423fe0348a31-fixed-boundary-approximation)

[F2] On a compact smooth Riemannian three-region, a Lipschitz function constant on neighborhoods of both boundary parts, with its constants on opposite sides of $I$, satisfies the coarea identity for every Borel band in $I$, with the gradient, volume and normalized Hausdorff area conventions in the Statement. The supplier also establishes the smooth case, including that a smooth function on compact $R$ is intrinsically Lipschitz by bounding its gradient and integrating along curves. [lem-author-423fe0348a31-riemannian-lipschitz-coarea](item-lem-author-423fe0348a31-riemannian-lipschitz-coarea)

[F3] The norm induced by a real or complex inner product satisfies $|v+w|\le|v|+|w|$. For almost every $x\in R$, apply this to the real inner product $k_x$ on $T_xR$ and to $v=\nabla_k u(x)$ and $w=\nabla_k u_j(x)-\nabla_k u(x)$. [math:cor-triangle-inequality-for-inner-product-norm](https://alphabetamath.cc/item/cor-triangle-inequality-for-inner-product-norm)

[A1] Work in ZFC, including the Axiom of Choice inherited from the approximation and coarea suppliers. It is used when invoking their conclusions, in particular coarea in step 3.1; the band inclusion and norm estimate require no further choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### Proof

**Given:** The region, functions, convergence, boundary constants and area hypothesis in the Statement.

**Goal:** Prove the band integral estimate and the upper limit for the average level area.

1.1 Since $[a,b]\subset\operatorname{int}I$ and $I$ is an interval, choose $\delta>0$ with $[a-\delta,b+\delta]\subset I$. Uniform convergence gives $e_j\to0$, so for all sufficiently large $j$ the Borel interval $J_j=(a-e_j,b+e_j)$ is contained in $I$. If $u_j(x)\in J$, then $u(x)\ge u_j(x)-e_j>a-e_j$ and $u(x)\le u_j(x)+e_j<b+e_j$. Thus $\{u_j\in J\}\subset\{u\in J_j\}$, including when $e_j=0$. [given, algebra, choose]

2.1 Apply the inner-product norm triangle inequality [F3] in each tangent space where the weak gradients exist. It gives $|\nabla_k u_j|_k\le|\nabla_k u|_k+|\nabla_k u_j-\nabla_k u|_k$. Integrating on $\{u_j\in J\}$, enlarging the first integration set by step 1.1 and bounding the second integral by its integral over $R$ yields $\int_{\{u_j\in J\}}|\nabla_k u_j|_k\,dV_k\le\int_{\{u\in J_j\}}|\nabla_k u|_k\,dV_k+d_j$. The assumed metric first-Sobolev convergence gives $d_j\to0$. [given, F3, step 1.1, algebra]

3.1 Both $u$ and $u_j$ have the Lipschitz regularity and the exact boundary constants required by [F2]; the boundary parts exhaust $\partial R$ and the constants lie outside $I$ on opposite sides. For smooth approximants the smooth case of [F2] gives the same conclusion. Apply [F2], under [A1], to $u_j$ on the Borel interval $J$ and to $u$ on the Borel interval $J_j$. The resulting identities turn step 2.1 into $\int_J\mathcal H_k^2(\{u_j=t\})\,dt\le\int_{J_j}\mathcal H_k^2(\{u=t\})\,dt+d_j\le A|J_j|+d_j=A(b-a+2e_j)+d_j$. The second inequality uses $J_j\subset I$ and the given almost-everywhere area bound. Divide by $b-a>0$ and use $e_j,d_j\to0$ for the claimed upper limit. No convergence of individual level sets or their areas is asserted. [given, F2, A1, step 1.1, step 2.1, algebra] ∎


## Choosing a smooth separating regular level from an average bound

[Open item](item-lem-author-423fe0348a31-regular-separating-level) · level 7


### Statement

Work in ZFC. Let $(R,k)$ be a compact smooth three-dimensional manifold with boundary and smooth Riemannian metric $k$. Suppose $\partial R=B_-\sqcup B_+$, where $B_-$ and $B_+$ are disjoint unions of boundary components. Let $f:R\to\mathbb R$ be smooth up to the boundary, with $f=c_-$ on $B_-$ and $f=c_+$ on $B_+$, where $c_-<a<b<c_+$. No constancy on boundary neighborhoods is assumed.

Let $A,\epsilon\in\mathbb R$. On each component of $R$, let $\mathcal H_{k,\mathrm{un}}^2$ be unnormalised Hausdorff measure for the intrinsic length metric, and set $\mathcal H_k^2=(\pi/4)\mathcal H_{k,\mathrm{un}}^2$, summing over components. This is the normalized two-dimensional metric Hausdorff cut-area convention. If $\int_a^b\mathcal H_k^2(\{x\in R:f(x)=s\})\,ds<(A+\epsilon)(b-a)$, then there is a regular value $t\in(a,b)$ of $f|_{R^\circ}$ whose full level $D=\{x\in R:f(x)=t\}$ has area at most $A+\epsilon$.

The level $D$ is a compact smooth embedded surface without boundary, possibly empty or disconnected, and meets every continuous path in $R$ from $B_-$ to $B_+$. It is nonempty whenever such a path exists. The sublevel $\Omega=\{x\in R:f(x)\le t\}$, with its induced smooth structure, is a compact embedded three-dimensional submanifold with boundary $\partial\Omega=B_-\sqcup D$.

### Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Under countable choice, the critical values of a smooth map between smooth manifolds form a null set. Apply this to the boundaryless interior and target $\mathbb R$. [math:thm-morse-sard-for-smooth-manifolds](https://alphabetamath.cc/item/thm-morse-sard-for-smooth-manifolds)

[F2] A nonempty regular level of a smooth map is an embedded submanifold of the stated codimension. [math:thm-a-regular-level-set-is-an-embedded-submanifold](https://alphabetamath.cc/item/thm-a-regular-level-set-is-an-embedded-submanifold)

[F3] For a Lipschitz height constant near boundary parts exhausting the boundary, scalar coarea supplies a measurable normalized Hausdorff level-area function on intervening intervals. The supplier also shows, by bounding the gradient and integrating along curves, that a smooth function on a compact Riemannian region is Lipschitz for the intrinsic length distance on each component. [lem-author-423fe0348a31-riemannian-lipschitz-coarea](item-lem-author-423fe0348a31-riemannian-lipschitz-coarea)

[F4] A continuous real function on a closed interval takes every value between its endpoint values. [math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)

[F5] At a submersion point, adapted coordinates put a smooth map in local projection form. [math:cor-local-normal-form-for-submersions](https://alphabetamath.cc/item/cor-local-normal-form-for-submersions)

[F6] The metric is smooth and positive definite, boundary smoothness uses half-space charts with local smooth extensions, smooth maps are continuous and have coordinate representatives smooth in the local-extension sense, and an embedded submanifold with boundary has a smooth structure making its inclusion a smooth embedding. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary) [math:def-smooth-map-between-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-map-between-manifolds-with-boundary)

[F7] The axiom of choice implies countable choice, supplying the hypothesis of [F1]. [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F8] Nonnegative integrals are monotone and positively homogeneous, and their restriction to a measurable null set vanishes. [math:prop-order-and-scalar-rules-for-the-nonnegative-integral](https://alphabetamath.cc/item/prop-order-and-scalar-rules-for-the-nonnegative-integral) [math:cor-integral-over-a-null-set-vanishes](https://alphabetamath.cc/item/cor-integral-over-a-null-set-vanishes)

[F9] A regular value is a target point all of whose fibre points are submersion points; an empty fibre is allowed. A critical value is a target point that is not regular. [math:def-regular-and-critical-points-and-values](https://alphabetamath.cc/item/def-regular-and-critical-points-and-values)

[F10] Unnormalised Hausdorff measure is the limit of infimal diameter-squared covering costs. The normalized cut-area convention here is $\mathcal H_k^2=(\pi/4)\mathcal H_{k,\mathrm{un}}^2$ on each metric component, with component measures summed. The factor is the dimension-two specialization of the cited coarea source's $\omega_r/2^r$ normalization. [math:def-hausdorff-measure](https://alphabetamath.cc/item/def-hausdorff-measure) [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

### Proof

**Given:** The region, metric, boundary partition, smooth function, constants and strict average bound in the Statement, working in ZFC.

**Goal:** Choose the stated regular level and prove its area, separation and sublevel-boundary properties.

1.1 Choose $\alpha=(c_-+a)/2$ and $\beta=(b+c_+)/2$, and define $P(s)=\min\{\beta,\max\{\alpha,s\}\}$ and $v=P\circ f$. For $r\le s$, the three intervals cut out by $\alpha,\beta$ give $0\le P(s)-P(r)\le s-r$; hence $P$ is $1$-Lipschitz. By compactness the smooth gradient of $f$ is bounded, and integrating $df$ along piecewise smooth curves proves the length-Lipschitz bound used in [F3]. Thus $v$ is length-Lipschitz on each component. Continuity and the exact boundary values give neighborhoods of $B_-$ and $B_+$ on which $f<\alpha$ and $f>\beta$, respectively. On these neighborhoods $v=\alpha$ and $v=\beta$. The full boundary is exhausted by these parts, so [F3] applies to $v$ on $(a,b)$. For every $s\in(a,b)$, $\{v=s\}=\{f=s\}$, and this set lies in $R^\circ$ because the only boundary values of $f$ are $c_-$ and $c_+$. Consequently the full level-area function in the hypothesis is measurable, with the normalization fixed in [F10] and the interior interpretation supplied by coarea. [given, A1, F3, F6, F10, choose, construct, algebra]

2.1 By [A1] and [F7], [F1] applies to $f|_{R^\circ}:R^\circ\to\mathbb R$. Its regular values in $(a,b)$ therefore have full Lebesgue measure $b-a$. Put $M=A+\epsilon$; the strict hypothesis and nonnegativity of area imply $M>0$. If every regular value in $(a,b)$ had area greater than $M$, monotonicity on that full-measure set and the null-set rule in [F8] would give $\int_a^b\mathcal H_k^2(\{f=s\})\,ds\ge M(b-a)$, contrary to the hypothesis. Hence choose a regular $t\in(a,b)$ with level area at most $M$. [given, A1, F1, F7, F8, F9, step 1.1, choose, algebra]

3.1 Since $\partial R=B_-\sqcup B_+$ and $c_-<t<c_+$, $D=f^{-1}(t)$ misses all of $\partial R$. It is closed in compact $R$ and hence compact. If nonempty, it is an embedded codimension-one submanifold of $R^\circ$ by [F2], so it is a smooth surface without boundary. If empty, the empty surface has all these properties. No connectedness is required. [given, F2, F6, F9, step 2.1]

3.2 For any continuous path $\gamma:[0,1]\to R$ with $\gamma(0)\in B_-$ and $\gamma(1)\in B_+$, the function $f\circ\gamma$ is continuous with endpoint values $c_-$ and $c_+$. By [F4], it takes the value $t$, so the path meets $D$. In particular the existence of such a path implies $D\ne\varnothing$. [given, F4, F6, step 2.1]

4.1 The sublevel $\Omega=f^{-1}(( -\infty,t])$ is closed in compact $R$, so it is compact. At a point with $f<t$ it agrees locally with $R$, while points with $f>t$ have a neighborhood disjoint from it. At every point of $D\subset R^\circ$, regularity and [F5] give a smooth transverse coordinate $y_1=f-t$ (compose the projection coordinate with the inverse target chart); thus $\Omega$ has the half-space chart $y_1\le0$ and boundary $y_1=0$. Near $B_-$ it agrees with $R$ by continuity and $c_-<t$, so its boundary there is exactly the original boundary part $B_-$. Near $B_+$ it is empty by $c_+>t$. These exhaust the boundary cases. The charts are restrictions or smooth changes of the given charts, so they give the induced smooth structure and a smooth embedding into $R$. Therefore $\partial\Omega=B_-\sqcup D$, as asserted. [given, F5, F6, F9, step 2.1, step 3.1] ∎


## Coarea smoothing with fixed boundary values and area control

[Open item](item-lem-lipschitz-cut-coarea-smoothing-input) · level 8


### Statement

Let $(R,k)$ be a compact smooth Riemannian three-region with boundary $\partial R=B_-\sqcup B_+$ consisting of two smooth boundary components. Let $u$ be a real Lipschitz function, equal to constants $c_-$ and $c_+$ on neighborhoods of $B_-$ and $B_+$, where $c_-\le\inf I<\sup I\le c_+$ for a nonempty open interval $I$. Suppose $\mathcal H_k^2(\{u=t\})\le A<\infty$ for almost every $t\in I$, with $A\ge0$ and normalized metric Hausdorff measure. Then there is a sequence $u_j\in C^\infty(R)$ converging to $u$ in $C^0\cap W^{1,1}(R,k)$, with the exact same constants on fixed boundary neighborhoods. For every $\epsilon>0$, some $u_j$ has a regular value $t_j\in I$ with interior level $D_\epsilon=u_j^{-1}(t_j)$ separating the boundary components with $|D_\epsilon|_k\le A+\epsilon$. The set $\Omega_\epsilon=\{u_j\le t_j\}$ is a smooth compact region with $\partial\Omega_\epsilon=B_-\sqcup D_\epsilon$. The surface may be disconnected; if the boundary components can be joined by a path in $R$, it is nonempty. An endpoint-map area bound is a separate geometric input and is not asserted here.

### Facts & Assumptions

[F1] Relative mollification supplies a single uniform and metric first-Sobolev approximating sequence preserving the boundary constants. [lem-author-423fe0348a31-fixed-boundary-approximation](item-lem-author-423fe0348a31-fixed-boundary-approximation)

[F2] Riemannian Lipschitz and smooth coarea hold on interior bands with normalized metric Hausdorff level areas. [lem-author-423fe0348a31-riemannian-lipschitz-coarea](item-lem-author-423fe0348a31-riemannian-lipschitz-coarea)

[F3] Interval enlargement transfers the almost-everywhere area bound to a limiting average bound for the smooth approximants. [lem-author-423fe0348a31-band-energy-transfer](item-lem-author-423fe0348a31-band-energy-transfer)

[F4] A strict average bound and Sard supply a regular smooth separating level and its smooth sublevel region. [lem-author-423fe0348a31-regular-separating-level](item-lem-author-423fe0348a31-regular-separating-level)

[F5] Lipschitz weak gradients and cut areas have the fixed Riemannian conventions; endpoint multiplicity and endpoint-area formulas are separate inputs. [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[F6] Smoothness and support at the boundary use the local-extension and subordinate-cutoff conventions. [math:def-smooth-partition-of-unity-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-partition-of-unity-on-a-manifold-with-boundary)

[F7] Work in ZFC, including the analytic and Sard suppliers' countable-choice assumptions. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F8] A smooth Riemannian three-region is a three-dimensional smooth manifold with boundary equipped with a smooth positive-definite metric; boundary charts use compatible half-space charts and smooth local extensions. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

### Proof

**Given:**The hypotheses in the Statement.

**Goal:** Establish the stated construction or identity.

1.1 Apply [F1] to obtain $u_j$ with the stated fixed boundary neighborhoods. Choose any interval $J=(a,b)$ with $[a,b]\subset I$ and $a<b$. The coarea identity [F2] applies to $u$ and all $u_j$ on these interior bands. By [F3], $\int_J\mathcal H_k^2(\{u_j=t\})dt\le A(|J|+2e_j)+d_j$, where $e_j,d_j\to0$. [given, F1, F2, F3, F5, F6, F7]

2.1 Choose $j$ large enough that $2Ae_j+d_j<\epsilon|J|$. Then the last integral is strictly less than $(A+\epsilon)|J|$. The exact boundary constants remain below $a$ and above $b$. Apply [F4] to $u_j$ and $J$ to obtain a regular value $t_j\in J\subset I$ and its level $D_\epsilon=u_j^{-1}(t_j)$ with the asserted area, separation, compactness and smooth sublevel boundary. This proves the full statement without identifying BV perimeter with level area or assuming convergence of individual level surfaces. [step 1.1, F4, given, algebra] ∎

### Remarks

The area hypothesis is an input on the original Lipschitz levels. It may be supplied by a correctly justified endpoint construction, but this result requires no endpoint map, multiplicity-one assertion or regularity of the original cut. The independent coarea theorem is recorded in its helper; relative C0 and W11 approximation is proved locally by finite chart mollification rather than imported from a theorem asserting only Lipschitz-controlled uniform approximation.


## General curvature coefficient in the outward hypersurface gauge

[Open item](item-lem-author-6413ea293c6d-curvature-coefficient-conversion) · level 8


### Statement

In [lem-author-6413ea293c6d-null-variation-normalization](item-lem-author-6413ea293c6d-null-variation-normalization) and [lem-author-6413ea293c6d-second-form-and-connection-signs](item-lem-author-6413ea293c6d-second-form-and-connection-signs), write $G=\operatorname{Ric}-\tfrac12\operatorname{Scal}_g g$ for the Einstein tensor, and define the scalar $Y:=V|\chi_l|_q^2+G(l,u)$. For the unit outward variation of [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data), $Y=\tfrac12|\chi_L|_q^2+G(L,n)=\tfrac12|\chi_L|_q^2+\tfrac12G(L,L)+G(L,\underline L)$. In particular, if $\chi_L=0$ and $G(L,L)=0$, then $Y=G(L,\underline L)$. Vanishing expansion alone is not substituted for these two conditions.

### Facts & Assumptions

[F1] The normalized null decomposition and second-form identifications hold under the declared surface hypotheses. [lem-author-6413ea293c6d-null-variation-normalization](item-lem-author-6413ea293c6d-null-variation-normalization) [lem-author-6413ea293c6d-second-form-and-connection-signs](item-lem-author-6413ea293c6d-second-form-and-connection-signs) [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data)

[F2] Ricci curvature, scalar curvature and the Einstein tensor are the smooth metric-derived tensors of [physics:def-gr-curvature-tensor-and-derived-tensors](https://alphabetamath.cc/physics/item/def-gr-curvature-tensor-and-derived-tensors), Definition (c), on the smooth time-oriented Lorentzian four-manifold of [F1]. In particular, $G$ is a covariant two-tensor and is bilinear on each tangent space.

### Proof

**Given:** The data and explicit hypotheses of the Statement.

**Goal:** Establish its identities with the indicated normalizations.

1.1 The normalization lemma gives $V=1/2$, $u=n$ and $l=L$. Substitution into the defining scalar gives the first formula, using the same second fundamental form as the expansion. [given, F1, algebra]

2.1 The gauge identity $n=L/2+\underline L$ and bilinearity give the second formula. Setting the explicitly assumed $\chi_L$ and $G(L,L)$ to zero yields the final equality, without discarding either term otherwise. [step 1.1, F1, F2, algebra] ∎


## General MOTS first variation before electrovac specialization

[Open item](item-thm-mots-first-variation-input) · level 9


### Statement

Let $S$ be a smooth spacelike codimension-two surface in a smooth time-oriented Lorentzian four-manifold, with null-expansion conventions as in [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data). Choose smooth future null normals $l,k$ with $g(l,k)=-2$, and assume the outgoing expansion $\theta_l=0$ identically. For a smooth normal field $v$ with $g(l,v)=1$, write $v=-k/2+Vl$, $u=k/2+Vl$, $s_A=-g(k,\nabla_A l)/2$, and $Y=V|\chi_l|^2+G(l,u)$, where $G=\operatorname{Ric}-\operatorname{Scal}_g g/2$ and $|\chi_l|^2$ uses the positive surface metric. For each smooth real function $\phi$ under consideration, supply a smooth map $\Phi:S\times I\to M$ on a common open interval $I\ni0$, with $\Phi_0$ the inclusion, $\partial_\sigma\Phi|_0=\phi v$, and each $\Phi_\sigma$ a spacelike immersion. Supply also a smooth field $l_\sigma(p)\in T_{\Phi_\sigma(p)}M$ of future nonzero null normals to these slices, with $l_0=l$. Let $\theta_\sigma$ denote their null expansion pulled back to $S$; equivalently, it is the $\Phi_\sigma^*g$-trace of $(X,Y)\mapsto g(\nabla^{\Phi_\sigma}_Xl_\sigma,d\Phi_\sigma(Y))$, where $\nabla^{\Phi_\sigma}$ is the pullback connection. Define $\delta_{\phi v}\theta_l=\left.\partial_\sigma\theta_\sigma\right|_0$. At the stated MOTS this derivative depends only on $\phi v$ and the base normal $l$, not on the other choices of the supplied family and changing null gauge. On a noncompact $S$, existence of a common interval is an explicit requirement; the same formula applies locally on any supplied surface patch.

For such a supplied variation, $\delta_{\phi v}\theta_l=L_v\phi$ with
$$L_v\phi=-\Delta_S\phi+2s\cdot D\phi+(R_S/2-Y-|s|^2+\operatorname{div}_Ss)\phi.$$
Here $R_S$ is the intrinsic scalar curvature, so $R_S/2$ is the positive-round-sphere Gauss curvature in two dimensions. Use the sign agreement in [lem-author-6413ea293c6d-second-form-and-connection-signs](item-lem-author-6413ea293c6d-second-form-and-connection-signs). In the outward hypersurface gauge [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data), take $l=L$, $k=2\underline L$, $v=\nu$; then $s=\zeta$ and $Y=|\chi_L|^2/2+G(L,n)$ by [lem-author-6413ea293c6d-null-variation-normalization](item-lem-author-6413ea293c6d-null-variation-normalization) and [lem-author-6413ea293c6d-curvature-coefficient-conversion](item-lem-author-6413ea293c6d-curvature-coefficient-conversion). Thus at a geometric electrovac surface, if additionally $\chi_L=0$ and $\operatorname{Ric}(L,L)=0$, the zeroth coefficient is $K_S+\operatorname{div}\zeta-|\zeta|^2-e^2-b^2$, by [lem-author-6413ea293c6d-electrovac-normal-contraction](item-lem-author-6413ea293c6d-electrovac-normal-contraction). The null Ricci condition is supplied by [lem-author-6413ea293c6d-zero-optics-curvature](item-lem-author-6413ea293c6d-zero-optics-curvature) when its actual open null-congruence hypotheses hold. Mere MOTS status does not justify this last specialization.

### Facts & Assumptions

[F1] The formulation uses [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data) under its actual stated hypotheses.

[F2] The formulation uses [def-surface-area-flux-and-null-variation-data](item-def-surface-area-flux-and-null-variation-data) under its actual stated hypotheses.

[F3] The formulation uses [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data) under its actual stated hypotheses.

[F4] The formulation uses [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) under its actual stated hypotheses.

[F5] The formulation uses [lem-author-6413ea293c6d-null-variation-normalization](item-lem-author-6413ea293c6d-null-variation-normalization) under its actual stated hypotheses.

[F6] The formulation uses [lem-author-6413ea293c6d-second-form-and-connection-signs](item-lem-author-6413ea293c6d-second-form-and-connection-signs) under its actual stated hypotheses.

[F7] The formulation uses [lem-author-6413ea293c6d-curvature-coefficient-conversion](item-lem-author-6413ea293c6d-curvature-coefficient-conversion) under its actual stated hypotheses.

[F8] The formulation uses [lem-author-6413ea293c6d-electrovac-normal-contraction](item-lem-author-6413ea293c6d-electrovac-normal-contraction) under its actual stated hypotheses.

[F9] The formulation uses [lem-author-6413ea293c6d-zero-optics-curvature](item-lem-author-6413ea293c6d-zero-optics-curvature) under its actual stated hypotheses.

[F10] The metric-selected connection is metric-compatible: $X(g(Z,l))=g(\nabla_XZ,l)+g(Z,\nabla_Xl)$. This identity applies along the surface by restricting local extensions, with the pullback derivatives of [F1]. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F11] Andersson–Mars–Simon, §2 and §3 through Lemma 3.2, use $\mathbf K(X,Z)=-(\nabla_XZ)^\perp$ and $H=\operatorname{tr}_q\mathbf K$, where $q=g|_{TS}$. For the supplied variation and null normals, their MOTS formula is the operator in the Statement with $Y_{\mathrm{AMS}}=V\mathbf K^\mu_{AB}\mathbf K^{\nu AB}l_\mu l_\nu+G(l,u)$, raising the surface indices with $q^{-1}$, and their expansion is $g(H,l)$. The variation depends only on the initial velocity and base null normal at a MOTS. This is the imported premise recorded in the source reference and External input section. [Andersson–Mars–Simon, printed pp. 5–8](https://arxiv.org/pdf/0704.2889)

[F12] For a smooth Riemannian metric, scalar curvature in an orthonormal basis $(e_1,\ldots,e_n)$ is $2\sum_{i<j}K(\operatorname{span}(e_i,e_j))$, under countable choice. On the positive two-dimensional surface metric $q$, the only plane is $T_pS$, whose sectional curvature is $q(R^q(e_1,e_2)e_2,e_1)=K_S$ in the convention of [F2]. The countable-choice hypothesis is inherited from [F4]. [math:prop-scalar-curvature-is-twice-the-sum-of-sectional-curvatures-of-coordinate-planes](https://alphabetamath.cc/item/prop-scalar-curvature-is-twice-the-sum-of-sectional-curvatures-of-coordinate-planes)

### External input

The general first-variation formula, including the curvature coefficient Y, is imported from Andersson–Mars–Simon, §3 Lemma 3.1 and Lemma 3.2, equations (2)–(7), printed pp. 7–8. The general immersed-surface family, its varying null normal and the MOTS independence assertion are imported from the preceding variation-family paragraph in §3, printed p. 7, and Lemma 3.1. The supplied family and its common parameter interval are explicit hypotheses in the Statement. No local derivation of the Appendix A covariant variation calculation is claimed.

The five local lemmas separate the algebraic null normalization, second-form and normal-connection signs, coefficient conversion, electrovac contraction, and null-hypersurface condition required by the application. For the outward hypersurface specialization only, the normal-graph supplier provides the actual family and its smooth null gauge, on its stated admissible domain. It is an instance of the general immersed-surface variation defined above; no such family for an arbitrary normal $v$ is obtained from that supplier. The article-specific horizon hypotheses must be supplied by the consumer; this input makes no claim that an arbitrary MOTS has zero null second form or zero null Ricci contraction.

### Proof

**Given:** The general surface, supplied variation and normalized null normals of the Statement, with the inherited choice assumptions in [F1]–[F4]. The hypersurface and electrovac data are imposed only for the corresponding specializations.

**Goal:** Convert the imported first-variation formula to the stated null-second-form convention and apply the existing specialization suppliers.

1.1 Work on an arbitrary surface patch with smooth tangent fields $X,Z$ and the given normal $l$. The positive metric $q=g|_{TS}$ makes the tangent plane nondegenerate, so orthogonal projection onto its normal complement is defined. Set $\mathbf K(X,Z)=-(\nabla_XZ)^\perp$ as in [F11]. Because $l$ is normal, projection does not change its pairing with $\nabla_XZ$. Also $g(Z,l)=0$ identically on the patch. Differentiating this identity along $X$ using [F10] gives $g(\mathbf K(X,Z),l)=-g(\nabla_XZ,l)=g(Z,\nabla_Xl)=\chi_l(X,Z)$. These are derivatives along the surface, so the identity is independent of the chosen local extensions. No hypersurface containing $S$ is assumed in this calculation. [given, F1, F10, F11, algebra]

2.1 Taking the $q$-trace of step 1.1 gives $g(H,l)=\theta_l$, so the source MOTS condition is precisely the one in the Statement. In a local tangent frame, contraction of step 1.1 with the two inverse surface metrics gives $\mathbf K^\mu_{AB}\mathbf K^{\nu AB}l_\mu l_\nu=q^{AC}q^{BD}\chi_{l,AB}\chi_{l,CD}=|\chi_l|_q^2$. Thus $Y_{\mathrm{AMS}}=V|\chi_l|_q^2+G(l,u)=Y$. The explicitly supplied family, its common interval, its smooth null normals and $g(l,v)=1$ satisfy [F11], which applies also to nonclosed surface patches. Substituting this coefficient in that imported formula proves the general displayed operator and its stated independence of the family and varying null gauge. This step imports the covariant variation calculation; it does not reconstruct it. [given, F1, F11, step 1.1, algebra]

3.1 Now impose the outward hypersurface gauge of [F2]. The normalization in [F5] gives $V=1/2$ and $u=n$ for $l=L$, $k=2\underline L$ and $v=\nu$. In this gauge [F6] gives $s=\zeta$, and [F7] gives $Y=|\chi_L|^2/2+G(L,n)$. The sign-agreement supplier [F6] is used only at this hypersurface specialization; the general conversion was proved in step 1.1. The family and null gauge supplied by [F2], on their admissible domain, are an instance of the supplied variation used in step 2.1. [F2, F5, F6, F7, step 2.1, algebra]

4.1 Finally impose the geometric electrovac equations of [F3] and the additional conditions $\chi_L=0$ and $\operatorname{Ric}(L,L)=0$. By [F8], $\operatorname{Scal}_g=0$, hence $G=\operatorname{Ric}$, and $G(L,\underline L)=e^2+b^2$. Since $g(L,L)=0$, the assumed null Ricci condition also gives $G(L,L)=0$. The coefficient conversion [F7] therefore reduces $Y$ to $e^2+b^2$. The smooth positive surface metric $q$ in [F2] satisfies [F12], with countable choice inherited from [F4]. In dimension two its sum has the single tangent plane, with sectional curvature $K_S=q(R^q(e_1,e_2)e_2,e_1)$ in the convention of [F2]. Thus $R_S=2K_S$, and substituting $R_S/2=K_S$ in step 2.1 gives the asserted specialized operator. If the open null-congruence hypotheses of [F9] hold, that supplier provides the required null Ricci condition. Otherwise it remains an explicit additional hypothesis, and it is never inferred from MOTS status alone. [given, F2, F3, F4, F7, F8, F9, F12, step 2.1, step 3.1, algebra] ∎
