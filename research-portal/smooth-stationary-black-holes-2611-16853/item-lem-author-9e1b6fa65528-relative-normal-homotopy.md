---
title: Relative homotopy primitive on a normal bundle
status: published
research_item: lem-author-9e1b6fa65528-relative-normal-homotopy
dependency_level: 0
---

## Prerequisites

- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)
- [math:def-normal-and-conormal-bundles-of-an-embedded-submanifold](https://alphabetamath.cc/item/def-normal-and-conormal-bundles-of-an-embedded-submanifold)
- [math:prop-normal-and-conormal-bundles-are-smooth-vector-bundles](https://alphabetamath.cc/item/prop-normal-and-conormal-bundles-are-smooth-vector-bundles)
- [math:def-vector-bundle-chart-and-transition-function](https://alphabetamath.cc/item/def-vector-bundle-chart-and-transition-function)
- [math:def-pullback-of-a-differential-form](https://alphabetamath.cc/item/def-pullback-of-a-differential-form)
- [math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges](https://alphabetamath.cc/item/prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges)
- [math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula)
- [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)
- [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle)
- [math:thm-local-coordinate-formula-for-the-exterior-derivative](https://alphabetamath.cc/item/thm-local-coordinate-formula-for-the-exterior-derivative)
- [math:thm-the-exterior-derivative-commutes-with-pullback](https://alphabetamath.cc/item/thm-the-exterior-derivative-commutes-with-pullback)
- [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)
- [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [math:def-smooth-differential-k-form](https://alphabetamath.cc/item/def-smooth-differential-k-form)
- [math:prop-local-coordinate-expression-for-a-differential-form](https://alphabetamath.cc/item/prop-local-coordinate-expression-for-a-differential-form)


## Statement

Work in ZFC, including the axiom of choice. Let $M$ be a smooth manifold and $S\subseteq M$ a smooth embedded submanifold, with smooth normal vector bundle $\nu(S)=TM|_S/TS$. Supply an open neighborhood $U$ of $S$ in $M$ and a diffeomorphism from $U$ onto an open neighborhood $V$ of the zero section in $\nu(S)$, taking each $p\in S$ to $(p,0)$. Assume $V$ is closed under the fibre dilations $\delta_\lambda(p,\xi)=(p,\lambda\xi)$ for $0\leq\lambda\leq1$, and use this identification throughout. Write $\pi:U\to S$ for the bundle projection, $\iota:S\hookrightarrow U$ for the zero-section inclusion, and $\mathcal R=\xi^a\partial_{\xi^a}$ for the radial vector field in bundle coordinates. For a smooth closed two-form $\Theta$ on $U$ and a smooth one-form $\beta$ on $S$ satisfying $d\beta=\iota^*\Theta$, the one-form $W=\pi^*\beta+\int_0^1\lambda^{-1}\delta_\lambda^*(i_{\mathcal R}\Theta)\,d\lambda$ is smooth and satisfies $dW=\Theta$ and $\iota^*W=\beta$. The integrand at $\lambda=0$ means its smooth extension proved below. Here closed means $d\Theta=0$, primitive means a one-form with exterior derivative $\Theta$, contraction means $(i_{\mathcal R}\Theta)(X)=\Theta(\mathcal R,X)$, and restriction to $TS$ means pullback by $\iota$.

## Facts & Assumptions

[A1] The ambient set theory is ZFC. Full choice supplies its countable restriction $\mathrm{AC}_\omega$ for the smooth-normal-bundle result in [F3]; no further choice is used in the homotopy calculation. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Cartan's identity is $\mathcal L_X=d i_X+i_Xd$. The Lie derivative is the derivative of pullback along the local flow at parameter zero. [math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula) [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)

[F2] A continuous integrand with continuous parameter derivatives on compact rectangles admits differentiation under its integral. Apply this coefficientwise and repeatedly in coordinate directions. The coordinate formula $d(\sum_I a_I dx^I)=\sum_I da_I\wedge dx^I$ then permits exterior differentiation under these smooth parameter integrals. [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle) [math:thm-local-coordinate-formula-for-the-exterior-derivative](https://alphabetamath.cc/item/thm-local-coordinate-formula-for-the-exterior-derivative)

[F3] Embedded submanifolds use slice charts. Their quotient normal bundles are smooth vector bundles under $\mathrm{AC}_\omega$, which [A1] supplies. Bundle charts have fibre-linear smooth transition maps. Thus the projection, zero section, fibre dilations and radial vector field are smooth and agree across charts; the neighborhood identification is supplied as a hypothesis, not inferred here. [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart) [math:def-normal-and-conormal-bundles-of-an-embedded-submanifold](https://alphabetamath.cc/item/def-normal-and-conormal-bundles-of-an-embedded-submanifold) [math:prop-normal-and-conormal-bundles-are-smooth-vector-bundles](https://alphabetamath.cc/item/prop-normal-and-conormal-bundles-are-smooth-vector-bundles) [math:def-vector-bundle-chart-and-transition-function](https://alphabetamath.cc/item/def-vector-bundle-chart-and-transition-function)

[F4] Pullback of a form evaluates it on the differential of the map, is smooth and functorial, preserves wedges, and satisfies $d(F^*\omega)=F^*(d\omega)$ for every smooth map $F$. In particular this applies to $\pi$, $\iota$ and every $\delta_\lambda$, including $\lambda=0$. [math:def-pullback-of-a-differential-form](https://alphabetamath.cc/item/def-pullback-of-a-differential-form) [math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges](https://alphabetamath.cc/item/prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges) [math:thm-the-exterior-derivative-commutes-with-pullback](https://alphabetamath.cc/item/thm-the-exterior-derivative-commutes-with-pullback)

[F5] For a continuously differentiable scalar function $a$ on an open interval containing $[0,1]$, $\int_0^1 a'(\lambda)\,d\lambda=a(1)-a(0)$. The endpoint evaluation below applies this identity to the smooth coordinate coefficients of $\delta_\lambda^*\Theta$. [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)

[F6] On every smooth coordinate chart, a smooth differential form has a unique expansion in increasing coordinate wedges with smooth coefficient functions. [math:prop-local-coordinate-expression-for-a-differential-form](https://alphabetamath.cc/item/prop-local-coordinate-expression-for-a-differential-form)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove smoothness of the stated one-form and both asserted identities.

1.1 The smooth normal-bundle structure in [F3] is applicable by [A1]. In a bundle chart, [F6] gives $\Theta=\tfrac12 A_{ij}(y,\xi)dy^i\wedge dy^j+B_{ia}(y,\xi)dy^i\wedge d\xi^a+\tfrac12 C_{ab}(y,\xi)d\xi^a\wedge d\xi^b$, with smooth coefficients and $C_{ab}=-C_{ba}$. For $\lambda>0$, the pullback definition gives $H_\lambda:=\lambda^{-1}\delta_\lambda^*(i_{\mathcal R}\Theta)=-\xi^aB_{ia}(y,\lambda\xi)dy^i+\lambda\xi^aC_{ab}(y,\lambda\xi)d\xi^b$. This expression extends smoothly to $\lambda=0$. The extensions in different charts agree, since they agree for positive $\lambda$ and are continuous at zero. At $\xi=0$ the extended one-form is zero. [A1, F3, F4, F6, given, algebra]

2.1 For each point of $U$, its dilated segment is a compact subset of the open set $V$. In a bundle chart about its base point, shrink a coordinate neighborhood so that its dilations remain in $V$ for $\lambda$ in an open interval containing $[0,1]$. The formula in step 1.1 is consequently smooth in all variables on that neighborhood and interval. On smaller compact coordinate rectangles every coefficient and every coordinate derivative is continuous. Repeated application of [F2] makes $A:=\int_0^1H_\lambda\,d\lambda$ a smooth one-form and gives $dA=\int_0^1 dH_\lambda\,d\lambda$. Step 1.1 also gives $\iota^*A=0$. [F2, F3, F4, step 1.1]

3.1 The radial vector field has local flow $(p,\xi)\mapsto(p,e^t\xi)$. For $\lambda>0$, the identity $\delta_{\lambda+h}=\delta_{1+h/\lambda}\circ\delta_\lambda$, the flow definition of Lie derivative and pullback functoriality give $\partial_\lambda(\delta_\lambda^*\Theta)=\lambda^{-1}\delta_\lambda^*(\mathcal L_{\mathcal R}\Theta)$. Cartan's identity, $d\Theta=0$ and commutation of $d$ with pullback therefore give $\partial_\lambda(\delta_\lambda^*\Theta)=dH_\lambda$. Both sides extend continuously to zero by the smooth coefficient expressions in steps 1.1 and 2.1. [F1, F4, step 1.1, step 2.1, given]

4.1 Apply [F5] coefficientwise on the interval provided in step 2.1. Since $\delta_1=\mathrm{id}_U$ and $\delta_0=\iota\circ\pi$, steps 2.1 and 3.1 give $dA=\Theta-\pi^*\iota^*\Theta$. Thus $W=\pi^*\beta+A$ is smooth and $dW=\pi^*d\beta+\Theta-\pi^*\iota^*\Theta=\Theta$. Finally $\pi\circ\iota=\mathrm{id}_S$ and $\iota^*A=0$ imply $\iota^*W=\beta$. [F4, F5, step 2.1, step 3.1, given] ∎
