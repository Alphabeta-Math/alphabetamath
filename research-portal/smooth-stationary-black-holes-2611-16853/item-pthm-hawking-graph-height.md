---
title: Existence and boost-coordinate description of Hawking-flow heights
status: draft
research_item: pthm-hawking-graph-height
dependency_level: 12
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 17, proof of Lemma 3.4 before equation (3.9)
      statement: The article defines the Hawking-flow height by the unique
        intersection with the candidate section and extends it smoothly to the
        bifurcation sphere using normal-exponential rapidity coordinates.
      hypotheses: The article's regular stationary vacuum construction, its common
        collar, and the existing candidate sections in the stated positive
        parameter range.
      reading_limits: Read the frozen article text at the cited passage. This
        reference attributes the claim and is not used as proof or as a
        prerequisite.
---

PDF p. 17: ` Proof of Lemma 3.4, before (3.9) `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product)
- [pthm-common-reference-collar](item-pthm-common-reference-collar)
- [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)
- [pthm-positive-transformed-lapse](item-pthm-positive-transformed-lapse)
- [lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors)
- [lem-author-ca4ffba327b3-compact-normal-exponential-tube](item-lem-author-ca4ffba327b3-compact-normal-exponential-tube)
- [lem-author-78c700cb9e03-invariant-normal-boost-coordinates](item-lem-author-78c700cb9e03-invariant-normal-boost-coordinates)
- [math:thm-parametrized-implicit-function-theorem-with-higher-regularity](https://alphabetamath.cc/item/thm-parametrized-implicit-function-theorem-with-higher-regularity)
- [math:thm-newton-leibniz-with-interior-derivative](https://alphabetamath.cc/item/thm-newton-leibniz-with-interior-derivative)
- [math:thm-continuous-implies-integrable](https://alphabetamath.cc/item/thm-continuous-implies-integrable)
- [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle)
- [math:lem-uniform-integral-error-bound](https://alphabetamath.cc/item/lem-uniform-integral-error-bound)
- [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)
- [math:lem-tube-lemma-for-a-compact-factor](https://alphabetamath.cc/item/lem-tube-lemma-for-a-compact-factor)
- [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)
- [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)
- [math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)
- [lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant](item-lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant)



## Statement

Adopt the regular stationary vacuum construction and stationary vacuum model, with $T|_S\not\equiv0$, maximal original exterior section $\Sigma_1$, and mass normalized to one. Fix $\delta\in(0,1)$ and $q\in[\delta,1]$. Assume an existing connected smooth spacelike maximal section $\Sigma_q$ with boundary $S$, whose interior is the stationary graph $t=u_q(x)$ over $\Sigma_1^\circ$ and satisfies the end hypotheses of the positive transformed-lapse result. Here the stationary product has $T=\partial_t$ and $\Sigma_1^\circ=\{t=0\}$.

Let $V$ be the common reference collar, $K=T+\Omega_H Z$ its complete Hawking field on the stationary collar saturation, and $\kappa>0$ its normal boost rate. For every $x\in V\setminus S$ there is exactly one real number $u_q^K(x)$ such that $\phi^K_{u_q^K(x)}(x)\in\Sigma_q$. This height is smooth on $V\setminus S$ and extends smoothly to $S$, for each fixed $q$.

More precisely, for the metric $g_q$, let $\bar n_q$ be the future unit normal of $\Sigma_1$ at $S$ and $\bar\nu_q$ its unit normal to $S$ pointing into its exterior. In a sufficiently small normal-exponential collar, the two sections have representations $\exp^{(q)}_\vartheta(r(\cosh\alpha_q\,\bar\nu_q+\sinh\alpha_q\,\bar n_q))$ and $\exp^{(q)}_\vartheta(r(\cosh\beta_q\,\bar\nu_q+\sinh\beta_q\,\bar n_q))$, respectively, with $r\ge0$, $\vartheta\in S$, and smooth rapidities $\alpha_q,\beta_q$. At corresponding values of $(r,\vartheta)$, $\alpha_q+\kappa u_q^K=\beta_q$. Since $\alpha_q(0,\vartheta)=0$, the boundary value is $u_q^K|_S=\beta_q(0,\vartheta)/\kappa$. The collar needed for these coordinates may depend on $q$; no uniform bound on the boundary values is asserted here.

The original-section maximality premise is imposed on the actual physical exterior section $C=\Sigma_0\cap\mathcal E$ for the original metric $g$, so $H_g|_C=0$. Where this result uses the original reference section $\Sigma_1$, it denotes the closure $B=C\cup S$ of this actual section. Maximality of a separately labelled chart-side region or another supplied section is not substituted for this premise. The spherical identification and the physical stationary end chart remain independent. [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

## Facts & Assumptions

[A1] The model and regularity data provide the stationary spacetime, bifurcation sphere and stated maximal original section. A stationary graph is the image of $x\mapsto(u_q(x),x)$ in the open stationary product; the supplied section is separately smooth up to its boundary. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-stationary-maximal-graph](item-def-stationary-maximal-graph) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F1] The original stationary flow identifies the exterior with $\mathbb R\times\Sigma_1^\circ$. On the common collar saturation, $K$ and $Z$ are complete commuting fields, $Z$ is periodic, $K=T+\Omega_H Z$, and $K$ is future timelike for $g_q$ along the complete $K$-orbits from $V\setminus S$. [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product) [pthm-common-reference-collar](item-pthm-common-reference-collar) [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)

[F2] The lapse $-g_q(T,n_q)$ of the supplied candidate section is positive in its interior. Its translates under the stationary isometry are spacelike graphs. [pthm-positive-transformed-lapse](item-pthm-positive-transformed-lapse) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F3] At $S$, $K=0$ and the differential of its flow acts on the oriented normal plane by a boost of rapidity $\kappa s$. The normal exponential map gives a tube around compact $S$ in the smooth frame $(\bar n_q,\bar\nu_q)$. The boost acts in this frame; smooth rapidity graphs for both sections, including the tilted candidate, are constructed in steps 2.1 and 3.1. [lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors) [lem-author-ca4ffba327b3-compact-normal-exponential-tube](item-lem-author-ca4ffba327b3-compact-normal-exponential-tube) [lem-author-78c700cb9e03-invariant-normal-boost-coordinates](item-lem-author-78c700cb9e03-invariant-normal-boost-coordinates)

[F4] A smooth equation with invertible derivative in its unknown block has a locally unique smooth solution in its remaining parameters. Apply this in charts, using local smooth extensions at a boundary. [math:thm-parametrized-implicit-function-theorem-with-higher-regularity](https://alphabetamath.cc/item/thm-parametrized-implicit-function-theorem-with-higher-regularity)

[F5] Continuous functions on closed intervals are Riemann integrable. Newton–Leibniz identifies the endpoint difference of a continuous function, differentiable in the interior, with the integral of its Riemann-integrable derivative extension. [math:thm-continuous-implies-integrable](https://alphabetamath.cc/item/thm-continuous-implies-integrable) [math:thm-newton-leibniz-with-interior-derivative](https://alphabetamath.cc/item/thm-newton-leibniz-with-interior-derivative)

[F6] A continuous parameter derivative on a compact rectangle can be passed through its Riemann integral, including one-sided derivatives at parameter endpoints. Integrals on $[0,1]$ differ by at most the uniform error between their integrands. [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle) [math:lem-uniform-integral-error-bound](https://alphabetamath.cc/item/lem-uniform-integral-error-bound)

[F7] A continuous real function on a nonempty compact metric space is bounded and attains its extrema. Closed Euclidean intervals are compact. An open neighborhood of a compact factor times a point contains a product neighborhood of that slice. For extrema on $S$, use the metric pulled back from the unit sphere under its supplied smooth spherical identification; its topology is the given compact topology of $S$. [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric) [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn) [math:lem-tube-lemma-for-a-compact-factor](https://alphabetamath.cc/item/lem-tube-lemma-for-a-compact-factor)

[F8] A function continuous on a closed interval and differentiable in its interior satisfies the mean value theorem; a continuous real function on a closed interval takes every value between its endpoint values. [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem) [math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)

[F9] For the original metric $g_1=g$, the horizon-axis lemma identifies the local exterior in the normal tube $\Xi_1(\vartheta,a,b)=\exp^{(1)}_\vartheta(a\bar n_1+b\bar\nu_1)$ as $\mathcal E\cap O=\{b>|a|\}$. Its end is the designated stationary end, its two boundaries are those of the regularity definition, and its hypersurface is $\Sigma_0$ with specified side $B=C\cup S$. The original-product result supplies this smooth side, and its inward boundary-normal collar in the common reference collar has positive points in $C\subset\mathcal E$, matching the lemma's side hypothesis. This is a statement about the original chronological exterior, not a claim that $\mathcal E$ is defined by the chronological sets of $g_q$. [lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant](item-lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product) [pthm-common-reference-collar](item-pthm-common-reference-collar)

## Proof

**Given:** The construction, fixed positive $q$, supplied candidate section, and collar in the Statement.

**Goal:** Prove unique intersection, interior smoothness, and the stated smooth boundary extension.

1.1 Put $F(t,x)=t-u_q(x)$. Its level sets are stationary translates of the spacelike candidate graph. The positive $T$-lapse fixes $dF$ to be positive on future timelike vectors: $dF(T)=1$ and $T$ has positive normal component. Thus $dF(K)>0$ on each complete orbit under consideration. The mean value theorem on every finite orbit-parameter interval shows that $s\mapsto F(\phi_s^Kx)$ is strictly increasing. [given, A1, F1, F2, F8]

1.2 At $y\in S$, put $B_y=(dK)_y$. Because $K|_S=0$, the connection term vanishes there, so this is $\nabla^{(q)}K$ for every $q$, including the original member. It annihilates $T_yS$ and is invertible on each metric's normal plane by [F3]. Thus both normal planes equal the same rank-two image $\operatorname{im}B_y$. Their intersections with $T_y\Sigma_1$ are the same line. Both $\bar\nu_q$ and $\bar\nu_1$ point into the same actual reference side $C$, so $\bar\nu_q=c_q\bar\nu_1$ for some $c_q>0$. The positive boost identities $B_y\bar\nu_q=\kappa\bar n_q$ and $B_y\bar\nu_1=\kappa\bar n_1$ then give $\bar n_q=c_q\bar n_1$. Choose any local inward candidate-boundary curve $\gamma(\lambda)$, with $\lambda\ge0$, $\gamma(0)=y$ and $\gamma'(0)$ transverse to $T_yS$, using its supplied embedded boundary parametrization. Decompose $\gamma'(0)=\xi+U\bar n_q+V\bar\nu_q$, where $\xi\in T_yS$. Subtracting $\xi$ leaves a nonzero candidate tangent vector, so its spacelikeness gives $V^2-U^2>0$. The zero-section differential of the normal tubes identifies the derivatives of its original coordinates as $a'(0)=c_qU$ and $b'(0)=c_qV$. For $\lambda>0$ sufficiently small, $\gamma(\lambda)$ is in the stationary graph and hence in the original exterior $\mathcal E$. By [F9], $b(\lambda)>|a(\lambda)|$. Divide by $\lambda$ and take its one-sided limit to obtain $V\ge|U|$; together with $V^2-U^2>0$ this gives $V>0$. The candidate therefore enters the positive-$v$ side of the $g_q$ normal tube, where $v$ is the coefficient of $\bar\nu_q$. The reference enters that side by its definition. Only the differentials of the two normal tubes at $S$ have been compared; their coordinate maps are not identified away from $S$. [given, A1, F1, F3, F9, algebra]

1.3 Commutation gives $\phi_s^K=\phi_s^T\circ\phi_{\Omega_Hs}^Z$ on the complete collar saturation. Since $T=\partial_t$ and $u_q$ is independent of $t$, $F(\phi_s^Kx)=s+F(\phi_{\Omega_Hs}^Zx)$. For a positive common period $P$ of $Z$, the function $a\mapsto F(\phi_a^Zx)$ is continuous on the nonempty compact metric interval $[0,P]$ and is bounded there by [F7]. Periodicity extends that bound to every real $a$, hence to $a=\Omega_Hs$. Thus $F(\phi_s^Kx)$ tends to opposite infinities as $s\to\pm\infty$. [F1, F7]

2.1 In the normal tube from [F3], write $u$ for the coefficient of $\bar n_q$ and $v$ for that of $\bar\nu_q$. Projection of either spacelike section to $(v,\vartheta)$ has invertible derivative at $S$: its kernel would be a timelike tangent vector, whereas the section is spacelike. Apply [F4] to the projection of a local smooth extension of a boundary parametrization, obtaining $u=w(v,\vartheta)$ with $w(0,\vartheta)=0$. Step 1.2 identifies the actual section side of each such graph as $v\ge0$. Local uniqueness glues these graphs, and compactness and the product-neighborhood assertion in [F7] give a common smaller collar. Spacelikeness gives $|\partial_vw(0,\vartheta)|<1$, with no zero-slope requirement for the candidate. Define $h(v,\vartheta)=\int_0^1\partial_vw(av,\vartheta)\,da$. For $v>0$, [F5] applied to $a\mapsto w(av,\vartheta)$ gives $w(v,\vartheta)=v h(v,\vartheta)$; at zero this identity still holds and $h(0,\vartheta)=\partial_vw(0,\vartheta)$. On closed coordinate rectangles, successive applications of [F6] differentiate this integral in every parameter. These derivatives are jointly continuous: for any resulting continuous integrand $H(a,p)$ and fixed $p_0$, the open set $|H(a,p)-H(a,p_0)|<\eta$ contains $[0,1]\times\{p_0\}$. Compactness of $[0,1]$ and the tube lemma in [F7] make this bound uniform in $a$ near $p_0$, and the integral-error bound in [F6] gives continuity of its integral. Applying this to all derivative orders proves that $h$ is jointly smooth, including at $v=0$ using the local smooth extensions. [given, A1, F3, F4, F5, F6, F7, step 1.2]

2.2 Choose finite parameters with opposite signs of $F(\phi_s^Kx)$ using step 1.3. The intermediate value theorem on that closed parameter interval gives a zero, and strict increase from step 1.1 gives uniqueness. At the zero the derivative in $s$ is $dF(K)>0$, so [F4] applied in interior charts gives smooth dependence of that zero on $x$. Uniqueness makes these local solutions agree, proving interior smoothness of $u_q^K$. [F4, F8, step 1.1, step 1.3]

3.1 For each section, [F7] on $S$ gives $m=\max_\vartheta|h(0,\vartheta)|<1$. Fix $m<\theta<1$ and shrink by the tube lemma to obtain $|h|<\theta$ on a common collar. Put $R(v,\vartheta)=v\sqrt{1-h(v,\vartheta)^2}$; then $\partial_vR(0,\vartheta)=\sqrt{1-h(0,\vartheta)^2}\ge\sqrt{1-m^2}$. A further use of the tube lemma gives $\partial_vR>c=\tfrac12\sqrt{1-m^2}>0$ there. Choose $\varepsilon>0$ with the closed interval $0\le v\le\varepsilon$ in that collar. The mean value theorem gives strict increase and $R(\varepsilon,\vartheta)>c\varepsilon$; the intermediate value theorem gives the unique inverse $v=b(r,\vartheta)$ for $0\le r<c\varepsilon$. By [F4], this inverse is smooth, using local extensions also at zero. Thus the rapidity is $\operatorname{arctanh}h(b(r,\vartheta),\vartheta)$, and the normal coordinates are $u=r\sinh(\text{rapidity})$, $v=r\cosh(\text{rapidity})$. This constructs the smooth functions $\alpha_q$ and $\beta_q$ on a common smaller collar for the two sections. The reference tangent is $\bar\nu_q$, so its slope is zero and $\alpha_q(0,\vartheta)=0$. [F3, F4, F7, F8, step 2.1]

4.1 The $K$-flow fixes each $\vartheta\in S$, is an isometry of $g_q$, and commutes with the normal exponential map wherever the displayed expressions are defined. Its differential adds $\kappa s$ to normal rapidity while preserving $r$ and $\vartheta$. Consequently the local intersection of the two rapidity graphs occurs at $s=(\beta_q-\alpha_q)/\kappa$. Their boundary values are bounded on $S$ by [F7], and continuity and the tube lemma give bounded rapidities on a smaller collar. Throughout this bounded flow segment the normal-vector coefficients are bounded by a constant times $r$, so a further shrinking keeps the entire segment in the tube. This local intersection is the unique global intersection from step 2.2. Its smooth formula extends $u_q^K$ to $r=0$ and gives $u_q^K|_S=\beta_q(0,\vartheta)/\kappa$. [F1, F3, F7, step 3.1, step 2.2] ∎


## Source notes

The article reference attributes the intersection and boundary-extension claims. The proof above uses the stated completed suppliers and does not infer uniform boundary estimates from smoothness for an individual $q$.

These premises specify the generated conditional scope and are not attributed to the original article. The substantive local horizon conclusions are retained. The immutable original extraction is unchanged; in particular, original Theorem 1.1 retains its unresolved source-assessment status.
