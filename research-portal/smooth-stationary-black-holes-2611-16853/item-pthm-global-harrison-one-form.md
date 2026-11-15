---
title: Closedness, periods and smooth global choice of W0
status: draft
research_item: pthm-global-harrison-one-form
dependency_level: 8
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 9–10, §2.2
      attribution: The article asserts closedness and vanishing periods of Theta_0 and
        constructs a global primitive with a smooth horizon choice and radial
        decay by a stationary cutoff.
      hypotheses: The article's regular stationary vacuum setting with maximal
        original exterior section and mass normalized to one.
      reading_limits: Frozen article text and rendered PDF pp. 9–10 were read for
        attribution and exact comparison. This reference is not used as proof.
---

PDF p. 9: ` §2.2, Stokes and cutoff construction `; PDF p. 10: ` §2.2, Stokes and cutoff construction `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-harrison-one-form-family](item-def-harrison-one-form-family)
- [def-killing-ernst-notation](item-def-killing-ernst-notation)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product)
- [pthm-ernst-and-one-form-decay](item-pthm-ernst-and-one-form-decay)
- [lem-spherical-exterior-period-input](item-lem-spherical-exterior-period-input)
- [lem-author-29145f41e94d-weak-data-equivariant-global-primitive](item-lem-author-29145f41e94d-weak-data-equivariant-global-primitive)
- [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)
- [lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant](item-lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant)
- [lem-author-9e1b6fa65528-radial-exterior-primitive](item-lem-author-9e1b6fa65528-radial-exterior-primitive)
- [math:thm-general-stokes-theorem](https://alphabetamath.cc/item/thm-general-stokes-theorem)
- [math:cor-homology-of-spheres](https://alphabetamath.cc/item/cor-homology-of-spheres)
- [math:cor-homotopic-maps-induce-the-same-map-on-singular-homology](https://alphabetamath.cc/item/cor-homotopic-maps-induce-the-same-map-on-singular-homology)
- [pthm-ernst-potential-existence](item-pthm-ernst-potential-existence)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [thm-vacuum-killing-ernst-input](item-thm-vacuum-killing-ernst-input)
- [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)
- [math:prop-interior-product-on-forms-is-a-graded-antiderivation](https://alphabetamath.cc/item/prop-interior-product-on-forms-is-a-graded-antiderivation)
- [math:def-fundamental-class-of-a-compact-oriented-manifold](https://alphabetamath.cc/item/def-fundamental-class-of-a-compact-oriented-manifold)
- [math:thm-top-homology-characterizes-compact-orientable-manifolds](https://alphabetamath.cc/item/thm-top-homology-characterizes-compact-orientable-manifolds)


## Statement

Assume the regular stationary vacuum model of [post-stationary-vacuum-model](item-post-stationary-vacuum-model) and [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime), with the specified exterior section maximal, mass normalized to one, and $T|_S\not\equiv0$. Use the stationary end coordinates and the normalized Ernst data $F=\tfrac12dT^\flat$, $f=-g(T,T)$ and $\sigma=f+i\psi\to1$ of [def-killing-ernst-notation](item-def-killing-ernst-notation). Let $\star_g$ be the oriented Lorentzian Hodge star and put $\Theta_0=4((f-1)F+\psi\star_gF)$ and $D_0=|1-\sigma|^2$, as in [def-harrison-one-form-family](item-def-harrison-one-form-family).

Then $d\Theta_0=0$. If $S_R$ is a stationary-coordinate sphere on the end, with orientation transported from the end to the bifurcation sphere $S$, then $\int_S\Theta_0=\lim_{R\to\infty}\int_{S_R}\Theta_0=0$. The class of an end sphere generates $H_2(\mathcal E;\mathbb R)$, and $\Theta_0$ has a global smooth primitive on the open exterior $\mathcal E$. There is a single smooth stationary real primitive $W_0$ on $\mathcal E$ and a neighborhood of $S$ with $dW_0=\Theta_0$, $W_0(T)=D_0(p)-D_0$ and spatial end components $(W_0)_i=O_5(r^{-3})$ in the unchanged original chart. Here $p\in S$ is a common zero of $T$ and the local rotational field $Z$. The choice is locally invariant under $Z$ and the commuting Hawking field $K=T+\Omega_HZ$ near $S$, and is obtained by stationary exact cutoff corrections retaining a smooth horizon gauge and a smooth decaying end gauge. The specified original section, including its maximality, is retained.

Separately, in the original chart the exact radial formula $A_i(x)=-\int_1^\infty s x^j(\Theta_0)_{ji}(sx)\,ds$ defines a $C^5$ spatial primitive $A=A_i\,dx^i$ of the spatial restriction of $\Theta_0$ on a far tail, with $A_i=O_5(r^{-3})$. If the spatial coefficients of $\Theta_0$ obey the corresponding differentiated decay at every finite order in that chart, the same radial formula is smooth. The smooth global choice $W_0$ above is not required to have these exact radial spatial coefficients. Throughout, $O_5$ includes the corresponding Cartesian spatial derivative bounds through order five.

## Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice. The model and regularity assumptions include the smooth four-dimensional stationary vacuum geometry, the asymptotically flat end, complete stationary flow, globally hyperbolic exterior, the prescribed spherical exterior section and the smooth bifurcate horizon. The original exterior section is maximal, the mass is one, and $T|_S\not\equiv0$. ZFC supplies the countable choice required by the Hodge-calculus and manifold-Stokes suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)

[F1] The stationary flow identifies $\mathcal E$ with $\mathbb R\times(1,\infty)\times S^2$. The differentiated end estimates give $(\Theta_0)_{ij}=O_5(r^{-4})$ and the radial end primitive with five differentiated bounds. The product uses the specified original spacelike section, whose smooth closure has boundary $S$. [pthm-original-lapse-and-product](item-pthm-original-lapse-and-product) [pthm-ernst-and-one-form-decay](item-pthm-ernst-and-one-form-decay) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] The normalized potential $\sigma=f+i\psi$ exists on $\mathcal E$ and extends smoothly to $\mathcal E\cup O$ for a neighborhood $O$ of $S$; it is stationary and normalized at infinity. In the declared Ernst convention, $df=2\iota_TF$ and $d\psi=2\iota_T\star_gF$. The vacuum Killing identities give $F=\tfrac12dT^\flat$ and $dF=d\star_gF=0$. [pthm-ernst-potential-existence](item-pthm-ernst-potential-existence) [def-killing-ernst-notation](item-def-killing-ernst-notation) [thm-vacuum-killing-ernst-input](item-thm-vacuum-killing-ernst-input)

[F3] On the product exterior, a closed two-form is exact exactly when its period on an end sphere vanishes; closed one-forms there are exact. [lem-spherical-exterior-period-input](item-lem-spherical-exterior-period-input)

[F4] The weak-data equivariant primitive lemma applies to smooth stationary vacuum data with the specified spherical stationary-flow product, the original mass-one $O_6$ end, a normalized smooth Ernst potential through $S$, and the outward normal-tube wedge attachment. Its local inputs are commuting Killing fields $K,Z$ with $K=T+\Omega_HZ$, $K|_S=0$, a period-$2\pi$ circle action, constant nonzero normal boost rate, and a common zero $p$ of $T,Z$. Under precisely these hypotheses it constructs one smooth stationary primitive with $W_0(T)+D_0=D_0(p)$, a smooth locally $K,Z$ invariant horizon gauge and original-chart spatial decay $O_5(r^{-3})$. Its end gauge uses an auxiliary all-order chart and returns to the original section before stationary exact cutoff gluing; it does not assert equality with the original-chart radial integral. [lem-author-29145f41e94d-weak-data-equivariant-global-primitive](item-lem-author-29145f41e94d-weak-data-equivariant-global-primitive)

[F5] General Stokes applies to a smooth two-form on a compact oriented three-manifold with boundary, with the outward-normal-first boundary orientation. Homotopic maps induce equal ordinary singular homology maps. The second real homology of $S^2$ is one-dimensional. For a nonempty connected compact oriented boundaryless two-manifold, restriction of top homology to a local stalk is injective and onto $\mathbb R$; the oriented fundamental class restricts to the local orientation generator. [math:thm-general-stokes-theorem](https://alphabetamath.cc/item/thm-general-stokes-theorem) [math:cor-homotopic-maps-induce-the-same-map-on-singular-homology](https://alphabetamath.cc/item/cor-homotopic-maps-induce-the-same-map-on-singular-homology) [math:cor-homology-of-spheres](https://alphabetamath.cc/item/cor-homology-of-spheres) [math:thm-top-homology-characterizes-compact-orientable-manifolds](https://alphabetamath.cc/item/thm-top-homology-characterizes-compact-orientable-manifolds) [math:def-fundamental-class-of-a-compact-oriented-manifold](https://alphabetamath.cc/item/def-fundamental-class-of-a-compact-oriented-manifold)

[F6] The Lorentzian Hodge star has symmetric exterior pairing, $P\wedge\star_gQ=\langle P,Q\rangle_g\,\mathrm{vol}_g$, and $\star_g^2=-\operatorname{id}$ on two-forms. Exterior differentiation obeys the graded product rule, and contraction obeys $\iota_T(\alpha\wedge\beta)=(\iota_T\alpha)\wedge\beta+(-1)^k\alpha\wedge\iota_T\beta$ for a $k$-form $\alpha$. The complex self-dual conventions are unchanged. [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus) [math:prop-interior-product-on-forms-is-a-graded-antiderivation](https://alphabetamath.cc/item/prop-interior-product-on-forms-is-a-graded-antiderivation) [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data) [def-harrison-one-form-family](item-def-harrison-one-form-family)

[F7] Under the model, regularity and maximality assumptions, the local Hawking-field result supplies commuting $K,Z$, the period-$2\pi$ action, $K=T+\Omega_HZ$, $K|_S=0$, a common zero $p$ and a constant positive normal boost rate. The horizon-axis lemma identifies the exterior near $S$ as $b>|a|$ in the orthonormal normal-exponential tube based on the original section, with future normal $n$ and outward spatial normal $\nu$. Its collar hypothesis is the exterior side of that section. [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields) [lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant](item-lem-author-ca4ffba327b3-horizon-axes-and-exterior-quadrant)

[F8] For a closed spatial $C^5$ two-form with coefficients $O_5(r^{-4})$, the exact radial integral in the Statement is a $C^5$ primitive with coefficients $O_5(r^{-3})$. All-order differentiated bounds in the same chart make that formula smooth. [lem-author-9e1b6fa65528-radial-exterior-primitive](item-lem-author-9e1b6fa65528-radial-exterior-primitive)

## Proof

**Given:** The model, maximal section, mass normalization and fields in the Statement, with the set-theoretic convention in [A1].

**Goal:** Establish closedness, the period and homology assertions, and the stated global stationary primitive.

1.1 Apply [F2] under [A1] to obtain the normalized stationary Ernst potential and its smooth extension across $S$. Shrink $O$ as necessary. All fields defining $\Theta_0$ are therefore smooth on the common domain $\mathcal E\cup O$. [A1, F2]

1.2 The ordinary singular fundamental class $[S^2]$ is nonzero by [F5]: its restriction to any local stalk is the nonzero orientation generator. It therefore generates the one-dimensional space $H_2(S^2;\mathbb R)$. In the product of [F1], let $j$ include an end sphere at fixed coordinates $(t_*,r_*)$ and let $\pi$ project onto $S^2$. One has $\pi j=\operatorname{id}$, while $j\pi$ is homotopic to the identity by $(t,r,\omega)\mapsto((1-u)t+ut_*,(1-u)r+ur_*,\omega)$, $0\le u\le1$. The radial coordinate stays greater than one. Homotopy invariance in [F5] gives inverse induced homology maps, so $j_*[S^2]$ is precisely a generator represented by the oriented end sphere. This argument concerns ordinary singular homology throughout and uses no integration on continuous singular chains. [F1, F5]

1.3 Apply the local Hawking-field result of [F7] under [A1]; it supplies all the stated local symmetry, pole and constant normal boost data. The closure of the original spacelike section in [F1] has a smooth inward collar on its exterior side. Its interior is in $I^-(M^{\mathrm{end}})\cap I^+(M^{\mathrm{end}})=\mathcal E$, while the regularity assumptions identify the smooth transverse null boundaries meeting at $S$. These are the horizon-axis lemma's hypotheses, so [F7] gives the whole local exterior attachment $b>|a|$ in the normal tube. Shrink the common neighborhood to a connected normal tube about $S$; its exterior attachment is the whole spacetime wedge. [A1, F1, F7]

2.1 Symmetry of the pairing in [F6] gives $(\star_gF)\wedge\star_gF=F\wedge\star_g(\star_gF)=-F\wedge F$. The product rule and [F2] give $d\Theta_0=8((\iota_TF)\wedge F+(\iota_T\star_gF)\wedge\star_gF)$. Contract the preceding four-form identity with $T$. The contraction rule in [F6] gives twice the expression in parentheses equal to zero, since a two-form commutes with a one-form under the wedge product. Thus $d\Theta_0=0$ on $\mathcal E\cup O$. [F2, F6, step 1.1, algebra]

2.2 Apply [F4]. The smooth oriented time-oriented Ricci-flat data, future-timelike far end and original mass-one $O_6$ metric bounds are in [A1]; the specified spherical stationary-flow product and smooth spacelike boundary section are [F1]. The normalized potential with $d\sigma=2\iota_T(F+i\star_gF)$ and its smooth extension are [F2] and step 1.1. The local fields, circle action, common pole, constant nonzero boost and outward wedge attachment were supplied in step 1.3. These meet every hypothesis of the weak-data primitive lemma. Its conclusion gives one smooth stationary $W_0$ on $\mathcal E$ and a neighborhood of $S$, with $dW_0=\Theta_0$, $W_0(T)=D_0(p)-D_0$, local $K,Z$ invariance and original-chart spatial decay $O_5(r^{-3})$. The original section is unchanged. [A1, F1, F2, F4, step 1.1, step 1.3]

3.1 On $S_R$ the integral is $O(R^{-2})$: the spatial coefficients are $O(R^{-4})$ and the coordinate sphere has area $O(R^2)$. In the closure of the specified exterior section, the region between $S$ and $S_R$ is a compact smooth annulus with boundary $S_R-S$ for the transported orientation. By step 1.1 the restricted form is smooth through its inner boundary; its support on this compact annulus is compact. General Stokes and step 2.1 give $\int_{S_R}\Theta_0-\int_S\Theta_0=0$. Taking $R\to\infty$ proves both period assertions. [A1, F1, F5, step 1.1, step 2.1]

3.2 For the cutoff description use the construction in [F4]: the smooth decaying end primitive is first returned from an auxiliary regular chart to the original section. A stationary global primitive then receives exact stationary corrections on disjoint end and horizon-collar regions, with equal contraction constants. The construction checks exactness of the differences, stationary cutoff supports and equality with the horizon gauge on a whole neighborhood intersection with $\mathcal E$. Thus its output in step 2.2 keeps both the smooth horizon gauge and the smooth decaying end gauge. This invokes the existing construction under its checked hypotheses. [F4, step 2.2]

4.1 The product hypothesis of [F3] is [F1], and its closedness and zero-period hypotheses are steps 2.1 and 3.1. Hence $\Theta_0$ has a global smooth primitive on the open exterior. [F1, F3, step 2.1, step 3.1]

5.1 Restrict $\Theta_0$ to the original spatial end. It is smooth and closed by step 2.1, and its spatial coefficients have the $O_5(r^{-4})$ bounds of [F1]. Apply [F8] to obtain exactly $A_i(x)=-\int_1^\infty s x^j(\Theta_0)_{ji}(sx)\,ds$, with $A\in C^5$, $dA=\Theta_0|_{t=0}$ and $A_i=O_5(r^{-3})$. Under its additional all-order hypothesis [F8] gives smoothness of that same integral. This finite-order end construction is separate from the smooth global choice in step 2.2. [F1, F8, step 2.1, step 2.2] ∎

## Source notes

The article reference attributes its closedness, period, primitive and cutoff claims on PDF pp. 9–10. The local proof uses independent Ernst, topology and geometric suppliers. The previous application of the Radu GR/SBS primitive input has been replaced by the existing weak-data construction after explicitly checking its product, boundary, symmetry and end hypotheses. No angular-momentum leading expansion or ambient partial-Cauchy assumption is added to this item.

**Article claim retained for coverage (not a proved conclusion here).** On PDF p. 9, equation (2.10) specifies $(W_0)_i(x)=-\int_1^\infty s x^j(\Theta_0)_{ji}(sx)\,ds$ near infinity in the original stationary coordinates, with $W_0(T)=d_0-D_0$. The cutoff paragraph continuing onto PDF p. 10 asserts that the same global choice can be regular near $S$ while retaining (2.10) near infinity: it uses $W_0-\overline W_0=d\chi$ on the overlap and $\overline W_0+d(\eta\chi)$, where the stationary cutoff is zero near $S$ and one near infinity. Thus the simultaneous smooth global choice and exact radial end gauge asserted in the article remain explicitly recorded, rather than being replaced in coverage by two separate choices. This paragraph attributes that assertion to the original PDF; it supplies no premise for the Proof above.

**Status of the simultaneous assertion.** The radial-primitive supplier guarantees the exact integral only as a $C^5$ form under the stated finite-order bounds, with smoothness conditional on all-order differentiated bounds in the same chart. The weak-data global-primitive supplier guarantees a smooth global form with the required horizon normalization, local invariance and original-chart $O_5(r^{-3})$ decay, without identifying its end coefficients with that exact integral. These two conclusions do not establish their simultaneous realization by one smooth form. The unresolved claim retained from the article is whether, under its stated hypotheses and in the original stationary coordinates used for (2.10), one smooth stationary $W_0$ on $\mathcal E$ and a neighborhood of $S$ has both those exact spatial coefficients on a far tail and the stated smooth horizon choice. No extra chart regularity is assumed here. The Statement and Proof retain all their established conclusions, including the conditional smoothness of the radial integral; they do not claim this unresolved simultaneous assertion. This is a repair of generated coverage, not a determination of an original-author defect or a claim that the exact radial gauge is impossible in a suitably chosen chart.
