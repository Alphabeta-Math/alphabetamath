---
id: lem-author-294e9b08725d-abstract-complete-boost-band
title: A complete stationary boost band with a global local-isometry certificate
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - lem-author-294e9b08725d-canonical-double-stationary-realization
  - thm-author-294e9b08725d-radu-local-bifurcate-collar-input
  - def-spacelike-maximal-hypersurface-data
  - def-causal-exterior-and-boundary-data
  - math:def-countable-choice
  - math:def-dependent-choice
  - physics:lem-gr-finite-smooth-volume-density
  - physics:thm-gr-volume-time-function
  - physics:thm-gr-smooth-cauchy-temporal-splitting
  - math:thm-fundamental-theorem-on-flows
  - math:def-pullback-of-a-covariant-tensor-field
  - math:def-lie-derivative-of-a-tensor-field
  - math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes
  - physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative
  - physics:thm-gr-curvature-tensoriality-and-coordinate-formula
  - physics:def-gr-curvature-tensor-and-derived-tensors
dependency_roles:
  lem-author-294e9b08725d-canonical-double-stationary-realization: mathematical-premise
  thm-author-294e9b08725d-radu-local-bifurcate-collar-input: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-dependent-choice: mathematical-premise
  physics:lem-gr-finite-smooth-volume-density: mathematical-premise
  physics:thm-gr-volume-time-function: mathematical-premise
  physics:thm-gr-smooth-cauchy-temporal-splitting: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  math:def-pullback-of-a-covariant-tensor-field: mathematical-premise
  math:def-lie-derivative-of-a-tensor-field: mathematical-premise
  math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes: mathematical-premise
  physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative: mathematical-premise
  physics:thm-gr-curvature-tensoriality-and-coordinate-formula: mathematical-premise
  physics:def-gr-curvature-tensor-and-derived-tensors: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references: []
proof_strategy: direct
dependency_level: 13
---

## Statement

Assume Countable Choice and Dependent Choice. Let $(\widehat M,\widehat g)$ be a smooth time-oriented globally hyperbolic vacuum four-manifold with complete Killing field $\widehat T$. Supply a nonempty compact smooth two-manifold $S$, a number $\eta>0$, and a product neighborhood embedding $F_0:W\to\widehat M$, where $W=(-\eta,\eta)^2\times S$ and $F_0(\{U=V=0\})$ is the bifurcation surface. Write $g_0=F_0^*\widehat g$. Require a constant $\kappa>0$ and a $g_0$-Killing field $K=\kappa(V\partial_V-U\partial_U)$. In the rotating case require a smooth circle action $\phi_s^Z$ on $S$ of period $2\pi$ whose product lift to $W$ is a $g_0$-isometry; its generator $Z$ is tangent to the $S$ factor, preserves $U,V$, and satisfies $[K,Z]=0$. Require a constant $\Omega$ and $F_0^*\widehat T=K-\Omega Z$. In the nonrotating case set $\Omega=0$, omit $Z$ and its action, and require $F_0^*\widehat T=K$.

For sufficiently small $0<\delta<\eta$, the abstract manifold $\mathcal B=\{(U,V,p)\in\mathbb R^2\times S:|UV|<\delta^2\}$ carries a smooth vacuum metric, the complete stationary isometric action $A_t(U,V,p)=(e^{-\kappa t}U,e^{\kappa t}V,\phi^Z_{-\Omega t}p)$, and a smooth local isometry $F:\mathcal B\to\widehat M$ agreeing with $F_0$ on $W\cap\mathcal B$ and intertwining $A_t$ with the complete $\widehat T$ flow. The map $F$ is not asserted injective. The lifted circle action is isometric, and the pure boost $K$ is also complete and Killing on the band. The band has a smooth temporal function pulled back from a smooth Cauchy temporal function on $\widehat M$; the pullback is not asserted Cauchy.

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** Construct the complete band, its local-isometry certificate and its temporal function.

[F1] The complete smooth field $\widehat T$ has a smooth global flow $\Phi_t$, with inverse $\Phi_{-t}$, the flow composition law and uniqueness of integral curves. [[math:thm-fundamental-theorem-on-flows]]

