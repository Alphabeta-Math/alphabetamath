---
id: pthm-ernst-potential-existence
title: Closed Ernst form and existence of normalized potential
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-killing-ernst-notation
  - thm-vacuum-killing-ernst-input
  - lem-spherical-exterior-period-input
  - math:def-axiom-of-choice
  - lem-author-e7cde3233cd7-cauchy-section-product
  - lem-author-e7cde3233cd7-one-sided-boundary-exclusion
  - lem-author-e7cde3233cd7-spherical-cauchy-portion
  - lem-author-e7cde3233cd7-normalized-end-primitive
  - lem-author-e7cde3233cd7-horizon-neighborhood-gluing
  - lem-author-a4a441da4986-doc-connected-and-causally-convex
  - math:cor-euclidean-spheres-are-path-connected
  - math:thm-path-connected-implies-connected
  - math:thm-connectedness-characterisations
  - def-causal-exterior-and-boundary-data
  - physics:def-gr-smooth-lorentzian-objects
  - physics:lem-gr-chronology-openness
  - physics:lem-gr-causal-curve-calculus
  - math:def-embedded-submanifold-and-slice-chart
  - math:thm-tubular-neighbourhood-theorem-in-a-smooth-ambient-manifold
  - math:thm-smooth-inverse-function-theorem-on-manifolds
  - math:lem-smooth-bump-between-concentric-euclidean-balls
  - math:thm-de-rham-cohomology-of-spheres
  - math:thm-de-rham-cohomology-is-smooth-homotopy-invariant
  - math:def-de-rham-cohomology
  - math:def-closed-and-exact-differential-forms
  - math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component
  - math:lem-ac-supplies-countable-and-dependent-choice-for-banach-integration
  - math:thm-every-smooth-vector-bundle-admits-a-smooth-bundle-metric
  - math:def-smooth-bundle-metric
  - math:def-tubular-neighbourhood-of-an-embedded-submanifold
  - math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-killing-ernst-notation: mathematical-premise
  thm-vacuum-killing-ernst-input: mathematical-premise
  lem-spherical-exterior-period-input: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  lem-author-e7cde3233cd7-cauchy-section-product: mathematical-premise
  lem-author-e7cde3233cd7-one-sided-boundary-exclusion: mathematical-premise
  lem-author-e7cde3233cd7-spherical-cauchy-portion: mathematical-premise
  lem-author-e7cde3233cd7-normalized-end-primitive: mathematical-premise
  lem-author-e7cde3233cd7-horizon-neighborhood-gluing: mathematical-premise
  lem-author-a4a441da4986-doc-connected-and-causally-convex: mathematical-premise
  math:cor-euclidean-spheres-are-path-connected: mathematical-premise
  math:thm-path-connected-implies-connected: mathematical-premise
  math:thm-connectedness-characterisations: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:lem-gr-chronology-openness: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  math:thm-tubular-neighbourhood-theorem-in-a-smooth-ambient-manifold: mathematical-premise
  math:thm-smooth-inverse-function-theorem-on-manifolds: mathematical-premise
  math:lem-smooth-bump-between-concentric-euclidean-balls: mathematical-premise
  math:thm-de-rham-cohomology-of-spheres: mathematical-premise
  math:thm-de-rham-cohomology-is-smooth-homotopy-invariant: mathematical-premise
  math:def-de-rham-cohomology: mathematical-premise
  math:def-closed-and-exact-differential-forms: mathematical-premise
  math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component: mathematical-premise
  math:lem-ac-supplies-countable-and-dependent-choice-for-banach-integration: mathematical-premise
  math:thm-every-smooth-vector-bundle-admits-a-smooth-bundle-metric: mathematical-premise
  math:def-smooth-bundle-metric: mathematical-premise
  math:def-tubular-neighbourhood-of-an-embedded-submanifold: mathematical-premise
  math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp.3–4 Definition 1.1 and the Ernst-potential paragraph; PDF p.7
        §2.1 final paragraph
      attribution: The article states that the vacuum Ernst one-form is closed and
        uses a globally defined potential normalized to one at infinity.
      hypotheses: The regular stationary vacuum spacetime conditions stated in
        Definition 1.1. This citation records article attribution only; the
        proof uses the explicit independent local/library prerequisite chain.
      reading_limits: Read the frozen original article text at these locations and
        inspected the supplied PDF page-4 image. The article is not used as
        proof of its own prerequisites. Read the exact declared library supplier
        Statements and existing authored local interfaces; no new reading or
        verification of the library suppliers’ external literature is asserted.
