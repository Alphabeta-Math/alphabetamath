---
title: Uniform coordinate-sphere area and null expansion
status: draft
research_item: pthm-sphere-area-expansion-estimates
dependency_level: 11
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 21–22, proof of Proposition 4.1 and equation (4.2)
      hypotheses: The article's mass-one stationary vacuum construction and specified
        Harrison family, with q in [0,1] and sufficiently large radius.
      reading_limits: Read the frozen article text at the page 21–22 markers, proof of
        Proposition 4.1 and equation (4.2), for attribution only. The local
        calculation uses declared suppliers; no independent PDF-image review is
        claimed.
      attribution: "Attribution only: the article states the uniform coordinate-sphere
        area and outgoing null-expansion estimates and the large-radius causal
        properties. Its assertion is not a premise of the local proof."
---

PDF p. 21: ` Proof of Proposition 4.1 `; PDF p. 22: ` Proof of Proposition 4.1; (4.2) `

## Prerequisites

- [pthm-harrison-component-asymptotics](item-pthm-harrison-component-asymptotics)
- [pthm-harrison-denominator-asymptotics](item-pthm-harrison-denominator-asymptotics)
- [pthm-harrison-lorentzian-algebra](item-pthm-harrison-lorentzian-algebra)
- [pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates)
- [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-harrison-normalization](item-def-harrison-normalization)
- [math:prop-round-sphere-model-geometry](https://alphabetamath.cc/item/prop-round-sphere-model-geometry)
- [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)
- [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density)
- [math:thm-determinant-differential-and-jacobis-formula](https://alphabetamath.cc/item/thm-determinant-differential-and-jacobis-formula)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in the inherited ZFC convention. Adopt the mass-one stationary vacuum end, pole, normalized Ernst potential and specified Harrison family of the component-asymptotics supplier, including its hypotheses. Write $T=\partial_t$, $r=|x|$, $q\in[0,1]$, $a=q+r^{-1}$ and $d_q=D_q(p)$ as in the Harrison normalization. For sufficiently large $r$, let $S_{t,r}$ be the coordinate sphere and $\gamma_q$ its induced metric. Let $\gamma_{\mathbb S^2}$ be the unit round metric. Fix finitely many smooth angular charts with compact subsets whose relative interiors cover $\mathbb S^2$, as in the null-normal supplier. Uniformly in $q$ and angle,
$$\gamma_{q,AB}=(1+qr)^2((\gamma_{\mathbb S^2})_{AB}+O(r^{-1})),\qquad \partial_r\log\sqrt{\det\gamma_q}=\frac{2q}{1+qr}+O(r^{-2}).$$
The unsigned area and the expansion of the future outward null normal $L_q$ normalized by $g_q(T,L_q)=-d_q/4$ therefore satisfy
$$|S_{0,R}|_{g_q}=4\pi(1+qR)^2(1+O(R^{-1})),\qquad \theta_{L_q}=\frac{2q}{1+qR}+O(R^{-2}).$$
One radius works for all $q\in[0,1]$: beyond it, each $t=\mathrm{constant}$ slice is spacelike, $dt$ is timelike, and the stationary translates of each coordinate sphere form a timelike cylinder. Here $O$ means a bound with a constant independent of $q$, radius and angle; the angular component estimates are understood on those compact chart subsets, with one constant for the finite collection.

## Statement references

[pthm-harrison-component-asymptotics](item-pthm-harrison-component-asymptotics)

[pthm-harrison-denominator-asymptotics](item-pthm-harrison-denominator-asymptotics)

[pthm-harrison-lorentzian-algebra](item-pthm-harrison-lorentzian-algebra)

[pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates)

[def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[def-harrison-normalization](item-def-harrison-normalization)

[math:prop-round-sphere-model-geometry](https://alphabetamath.cc/item/prop-round-sphere-model-geometry)

[math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)

[math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density)

[math:thm-determinant-differential-and-jacobis-formula](https://alphabetamath.cc/item/thm-determinant-differential-and-jacobis-formula)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[F1] On the specified end, with constants and spatial derivatives uniform in $q$, $(g_q)_{ij}=a^2(\delta_{ij}+O_5(r^{-1}))$ and $(g_q)_{ti}=d_q a^{-1}O_5(r^{-2})$; the time-time component is $-d_q^2(16a^2)^{-1}(1+O(r^{-1}))$. The definition of differentiated $O$ bounds controls derivatives in Cartesian coordinates. [pthm-harrison-component-asymptotics](item-pthm-harrison-component-asymptotics) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] The pole factor $d_q$ is bounded above and away from zero uniformly on $[0,1]$. [pthm-harrison-denominator-asymptotics](item-pthm-harrison-denominator-asymptotics) [def-harrison-normalization](item-def-harrison-normalization)

[F3] The transformed metric is Lorentzian and stationary. The normalized future outward null normal has $L_q^r=1+O(r^{-1})$, $L_q^t=(4/d_q)a^2(1+O(r^{-1}))$, and $L_q^A=O(r^{-2})$; its expansion is $\frac12\gamma_q^{AB}(\mathcal L_{L_q}g_q)_{AB}$. [pthm-harrison-lorentzian-algebra](item-pthm-harrison-lorentzian-algebra) [pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[A1] The inherited ZFC convention includes the axiom of choice. In particular it supplies countable choice: applying a choice function to the family of values of a sequence of nonempty sets gives a choice in each term. This meets the round-sphere and density-integration suppliers' choice hypotheses; the null-screen interface already assumes this convention. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F4] The unit round sphere is $\mathbb S^2=\{\omega\in\mathbb R^3:|\omega|=1\}$ with the Euclidean induced metric; it is a compact smooth boundaryless Riemannian surface, and $T_\omega\mathbb S^2=\omega^\perp$. The round-sphere model supplier applies with $n=2$ and radius $1$, under [A1]. [math:prop-round-sphere-model-geometry](https://alphabetamath.cc/item/prop-round-sphere-model-geometry)

[F5] On a smooth Riemannian two-surface the unsigned area density in local coordinates is $\mu_\gamma=\sqrt{\det(\gamma_{AB})}\,|dy^1dy^2|$. Under [A1] this defines a Borel measure finite on compact sets, whose integral agrees with smooth density integration. Thus $|S|_\gamma=\int_S\mu_\gamma$ for a compact surface; no orientation is required. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density)

[F6] For an invertible real square matrix $G$ and a matrix direction $H$, $D\det(G)[H]=\det(G)\operatorname{tr}(G^{-1}H)$. In particular, along a differentiable positive-definite matrix family, the ordinary chain rule gives $\partial_r\log\sqrt{\det G}=\frac12\operatorname{tr}(G^{-1}\partial_rG)$. [math:thm-determinant-differential-and-jacobis-formula](https://alphabetamath.cc/item/thm-determinant-differential-and-jacobis-formula)

## Proof

**Given:** The inherited ZFC convention, the end and family in the Statement, with $q\in[0,1]$ and sufficiently large $r$.

**Goal:** Prove the uniform metric, area, expansion and causal estimates.

1.1 In angular coordinates $x^i=r\omega^i(y)$, the Euclidean identities $\delta_{ij}\partial_A\omega^i\partial_B\omega^j=(\gamma_{\mathbb S^2})_{AB}$ and $\delta_{ij}\omega^i\partial_A\omega^j=0$ (the second obtained by differentiating $|\omega|^2=1$) turn [F1] into $\gamma_{q,AB}=a^2r^2((\gamma_{\mathbb S^2})_{AB}+h_{AB})$, where $h$ and its first angular derivatives are $O(r^{-1})$ and $\partial_r h=O(r^{-2})$. These bounds follow by the chain rule from the differentiated Cartesian estimates. Since $ar=1+qr$, this gives the first display. The inverse of the parenthesized matrix is uniformly bounded relative to the round metric for large $r$. [given, F1, F4, algebra]

1.2 The spatial block in [F1] is positive definite for large $r$, so the coordinate slices are spacelike. After scaling the time basis vector by $4a/d_q$ and spatial basis vectors by $a^{-1}$, the metric matrix is the Minkowski diagonal matrix plus $O(r^{-1})$; the mixed terms have this order because $a\ge r^{-1}$. Its inverse consequently has negative time-time entry for one common large radius, so $dt$ is timelike. The displayed time-time estimate makes $T$ timelike there. Since $T$ is tangent to the stationary cylinder and the sphere directions form a positive two-plane orthogonal to a suitable timelike combination within its tangent space, the induced cylinder metric is Lorentzian. [F1, F2, F3, algebra]

1.3 Compute the round area in these conventions. Away from one meridian and the poles, write $\omega(\vartheta,\varphi)=(\sin\vartheta\cos\varphi,\sin\vartheta\sin\varphi,\cos\vartheta)$ for $0<\vartheta<\pi$ and $0<\varphi<2\pi$. Taking Euclidean inner products of its two derivatives gives the induced matrix $\operatorname{diag}(1,\sin^2\vartheta)$, so [F5] gives density $\sin\vartheta\,d\vartheta\,d\varphi$. The omitted meridian and poles have zero area: in finitely many regular charts covering them the smooth density is bounded, each compact smooth arc has bounded coordinate derivative and can be covered by $N$ squares of side $O(N^{-1})$ with total area $O(N^{-1})$, and each point has arbitrarily small square covers. Hence $|\mathbb S^2|=\int_0^{2\pi}\int_0^\pi\sin\vartheta\,d\vartheta\,d\varphi=2\pi[-\cos\vartheta]_0^\pi=4\pi$. [A1, F4, F5, algebra]

2.1 The determinant identity in [F6], applied to the positive matrix of step 1.1, gives $\partial_r\log\sqrt{\det\gamma_q}=2\partial_r\log(ar)+\frac12\operatorname{tr}((\gamma_{\mathbb S^2}+h)^{-1}\partial_rh)$. As $\partial_r\log(ar)=q/(1+qr)$, the error is $O(r^{-2})$. Likewise $\sqrt{\det\gamma_q}=(ar)^2\sqrt{\det\gamma_{\mathbb S^2}}(1+O(r^{-1}))$ uniformly. Using [F5] and step 1.3, integrate this density over the compact unit sphere. After factoring out $(ar)^2$, the density error is bounded in absolute value by $Cr^{-1}$ times the round density, uniformly in $q$ and angle, so the integral is $4\pi(ar)^2(1+O(r^{-1}))$. At $r=R$ this is the stated area estimate. [A1, F1, F5, F6, step 1.1, step 1.3, algebra]

2.2 The differentiated component estimates and the explicit quadratic-root construction of the normal in [pthm-coordinate-null-normal-estimates](item-pthm-coordinate-null-normal-estimates) also give, on the fixed compact chart subsets, $\partial_A L_q^r=O(r^{-1})$, $\partial_A L_q^t=a^2O(r^{-1})$, and $\partial_A L_q^B=O(r^{-2})$. Indeed angular differentiation is $r\partial_A\omega^i\partial_i$; differentiating the scaled inverse matrix and the positive square root preserves the uniform estimates because their denominators are bounded away from zero by [F2] and the scaled metric is uniformly close to Minkowski space. [F1, F2, F3, step 1.2, algebra]

3.1 Stationarity eliminates the $L_q^t\partial_t\gamma_{AB}$ term in the coordinate formula for the Lie derivative. The bounds from steps 1.1 and 2.2, together with $(g_q)_{tA}=d_q a^{-1}O(r^{-1})$, $(g_q)_{rA}=a^2O(1)$ and $\gamma_q^{AB}=a^{-2}r^{-2}O(1)$ on the fixed compact chart subsets, show that all terms other than $\frac12L_q^r\gamma_q^{AB}\partial_r\gamma_{q,AB}$ contribute $O(r^{-2})$ to the trace. In particular, $a^{-1}\le r$ controls the mixed time term uniformly at $q=0$. Thus $\theta_{L_q}=L_q^r\partial_r\log\sqrt{\det\gamma_q}+O(r^{-2})$. Since $q/(1+qr)\le r^{-1}$, replacing $L_q^r$ by $1$ changes this by $O(r^{-2})$. Step 2.1 gives the asserted expansion. [F1, F2, F3, step 1.1, step 2.1, step 2.2, algebra] ∎