[F2] Under their own hypotheses, the canonical-realization and local-collar suppliers describe the intended ambient spacetime and positive-$\kappa$ commuting boost/circle germs. These are contextual descriptions of the intended application. The abstract construction assumes the ambient data and full product geometry explicitly as stated; neither supplier is invoked here to derive those hypotheses from global hyperbolicity. [[lem-author-294e9b08725d-canonical-double-stationary-realization]] [[thm-author-294e9b08725d-radu-local-bifurcate-collar-input]]

[F3] Global hyperbolicity, the time orientation and the temporal-function convention are those of the causal-data interface; the induced spacelike geometry has the hypersurface-data convention. Pullback tensors are evaluated by applying the differential to each vector argument. [[def-causal-exterior-and-boundary-data]] [[def-spacelike-maximal-hypersurface-data]] [[math:def-pullback-of-a-covariant-tensor-field]]

[A1] Countable Choice and Dependent Choice are assumed for the temporal-function suppliers. [[math:def-countable-choice]] [[math:def-dependent-choice]]

[F4] On a nonempty time-oriented smooth Lorentzian four-manifold, Countable Choice supplies a positive smooth density with total measure one, positive measure on every nonempty open set, and zero measure on chart-Lebesgue-null Borel sets. On a globally hyperbolic such manifold, Countable Choice and Dependent Choice then give the continuous volume time function. With that volume time, the smooth Cauchy temporal splitting theorem supplies a smooth Cauchy temporal function with past timelike gradient. [[physics:lem-gr-finite-smooth-volume-density]] [[physics:thm-gr-volume-time-function]] [[physics:thm-gr-smooth-cauchy-temporal-splitting]]

[F5] The Lie derivative is the derivative at zero of tensor pullback by the local flow. A smooth tensor is invariant on every common local flow domain exactly when its Lie derivative vanishes; the flow derivative is $\frac{d}{dt}\Phi_t^*H=\Phi_t^*(\mathcal L_XH)$ for a smooth tensor $H$ and the flow of $X$. Applied to a complete Killing field this gives metric invariance for every real flow parameter. [[math:def-lie-derivative-of-a-tensor-field]] [[math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes]]

[F6] Under Countable Choice, a smooth nondegenerate metric on a smooth four-manifold has its unique Levi–Civita connection, whose Christoffel symbols in a chart are $\Gamma^a{}_{bc}=\tfrac12g^{ad}(\partial_bg_{dc}+\partial_cg_{bd}-\partial_dg_{bc})$. For a time-oriented smooth Lorentzian four-manifold the curvature formula is $R^a{}_{bcd}=\partial_c\Gamma^a{}_{db}-\partial_d\Gamma^a{}_{cb}+\sum_e(\Gamma^a{}_{ce}\Gamma^e{}_{db}-\Gamma^a{}_{de}\Gamma^e{}_{cb})$, and $\operatorname{Ric}_{bd}=\sum_a R^a{}_{bad}$. The last identity is the defining metric contraction $\sum_{a,c}g^{ac}R_{abcd}$ after lowering the first index of $R$. Here vacuum means precisely $\operatorname{Ric}=0$, with no physical field-law premise. [[physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative]] [[physics:thm-gr-curvature-tensoriality-and-coordinate-formula]] [[physics:def-gr-curvature-tensor-and-derived-tensors]]

## Proof

1.1 Fix $0<\delta<\eta$. The product circle action and the boost define $A_t$ for every $t\in\mathbb R$, preserve $UV$, and commute. Every $q\in\mathcal B$ has a parameter $t$ with $A_{-t}q\in W$. If $UV\ne0$, the equation $e^{\kappa t}|U|=e^{-\kappa t}|V|$ has a real solution because $\kappa>0$, and both balanced absolute coordinates equal $\sqrt{|UV|}<\delta<\eta$. If exactly one coordinate is nonzero, choose the sign and size of $t$ to shrink it below $\eta$; if both vanish, every parameter works. Define $F(q)=\Phi_t(F_0(A_{-t}q))$ using any such parameter. This construction uses only the explicitly assumed local geometry, with the circle factor omitted in the nonrotating case. [given, F1, algebra]