physical_scope: Conditional deduction in the smooth four-dimensional stationary
  vacuum model, with the precise regularity and asymptotic hypotheses of the
  declared definition; no measurement or existence of such a spacetime is
  asserted.
dependency_level: 6
---

## Statement

For the article's regular stationary vacuum spacetime, the complex one-form $\eta_a=2T^b\mathcal F_{ba}$ is closed and has a unique normalized smooth potential $\sigma=f+i\psi$ on the exterior $E$, with $\mathrm d\sigma=\eta$, $f=-g(T,T)$ and $\sigma\to1$ at its asymptotically flat end. After shrinking a neighborhood $O$ of the bifurcation sphere, this potential extends smoothly to $E\cup O$. It is stationary and the normalization is consistent across the end and the horizon overlap. This is a conditional consequence of the regularity and vacuum hypotheses; no maximal-slice assumption is required for this generic topological product argument.

## Facts & Assumptions

[A1] Adopt the stationary vacuum model [[post-stationary-vacuum-model]] and exactly the geometric and asymptotic conditions of [[def-regular-stationary-vacuum-spacetime]], with the notation [[def-killing-ernst-notation]]. Work in ZFC including [[math:def-axiom-of-choice]]. In particular, $C=\Sigma_0\cap E$ is a smooth spacelike Cauchy hypersurface, a supplied diffeomorphism $\chi:\{|x|>1/2\}\to\Sigma_0$ identifies $S$ with $|x|=1$, and the two ambient chronological boundaries are smooth transverse null hypersurfaces near $S$. The end section is $t=0$ in its own supplied end coordinates. No equality between those coordinates and $\chi$ is assumed.

[F1] The vacuum Killing identities give $\mathrm d\eta=0$ on the ambient spacetime and $\operatorname{Re}\eta=\mathrm df$. [[thm-vacuum-killing-ernst-input]]

[F2] A specified spherical product has exact closed complex one-forms. [[lem-spherical-exterior-period-input]]

[F3] For connected open $U$, the causal-exterior result gives connectedness of $E=I^-_M(U)\cap I^+_M(U)$ and $U\subset E$. The generic Cauchy-flow result then gives connectedness of $C$ and $E\cong\mathbb R\times C$; the one-sided-boundary result confines ambient closure points of $C$ outside $E$ to the double boundary $S$. [[lem-author-a4a441da4986-doc-connected-and-causally-convex]] [[lem-author-e7cde3233cd7-cauchy-section-product]] [[lem-author-e7cde3233cd7-one-sided-boundary-exclusion]] The explicit polar-coordinate construction in Proof 4.1 of [[lem-author-e7cde3233cd7-spherical-cauchy-portion]] gives the smooth maps $x\mapsto(|x|,x/|x|)$ and $(r,\omega)\mapsto r\omega$ in sphere product charts. Only that coordinate calculation is used below, not that lemma's additional end-coordinate matching hypothesis or its selection of the outer component.

[F4] Integrable asymptotic twist fixes the complex constant by [[lem-author-e7cde3233cd7-normalized-end-primitive]]. The horizon argument below adapts the defining-function, tubular-coordinate and constant-matching construction in [[lem-author-e7cde3233cd7-horizon-neighborhood-gluing]], but supplies the local proof using [F6]–[F11]. It does not apply that helper's Statement, whose global coordinate-matching hypothesis is absent here.

[F5] The unit sphere in $\mathbb R^3$ is path connected. A path-connected space is connected, and a connected space has only the empty set and itself as clopen subsets. [[math:cor-euclidean-spheres-are-path-connected]] [[math:thm-path-connected-implies-connected]] [[math:thm-connectedness-characterisations]]

[F6] The ambient manifold is Hausdorff and second countable, and the time orientation is a smooth future timelike field $N$. The future timelike cone is convex. These are the geometric conventions of [[physics:def-gr-smooth-lorentzian-objects]]. AC supplies Countable Choice and Dependent Choice by [[math:lem-ac-supplies-countable-and-dependent-choice-for-banach-integration]], covering the choice hypotheses of the causal, tubular, bundle-metric and sphere-cohomology inputs below.

