---
title: From a Schwarzschild spatial isometry to the normalized spacetime exterior
status: published
research_item: lem-author-f247c641a714-schwarzschild-static-data-lift
dependency_level: 4
---

## Prerequisites

- [def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)
- [lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction)
- [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)
- [lem-author-f247c641a714-static-boundary-and-positive-mass](item-lem-author-f247c641a714-static-boundary-and-positive-mass)
- [physics:def-gr-schwarzschild-exterior-model](https://alphabetamath.cc/physics/item/def-gr-schwarzschild-exterior-model)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)
- [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)
- [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing)
- [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)
- [math:thm-monotone-convergence-for-the-integral](https://alphabetamath.cc/item/thm-monotone-convergence-for-the-integral)


## Statement

Suppose the regular static exterior data satisfy the reduced equations and their spatial metric is isometric, with its boundary and asymptotic end, to
$$h_{\rm S}=\left(1+\frac{\mu}{2s}\right)^4(ds^2+s^2d\omega^2),\qquad s>\mu/2,\quad \mu>0.$$
Then the normalized lapse is $V_{\rm S}=(1-\mu/(2s))/(1+\mu/(2s))$, the lapse coefficient is $m=\mu$, and the full static product is isometric to the Schwarzschild spacetime exterior. No assumption about maximal analytic extension of the spacetime is needed for this lifting step.

## Statement references

[def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)

[lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction)

[math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)

[lem-author-f247c641a714-static-boundary-and-positive-mass](item-lem-author-f247c641a714-static-boundary-and-positive-mass)

[physics:def-gr-schwarzschild-exterior-model](https://alphabetamath.cc/physics/item/def-gr-schwarzschild-exterior-model)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[F1] The regular static exterior data supply the global product, its future field $\partial_t$, the boundary and normalized end, and the inherited ZFC convention. The static reduction supplies $\Delta_hV=0$. [def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data) [lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction)

[F2] The inherited ZFC convention includes full choice and hence countable choice $\mathrm{AC}_\omega$, as required by the divergence theorem and the Schwarzschild model definition. Explicitly, for a sequence of nonempty sets, apply full choice to its set of values and compose that choice function with the sequence. No new choice hypothesis is being imposed. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F3] Under countable choice the divergence theorem applies to smooth fields on compact oriented smooth Riemannian domains, with outward unit normals; compactness makes the support condition automatic. The boundary-and-mass lemma supplies $\int_X|DV|_h^2\,d\mu_h=4\pi m$. Only that energy identity is imported from this lemma. All divergence applications below take place inside $X$, where the metric is smooth. [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem) [lem-author-f247c641a714-static-boundary-and-positive-mass](item-lem-author-f247c641a714-static-boundary-and-positive-mass)

[F4] The Schwarzschild exterior model is the product $\mathbb R_{x^0}\times(s_{\rm Sch},\infty)\times S^2$ with metric $-(1-s_{\rm Sch}/r)d(x^0)^2+(1-s_{\rm Sch}/r)^{-1}dr^2+r^2\gamma_{S^2}$, future field $\partial_{x^0}$, and $s_{\rm Sch}=2G_Nm_*/c^2$. Here use the purely mathematical parameters $c=G_N=1$, $m_*=\mu$, $x^0=t$, $r=\mathcal R$ and $s_{\rm Sch}=2\mu$; $d\omega^2=\gamma_{S^2}$ is the unit round sphere metric. The symbol $s_{\rm Sch}$ is distinct from the isotropic radius $s$ in the Statement. No physical law or measured constant is imported by these parameter choices. [physics:def-gr-schwarzschild-exterior-model](https://alphabetamath.cc/physics/item/def-gr-schwarzschild-exterior-model)

[F5] On the smooth interior, $d\mu_h$ is the intrinsic Borel measure of the positive smooth Riemannian density $\sqrt{\det h}\,|dx^1dx^2dx^3|$. Under countable choice this measure has the coordinate integral formula, and integration against it agrees with smooth density integration on compact smooth domains. With the inherited orientation this also equals the volume-form integral in [F3], since both have coefficient $\sqrt{\det h}$. These interfaces apply to the compact annuli below, without any boundary regularity requirement at $B$, which is outside each annulus. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing) [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)

[F6] On any measure space, an increasing sequence of nonnegative measurable functions with pointwise limit $f$ has integrals increasing to $\int f$, without a prior finiteness assumption. [math:thm-monotone-convergence-for-the-integral](https://alphabetamath.cc/item/thm-monotone-convergence-for-the-integral)

[F7] On the smooth Riemannian interior, $Df=(df)^\sharp$, $D^2f(A,C)=h(D_ADf,C)$ and $\operatorname{div}_hY=\operatorname{tr}(A\mapsto D_AY)$. Tracing the connection product rule gives $\operatorname{div}_h(fDf)=|Df|_h^2+f\Delta_hf$. In coordinates the divergence is $(\det h)^{-1/2}\partial_i((\det h)^{1/2}Y^i)$. [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)

## Proof

**Given:** The boundary-preserving spatial isometry in the Statement, the regular static data and harmonic lapse equation of [F1], their inherited countable choice in [F2], the divergence, energy and model interfaces in [F3]–[F4], and the integration and differential-operator interfaces in [F5]–[F7].

**Goal:** Recover the lapse and global product, rather than infer a global spacetime result from a merely local isometry.

1.1 Pull back the radial function $U=(1-\mu/(2s))/(1+\mu/(2s))$ through the spatial isometry, and write $a=\mu/2$ and $\phi(s)=1+a/s$. By the coordinate divergence formula in [F7], its radial Laplacian is $(\phi^6s^2)^{-1}\partial_s(s^2\phi^2\partial_sU)=0$, since $s^2\phi^2\partial_sU=\mu$. Thus $U$ is harmonic, zero at $B$, and tends to one. The difference $w=V-U$ is harmonic and zero on $B$. Outside compact cores both asymptotically Euclidean metrics are uniformly comparable to their Euclidean metrics, so distance from a fixed compact set is bounded above and below by positive multiples of the corresponding radius. The isometry preserves those distances, hence the original end radius and $s$ are comparable. The given end estimates and preservation of gradient norms consequently give $w=O(s^{-1})$ and $|Dw|_h=O(s^{-2})$. [given, F1, F7]

2.1 Use the spatial isometry to identify $X$ with $(a,\infty)\times S^2$. For integers $j\ge1$, put $\varepsilon_j=1/(j+1)$, $R_j=a+j+1$ and $D_j=\{a+\varepsilon_j\le s\le R_j\}$. These are compact oriented smooth Riemannian domains entirely in $X$, with two disjoint smooth boundary spheres; they increase and their union is $X$. On a sphere $s=b$, the unit normals are $\pm\phi(b)^{-2}\partial_s$ and the area density is $\phi(b)^4b^2d\omega$. In a fixed compact strip adjacent to $B$, the $C^2$ regular data give a uniform bound for $|DV|_h$, and the explicit $U$ has bounded gradient, hence $|Dw|_h\le C$. The radial segments from $s=a$ to $a+\varepsilon$ have length $\int_a^{a+\varepsilon}\phi(s)^2ds=O(\varepsilon)$. The zero boundary value of $w$ then gives $w=O(\varepsilon)$ on the inner face, whose area is uniformly bounded by the displayed formula. Thus the absolute inner flux of $wDw$ is $O(\varepsilon_j)$. The outer area is $O(R_j^2)$, and the bounds in step 1.1 make its absolute outer flux $O(R_j^{-1})$. This constructs the exhaustion and both estimates directly for $w$. [given, F1, step 1.1]

3.1 By [F7], $\operatorname{div}_h(wDw)=|Dw|_h^2$. Apply the divergence theorem [F3] on each $D_j$, using countable choice [F2] and the integration convention [F5]. Step 2.1 bounds the nonnegative energy by $\int_{D_j}|Dw|_h^2\,d\mu_h\le C(\varepsilon_j+R_j^{-1})\to0$. The compact domains are Borel and $\mathbf1_{D_j}|Dw|_h^2$ are nonnegative Borel functions increasing pointwise to $|Dw|_h^2$. Monotone convergence [F6] therefore gives $\int_X|Dw|_h^2\,d\mu_h=0$. A nonzero value of $|Dw|_h$ would, by continuity, give an interior coordinate ball with the integrand bounded below by a positive constant, and the positive continuous coordinate density in [F5] gives that ball positive measure. Hence $Dw=0$ everywhere. Connectedness makes $w$ constant, and its zero limit at infinity makes it zero. [F1, F2, F3, F5, F6, F7, step 1.1, step 2.1]

4.1 Set $\mathcal R=s(1+\mu/(2s))^2$. This is strictly increasing from $2\mu$ to infinity on $s>\mu/2$, and direct differentiation gives $h_{\rm S}=(1-2\mu/\mathcal R)^{-1}d\mathcal R^2+\mathcal R^2d\omega^2$ and $U^2=1-2\mu/\mathcal R$. Taking the product of the spatial isometry with the identity on all $t\in\mathbb R$ therefore gives a global isometry of the full static exterior to $-(1-2\mu/\mathcal R)dt^2+(1-2\mu/\mathcal R)^{-1}d\mathcal R^2+\mathcal R^2d\omega^2$. With the parameter and unit-round-metric identifications in [F4], this is precisely the Schwarzschild exterior model, and the map sends $\partial_t$ to $\partial_{x^0}$, preserving the time orientation. [given, F1, F4, step 3.1]

5.1 On the same $D_j$, the product identity [F7] and the harmonicity of $U$ give $\operatorname{div}_h(UDU)=|DU|_h^2$. Apply [F3] with [F2] and [F5]. The sphere normal and area formula of step 2.1 give the flux of $UDU$ through $s=b$, oriented toward increasing $s$, as $4\pi U(b)b^2\phi(b)^2\partial_sU(b)=4\pi\mu U(b)$. The inner outward normal has the opposite sign, so $\int_{D_j}|DU|_h^2\,d\mu_h=4\pi\mu\bigl(U(R_j)-U(a+\varepsilon_j)\bigr)\to4\pi\mu$. Apply [F6] to $\mathbf1_{D_j}|DU|_h^2$ as in step 3.1 to obtain $\int_X|DU|_h^2\,d\mu_h=4\pi\mu$. These computations on the model are also computations on $X$: an isometry preserves gradient norms, and its metric pullback identity gives $\sqrt{\det(F^*h_{\rm S})}=|\det dF|\sqrt{\det h_{\rm S}}\circ F$ in coordinates, exactly the transformation law of the intrinsic density in [F5]. Since $V=U$ on $X$ by step 3.1, comparison with the independently supplied identity $\int_X|DV|_h^2\,d\mu_h=4\pi m$ in [F3] gives $\mu=m$, without presuming invariance of an end-coordinate coefficient. [F2, F3, F5, F6, F7, step 1.1, step 2.1, step 3.1, step 4.1] ∎