2.1 The working parameters for each $q$ form an interval: each absolute normal coordinate is monotone in $t$, and the circle action keeps the $S$ factor inside $S$. For any two working parameters the entire intervening segment therefore stays in $W$. On that segment, $F_0$ carries the generator $K-\Omega Z$ to $\widehat T$, so uniqueness of integral curves gives equality of the two definitions of $F(q)$. This also applies at $U=V=0$, where the full circle orbit stays in $W$. A fixed working parameter remains working near $q$ by openness; on this neighborhood $F=\Phi_t\circ F_0\circ A_{-t}$ is smooth and a local diffeomorphism. The parameter $t=0$ gives $F=F_0$ on $W\cap\mathcal B$. If $t$ works for $q$, then $t+s$ works for $A_s q$; the flow law yields $F(A_s q)=\Phi_s(F(q))$ for every real $s$. [given, step 1.1, F1]

3.1 Set $g_{\mathcal B}=F^*\widehat g$. The pullback evaluation formula and the invertibility of $dF$ give a smooth nondegenerate Lorentzian metric of the same signature as $\widehat g$, agreeing with $g_0$ on $W\cap\mathcal B$. Pull back the ambient time orientation through $dF$: the inverse image of any ambient smooth future timelike orientation field is smooth and timelike, and selects the future cone on the band. Thus $F$ is a time-orientation-preserving local isometry. [step 2.1, F3, algebra]

4.1 To verify the vacuum assertion locally, fix $q\in\mathcal B$ and restrict $F$ to a diffeomorphism from a neighborhood $O$ of $q$ onto a chart neighborhood $(Q,x)$ in $\widehat M$. Use $y=x\circ F$ as the coordinates on $O$. In these coordinates the coefficient functions of $g_{\mathcal B}$ and $\widehat g$, viewed on the same open subset of $\mathbb R^4$, are identical by the pullback formula. Their inverse matrices and all derivatives are therefore identical. Countable Choice from [A1] permits the Levi–Civita formula in [F6] for these smooth nondegenerate four-dimensional metrics. That formula gives identical Christoffel coefficient functions, and the curvature formula and Ricci contraction of [F6] give identical Ricci coefficient functions. The ambient ones vanish by hypothesis, hence $\operatorname{Ric}(g_{\mathcal B})=0$ on $O$. Since $q$ was arbitrary, the band is vacuum everywhere. This proves the needed local naturality directly in matching charts. [given, step 3.1, A1, F3, F6, algebra]

5.1 By [F5], $\mathcal L_{\widehat T}\widehat g=0$ implies $\Phi_t^*\widehat g=\widehat g$ for every real $t$. Equivariance from step 2.1 and the pullback formula then give $A_t^*g_{\mathcal B}=g_{\mathcal B}$. In the rotating case write $R_s(U,V,p)=(U,V,\phi_s^Zp)$. Take the same working parameter in neighborhoods of $q$ and $R_s q$, which is possible because $R_s$ changes neither normal coordinate. The expression $F=\Phi_t\circ F_0\circ A_{-t}$ and commutation of $R_s$ with $A_{-t}$ reduce $R_s^*g_{\mathcal B}=g_{\mathcal B}$ to the assumed $R_s^*g_0=g_0$. The stationary field is complete because $A_t$ is defined for all real $t$. The commuting isometric action $A_tR_{\Omega t}$ is the pure boost flow, proving that $K$ too is complete and Killing by differentiation at zero in [F5]. In the nonrotating case the circle terms are omitted and $A_t$ itself is the complete pure boost flow. [given, step 2.1, step 3.1, step 4.1, F1, F3, F5, algebra]

6.1 Apply the finite-density supplier to $\widehat M$ (nonempty because it contains the product neighborhood), then the volume-time theorem and the smooth Cauchy temporal splitting theorem. Their hypotheses hold: $\widehat M$ is a time-oriented smooth globally hyperbolic Lorentzian four-manifold, and both choice assumptions are [A1]. This produces a smooth Cauchy temporal function $\widehat\tau$. For $\tau=\widehat\tau\circ F$, the local-isometry identity gives $g_{\mathcal B}^{-1}(d\tau,d\tau)=\widehat g^{-1}(d\widehat\tau,d\widehat\tau)\circ F<0$. The pulled-back time orientation gives $d\tau(v)>0$ for every nonzero future causal $v$. Thus $\tau$ is temporal on the whole band. Neither injectivity of $F$ nor a Cauchy property of its pulled-back levels is used. [step 5.1, A1, F3, F4, algebra] ∎