[F7] Chronology and ambient boundaries use [[def-causal-exterior-and-boundary-data]]. Chronological point futures and pasts are open; if $p$ is in the closure of a past set $P$, then $I^-_M(p)\subset P$, and dually for future sets. These are clauses (a) and (c) of [[physics:lem-gr-chronology-openness]]. Smooth future timelike arcs and their finite concatenations are admissible timelike curves by clauses (c) and (d) of [[physics:lem-gr-causal-curve-calculus]], so chronology is transitive.

[F8] A smooth embedded hypersurface has slice charts, hence local defining functions with nonzero differential. [[math:def-embedded-submanifold-and-slice-chart]] A smooth map with invertible differential has a smooth local inverse. [[math:thm-smooth-inverse-function-theorem-on-manifolds]] Given concentric chart balls of radii $0<r<R$, there is a smooth $[0,1]$-valued bump equal to one on the closed smaller ball and supported in the larger ball. [[math:lem-smooth-bump-between-concentric-euclidean-balls]]

[F9] A closed embedded submanifold has a tubular neighborhood, diffeomorphic to an open neighborhood of its zero section in the quotient normal bundle, with smooth projection to the submanifold. [[math:thm-tubular-neighbourhood-theorem-in-a-smooth-ambient-manifold]] Every smooth vector bundle admits a smooth fibrewise positive-definite inner product under Countable Choice. [[math:thm-every-smooth-vector-bundle-admits-a-smooth-bundle-metric]] [[math:def-smooth-bundle-metric]] The tubular-map and local linear bundle-chart conventions are [[math:def-tubular-neighbourhood-of-an-embedded-submanifold]] and [[math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle]].

[F10] Smooth homotopy equivalences induce isomorphisms in real de Rham cohomology; under Countable Choice $H^1_{\mathrm{dR}}(S^2)=0$. [[math:thm-de-rham-cohomology-is-smooth-homotopy-invariant]] [[math:thm-de-rham-cohomology-of-spheres]] A zero class of a closed one-form means that it is the differential of a smooth real function. Apply this separately to real and imaginary parts for a complex form. [[math:def-de-rham-cohomology]] [[math:def-closed-and-exact-differential-forms]]

[F11] A smooth real function with zero differential is constant on each connected component. Apply this to both components of a complex function. [[math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component]]

## Proof

**Given:** The model, regularity, end and horizon hypotheses in the Statement and [A1], without an additional coordinate-matching hypothesis.

**Goal:** Construct and normalize the exterior potential and extend it across the bifurcation sphere.

1.1 Put $U=M^{\mathrm{end}}$, $P=I^-_M(U)$ and $Q=I^+_M(U)$. The end is a nonempty connected open product, so [F3] gives connected nonempty $E=P\cap Q$ with $U\subset E$. Its supplied smooth spacelike Cauchy section $C$ is connected, and the generic Cauchy-flow diffeomorphism gives $E\cong\mathbb R\times C$. Since $E$ is open, $C$ is open in $\Sigma_0$. Every relative boundary point of $C$ in $\Sigma_0$ is an ambient closure point outside $E$, so the one-sided-boundary result puts it in $S$. The set $S$ is disjoint from $E$, since it is contained in the boundary of each of the open sets $P,Q$. Hence $C$ is nonempty and clopen in $\Sigma_0\setminus S$. [A1, F3]

2.1 In the chart $\chi$, the complement of $S$ is the disjoint union of the clopen radial shells $A_-:=\{1/2<|x|<1\}$ and $A_+:=\{|x|>1\}$. Each is path connected: join two points radially to a common radius within its interval, join their directions on the unit sphere using [F5], and reverse the second radial segment. Thus both shells are connected by [F5]. Connectedness of $C$ prevents it from meeting both shells. Its intersection with the one it meets is nonempty and clopen there, so [F5] makes that intersection the whole shell. Consequently $\chi^{-1}(C)$ is exactly one of $A_-,A_+$. Selecting which shell contains the physical end is unnecessary for the following exactness argument. [A1, F5, step 1.1]

