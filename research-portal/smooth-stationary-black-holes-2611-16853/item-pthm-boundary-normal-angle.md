---
title: Boundary angle bound and normal-graph cone
status: draft
research_item: pthm-boundary-normal-angle
dependency_level: 17
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp.18–19, equation (3.12), following Gaussian expansions and
        normal-graph assertion
      reading_limits: Historical attribution-reading record retained; this maintenance
        revision checked current item and supplier statements and the local
        background construction, without new article-PDF or external-proof
        reading. Consulted the frozen extracted article text at Lemmas 3.3–3.4,
        including PDF pp.18–19, equation (3.12), the Gaussian expansions and
        normal-graph paragraph. This reference attributes those claims only. The
        proof uses the existing local geometric helpers and a locally authored
        saturation argument in exact boost coordinates; the article is not used
        to prove its own claim.
---

PDF p. 18: ` (3.12) and following expansions `; PDF p. 19: ` (3.12) and following expansions `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [pthm-common-reference-collar](item-pthm-common-reference-collar)
- [pthm-normal-boost-action](item-pthm-normal-boost-action)
- [pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation)
- [pthm-hawking-graph-height](item-pthm-hawking-graph-height)
- [pthm-hawking-graph-barriers](item-pthm-hawking-graph-barriers)
- [lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets](https://alphabetamath.cc/item/thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets)
- [lem-author-840894718169-fixed-boundary-flow-normal-boost](item-lem-author-840894718169-fixed-boundary-flow-normal-boost)
- [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone)
- [lem-author-840894718169-normal-projection-local-and-boundary-jets](item-lem-author-840894718169-normal-projection-local-and-boundary-jets)
- [lem-author-840894718169-fixed-target-collar-properness](item-lem-author-840894718169-fixed-target-collar-properness)
- [lem-author-840894718169-boundary-one-sheet-normal-graph](item-lem-author-840894718169-boundary-one-sheet-normal-graph)
- [lem-author-78c700cb9e03-invariant-normal-boost-coordinates](item-lem-author-78c700cb9e03-invariant-normal-boost-coordinates)
- [lem-author-78c700cb9e03-bounded-rapidity-reference-graph](item-lem-author-78c700cb9e03-bounded-rapidity-reference-graph)
- [lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant](item-lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant)
- [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)
- [math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves](https://alphabetamath.cc/item/thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves)
- [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)
- [math:thm-newton-leibniz-with-interior-derivative](https://alphabetamath.cc/item/thm-newton-leibniz-with-interior-derivative)
- [math:thm-continuous-implies-integrable](https://alphabetamath.cc/item/thm-continuous-implies-integrable)
- [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle)
- [math:lem-uniform-integral-error-bound](https://alphabetamath.cc/item/lem-uniform-integral-error-bound)
- [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)
- [math:lem-tube-lemma-for-a-compact-factor](https://alphabetamath.cc/item/lem-tube-lemma-for-a-compact-factor)
- [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)
- [math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)


## Statement

In the regular mass-one stationary vacuum/Harrison construction, fix $\delta>0$ and assume the existing smooth spacelike maximal stationary graph sections for $q\in[\delta,1]$ satisfy the complete height/barrier hypotheses, with compact boundary $S$. Let $u_q^K$ be their Hawking-flow heights over the common reference collar, and let $|u_q^K|\le C_\delta$ be the supplied uniform bound, including $S$. With future normals $n_q$ to the candidate and $\bar n_q$ to the reference and outward reference boundary normal $\bar\nu_q$, one has on $S$
$$n_q=\cosh(\kappa u_q^K)\bar n_q+\sinh(\kappa u_q^K)\bar\nu_q,\qquad -g_q(n_q,\bar n_q)\le\cosh(\kappa C_\delta).$$
There are common Gaussian normal geodesic coordinates $\tau_q$ and projection $\pi_q^\perp$ from the reference section, and reference distance $\rho_q$, such that for bounded $s$
$$\tau_q(\phi_s^Kx)=\rho_q(x)\sinh(\kappa s)+O_s(\rho_q(x)^2),\qquad \rho_q(\pi_q^\perp\phi_s^Kx)=\rho_q(x)\cosh(\kappa s)+O_s(\rho_q(x)^2).$$
The remainders are uniform in $q\in[0,1]$ on any fixed bounded interval of $s$. Thus there are $\theta_\delta<1$ and a positive reference radius $r_\delta$, independent of the candidates and of $q\in[\delta,1]$, such that each candidate near $S$ is a one-to-one normal graph over $0\le\rho_q<r_\delta$ and satisfies $|\tau_q|\le\theta_\delta\rho_q\circ\pi_q^\perp$. The graph is smooth up to $S$ for each fixed $q$. This claim supplies a common graph domain and a cone bound, not yet uniform higher derivative or interior normal-angle estimates. For $U_q=-\operatorname{grad}_{g_q}\tau_q$, one has $U_q=\bar n_q$ on $S$, so the same displayed boundary angle estimate holds there with $U_q$.

More precisely, choose a common closed source collar $c_q([0,a]\times S)$ within the height-bound collar, with $\rho_q(c_q(\rho,\eta))=\rho$, and put $\Phi_q(x)=\phi^K_{u_q^K(x)}(x)$. In the common Gaussian coordinates write $R_q=\rho_q\circ\pi_q^\perp$. There are common constants $c_1,c_2>0$ and a target radius $0<b<c_1a/2$ such that $c_1\rho\le R_q(\Phi_q(c_q(\rho,\eta)))\le c_2\rho$. The unique zero-boundary normal graph $G_q:[0,b)\times S\to M$ has image exactly $\{\Phi_q(c_q(\rho,\eta)):0\le\rho\le a,\ 0\le R_q(\Phi_q(c_q(\rho,\eta)))<b\}$ and obeys $|\tau_q|\le\theta_\delta R_q$ there. There is also one ambient open neighborhood $U$ of $S$, independent of $q$ and the candidates under these same bounds, such that $\Sigma_q\cap U\subset G_q([0,b)\times S)$. Thus no additional candidate portion near $S$ is omitted. The target radius may be reduced further, with $U$ shrunk accordingly, while retaining the image equality, radial comparison and capture conclusions. These conclusions use the complete standing original-background and candidate height/barrier hypotheses already specified; they assume no uniform derivatives of $u_q^K$.

For the original background alone, assume only the standing regular mass-one construction with actual original exterior section maximal and $T|_S\not\equiv0$, without any candidate-section existence or height/barrier assumption. Its local fields admit a circle-invariant future/outward orthonormal normal frame and an invariant normal-exponential tube $\Xi(y,u,v)$ with $K=\kappa(v\partial_u+u\partial_v)$. On the exterior wedge write $u=r\sinh(\kappa\eta)$ and $v=r\cosh(\kappa\eta)$, so $K=\partial_\eta$. The original reference collar is a smooth graph $\eta=b(r,y)$ down to $r=0$, with $|b|\le B$ on a smaller fixed collar. Its reference normal may have any smooth spacelike tilt relative to this invariant frame; tangent alignment with the frame is not required. This background conclusion is independent of the candidate family used for the preceding estimates.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-harrison-normalization](item-def-harrison-normalization)

[def-stationary-maximal-graph](item-def-stationary-maximal-graph)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[pthm-common-reference-collar](item-pthm-common-reference-collar)

[pthm-normal-boost-action](item-pthm-normal-boost-action)

[pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation)

[pthm-hawking-graph-height](item-pthm-hawking-graph-height)

[pthm-hawking-graph-barriers](item-pthm-hawking-graph-barriers)

[lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets](https://alphabetamath.cc/item/thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets)

[lem-author-840894718169-fixed-boundary-flow-normal-boost](item-lem-author-840894718169-fixed-boundary-flow-normal-boost)

[lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone)

[lem-author-840894718169-normal-projection-local-and-boundary-jets](item-lem-author-840894718169-normal-projection-local-and-boundary-jets)

[lem-author-840894718169-fixed-target-collar-properness](item-lem-author-840894718169-fixed-target-collar-properness)

[lem-author-840894718169-boundary-one-sheet-normal-graph](item-lem-author-840894718169-boundary-one-sheet-normal-graph)

## Facts & Assumptions

[A1] Adopt the stationary vacuum model and regular data, with actual original exterior section maximal, $T|_S\not\equiv0$, and mass-one normalization. For the candidate estimates, existing candidate sections and their end hypotheses are additional premises, not an eventual existence conclusion. The final background conclusion uses only the standing original data and does not assume candidate sections. Work in ZFC, including the axiom of choice. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-harrison-normalization](item-def-harrison-normalization) [def-stationary-maximal-graph](item-def-stationary-maximal-graph) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The common reference collar is uniformly spacelike for the smooth Harrison family, with smooth uniformly controlled unit normals and boundary distance/exponential data. Its stationary saturation has the complete isometric $K$ flow and reference $K$ product. [pthm-common-reference-collar](item-pthm-common-reference-collar)

[F2] The fixed field vanishes on $S$ and its flow acts by boost rapidity $\kappa s$ with the same positive $\kappa$ for all $q$. The preserved branches are smooth null boundaries meeting transversely. [pthm-normal-boost-action](item-pthm-normal-boost-action) [pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation) [lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors)

[F3] Each candidate has its unique smooth Hawking-flow height extending individually to $S$, and the barrier theorem supplies $|u_q^K|\le C_\delta$ on a uniform closed reference collar. No uniform bound on derivatives of these heights is assumed. [pthm-hawking-graph-height](item-pthm-hawking-graph-height) [pthm-hawking-graph-barriers](item-pthm-hawking-graph-barriers)

[F4] Spacelike sections, future unit normals and maximality use the hypersurface-data convention. Flow graphs and normal exponential graphs use the normal-graph convention. Lorentzian signature, time orientation and Killing fields use the stationary-data convention. Bifurcate Killing horizons and their signed surface gravities use the horizon-data convention. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[F5] The five geometric helpers supply the boundary normal identity, common Gaussian/Taylor/cone bounds, local normal invertibility and its boundary jet, properness onto a fixed positive-width target collar, and propagation of the one-sheet boundary germ. [lem-author-840894718169-fixed-boundary-flow-normal-boost](item-lem-author-840894718169-fixed-boundary-flow-normal-boost) [lem-author-840894718169-uniform-gaussian-flow-cone](item-lem-author-840894718169-uniform-gaussian-flow-cone) [lem-author-840894718169-normal-projection-local-and-boundary-jets](item-lem-author-840894718169-normal-projection-local-and-boundary-jets) [lem-author-840894718169-fixed-target-collar-properness](item-lem-author-840894718169-fixed-target-collar-properness) [lem-author-840894718169-boundary-one-sheet-normal-graph](item-lem-author-840894718169-boundary-one-sheet-normal-graph) For nonempty Euclidean open sets of equal dimension with connected target, a proper $C^1$ map with everywhere invertible derivative is surjective and has finite evenly covered fibres; the fixed-target helper applies this theorem after identifying the positive $S^2$ collars with Euclidean annuli. [math:thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets](https://alphabetamath.cc/item/thm-proper-local-diffeomorphisms-have-finite-diffeomorphic-sheets)

[F6] For the original metric $g_1=g$, the local Hawking/circle-field theorem supplies the same commuting Killing fields $K,Z$, with $K|_S=0$, $K=T+\Omega_HZ$, and a periodic local $Z$ action. The invariant-normal-coordinate lemma supplies a fixed normal tube $\Xi(y,u,v)$ with $K=\kappa(v\partial_u+u\partial_v)$. For methodological attribution only, Proof steps 1.1–2.1 of the bounded-rapidity reference lemma motivate the projection-and-division method; no conclusion of that lemma is invoked. We prove the representation below for the original reference section using its actual spacelike tangent slope, the invariant tube and the inverse-function, integral and compactness facts in [F8]–[F11]; the earlier lemma's tangent-alignment hypothesis is not assumed. Write its boost-time height as $b(r,y)$ and its rapidity as $a(r,y)=\kappa b(r,y)$, so the resulting representation is $u=r\sinh a(r,y)$, $v=r\cosh a(r,y)$, with $a$ smooth and bounded. The event-boundary quadrant lemma identifies the original exterior near $S$ with $v>|u|$: its frame is the reference normal frame, and the future/outward boost changing to the invariant frame preserves this wedge. These inputs concern only the original metric and fixed reference section; they impose no new condition on the candidate family. [lem-author-78c700cb9e03-invariant-normal-boost-coordinates](item-lem-author-78c700cb9e03-invariant-normal-boost-coordinates) [lem-author-78c700cb9e03-bounded-rapidity-reference-graph](item-lem-author-78c700cb9e03-bounded-rapidity-reference-graph) [lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant](item-lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant) [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)

[F7] Smooth vector fields have locally unique integral curves through each point. This applies both to $Z|_S$ and to the ambient fields $Z,K$. [math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves](https://alphabetamath.cc/item/thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves)

[F8] A smooth map with an isomorphism as its differential at a point is a diffeomorphism on suitable neighborhoods of that point. We apply this to projection of the reference section to $(v,y)$ and to the radial map $(v,y)\mapsto(r,y)$. Smoothness through the boundary is checked on a local smooth extension of the supplied section. [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds)

[F9] Continuous functions on closed intervals are Riemann integrable. Newton–Leibniz gives $w(v,y)-w(0,y)=v\int_0^1\partial_vw(tv,y)\,dt$. Continuous parameter derivatives may be passed through the integral on a compact rectangle; iterating this and using the uniform integral-error bound proves smoothness and joint continuity of these parameter integrals. [math:thm-continuous-implies-integrable](https://alphabetamath.cc/item/thm-continuous-implies-integrable) [math:thm-newton-leibniz-with-interior-derivative](https://alphabetamath.cc/item/thm-newton-leibniz-with-interior-derivative) [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle) [math:lem-uniform-integral-error-bound](https://alphabetamath.cc/item/lem-uniform-integral-error-bound)

[F10] A continuous real function on a nonempty compact metric space attains its extrema. An open neighborhood of $S\times\{0\}$ contains $S\times(-\epsilon,\epsilon)$ for some $\epsilon>0$, by the tube lemma. For the metric assertion use the metric pulled back from the unit sphere by a fixed smooth identification $S\cong S^2$. [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric) [math:lem-tube-lemma-for-a-compact-factor](https://alphabetamath.cc/item/lem-tube-lemma-for-a-compact-factor)

[F11] The mean value theorem applies to a function continuous on a closed interval and differentiable in its interior; a continuous function on a closed interval takes every intermediate value. We use these facts for the strictly increasing radial map at each fixed $y$. [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem) [math:thm-intermediate-value](https://alphabetamath.cc/item/thm-intermediate-value)

## Proof

**Given:**The stated data and complete hypotheses.

**Goal:** Establish the conclusions with the asserted parameter uniformity and domains.

1.1 Write $\Phi_q(x)=\phi_{u_q^K(x)}^K(x)$ on the reference collar. The complete reference $K$ product makes this an embedding in the interior, and [F3] gives its individual smooth extension to $S$. Apply the fixed-boundary normal lemma in [F5]: the variable-height derivative term is multiplied by $K=0$ on $S$. Thus the future candidate normal is exactly the boost of the reference normal, and its pairing is $\cosh(\kappa u_q^K)$. The bound in [F3] proves the stated uniform boundary angle estimate. [A1, F1, F2, F3, F4, F5]

1.2 Apply the uniform Gaussian-flow lemma with the fixed time bound $C_\delta$. The smooth background family and compact $S$ give one chart and one Taylor remainder bound for all bounded times and all $q$. Its pointwise ratio estimate yields a strict cone constant $\theta_\delta<1$, while its radial comparison gives constants $c_1,c_2>0$ such that $c_1\rho_q(x)\le\rho_q(\pi_q^\perp\Phi_q(x))\le c_2\rho_q(x)$ on a common reference collar. This substitution requires no derivative estimate for $u_q^K$, since it uses only its bounded value at each point. [F1, F2, F3, F5]

1.3 Verify the action hypotheses for the fixed original-metric tube in [F6]. Since $T|_S\not\equiv0$ and $K|_S=0$, the identity $K=T+\Omega_HZ$ forces $\Omega_H\ne0$. Regularity makes $T$ tangent to both transverse horizon branches, hence to their intersection $S$; therefore $Z|_S=-\Omega_H^{-1}T|_S$ is tangent to $S$. Local existence for $Z|_S$ and ambient uniqueness in [F7] make the periodic $Z$ action preserve $S$. Its Killing flow preserves the metric: differentiating its pullback gives the pullback of $\mathcal L_Zg=0$. Along the flow, the differential carries a future timelike vector to a continuous timelike vector starting in the future component, so it cannot leave that component. Thus this circle action preserves future orientation, and the invariant-normal-coordinate lemma applies with the commuting fields, fixed sphere and positive boost rate in [F2] and [F6]. [A1, F1, F2, F4, F6, F7]

1.4 The invariant frame need not be tangent-adapted to the reference section. Let $(n,\nu)=(\bar n_1,\bar\nu_1)$ be its future/outward orthonormal normal frame on $S$. Since $(e_0,e_1)$ is also future/outward, a smooth real function $\beta(y)$ satisfies $\nu=\sinh\beta\,e_0+\cosh\beta\,e_1$: explicitly $\beta=\operatorname{arsinh}(-g(\nu,e_0))$, with the positive $e_1$ coefficient fixed by the outward orientation. Projection of the reference section in the tube to $(v,y)$ has timelike kernel $\mathbb R e_0$ at $S$, so its differential on the spacelike section is an isomorphism. By [F8] it gives local smooth graphs $u=w(v,y)$ with $w(0,y)=0$ and $\partial_vw(0,y)=\tanh\beta(y)$. The exterior side has positive $v$ derivative, since its boundary tangent is a positive multiple of $\nu$ modulo $TS$ and $\cosh\beta>0$. These are graphs of the germ of the embedded reference section, not arbitrary other sheets: local uniqueness, compactness of $S$ and [F10] allow a common shrinking and make the local graph germs agree. Thus one obtains $w$ for $0\le v<\epsilon$ on all of $S$. This verifies the available orientation condition without asserting $\nu=e_1$. [F1, F4, F6, F8, F10, algebra]

2.1 Normal projection is locally invertible on each spacelike candidate because its kernel is a timelike Gaussian fibre. On $S$ its composite with the reference flow parametrization is the identity and has radial derivative $\cosh(\kappa u_q^K)>0$ and tangential identity. Hence each fixed $q$ has an individual one-sheet boundary germ, but no uniform inverse-function radius has been presumed. Restrict the target to $0<R<r_\delta<c_1\rho_0/2$, where $\rho_0$ is a common reference radius from step 1.2. Radial comparison bounds preimages of every compact target set inside a compact reference subannulus, so projection is proper onto this common target. The finite-sheet theorem then gives a finite covering. [F3, F4, F5, step 1.1, step 1.2]

2.2 Carry out [F6]'s projection-and-division construction with this actual slope. Set $h(v,y)=\int_0^1\partial_vw(tv,y)\,dt$. The continuous integrand is integrable by [F9], and Newton–Leibniz gives $w(v,y)=v h(v,y)$ and $h(0,y)=\partial_vw(0,y)$. In surface charts, iterate differentiation under the integral sign on compact coordinate rectangles to obtain all parameter derivatives. Their joint continuity follows from [F10] applied to the compact $t$ interval and the uniform integral-error bound in [F9]. Therefore $h$ is smooth up to zero, also seen using the local smooth extensions in [F8]. By spacelikeness, $|h(0,y)|=|\tanh\beta(y)|<1$; compact extrema in [F10] give $m=\max_S|h(0,y)|<1$, and the tube lemma gives $|h(v,y)|<\theta<1$ on a common smaller collar, for any fixed $m<\theta<1$. [F6, F8, F9, F10, step 1.4]

3.1 Put $R(v,y)=v\sqrt{1-h(v,y)^2}$. It is smooth and $\partial_vR(0,y)=\sqrt{1-h(0,y)^2}\ge\sqrt{1-m^2}>0$. By [F10] shrink once to have $\partial_vR>c=\tfrac12\sqrt{1-m^2}$ throughout. Fix $\epsilon_1>0$ inside this collar. The mean value theorem in [F11] gives $R(\epsilon_1,y)>c\epsilon_1$ and strict increase of $R(\cdot,y)$; the intermediate value theorem gives a unique inverse $v=V(r,y)$ for every $0\le r<r_0=c\epsilon_1$. The differential of $(v,y)\mapsto(R(v,y),y)$ is invertible, so [F8] makes its inverse smooth, including at zero by the smooth extensions; uniqueness patches these inverses. Set $a(r,y)=\operatorname{arctanh}h(V(r,y),y)$. Then $|a|\le A=\operatorname{arctanh}\theta$, and the original reference collar is $x(r,y)=\Xi(y,r\sinh a(r,y),r\cosh a(r,y))$. Here $a$ is rapidity and $b=a/\kappa$ is the boost-time height in the supplier's notation. Neither the positive-lapse monotonic-crossing conclusion of that supplier nor its stronger tangent alignment is invoked. [F6, F8, F10, F11, step 2.2, algebra]

3.2 For fixed $q$, sufficiently small target radius forces all preimages into its individual injective boundary germ by the radial comparison in step 1.2. The germ supplies a fibre with one point. The finite sheet number is constant on the connected target annulus, hence is one on the entire common collar. The last helper in [F5] gives the smooth normal graph and its smooth individual boundary extension. Its values obey the cone inequality already proved. This establishes the graph for the candidate portion parametrized by $\Phi_q$. [F3, F4, F5, step 1.2, step 2.1]

4.1 Now prove local saturation in that tube. Set $r=(v^2-u^2)^{1/2}$ and $\eta=\operatorname{arctanh}(u/v)$ on $v>|u|$, so $u=r\sinh\eta$, $v=r\cosh\eta$. Choose $r_*>0$ so that all $x(r,y)$ with $0\le r\le r_*$ lie in the closed source collar $0\le\rho_q\le\rho_0$ used in steps 1.2 and 2.1, for every $q\in[\delta,1]$. This follows from joint smoothness of the reference distance collars, compactness of $[\delta,1]\times S$, and $\rho_q(x(0,y))=0$. Choose $b>0$ so that the closed box $|u|\le b$, $|v|\le b$ over $S$ lies in the original tube and its exterior-quadrant neighborhood. Finally choose $0<\varepsilon<\min\{r_*,b\}$ with $\varepsilon\cosh A<b$. All these choices depend on the background and $\delta$, not on a candidate. [A1, F1, F2, F4, F6, F10, step 1.2, step 3.1]

5.1 Let $p=\Xi(y,u,v)$ be any original exterior point with $0<v<\varepsilon$. Then $|u|<v$ and $0<r\le v<r_*$. Its rapidity $\eta_p$ is finite. Join $x(r,y)$ to $p$ by keeping $(r,y)$ fixed and varying rapidity monotonically from $a(r,y)$ to $\eta_p$. On this entire segment, $v=r\cosh\eta\le\max\{r\cosh a(r,y),v(p)\}<b$ and $|u|<v$, since $\cosh$ is even and increasing with absolute value. Thus the segment remains in the actual local tube, where the exact field formula in [F6] makes it a $K$ integral curve with elapsed time $s=(\eta_p-a(r,y))/\kappa$. The complete field in [F1] extends this same local field, so uniqueness of integral curves in [F7], continued along the finite segment, identifies it with its complete orbit from $x(r,y)$. Hence $p=\phi_s^Kx(r,y)$. The open normal box $|u|<\varepsilon$, $|v|<\varepsilon$ is an ambient neighborhood of $S$, and its entire exterior part is therefore in the saturation of the chosen source collar. This argument permits arbitrarily large finite $|s|$ as $p$ approaches either null branch; no uniform time bound is used. [F1, F2, F6, F7, step 3.1, step 4.1, algebra]

6.1 If a candidate point lies in the exterior neighborhood from step 5.1, it lies on the complete $K$ orbit of some $x$ in the chosen source collar. The unique candidate intersection on that orbit in [F3] forces it to be $\Phi_q(x)$. Consequently no additional near-boundary candidate portion is omitted. Put $a=\rho_0$ for the closed source radius used in steps 1.2 and 2.1, and write its jointly smooth boundary-distance parametrization as $c_q(\rho,\eta)$. Choose $0<b<c_1a/2$ below the common target radius in step 3.2. That step's one-sheet normal graph is exactly the portion of $\Phi_q(c_q([0,a]\times S))$ projecting to $0\le R_q<b$, including its zero boundary on $S$; the radial bounds are those of step 1.2. Joint smoothness of the Gaussian family and compactness of $[\delta,1]\times S$ allow one ambient open neighborhood $U$ of $S$ inside the normal box from step 5.1 and all the Gaussian domains, with target radial coordinates less than $b$ for every $q$. Every candidate point in $U$ is therefore in this graph, and every graph point is a candidate point. Reducing $b$ further preserves the image equality by restriction; shrink $U$ again using the same joint smoothness to preserve capture. The cone bound and individual smooth boundary extension from step 3.2 are unchanged. Finally the Gaussian proper-time normal is $-\operatorname{grad}_{g_q}\tau_q=\bar n_q$ on $S$, so step 1.1 gives the last boundary angle estimate. [F1, F3, F4, F5, step 1.1, step 1.2, step 5.1, step 3.2]

7.1 For the separate background conclusion, retain only the standing original data in [A1]. Steps 1.3 and 1.4 construct the invariant frame and the original reference graph in it from those background data, allowing its actual smooth spacelike tilt. Steps 2.2 and 3.1 give $u=r\sinh a(r,y)$, $v=r\cosh a(r,y)$ with smooth bounded rapidity $a$, using no candidate height or candidate section. Put $b=a/\kappa$ and $\eta=\operatorname{arctanh}(u/v)/\kappa$. Since $\kappa>0$ is fixed, $b$ is smooth and bounded and the exact boost-field formula gives $K=\partial_\eta$. These steps did not use the candidate premises in [F3] or the candidate conclusions in steps 1.1, 1.2, 2.1, 3.2, 4.1, 5.1 and 6.1. Thus they prove the stated background result independently of existence at any candidate parameter. [A1, F1, F2, F4, F6, F7, step 1.3, step 1.4, step 2.2, step 3.1, algebra] ∎
