---
title: Raychaudhuri expansion and generator Jacobians
status: draft
research_item: pthm-raychaudhuri-endpoint-jacobians
dependency_level: 28
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 25–26, proof of Lemma 4.4, sentence spanning the page break
      attribution: The article invokes positive initial expansion and Raychaudhuri to
        compare the Jacobians of the negative-time and zero-time generator maps
        with one.
      hypotheses: The Section 4 stationary vacuum Harrison construction, comparison
        sphere, boundary generators and cuts used in the proof of Lemma 4.4.
      reading_limits: Historical reading note retained from the current source; this
        maintenance revision claims no fresh article or external full-text
        reading. Read the frozen article text at the cited passage. This
        reference attributes the original assertion and is not used as a proof
        premise.
---

PDF p. 25: ` Proof of Lemma 4.4, sentence spanning page break `; PDF p. 26: ` Proof of Lemma 4.4, sentence spanning page break `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets)
- [def-truncated-null-boundary-height](item-def-truncated-null-boundary-height)
- [def-stationary-section-time](item-def-stationary-section-time)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)
- [pthm-comparison-sphere-properties](item-pthm-comparison-sphere-properties)
- [pthm-past-boundary-localization](item-pthm-past-boundary-localization)
- [pthm-null-endpoint-map-properties](item-pthm-null-endpoint-map-properties)
- [pthm-electrovacuum-energy-conditions](item-pthm-electrovacuum-energy-conditions)
- [lem-author-2632702918ef-target-segment-boundary-containment](item-lem-author-2632702918ef-target-segment-boundary-containment)
- [lem-author-2632702918ef-target-interior-focal-exclusion](item-lem-author-2632702918ef-target-interior-focal-exclusion)
- [lem-null-optics-jacobian-comparison-input](item-lem-null-optics-jacobian-comparison-input)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [pthm-transformed-cauchy-sections](item-pthm-transformed-cauchy-sections)
- [math:thm-parametrized-implicit-function-theorem-with-higher-regularity](https://alphabetamath.cc/item/thm-parametrized-implicit-function-theorem-with-higher-regularity)
- [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)
- [def-harrison-one-form-family](item-def-harrison-one-form-family)
- [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive)
- [pthm-harrison-lorentzian-algebra](item-pthm-harrison-lorentzian-algebra)
- [def-harrison-normalization](item-def-harrison-normalization)
- [pthm-harrison-denominator-asymptotics](item-pthm-harrison-denominator-asymptotics)
- [pthm-harrison-component-asymptotics](item-pthm-harrison-component-asymptotics)
- [pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates)
- [pthm-sphere-area-expansion-estimates](item-pthm-sphere-area-expansion-estimates)


## Statement

Work in ZFC in the regular mass-one stationary vacuum Harrison construction, with original maximal exterior section and $T|_S\not\equiv0$. Fix a sufficiently small positive $q$, a supplied complete smooth maximal stationary section, and a sufficiently late comparison sphere $C=C_t$ for which the past-boundary localization and endpoint results apply. Use the temporal section time $v=v_q$, the compact zero-time cut $D$, its initial set $A$ and endpoint map $F:A\to D$. Use the negative-time cuts $D_z$, their initial sets $A_z$ and endpoint maps $F_z$ from the truncated-height construction, with $z<0$ in its specified flow interval. Assume also $\min_C v>0$.

For each $c\in A_z$, the ray reaches $D$ before it reaches $D_z$ when followed into the past; hence $A_z\subseteq A$. On every regular part of any selected ray from $C$ to $D$ or $D_z$, the expansion of the future-directed affine tangent normalized at $C$ is strictly positive. At each endpoint, let $J(F)$ or $J(F_z)$ be the nonnegative Gram two-Jacobian of a local smooth transverse hitting-map extension, using the induced metrics on $C$ and the relevant spacelike section. Then, pointwise on $A_z$,

$$0\le J(F_z)(c)\le J(F)(c)\le1.$$

In addition, the zero-time estimate holds on its entire initial domain: $0\le J(F)(c)\le1$ for every $c\in A$, whether or not $c$ belongs to any $A_z$. The endpoint inequalities include possible focality at a cut: positivity of expansion is asserted only before a focal endpoint. They do not assert injectivity or an area formula for the image of a cut.

## Statement references

[post-stationary-vacuum-model](item-post-stationary-vacuum-model)

[def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets)

[def-truncated-null-boundary-height](item-def-truncated-null-boundary-height)

[def-stationary-section-time](item-def-stationary-section-time)

[def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[pthm-comparison-sphere-properties](item-pthm-comparison-sphere-properties)

[pthm-past-boundary-localization](item-pthm-past-boundary-localization)

[pthm-null-endpoint-map-properties](item-pthm-null-endpoint-map-properties)

## Facts & Assumptions

[A1] Use the stated regular stationary vacuum model, maximal section and mass-one construction, and assume the Axiom of Choice. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The section time is $v(t,x)=t-u_q(x)$, the stationary flow preserves $g_q$, and its level sections are spacelike. For the same family matched in [F8], the comparison sphere has positive future outward null expansion, and its stationary cylinder is timelike. [def-stationary-section-time](item-def-stationary-section-time) [pthm-comparison-sphere-properties](item-pthm-comparison-sphere-properties)

[F2] The zero-time cut is the portion of the relative past boundary of $C$ inside the cylinder. The definitions specify the past-directed null-normal rays, $A$, $F$, $D_z$, $A_z$ and $F_z$; the endpoint result supplies the zero-time hitting-map regularity. [pthm-past-boundary-localization](item-pthm-past-boundary-localization) [def-near-horizon-past-boundary-sets](item-def-near-horizon-past-boundary-sets) [def-truncated-null-boundary-height](item-def-truncated-null-boundary-height) [pthm-null-endpoint-map-properties](item-pthm-null-endpoint-map-properties)

[F3] A causal segment from a point of the relative past boundary to the compact spacelike target $C$ stays on that boundary; such a null normal segment has no focal point to $C$ in its interior. [lem-author-2632702918ef-target-segment-boundary-containment](item-lem-author-2632702918ef-target-segment-boundary-containment) [lem-author-2632702918ef-target-interior-focal-exclusion](item-lem-author-2632702918ef-target-interior-focal-exclusion)

[F4] The transformed Einstein–Maxwell geometry has $\operatorname{Ric}(L,L)\ge0$ for every nonzero null $L$. On a regular null-normal congruence with this convergence condition and positive future expansion at the initial surface, the expansion is positive to its past and the screen area Jacobian is nonincreasing toward the past. [pthm-electrovacuum-energy-conditions](item-pthm-electrovacuum-energy-conditions) [lem-null-optics-jacobian-comparison-input](item-lem-null-optics-jacobian-comparison-input)

[F5] The screen is $L^\perp/\mathbb RL$ with the induced positive metric; the null-normal Jacobi map and its focal points are as in the screen definition. Geodesics depend smoothly on their initial data, and a nonzero null tangent meets a spacelike section transversely. The cut Jacobian is the Gram two-Jacobian of a smooth local hitting-map extension. The parametrized implicit function theorem gives a local $C^k$ solution of a $C^k$ equation when the derivative in the solved variable is invertible; its application for every finite $k$ to the smooth hitting equation gives a smooth solution by uniqueness. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data) [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map) [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data) [math:thm-parametrized-implicit-function-theorem-with-higher-regularity](https://alphabetamath.cc/item/thm-parametrized-implicit-function-theorem-with-higher-regularity)

[F6] Under the regular vacuum, original maximal-section, mass-one and nontrivial $T|_S$ hypotheses in [A1], the global one-form construction supplies a smooth stationary primitive $W_0$ and the normalized Ernst potential on the exterior and a neighborhood of $S$, with original-chart spatial components $(W_0)_i=O_5(r^{-3})$. Use its same pole $p$ and the family $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. The family definition gives the contraction $W_q(T)=d_q-D_q$. Its smoothness and stationarity follow from the supplied smooth stationary $W_0$ and $T^\flat$. The denominator result gives $D_q>0$ on the exterior for every $q\in[0,1]$. The Harrison algebra theorem therefore applies to this supplied metric and gives $d_q>0$ and the exact identity $g_q(T,T)=d_q^2g(T,T)/(4D_q)$. In particular the stationary field has the same timelike character for the original and transformed metrics on their common domain. This argument uses no exact radial formula for the spatial coefficients of $W_0$. [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form) [def-harrison-one-form-family](item-def-harrison-one-form-family) [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive) [pthm-harrison-lorentzian-algebra](item-pthm-harrison-lorentzian-algebra)

[F7] For the fixed positive $q$ and supplied section, the transformed exterior is a smooth globally hyperbolic time-oriented Lorentzian four-manifold. The comparison target is a compact smooth embedded spacelike two-sphere without boundary. Together with temporal $v$ and $v(p)<\min_Cv$, these are the compact-target hypotheses of [F3]. [pthm-transformed-cauchy-sections](item-pthm-transformed-cauchy-sections) [pthm-comparison-sphere-properties](item-pthm-comparison-sphere-properties)

[F8] The mass-one convention stipulates a supplied original smooth spacelike maximal section $\Sigma_1$ with an ADM mass limit in its end coordinates $x^i$ that exists and equals one; existence of the section and convergence of the limit are assumptions. The denominator and component estimates allow the supplied stationary-primitive alternative $(W_0)_i=O_5(r^{-3})$ in the original chart, keeping their mass-one end, original supplied maximal section, normalized Ernst potential, pole and Harrison one-form conditions. Their conclusions are uniform for $q\in[0,1]$. The coordinate-null-normal and sphere-area-expansion results inherit precisely those data and estimates, and the comparison-sphere result uses that same family at $r=R_0q^{-2/3}$. Thus none of these estimate applications requires exact radial coefficients when the differentiated spatial bound is supplied. [pthm-harrison-denominator-asymptotics](item-pthm-harrison-denominator-asymptotics) [pthm-harrison-component-asymptotics](item-pthm-harrison-component-asymptotics) [pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates) [pthm-sphere-area-expansion-estimates](item-pthm-sphere-area-expansion-estimates) [pthm-comparison-sphere-properties](item-pthm-comparison-sphere-properties) [def-harrison-normalization](item-def-harrison-normalization)

## Proof

**Given:** The construction, cuts and negative $z$ in the Statement.

**Goal:** Prove the inclusion, expansion sign, zero-cut bound on all of $A$ and negative-cut Jacobian comparison.

1.1 In the original stationary end, regularity in [A1] gives $g(T,T)=g_{00}\to-1$ uniformly in angle. Choose a fixed radius beyond which $g(T,T)<0$, and choose the free comparison constant $R_0$ beyond that radius, retaining the large-radius requirements of the comparison-sphere supplier. Since $0<q\le1$, the comparison cylinder has radius $R_0q^{-2/3}\ge R_0$. For the same selected primitive and pole, [F6] gives a smooth stationary $W_q$, its normalization $W_q(T)=d_q-D_q$, and a positive denominator on the whole exterior. In the notation of the global construction, $dW_0=4((f-1)F+\psi\star_gF)$ and $dT^\flat=2F$, so direct differentiation gives $dW_q=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$, the required Harrison curl identity. Thus the supplied metric and one-form meet the algebra theorem's hypotheses. Its exact algebraic identity gives $g_q(T,T)=d_q^2g(T,T)/(4D_q)<0$ on and outside the cylinder. The temporal section time satisfies $dv(T)=1$ by [F1], so this timelike field is future-directed: a past-directed timelike vector has negative pairing with the temporal covector. The complete stationary product and the invariance of $g_q$ preserve this conclusion along every cylinder orbit. This establishes future timelike cylinder orbits for the supplied smooth Harrison family. To match the expansion input as well, [F6] gives $(W_0)_i=O_5(r^{-3})$ in the unchanged original chart. Use the same mass-one end, supplied original maximal section with its stipulated ADM mass-one limit in $x^i$, normalized potential and pole in [F8]. The stationarity, curl and contraction identities just checked are the component supplier's Harrison one-form conditions, and its positivity domain is supplied by [F6]. Its remaining spatial-decay condition is exactly the bound in [F6], so the denominator and component estimates apply to this same $W_q$ and $g_q$, not to an auxiliary radial choice. The coordinate-null-normal and sphere-area-expansion suppliers then apply with those same data. Their uniform expansion estimate is $\theta_{L_q}=2q/(1+qr)+O(r^{-2})$. At $r=R_0q^{-2/3}$, the ratio of the leading term to $r^{-2}$ is at least $2R_0^2/(1+R_0)$ for $0<q\le1$; enlarge the same free $R_0$ so this exceeds the uniform error constant, retaining every other end threshold. This is precisely the positive-expansion application of the comparison-sphere supplier in [F1]. Stationary translation carries that sign to $C=C_t$. No equality between the smooth primitive and the radial integral is used. [given, A1, F1, F6, F8, algebra]

1.2 Consider either an arbitrary $c\in A$ with endpoint $p=F(c)$, or an arbitrary $c\in A_z$ with endpoint $p=F_z(c)$. In both cases [F2] gives $p\in\partial I^-(C)$ and $v(p)<\min_Cv$. By [F3] and [F7], the entire selected null segment is on that boundary and has no focal point strictly between $C$ and $p$. Choose the affine parameter $\lambda=0$ at $C$, with future-directed tangent $L=\partial_\lambda$; its endpoint parameter $\lambda_p$ is negative. The stationary isometry carries the positive future outward expansion to $C$, and positive affine rescaling preserves its sign. Null convergence holds along the segment. The screen Jacobi map is initially the identity and is invertible on $(\lambda_p,0]$ by focal exclusion. Applying the optical comparison on every closed regular subinterval ending at $0$ gives $\theta(\lambda)>0$ and a positive screen Jacobian $j$ satisfying $j(\lambda_1)\le j(\lambda_2)\le j(0)=1$ for $\lambda_p<\lambda_1\le\lambda_2\le0$. This treats all of $A$ directly, without an exhaustion by the $A_z$. [A1, F1, F2, F3, F4, F5, F7, given]

2.1 Fix $c\in A_z$ and let $p_z=F_z(c)$. The chosen ray segment from $p_z$ to $c$ is causal, and $p_z$ lies on the relative past boundary of $C$, with $v(p_z)=z<\min_Cv$. The compact-target hypotheses hold by [F7], so [F3] puts the whole segment on that boundary. Since $z<0<\min_Cv$, temporal monotonicity gives a unique crossing $p_0$ of $v=0$ between $p_z$ and $c$. If $p_0$ were outside the cylinder, continuity from the inside point $p_z$ would give a cylinder crossing $y$ at $v(y)\le0$. At its spatial coordinate $x$, $v(y)=t(y)-u_q(x)$ and the point of $C$ on the same stationary orbit has $v=t-u_q(x)\ge\min_Cv>0$. Thus $t(y)<t$, and the future timelike stationary orbit from $y$ reaches $C$, placing $y$ in $I^-(C)$, contrary to boundary membership. The same orbit argument excludes $p_0$ on the cylinder. Hence $p_0$ is inside it, and localization identifies $p_0$ with a point of $D$. Uniqueness of the temporal hit gives $c\in A$ and $F(c)=p_0$. [given, F1, F2, F3, F7, step 1.1]

2.2 At either type of endpoint use a smooth local normalized null-normal field on $C$. Smooth geodesic dependence gives a smooth evaluation map $G(x,\lambda)$ on an open neighborhood of its finite included hit. For $b=0$ or $b=z$, the scalar hitting equation is $H(x,\lambda)=v(G(x,\lambda))-b=0$. Its solved-variable derivative at the hit is $\partial_\lambda H=dv(L)>0$, since $L$ is nonzero future null and $v$ is temporal. In local coordinates on $C$, apply [F5]'s implicit function theorem with the two coordinates as the free variables and $\lambda$ as the one solved variable (and no additional parameter block). It supplies a unique smooth local hitting parameter $\lambda_b(x)$ and the extension $x\mapsto G(x,\lambda_b(x))$ into the smooth spacelike level $v=b$; temporal uniqueness identifies its restriction with the selected endpoint map. This construction remains valid at a focal endpoint because it uses $dv(L)$, not the rank of the screen map. Differentiating this extension adds a multiple of $L$ to each fixed-affine-parameter variation vector $V$. The normal congruence has $g(L,V)=0$ and $g(L,L)=0$, so these additions change neither its Gram matrix nor its determinant. The Gram two-Jacobian of each hitting map is therefore the screen Jacobian at the corresponding hit, also when the determinant vanishes. [F1, F2, F5, step 1.2, algebra]

3.1 For any $c\in A$, apply step 1.2 with $p=F(c)$. The screen Jacobi fields and their nonnegative Gram Jacobian are continuous through the finite endpoint by smooth geodesic dependence, including when that endpoint is focal. Taking the limit $\lambda\downarrow\lambda_p$ of $0<j(\lambda)\le1$ and using step 2.2 gives $0\le J(F)(c)\le1$. This proves the zero-cut estimate on every point of $A$ and positivity of future expansion on each regular part before its endpoint. [F5, step 1.2, step 2.2]

4.1 For $c\in A_z$, step 2.1 gives the intermediate point $p_0=F(c)$ and parameters $\lambda_z<\lambda_0<0$. Step 1.2 with endpoint $p_z$ makes $p_0$ an interior regular point. Its regular comparison gives $j(\lambda)\le j(\lambda_0)\le1$ for $\lambda_z<\lambda\le\lambda_0$. Continuity through $p_z$ and step 2.2 therefore give $0\le J(F_z)(c)\le J(F)(c)\le1$, allowing a focal endpoint at $p_z$. The argument is pointwise and does not use injectivity or an image-area identity. [F3, F5, step 2.1, step 1.2, step 2.2] ∎

## Source notes

The article citation attributes the comparison. The proof uses the declared causal, optical, energy, global-primitive, Harrison-algebra, end-estimate, smooth-flow and implicit-function suppliers; the article's assertion is not used as a premise. The comparison family is matched by differentiated spatial decay of the very same smooth global primitive, not by identifying it with the radial integral. All endpoint, focal and all-domain zero-cut conclusions are unchanged; the simultaneous smooth-global/exact-radial assertion remains outside this proof.