2.2 By [F6] all the choice requirements below hold. By [F7], $P$ and $Q$ are open unions of chronological point pasts and futures; transitivity makes $P$ a past set and $Q$ a future set. At $p\in\partial_M P$, let a short smooth future timelike arc $\gamma$ pass through $p=\gamma(0)$. For $t<0$ the closure rule gives $\gamma(t)\in I^-_M(p)\subset P$. For $t>0$, membership $\gamma(t)\in\overline P$ would give $p\in I^-_M(\gamma(t))\subset P$, impossible since $P$ is open and $p\in\partial_M P$. Thus the positive-time side is outside $\overline P$. Reversing time, at $p\in\partial_M Q$ the positive-time side is in $Q$ and the negative-time side is outside $\overline Q$. [F6, F7, step 1.1]

3.1 The polar maps in [F3] identify either shell smoothly with its radial interval times $S^2$: the same stereographic-coordinate formulas in that proof are smooth for every $r>0$. For $A_+$ retain $R=r$. For $A_-$ set $R=(2r-1)^{-1}>1$, with smooth inverse $r=(1+R^{-1})/2$. These explicit maps identify either possible $C$ with $(1,\infty)\times S^2$. Compose with the generic product from step 1.1 to obtain a specified diffeomorphism $E\cong\mathbb R\times(1,\infty)\times S^2$. This product need not be generated by the stationary field, and no spatial identification with the asymptotic chart has been made. [F3, step 1.1, step 2.1, algebra]

3.2 Work near $S$ where the two boundaries are smooth and null by [A1]. A null tangent hyperplane has nonnegative induced metric, so it contains no timelike vector; hence $N$ is transverse to each branch. At each boundary point choose coordinates $(y,t)$ with $\partial_t$ equal to $N$ at that point, and shrink so $\partial_t$ remains future timelike. For a local defining function $h$ from [F8], $\partial_t h\ne0$ at the point. Applying the inverse function theorem to $(y,t)\mapsto(y,h(y,t))$ writes the boundary as a graph $t=a(y)$ in a smaller box. Each vertical segment through this graph is an arc in step 2.2. Thus $r_i=a(y)-t$ is positive precisely on $P$, zero on its boundary and negative outside $\overline P$ in a box for $\partial_M P$; $r_i=t-a(y)$ has the corresponding signs for $Q$. On the boundary, $dr_i$ is nonzero on every timelike vector. Convexity of the future timelike cone in [F6] implies that $dr_i(N)$ has the sign of $dr_i(\partial_t)$, negative for $P$ and positive for $Q$: otherwise it vanishes on a vector on their timelike line segment. [A1, F6, F7, F8, step 2.2]

4.1 The ambient complex one-form $\eta$ is smooth and closed by [F1]. The product in step 3.1 verifies the exact hypothesis of [F2], so there is a smooth primitive on $E$. The original end has $T=\partial_t$ and exactly the differentiated vacuum metric bounds in [A1]. Thus the normalization result in [F4] applies in that end's own chart and shifts the primitive by one complex constant to $\sigma=f+i\psi\to1$, with $f=-g(T,T)$. Its stationary end conclusion makes the limit uniform in the time coordinate as well as in angle. This application is independent of the auxiliary coordinates used in step 3.1. [A1, F1, F2, F4, step 3.1]

4.2 For each branch separately, take finitely many smaller coordinate balls covering the compact sphere $S$, with closures inside boxes of step 3.2, and choose the bumps $b_i$ of [F8] equal to one on the smaller balls and supported inside their boxes. Extend $b_i$ and $b_i r_i$ by zero outside each box; the extensions are smooth since their supports stay inside the boxes. On the neighborhood $W=\{\sum_i b_i>0\}$ define $r=(\sum_i b_i r_i)/(\sum_i b_i)$. All active $r_i$ have the same sign, determined by membership in the chronological set, its boundary or the complement of its closure; hence $r$ has those same signs and zeros. On the boundary, differentiating the weights contributes zero because each $r_i$ there is zero. Thus $dr(N)$ is a weighted average of strictly negative numbers for $P$, or of strictly positive numbers for $Q$, and is nonzero. Intersect the two resulting neighborhoods to obtain functions $u,v$ near $S$ with $P=\{u>0\}$, $Q=\{v>0\}$ and the respective boundaries as their zero sets. Transversality in [A1] makes $du,dv$ independent along $S$, with common kernel $TS$. [A1, F8, step 3.2]

5.1 The compact embedded sphere $S$ is closed in the Hausdorff manifold $M$. Take a tubular map $\Phi$ and projection $\pi$ from [F9], restricting its image to the neighborhood of step 4.2, and consider $G=(\pi,u,v)$. Along $S$, $d\pi$ is the identity on $TS$, while $du,dv$ have common kernel $TS$, so $dG$ is invertible. By [F8], $G$ is a local diffeomorphism near $S$. Choose the smooth normal-bundle metric of [F9]. Compactness of the zero section gives a uniform $\varepsilon_0>0$ such that the tube $\{(p,w):p\in S,\ \|w\|<\varepsilon_0\}$ is in the domain of $\Phi$ and $G$ is a local diffeomorphism throughout its image: finite bundle charts and equivalence of their continuous fibre norms give this uniform shrinking. There is $0<\varepsilon<\varepsilon_0$ on whose tube image $G$ is injective. Otherwise choose unequal pairs $\Phi(p_n,w_n)$, $\Phi(q_n,z_n)$ with equal $G$ images and fibre norms less than $\min\{\varepsilon_0/2,1/n\}$. Equality of the $\pi$ coordinates gives $p_n=q_n$; a subsequence tends to some $p\in S$. Both fibre vectors tend to zero in a bundle chart, so both image points tend to $p$ and eventually lie in one inverse chart for $G$, a contradiction. Thus $G$ on that tube image is a diffeomorphism onto an open neighborhood of $S\times\{(0,0)\}$ in $S\times\mathbb R^2$. A finite product-neighborhood cover of $S\times\{(0,0)\}$ gives $\delta>0$ for which its image contains $S\times(-\delta,\delta)^2$. [A1, F6, F8, F9, step 4.2]

6.1 Set $O=G^{-1}(S\times(-\delta,\delta)^2)$ inside the injective tube of step 5.1. In these coordinates $O$ retracts smoothly to $S$ by $(p,u,v)\mapsto(p,(1-\tau)u,(1-\tau)v)$, $0\le\tau\le1$. By step 4.2 and $E=P\cap Q$, its overlap with $E$ is exactly $S\times(0,\delta)^2$. Both $O$ and this nonempty overlap are path connected: move the two interval coordinates along straight segments and join the sphere coordinates by a path from [F5]. Hence they are connected and $E\cup O$ is connected, since $E$ is connected and the overlap is nonempty. The retraction and [F10] give $H^1_{\mathrm{dR}}(O)\cong H^1_{\mathrm{dR}}(S^2)=0$. [F5, F10, step 1.1, step 4.2, step 5.1]

7.1 By [F1] the form $\eta$ is smooth and closed on the ambient manifold. By [F10] and step 6.1, its real and imaginary parts on $O$ have smooth real primitives, giving a smooth complex primitive $s_O$. The normalized exterior primitive $\sigma_E$ of step 4.1 satisfies $d(s_O-\sigma_E)=0$ on the connected overlap. By [F11] their difference is one complex constant. Subtract it from $s_O$ and glue the two agreeing functions on their open overlap. This gives a smooth primitive $\sigma$ on $E\cup O$ extending the normalized $\sigma_E$. Every ingredient used here follows from the local geometric hypotheses in [A1]; no compatibility of the radial section chart with the end chart has entered. [A1, F1, F10, F11, step 4.1, step 6.1]

8.1 Antisymmetry gives $d\sigma(T)=2\mathcal F(T,T)=0$, so the extended primitive is stationary wherever defined. Also $d(\operatorname{Re}\sigma-f)=0$ by [F1]; connectedness and [F11], together with its vanishing on $E$, imply $\operatorname{Re}\sigma=f$ throughout $E\cup O$. On this connected domain any two primitives differ by a complex constant by [F11], and the common end limit forces that constant to vanish. The exterior normalization and the horizon extension therefore agree on their overlap and are unique as stated. [A1, F1, F11, step 4.1, step 6.1, step 7.1, algebra] ∎

## Source notes

The original article citation attributes the preserved claim. The proof uses the existing mathematical suppliers; the local horizon construction is supplied here from its direct mathematical inputs. It does not assume that the radial identification of the original section agrees with its asymptotic coordinates, does not select a stationary Cauchy-flow product, and does not add a maximal-slice assumption. No original-article defect or independent acceptance is claimed.
