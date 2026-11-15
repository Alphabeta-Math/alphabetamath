---
title: Harrison fields, horizons and uniqueness inputs
description: Connect the common data to Ernst potentials, Harrison
  transformations, invariant horizon tensors, stationary slices and established
  uniqueness criteria. Keep each imported result tied to its stated hypotheses
  and each local consequence tied to its existing argument before article
  applications.
status: published
dependency_level: 1
---

**Purpose:** Connect the common data to Ernst potentials, Harrison transformations, invariant horizon tensors, stationary slices and established uniqueness criteria. Keep each imported result tied to its stated hypotheses and each local consequence tied to its existing argument before article applications.

## Periods and primitives on a spherical exterior

[Open item](item-lem-spherical-exterior-period-input) · level 0


### Statement

Work in ZFC. Let $E$ be a smooth manifold with a specified diffeomorphism $\Phi:\mathbb R\times(1,\infty)\times S^2\to E$. A smooth real or complex differential form is closed if its exterior derivative vanishes and exact if it is the exterior derivative of a smooth form of one lower degree. Every smooth closed real or complex one-form on $E$ is exact. A smooth closed real or complex two-form on $E$ is exact if and only if its integral over one sphere $\Phi(\{t\}\times\{r\}\times S^2)$ vanishes, where $r>1$ and the sphere carries the orientation transported from the outward orientation of $S^2$. For a complex form the integral is taken componentwise. Applying this criterion to a particular stationary exterior requires a product diffeomorphism as a separate hypothesis; this result does not establish one.

### Statement references

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:def-closed-and-exact-differential-forms](https://alphabetamath.cc/item/def-closed-and-exact-differential-forms)

[math:def-pullback-of-a-differential-form](https://alphabetamath.cc/item/def-pullback-of-a-differential-form)

[math:lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary](https://alphabetamath.cc/item/lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary)

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[math:ex-the-n-sphere-with-its-standard-smooth-atlas](https://alphabetamath.cc/item/ex-the-n-sphere-with-its-standard-smooth-atlas)

[math:def-oriented-smooth-manifold-and-oriented-chart](https://alphabetamath.cc/item/def-oriented-smooth-manifold-and-oriented-chart)

[math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

[math:def-smooth-differential-k-form](https://alphabetamath.cc/item/def-smooth-differential-k-form)

### Facts & Assumptions

[A1] ZFC supplies the countable choice assumed in the sphere cohomology calculation. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The degree-$k$ de Rham cohomology is the real vector space of closed smooth $k$-forms modulo exact forms; a closed form has zero class precisely when it is exact. [math:def-de-rham-cohomology](https://alphabetamath.cc/item/def-de-rham-cohomology) [math:def-closed-and-exact-differential-forms](https://alphabetamath.cc/item/def-closed-and-exact-differential-forms)

[F2] Under countable choice, $H^1_{\mathrm{dR}}(S^2)=0$ and $H^2_{\mathrm{dR}}(S^2)$ is one-dimensional over $\mathbb R$. [math:thm-de-rham-cohomology-of-spheres](https://alphabetamath.cc/item/thm-de-rham-cohomology-of-spheres)

[F3] A smooth homotopy equivalence induces an isomorphism on de Rham cohomology by pullback. Pullback commutes with exterior differentiation. [math:thm-de-rham-cohomology-is-smooth-homotopy-invariant](https://alphabetamath.cc/item/thm-de-rham-cohomology-is-smooth-homotopy-invariant) [math:thm-the-exterior-derivative-commutes-with-pullback](https://alphabetamath.cc/item/thm-the-exterior-derivative-commutes-with-pullback) [math:def-pullback-of-a-differential-form](https://alphabetamath.cc/item/def-pullback-of-a-differential-form)

[F4] On a compact oriented boundaryless manifold, an exact top form has zero integral. Integration of top forms on such a manifold is real-linear, strictly positive on a nonzero nonnegative form, and invariant under orientation-preserving diffeomorphisms. [math:cor-a-closed-oriented-manifold-has-no-top-form-with-nonzero-integral-that-is-exact](https://alphabetamath.cc/item/cor-a-closed-oriented-manifold-has-no-top-form-with-nonzero-integral-that-is-exact) [math:lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary](https://alphabetamath.cc/item/lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary)

[F5] A smooth manifold is equipped with a smooth atlas; a diffeomorphism is a smooth bijection with smooth inverse. Finite products carry the smooth structure given by product charts. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds) [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[F6] The unit sphere $S^2$ has its standard stereographic smooth atlas. An orientation is a smooth choice of a ray in each tangent determinant line; an embedded submanifold is locally a coordinate slice and carries the subspace topology. [math:ex-the-n-sphere-with-its-standard-smooth-atlas](https://alphabetamath.cc/item/ex-the-n-sphere-with-its-standard-smooth-atlas) [math:def-oriented-smooth-manifold-and-oriented-chart](https://alphabetamath.cc/item/def-oriented-smooth-manifold-and-oriented-chart) [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

[F7] A smooth real $k$-form is a smooth section of the $k$th exterior power of the cotangent bundle. The wedge of differential forms is defined pointwise by the wedge of alternating covectors; complex forms are pairs of real forms with componentwise linear operations. [math:def-smooth-differential-k-form](https://alphabetamath.cc/item/def-smooth-differential-k-form) [math:def-wedge-product-of-differential-forms](https://alphabetamath.cc/item/def-wedge-product-of-differential-forms)

### Proof

**Given:** The specified diffeomorphism, $t\in\mathbb R$, and $r>1$. Let $i:S^2\to E$ be $i(x)=\Phi(t,r,x)$, and let $p:E\to S^2$ be projection to the sphere factor after applying $\Phi^{-1}$.

**Goal:** Prove the stated exactness and period criteria.

1.1 Set $S_{t,r}=i(S^2)$. If $z:U\to V\subset\mathbb R^2$ is a sphere chart and $I,J$ are open intervals about $t,r$ with $J\subset(1,\infty)$, the coordinates $(z(x),u-t,v-r)$ on $\Phi(I\times J\times U)$ are smooth charts of $E$. They identify its intersection with $S_{t,r}$ with $V\times\{0\}\times\{0\}$. Thus $S_{t,r}$ is an embedded smooth surface with the subspace topology. In these charts $i$ is $z\mapsto(z,0,0)$, and its inverse on the image is the restriction of $p$; both are smooth, so $i:S^2\to S_{t,r}$ is a diffeomorphism. Give $S^2$ the outward orientation, in which $(v,w)$ is positive when $\det(x,v,w)>0$, and transport it by $i$ to $S_{t,r}$. This is a smooth orientation since the displayed determinant varies smoothly and never vanishes on a tangent basis. For a two-form $\alpha$ on $E$, its integral over $S_{t,r}$ is the integral of its pullback by the inclusion $S_{t,r}\hookrightarrow E$. The orientation-preserving diffeomorphism $i$ and [F4] identify that integral with $\int_{S^2}i^*\alpha$. [given, F3, F4, F5, F6, construct]

2.1 We have $p\circ i=\operatorname{id}_{S^2}$. A smooth homotopy from $\operatorname{id}_E$ to $i\circ p$ is obtained in product coordinates by $(u,v,x)\mapsto((1-s)u+st,(1-s)v+sr,x)$ for $0\leq s\leq1$; the second coordinate remains greater than $1$. Hence $i$ and $p$ are smooth homotopy inverses. Pullback by $i$ is therefore an isomorphism in every de Rham degree. In degree one, [F2] and [F1] imply that every closed real one-form on $E$ is exact. [given, F1, F2, F3, F5, step 1.1]

2.2 On the outward-oriented unit sphere define $\sigma=x_1\,dx_2\wedge dx_3-x_2\,dx_1\wedge dx_3+x_3\,dx_1\wedge dx_2$, restricted to $S^2$. Its value on a tangent basis $(v,w)$ is $\det(x,v,w)$, so it is a positive smooth top form. It is closed because every three-form on the two-dimensional sphere vanishes. By [F4], $\int_{S^2}\sigma>0$ and an exact two-form has zero integral. Thus $[\sigma]$ is nonzero and, by the one-dimensionality in [F2], generates $H^2_{\mathrm{dR}}(S^2)$. For any closed real two-form $\beta$ on $S^2$, write $[\beta]=c[\sigma]$; then $\beta-c\sigma$ is exact, and linearity and [F4] give $\int\beta=c\int\sigma$. Consequently $\beta$ is exact exactly when its integral vanishes. [F1, F2, F4, F6, F7, step 1.1, algebra]

3.1 Let $\alpha$ be a closed real two-form on $E$. Its pullback $i^*\alpha$ is closed, and the integral over the specified oriented sphere is $\int_{S^2}i^*\alpha$. By step 2.2 this integral vanishes exactly when $i^*[\alpha]=0$; the isomorphism in step 2.1 makes that equivalent to $[\alpha]=0$, hence to exactness of $\alpha$. The argument works for every choice of $t$ and $r>1$, so a vanishing period on any one such sphere suffices. [given, F1, F3, F4, step 1.1, step 2.1, step 2.2]

4.1 For complex forms, write the form as its real part plus $i$ times its imaginary part. Exterior differentiation and integration act componentwise, and a complex form is exact precisely when both real components are exact: combine their real primitives into a complex primitive. Applying the real one-form result and the real two-form criterion to both components proves the stated complex cases. [F1, F7, step 2.1, step 3.1] ∎



## Relative homotopy primitive on a normal bundle

[Open item](item-lem-author-9e1b6fa65528-relative-normal-homotopy) · level 0


### Statement

Work in ZFC, including the axiom of choice. Let $M$ be a smooth manifold and $S\subseteq M$ a smooth embedded submanifold, with smooth normal vector bundle $\nu(S)=TM|_S/TS$. Supply an open neighborhood $U$ of $S$ in $M$ and a diffeomorphism from $U$ onto an open neighborhood $V$ of the zero section in $\nu(S)$, taking each $p\in S$ to $(p,0)$. Assume $V$ is closed under the fibre dilations $\delta_\lambda(p,\xi)=(p,\lambda\xi)$ for $0\leq\lambda\leq1$, and use this identification throughout. Write $\pi:U\to S$ for the bundle projection, $\iota:S\hookrightarrow U$ for the zero-section inclusion, and $\mathcal R=\xi^a\partial_{\xi^a}$ for the radial vector field in bundle coordinates. For a smooth closed two-form $\Theta$ on $U$ and a smooth one-form $\beta$ on $S$ satisfying $d\beta=\iota^*\Theta$, the one-form $W=\pi^*\beta+\int_0^1\lambda^{-1}\delta_\lambda^*(i_{\mathcal R}\Theta)\,d\lambda$ is smooth and satisfies $dW=\Theta$ and $\iota^*W=\beta$. The integrand at $\lambda=0$ means its smooth extension proved below. Here closed means $d\Theta=0$, primitive means a one-form with exterior derivative $\Theta$, contraction means $(i_{\mathcal R}\Theta)(X)=\Theta(\mathcal R,X)$, and restriction to $TS$ means pullback by $\iota$.

### Facts & Assumptions

[A1] The ambient set theory is ZFC. Full choice supplies its countable restriction $\mathrm{AC}_\omega$ for the smooth-normal-bundle result in [F3]; no further choice is used in the homotopy calculation. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] Cartan's identity is $\mathcal L_X=d i_X+i_Xd$. The Lie derivative is the derivative of pullback along the local flow at parameter zero. [math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula) [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)

[F2] A continuous integrand with continuous parameter derivatives on compact rectangles admits differentiation under its integral. Apply this coefficientwise and repeatedly in coordinate directions. The coordinate formula $d(\sum_I a_I dx^I)=\sum_I da_I\wedge dx^I$ then permits exterior differentiation under these smooth parameter integrals. [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle) [math:thm-local-coordinate-formula-for-the-exterior-derivative](https://alphabetamath.cc/item/thm-local-coordinate-formula-for-the-exterior-derivative)

[F3] Embedded submanifolds use slice charts. Their quotient normal bundles are smooth vector bundles under $\mathrm{AC}_\omega$, which [A1] supplies. Bundle charts have fibre-linear smooth transition maps. Thus the projection, zero section, fibre dilations and radial vector field are smooth and agree across charts; the neighborhood identification is supplied as a hypothesis, not inferred here. [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart) [math:def-normal-and-conormal-bundles-of-an-embedded-submanifold](https://alphabetamath.cc/item/def-normal-and-conormal-bundles-of-an-embedded-submanifold) [math:prop-normal-and-conormal-bundles-are-smooth-vector-bundles](https://alphabetamath.cc/item/prop-normal-and-conormal-bundles-are-smooth-vector-bundles) [math:def-vector-bundle-chart-and-transition-function](https://alphabetamath.cc/item/def-vector-bundle-chart-and-transition-function)

[F4] Pullback of a form evaluates it on the differential of the map, is smooth and functorial, preserves wedges, and satisfies $d(F^*\omega)=F^*(d\omega)$ for every smooth map $F$. In particular this applies to $\pi$, $\iota$ and every $\delta_\lambda$, including $\lambda=0$. [math:def-pullback-of-a-differential-form](https://alphabetamath.cc/item/def-pullback-of-a-differential-form) [math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges](https://alphabetamath.cc/item/prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges) [math:thm-the-exterior-derivative-commutes-with-pullback](https://alphabetamath.cc/item/thm-the-exterior-derivative-commutes-with-pullback)

[F5] For a continuously differentiable scalar function $a$ on an open interval containing $[0,1]$, $\int_0^1 a'(\lambda)\,d\lambda=a(1)-a(0)$. The endpoint evaluation below applies this identity to the smooth coordinate coefficients of $\delta_\lambda^*\Theta$. [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)

[F6] On every smooth coordinate chart, a smooth differential form has a unique expansion in increasing coordinate wedges with smooth coefficient functions. [math:prop-local-coordinate-expression-for-a-differential-form](https://alphabetamath.cc/item/prop-local-coordinate-expression-for-a-differential-form)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove smoothness of the stated one-form and both asserted identities.

1.1 The smooth normal-bundle structure in [F3] is applicable by [A1]. In a bundle chart, [F6] gives $\Theta=\tfrac12 A_{ij}(y,\xi)dy^i\wedge dy^j+B_{ia}(y,\xi)dy^i\wedge d\xi^a+\tfrac12 C_{ab}(y,\xi)d\xi^a\wedge d\xi^b$, with smooth coefficients and $C_{ab}=-C_{ba}$. For $\lambda>0$, the pullback definition gives $H_\lambda:=\lambda^{-1}\delta_\lambda^*(i_{\mathcal R}\Theta)=-\xi^aB_{ia}(y,\lambda\xi)dy^i+\lambda\xi^aC_{ab}(y,\lambda\xi)d\xi^b$. This expression extends smoothly to $\lambda=0$. The extensions in different charts agree, since they agree for positive $\lambda$ and are continuous at zero. At $\xi=0$ the extended one-form is zero. [A1, F3, F4, F6, given, algebra]

2.1 For each point of $U$, its dilated segment is a compact subset of the open set $V$. In a bundle chart about its base point, shrink a coordinate neighborhood so that its dilations remain in $V$ for $\lambda$ in an open interval containing $[0,1]$. The formula in step 1.1 is consequently smooth in all variables on that neighborhood and interval. On smaller compact coordinate rectangles every coefficient and every coordinate derivative is continuous. Repeated application of [F2] makes $A:=\int_0^1H_\lambda\,d\lambda$ a smooth one-form and gives $dA=\int_0^1 dH_\lambda\,d\lambda$. Step 1.1 also gives $\iota^*A=0$. [F2, F3, F4, step 1.1]

3.1 The radial vector field has local flow $(p,\xi)\mapsto(p,e^t\xi)$. For $\lambda>0$, the identity $\delta_{\lambda+h}=\delta_{1+h/\lambda}\circ\delta_\lambda$, the flow definition of Lie derivative and pullback functoriality give $\partial_\lambda(\delta_\lambda^*\Theta)=\lambda^{-1}\delta_\lambda^*(\mathcal L_{\mathcal R}\Theta)$. Cartan's identity, $d\Theta=0$ and commutation of $d$ with pullback therefore give $\partial_\lambda(\delta_\lambda^*\Theta)=dH_\lambda$. Both sides extend continuously to zero by the smooth coefficient expressions in steps 1.1 and 2.1. [F1, F4, step 1.1, step 2.1, given]

4.1 Apply [F5] coefficientwise on the interval provided in step 2.1. Since $\delta_1=\mathrm{id}_U$ and $\delta_0=\iota\circ\pi$, steps 2.1 and 3.1 give $dA=\Theta-\pi^*\iota^*\Theta$. Thus $W=\pi^*\beta+A$ is smooth and $dW=\pi^*d\beta+\Theta-\pi^*\iota^*\Theta=\Theta$. Finally $\pi\circ\iota=\mathrm{id}_S$ and $\iota^*A=0$ imply $\iota^*W=\beta$. [F4, F5, step 2.1, step 3.1, given] ∎



## Stationary lifting of a spatial primitive

[Open item](item-lem-author-9e1b6fa65528-stationary-spatial-lifting) · level 0


### Statement

Let $\Sigma$ be a smooth manifold and give $E=\mathbb R_t\times\Sigma$ its product smooth structure. Write $t:E\to\mathbb R$ for the first coordinate, $\pi:E\to\Sigma$ for the projection and $T=\partial_t$. Suppose $\Theta\in\Omega^2(E)$ is smooth, closed and stationary, $D\in C^\infty(E)$ is stationary and $\iota_T\Theta=dD$. Put $B=\Theta-dt\wedge dD$. Then there is a unique smooth closed two-form $b$ on $\Sigma$ such that $B=\pi^*b$. If $b$ has a smooth primitive $a\in\Omega^1(\Sigma)$, meaning $da=b$, every real constant $c$ gives the smooth one-form $V=(c-D)dt+\pi^*a$ on $E$ with $dV=\Theta$, $\mathcal L_TV=0$ and $V(T)+D=c$. Here a function or form is stationary when its coefficients in product coordinates $(t,x)$, with $x$ a chart on $\Sigma$, are independent of $t$; a form descends to $\Sigma$ when it is a pullback by $\pi$.

### Statement references

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[math:def-smooth-differential-k-form](https://alphabetamath.cc/item/def-smooth-differential-k-form)

[math:def-closed-and-exact-differential-forms](https://alphabetamath.cc/item/def-closed-and-exact-differential-forms)

[math:def-interior-product-of-a-form-by-a-vector-field](https://alphabetamath.cc/item/def-interior-product-of-a-form-by-a-vector-field)

[math:def-wedge-product-of-differential-forms](https://alphabetamath.cc/item/def-wedge-product-of-differential-forms)

[math:def-pullback-of-a-differential-form](https://alphabetamath.cc/item/def-pullback-of-a-differential-form)

[math:def-lie-derivative-of-a-differential-form](https://alphabetamath.cc/item/def-lie-derivative-of-a-differential-form)

[math:prop-local-coordinate-expression-for-a-differential-form](https://alphabetamath.cc/item/prop-local-coordinate-expression-for-a-differential-form)

[math:thm-local-coordinate-formula-for-the-exterior-derivative](https://alphabetamath.cc/item/thm-local-coordinate-formula-for-the-exterior-derivative)

[math:prop-exterior-derivative-of-a-function-is-its-differential](https://alphabetamath.cc/item/prop-exterior-derivative-of-a-function-is-its-differential)

[math:prop-interior-product-is-a-graded-antiderivation](https://alphabetamath.cc/item/prop-interior-product-is-a-graded-antiderivation)

[math:prop-differential-forms-form-a-graded-commutative-algebra](https://alphabetamath.cc/item/prop-differential-forms-form-a-graded-commutative-algebra)

[math:thm-the-exterior-derivative-is-a-graded-derivation](https://alphabetamath.cc/item/thm-the-exterior-derivative-is-a-graded-derivation)

[math:thm-the-exterior-derivative-squares-to-zero](https://alphabetamath.cc/item/thm-the-exterior-derivative-squares-to-zero)

[math:thm-the-exterior-derivative-commutes-with-pullback](https://alphabetamath.cc/item/thm-the-exterior-derivative-commutes-with-pullback)

[math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula)

### Facts & Assumptions

[F1] Smooth manifolds and their product charts have the declared meanings; in these charts the projection $\pi(t,x)=x$ and the slice map $j(x)=(0,x)$ are smooth. [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold) [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[F2] Use smooth differential forms, closedness $d\omega=0$, exactness $\omega=d\eta$, interior product, wedge product, pullback and Lie derivative with their declared meanings. In particular, $(F^*\omega)_p(v_1,\ldots,v_k)=\omega_{F(p)}(dF_pv_1,\ldots,dF_pv_k)$. [math:def-smooth-differential-k-form](https://alphabetamath.cc/item/def-smooth-differential-k-form) [math:def-closed-and-exact-differential-forms](https://alphabetamath.cc/item/def-closed-and-exact-differential-forms) [math:def-interior-product-of-a-form-by-a-vector-field](https://alphabetamath.cc/item/def-interior-product-of-a-form-by-a-vector-field) [math:def-wedge-product-of-differential-forms](https://alphabetamath.cc/item/def-wedge-product-of-differential-forms) [math:def-pullback-of-a-differential-form](https://alphabetamath.cc/item/def-pullback-of-a-differential-form) [math:def-lie-derivative-of-a-differential-form](https://alphabetamath.cc/item/def-lie-derivative-of-a-differential-form)

[F3] A smooth form has a unique expansion in increasing coordinate wedges, $d(\sum_I\omega_I dx^I)=\sum_I d\omega_I\wedge dx^I$, and $df(X)=Xf$. [math:prop-local-coordinate-expression-for-a-differential-form](https://alphabetamath.cc/item/prop-local-coordinate-expression-for-a-differential-form) [math:thm-local-coordinate-formula-for-the-exterior-derivative](https://alphabetamath.cc/item/thm-local-coordinate-formula-for-the-exterior-derivative) [math:prop-exterior-derivative-of-a-function-is-its-differential](https://alphabetamath.cc/item/prop-exterior-derivative-of-a-function-is-its-differential)

[F4] Pointwise contraction satisfies $\iota_X(\alpha\wedge\beta)=(\iota_X\alpha)\wedge\beta+(-1)^k\alpha\wedge\iota_X\beta$ when $\alpha$ has degree $k$. Wedge products of smooth forms are smooth and graded commutative. [math:prop-interior-product-is-a-graded-antiderivation](https://alphabetamath.cc/item/prop-interior-product-is-a-graded-antiderivation) [math:prop-differential-forms-form-a-graded-commutative-algebra](https://alphabetamath.cc/item/prop-differential-forms-form-a-graded-commutative-algebra)

[F5] Exterior differentiation is real linear, satisfies $d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^k\alpha\wedge d\beta$ for $\alpha$ of degree $k$, squares to zero, and commutes with pullback along smooth maps. [math:thm-the-exterior-derivative-is-a-graded-derivation](https://alphabetamath.cc/item/thm-the-exterior-derivative-is-a-graded-derivation) [math:thm-the-exterior-derivative-squares-to-zero](https://alphabetamath.cc/item/thm-the-exterior-derivative-squares-to-zero) [math:thm-the-exterior-derivative-commutes-with-pullback](https://alphabetamath.cc/item/thm-the-exterior-derivative-commutes-with-pullback)

[F6] Cartan's formula is $\mathcal L_X\omega=d(\iota_X\omega)+\iota_X(d\omega)$. [math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula)

### Proof

**Given:** The smooth product, forms, function and hypotheses in the Statement.

**Goal:** Construct the descended closed form and its stationary lift with every stated identity.

1.1 The product coordinates give $dt(T)=1$ and $T(D)=0$, hence $\iota_TdD=0$. The contraction rule gives $\iota_T(dt\wedge dD)=dD-dt\,T(D)=dD$, so $\iota_TB=0$. The coordinate formula for $dD$ and stationarity of $D$ show that $dD$ has no $dt$ component and its coefficients are independent of $t$. Thus $B$ is stationary as well. [given, F1, F2, F3, F4]

2.1 Define $b=j^*B$. In every product chart the unique two-form expansion of $B$ has no $dt$ terms because $\iota_TB=0$, and its remaining coefficients are independent of $t$. Evaluating the pullback formulas for $j$ and $\pi$ therefore gives $B=\pi^*b$; it also proves uniqueness by evaluating this equality on the slice $t=0$. The form $b$ is globally smooth by its definition. Since $d(dt)=d^2t=0$, $d^2D=0$ and $d\Theta=0$, the graded product rule gives $dB=0$. Smoothness of $j$ and commutation with pullback now give $db=d(j^*B)=j^*(dB)=0$. [given, F1, F2, F3, F5, step 1.1]

3.1 Let $a$ be the supplied smooth primitive, $da=b$, and let $c\in\mathbb R$. The pullback $\pi^*a$ is a smooth form on $E$, so $V=(c-D)dt+\pi^*a$ is well defined and smooth. Differentiation and graded commutativity give $dV=-dD\wedge dt+\pi^*(da)=dt\wedge dD+\pi^*b=\Theta$. Since $d\pi(T)=0$, the pullback formula gives $(\pi^*a)(T)=a(d\pi(T))=0$, whence $V(T)=c-D$. [given, F1, F2, F3, F4, F5, step 2.1]

4.1 The coefficients of $\pi^*a$ in product coordinates depend only on $x$, so $V$ is stationary in the stated coordinate sense. Moreover Cartan's formula, $dV=\Theta$ and $\iota_T\Theta=dD$ give $\mathcal L_TV=d(V(T))+\iota_TdV=d(c-D)+dD=0$, and $V(T)+D=c$. The construction assumes the smooth primitive $a$; it does not assert that every closed form is exact. [given, F2, F5, F6, step 3.1] ∎



## Rank-one tangent changes, signature and Hodge transfer

[Open item](item-lem-rank-one-lorentzian-hodge-transfer) · level 1


### Statement

Let $V$ be an oriented four-dimensional real vector space with a Lorentz form $g$ of signature $(-,+,+,+)$, meaning a nondegenerate symmetric bilinear form with one negative and three positive directions. Let $T\in V$, $W\in V^*$, and $D,d>0$ satisfy $W(T)=d-D$. Define $A=I+D^{-1}T\otimes W$, where $(T\otimes W)(v)=W(v)T$, and $g'=(D/4)A^*g$, where $(A^*g)(u,v)=g(Au,Av)$. Give the domain of $A$ the transported orientation: a basis is positive exactly when its image under $A$ is positive.

Then $\det A=d/D$, $A^{-1}=I-d^{-1}T\otimes W$, and $g'$ has the same inertia as $g$. For every real or complex two-form $F$, with $(A^*F)(u,v)=F(Au,Av)$, the corresponding metric Hodge stars satisfy $\star_{g'}(A^*F)=A^*(\star_gF)$. For any two such forms $F,H$, their full complex-bilinear contractions satisfy $(A^*F)_{ab}(A^*H)^{ab}_{g'}=(4/D)^2F_{ab}H^{ab}_g$, where both indices are raised with the indicated inverse metric and no complex conjugation or factor of one half is used.

### Statement references

[math:def-orientation-of-a-finite-dimensional-real-vector-space](https://alphabetamath.cc/item/def-orientation-of-a-finite-dimensional-real-vector-space)

[def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[math:lem-determinant-rank-one-update-over-a-commutative-ring](https://alphabetamath.cc/item/lem-determinant-rank-one-update-over-a-commutative-ring)

[math:thm-sylvesters-law-of-inertia](https://alphabetamath.cc/item/thm-sylvesters-law-of-inertia)

[physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[physics:lem-emg-conformal-hodge-multiplier](https://alphabetamath.cc/physics/item/lem-emg-conformal-hodge-multiplier)

### Facts & Assumptions

**Given:** The oriented Lorentz space, $T$, $W$, $D$ and $d$ in the statement.

**Goal:** Establish the determinant, inverse, inertia, Hodge transfer and contraction formulas in the statement.

[A1] Work in the ZFC background, including the choice assumptions inherited by the geometric suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The rank-one determinant identity gives $\det(B+uv^{\mathsf T})=\det B+v^{\mathsf T}\operatorname{adj}(B)u$ over a commutative ring. [math:lem-determinant-rank-one-update-over-a-commutative-ring](https://alphabetamath.cc/item/lem-determinant-rank-one-update-over-a-commutative-ring)

[F2] A real symmetric form has basis-independent inertia under congruence. [math:thm-sylvesters-law-of-inertia](https://alphabetamath.cc/item/thm-sylvesters-law-of-inertia)

[F3] Algebraic pullback composes each covariant slot with the given linear map; inverse metrics raise indices, and the full two-form contraction is complex bilinear. [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[F4] The metric Hodge star is uniquely characterized by $\alpha\wedge\star_g\beta=\langle\alpha,\beta\rangle_g\operatorname{vol}_g$, with the exterior pairing induced by the inverse metric and the metric volume determined by the orientation. [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[F5] In four dimensions a positive conformal rescaling leaves the Hodge star on two-forms unchanged. [physics:lem-emg-conformal-hodge-multiplier](https://alphabetamath.cc/physics/item/lem-emg-conformal-hodge-multiplier)

[F6] An orientation of a finite-dimensional real vector space is an equivalence class of ordered bases, where two bases are equivalent when their change-of-basis isomorphism has positive determinant. [math:def-orientation-of-a-finite-dimensional-real-vector-space](https://alphabetamath.cc/item/def-orientation-of-a-finite-dimensional-real-vector-space)

[F7] A linear isomorphism of an oriented real vector space of positive dimension preserves its orientation exactly when its determinant is positive. [math:thm-determinant-sign-detects-orientation-change](https://alphabetamath.cc/item/thm-determinant-sign-detects-orientation-change)

[F8] Linear pullback respects tensor products and permutations of covariant slots. [math:prop-linear-pullback-respects-tensor-products-and-permutations](https://alphabetamath.cc/item/prop-linear-pullback-respects-tensor-products-and-permutations)

[F9] The wedge product of a $k$-covector and an $\ell$-covector is $(k+\ell)!/(k!\ell!)$ times the alternation of their tensor product. [math:def-wedge-product-of-alternating-covectors](https://alphabetamath.cc/item/def-wedge-product-of-alternating-covectors)

### Proof

1.1 Put $K=T\otimes W$. For every $v\in V$, $K^2v=W(v)W(T)T=(d-D)Kv$. Thus $(I+D^{-1}K)(I-d^{-1}K)=I+(D^{-1}-d^{-1}-(d-D)/(Dd))K=I$, and the same calculation in the opposite order gives $A^{-1}=I-d^{-1}K$. In any basis, [F1] with $B=I$, $u=D^{-1}T$ and $v^{\mathsf T}=W$ gives $\det A=1+D^{-1}W(T)=d/D>0$. [given, F1, algebra]

2.1 Since $A$ is invertible and $D/4>0$, a basis in which $g$ is diagonal with one negative and three positive entries pulls back by $A^{-1}$ to a basis in which $g'$ has those entries multiplied by $D/4$. Hence $g'$ has the same inertia as $g$, independently of basis by [F2]. By [F7], $A$ preserves the original orientation because $\dim V=4$ and $\det A>0$. Hence the transported positive-basis class in the sense of [F6] agrees with the original orientation on $V$. [step 1.1, F2, F6, F7, algebra]

3.1 Write $h=A^*g$. The map $A$ is an orientation-preserving isometry from $(V,h)$ with transported orientation to $(V,g)$. For two-forms $\alpha,\beta$, the induced inverse-metric pairing satisfies $\langle A^*\alpha,A^*\beta\rangle_h=\langle\alpha,\beta\rangle_g$: in a basis this follows by substituting $h^{-1}=A^{-1}g^{-1}A^{-\mathsf T}$ into the two raised slots. Also $\operatorname{vol}_h=A^*\operatorname{vol}_g$, as both sides take value $1$ on a transported positively oriented $h$-orthonormal basis. By [F8] and [F9], slotwise pullback commutes with the normalized alternating sum defining the wedge: it is linear, respects tensor products and commutes with every permutation of the slots. Thus $A^*(\alpha\wedge\gamma)=(A^*\alpha)\wedge(A^*\gamma)$ for alternating covectors $\alpha,\gamma$. Pulling back the identity in [F4] therefore gives $(A^*\alpha)\wedge A^*(\star_g\beta)=\langle A^*\alpha,A^*\beta\rangle_h\operatorname{vol}_h$. Since every two-form is an $A^*\alpha$, uniqueness in [F4] yields $\star_h(A^*\beta)=A^*(\star_g\beta)$. [step 1.1, step 2.1, F3, F4, F8, F9, algebra]

4.1 Regard $V$ as an affine manifold with constant metric $h$, a constant time orientation and the transported orientation. Applying [F5] to the constant positive factor $D/4$ gives $\star_{g'}=\star_h$ on two-forms, so step 3.1 proves the Hodge transfer. Moreover $g'^{-1}=(4/D)h^{-1}$, and the full contraction uses two inverse-metric factors. The pairing calculation in step 3.1, with the factor of two converting the exterior pairing to the full two-form contraction, therefore gives $(A^*F)_{ab}(A^*H)^{ab}_{g'}=(4/D)^2F_{ab}H^{ab}_g$. Real linearity extends both identities to complex forms by complex bilinearity. [step 3.1, F3, F4, F5, A1, algebra] ∎


## Normal boost action and invariant two-forms at a fixed surface

[Open item](item-lem-killing-normal-boost-and-invariant-tensors) · level 1


### Statement

Let $(M,g,N)$ be a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$, with Levi–Civita connection $\nabla$. Let $S$ be a smooth embedded spacelike two-surface and let $K$ be a smooth Killing field that vanishes on $S$. Write $\Phi_t$ for its local flow. At each $p\in S$, suppose that the map $B_p:v\mapsto\nabla_vK$ restricts to the normal plane $(T_pS)^\perp$ and has matrix $\kappa_p\begin{pmatrix}0&1\\1&0\end{pmatrix}$ in an orthonormal normal basis $(e_0,e_1)$, where $e_0$ is future timelike, $e_1$ is the chosen outward spacelike normal, and $\kappa_p>0$.

Then $\Phi_t(p)=p$ whenever the local flow is defined at $(t,p)$, and its differential is the identity on $T_pS$ and the Lorentz boost with matrix $\begin{pmatrix}\cosh(\kappa_pt)&\sinh(\kappa_pt)\\\sinh(\kappa_pt)&\cosh(\kappa_pt)\end{pmatrix}$ on the normal plane. If a smooth two-form $F$ is invariant under the local flow, meaning $\Phi_t^*F=F$ wherever both sides are defined, then $F_p(v,X)=0$ for every normal vector $v$ and every $X\in T_pS$.

Suppose additionally that a smooth $2\pi$-periodic flow $\phi_s$ of isometries preserves $S$ and future cones, and that $n$ is a smooth future timelike normal field along $S$. Its average $\bar n_p=(2\pi)^{-1}\int_0^{2\pi}d\phi_s|_{\phi_{-s}(p)}n_{\phi_{-s}(p)}\,ds$ is a smooth future timelike normal field. The normalized field $\widehat n=\bar n/\sqrt{-g(\bar n,\bar n)}$ is future unit timelike, normal to $S$, and invariant under $\phi_s$.

### Statement references

[def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:def-pullback-of-a-differential-form](https://alphabetamath.cc/item/def-pullback-of-a-differential-form)

### Facts & Assumptions

[A1] Work in ZFC, including the Axiom of Choice: every set-indexed family of nonempty sets has a choice function. Restricting to countably indexed families supplies countable choice. This assumption is used here in the inherited smooth-manifold, tangent-bundle and smooth-field conventions of F1, F3 and F4; the local boost, two-form and averaging calculations require no additional choice principle. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] A spacelike surface has positive definite induced metric; the Killing-field and time-oriented Lorentzian conventions are those of the bifurcate-horizon definition. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[F2] A local flow consists of integral curves and obeys the local flow law. Integral curves through a given point are unique on their common domain. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)

[F3] The Levi–Civita connection is an affine connection; in coordinates, $\nabla_vK$ is the ordinary directional derivative of the components of $K$ plus a connection term linear in $K$. [physics:def-gr-metric-selected-connection](https://alphabetamath.cc/physics/item/def-gr-metric-selected-connection)

[F4] The smooth-field, normality and time-orientation conventions are those of the circle-action definition. For the arbitrary smooth $2\pi$-periodic flow in the Statement, interpret its displayed average componentwise in any fixed basis of $T_pM$, using scalar Riemann integrals, and call a field $u$ along $S$ invariant when $d\phi_t|_pu_p=u_{\phi_t(p)}$ for every $p\in S$ and $t\in\mathbb R$. The integral is basis independent because a change-of-basis matrix is constant in the integration variable and scalar integration is linear. These local definitions impose no least-period condition. [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[F5] A smooth two-form is a smooth alternating covariant two-tensor. For a smooth map $f$ and a smooth two-form $F$ on its target, the pullback is given by $(f^*F)_p(u,v)=F_{f(p)}(df|_pu,df|_pv)$. [math:def-pullback-of-a-differential-form](https://alphabetamath.cc/item/def-pullback-of-a-differential-form)

[F6] Let $a<b$ and $c<d$. If $f,h:[a,b]\times[c,d]\to\mathbb R$ are continuous and $\partial_xf(x,s)=h(x,s)$ for every $x\in(a,b)$ and $s\in[c,d]$, then $G(x)=\int_c^d f(x,s)\,ds$ is differentiable on $[a,b]$ with $G^{\prime}(x)=\int_c^d h(x,s)\,ds$; at the endpoints the derivatives are relative and one-sided. [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle)

### Proof

**Given:** The manifold, surface, fields, flows, and hypotheses in the Statement, with the set-theoretic convention A1 for the inherited smooth structures and fields.

**Goal:** Establish the boost, mixed-component vanishing, and normalized invariant normal.

1.1 For $p\in S$, the constant curve at $p$ is an integral curve of $K$ because $K_p=0$. Uniqueness makes $\Phi_t(p)=p$ throughout the interval on which the flow at $p$ is defined. Since the flow fixes every point of $S$, differentiating its restriction to $S$ gives $d\Phi_t|_pX=X$ for $X\in T_pS$. [F2, given]

1.2 For the circle average, the flow law makes $\phi_s$ a diffeomorphism with inverse $\phi_{-s}$. Because it preserves $S$ and $g$, each transported vector in the integrand is normal to $S$ at $p$; it is future timelike by the stated cone preservation. In a future orthonormal frame at $p$, each such vector has time component $a(s)>|b(s)|$, where $b(s)$ denotes its spatial components. Continuity on $[0,2\pi]$ gives a positive minimum of $a(s)-|b(s)|$; the triangle inequality for integrals therefore gives $\bar a>|\bar b|$. Thus the average is future timelike and, by linearity, normal. [F1, F4, given, algebra]

1.3 Put $V(s,p)=d\phi_s|_{\phi_{-s}(p)}n_{\phi_{-s}(p)}$. Smoothness of the action and $n$ makes the components $V^a(s,x)$ smooth jointly in $s$ and the slice coordinates $x$ on $S$, with the output expressed in one ambient chart around $p$; the moving source point can use different charts. Choose a closed coordinate rectangle $Q$ contained in this slice chart, with $p$ in its interior. On $[0,2\pi]\times Q$ all derivatives of $V^a$ are continuous. Fixing the other coordinates, apply F6 on a compact rectangle in $(x_i,s)$, and repeat for every partial derivative. For each multi-index $\alpha$ this gives $\partial_x^\alpha\bar n^a(x)=(2\pi)^{-1}\int_0^{2\pi}\partial_x^\alpha V^a(s,x)\,ds$ in the interior of $Q$. These derivatives are continuous: their difference at $x,y$ is bounded in absolute value by $\sup_{s\in[0,2\pi]}|\partial_x^\alpha V^a(s,x)-\partial_x^\alpha V^a(s,y)|$, which tends to zero as $y\to x$ by uniform continuity on the compact rectangle. Hence $\bar n$ is smooth near each $p$. [F4, F6, given, algebra]

2.1 Fix $p\in S$ and put $A(t)=d\Phi_t|_p$. Differentiating the flow law at the fixed point gives $A(t+h)=A(h)A(t)$ whenever the times are admissible. In a coordinate chart, differentiating the flow equation at $t=0$ in the initial point gives $A'(0)=DK_p$. The connection term in $\nabla_vK$ vanishes at $p$ because $K_p=0$, so $A'(0)=B_p$. It follows from the flow law that $A'(t)=B_pA(t)$ and $A(0)=I$. [step 1.1, F2, F3]

3.1 The positive definite induced metric gives the direct sum $T_pM=T_pS\oplus(T_pS)^\perp$. Differentiating $A(t)X=X$ from step 1.1 at zero and using step 2.1 gives $B_pX=0$ for $X\in T_pS$. On the normal plane, the stated matrix of $B_p$ has square $\kappa_p^2I$. Let $C(t)$ be the displayed hyperbolic matrix on that plane and extend it to $\widetilde C(t)$ on $T_pM$ by the identity on $T_pS$. Since $B_p$ preserves the normal plane and vanishes on $T_pS$, direct block-matrix differentiation gives $\widetilde C(0)=I$, $\widetilde C^{\prime}(t)=B_p\widetilde C(t)=\widetilde C(t)B_p$, and $\widetilde C(-t)\widetilde C(t)=I$. Thus the full-space product satisfies $\frac{d}{dt}(\widetilde C(-t)A(t))=-\widetilde C(-t)B_pA(t)+\widetilde C(-t)B_pA(t)=0$. Its value at zero is $I$, so $A(t)=\widetilde C(t)$ on the interval of definition. In particular, $A(t)$ preserves the normal plane, where it equals $C(t)$, and is the identity on $T_pS$. [F1, step 1.1, step 2.1, given, algebra]

4.1 Set $v_+=e_0+e_1$ and $v_-=e_0-e_1$. Step 3.1 gives $A(t)v_\pm=e^{\pm\kappa_pt}v_\pm$. For $X\in T_pS$, invariance of $F$, the pullback rule and step 1.1 give $F_p(v_\pm,X)=(\Phi_t^*F)_p(v_\pm,X)=F_p(A(t)v_\pm,A(t)X)=e^{\pm\kappa_pt}F_p(v_\pm,X)$. The flow domain contains an interval about zero, so a nonzero admissible $t$ exists; since $\kappa_p>0$, each exponential factor differs from one. Thus both values vanish, and $v_+,v_-$ span the normal plane. [step 1.1, step 3.1, F5, given, algebra]

5.1 The flow law gives $d\phi_t|_pV(s,p)=V(s+t,\phi_t(p))$. The integrand $V$ is $2\pi$-periodic in $s$, so substitution $u=s+t$ in its full-period integral gives $d\phi_t|_p\bar n_p=\bar n_{\phi_t(p)}$. This uses only $2\pi$-periodicity, so shorter common periods and the identity flow are included. The denominator in the normalization is smooth and strictly positive by step 1.2, and is preserved by the isometries. Consequently $\widehat n$ is smooth, future unit timelike, normal, and invariant. [step 1.2, step 1.3, F2, F4, given, algebra] ∎


## Maxwell algebra supplies timelike and null convergence

[Open item](item-lem-geometric-maxwell-convergence-input) · level 1


### Statement

Assume the Axiom of Choice and let $(M,g,N,o,F)$ be a source-free geometric electrovacuum datum with zero cosmological constant. Put $Q_{ab}=F_{ac}F_b{}^c-\frac14g_{ab}F_{cd}F^{cd}$. Then $Q$ is symmetric and trace-free and obeys the dominant and strong energy conditions: for every future timelike $v$, $-Q^a{}_bv^b$ is future causal or zero, and $(Q_{ab}-\frac12(g^{cd}Q_{cd})g_{ab})v^av^b\ge0$. Consequently $\operatorname{Ric}(n,n)\ge0$ for every unit timelike $n$, and $\operatorname{Ric}(L,L)\ge0$ for every nonzero null $L$.

For such an $L$, its screen is $L^\perp/\mathbb RL$ with the positive quotient metric. If $e_1,e_2\in L^\perp$ represent an orthonormal screen basis, then $\operatorname{Ric}(L,L)=2\sum_{A=1}^2F(L,e_A)^2$. The right side is independent of the representatives. These are conditional tensor identities and inequalities, without a physical interpretation of $F$.

### Facts & Assumptions

**Given:** A datum and vectors as in the Statement.

**Goal:** Establish the energy conditions, both convergence inequalities and the screen formula.

[A1] The Axiom of Choice includes the choice assumptions in the geometric suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The datum has a smooth Lorentzian metric of signature $(-,+,+,+)$, a smooth real two-form $F$, and $\operatorname{Ric}=2Q$. [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data)

[F2] For positive formal parameters, the formal Maxwell tensor satisfies $T^{\mathrm{EM}}_{ab}=\mu_0^{-1}Q_{ab}$. [physics:def-emg-matter-formal-systems](https://alphabetamath.cc/physics/item/def-emg-matter-formal-systems)

[F3] The formal Maxwell tensor is symmetric and trace-free and satisfies the dominant, strong and null energy conditions. [physics:thm-emg-selected-matter-energy-conditions](https://alphabetamath.cc/physics/item/thm-emg-selected-matter-energy-conditions)

[F4] The dominant condition means that the raised negative energy current of every future timelike vector is future causal or zero; the strong condition is nonnegativity on future timelike vectors of the trace-reversed tensor, and the null condition is nonnegativity on future null vectors. [physics:def-emg-pointwise-energy-conditions](https://alphabetamath.cc/physics/item/def-emg-pointwise-energy-conditions)

[F5] For a supplied null geodesic congruence normal to a spacelike two-surface, the screen is $L^\perp/\mathbb RL$ with metric induced by $g$. This supplies the screen convention in that setting; the pointwise extension to arbitrary nonzero null vectors is proved below. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F6] Every symmetric bilinear form on a finite-dimensional real vector space admits a diagonal basis with entries $1,-1,0$, and their respective counts are independent of the basis. [math:thm-sylvesters-law-of-inertia](https://alphabetamath.cc/item/thm-sylvesters-law-of-inertia)

### Proof

**Given:**A datum and vectors as in the Statement.

**Goal:** Establish the energy conditions, both convergence inequalities and the screen formula.

[A1] The Axiom of Choice includes the choice assumptions in the geometric suppliers. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The datum has a smooth Lorentzian metric of signature $(-,+,+,+)$, a smooth real two-form $F$, and $\operatorname{Ric}=2Q$. [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data)

[F2] For positive formal parameters, the formal Maxwell tensor satisfies $T^{\mathrm{EM}}_{ab}=\mu_0^{-1}Q_{ab}$. [physics:def-emg-matter-formal-systems](https://alphabetamath.cc/physics/item/def-emg-matter-formal-systems)

[F3] The formal Maxwell tensor is symmetric and trace-free and satisfies the dominant, strong and null energy conditions. [physics:thm-emg-selected-matter-energy-conditions](https://alphabetamath.cc/physics/item/thm-emg-selected-matter-energy-conditions)

[F4] The dominant condition means that the raised negative energy current of every future timelike vector is future causal or zero; the strong condition is nonnegativity on future timelike vectors of the trace-reversed tensor, and the null condition is nonnegativity on future null vectors. [physics:def-emg-pointwise-energy-conditions](https://alphabetamath.cc/physics/item/def-emg-pointwise-energy-conditions)

[F5] For a supplied null geodesic congruence normal to a spacelike two-surface, the screen is $L^\perp/\mathbb RL$ with metric induced by $g$. This supplies the screen convention in that setting; the pointwise extension to arbitrary nonzero null vectors is proved below. [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F6] Every symmetric bilinear form on a finite-dimensional real vector space admits a diagonal basis with entries $1,-1,0$, and their respective counts are independent of the basis. [math:thm-sylvesters-law-of-inertia](https://alphabetamath.cc/item/thm-sylvesters-law-of-inertia)



1.1 The assumed Axiom of Choice supplies the inherited choice hypotheses when applying [F1], [F2] and [F3]. Choose the formal positive parameters in [F2], for example $\mu_0=c=G_N=1$, and use the same smooth two-form and metric as in [F1]. The smooth field has the regularity required by [F2] and [F3]. Lowering the indices in the formal tensor formula gives $Q=\mu_0T^{\mathrm{EM}}$. Thus $Q$ is symmetric and trace-free. Since multiplication by $\mu_0>0$ preserves nonnegativity and the future causal cone, [F3] and [F4] give the stated dominant and strong conditions for $Q$, as well as $Q(L,L)\ge0$ for future null $L$. [A1, F1, F2, F3, F4, choose, algebra]

1.2 Work at a point, with $V=T_pM$. Normalize the supplied timelike vector to $n=N/\sqrt{-g(N,N)}$. The decomposition $v=-g(v,n)n+(v+g(v,n)n)$ gives $V=\mathbb Rn\oplus n^\perp$ as an orthogonal direct sum. Diagonalize $g|_{n^\perp}$ by [F6] and append $n$; uniqueness of the inertia counts, with the signature in [F1], makes $g|_{n^\perp}$ positive definite. A nonzero null $L$ therefore cannot be orthogonal to $N$, so $a=g(N,L)\ne0$. Put $K=-2N/a+g(N,N)L/a^2$; direct substitution gives $g(K,L)=-2$ and $g(K,K)=0$. [F1, F6, given, construct, algebra]

2.1 Let $P=\operatorname{span}\{L,K\}$ and $E=P^\perp$. The Gram matrix on $P$ is $\left(\begin{smallmatrix}0&-2\\-2&0\end{smallmatrix}\right)$; the vectors $L+K$ and $L-K$ are orthogonal with squared norms $-4$ and $4$. For any $v\in V$, the vector $v+\frac12g(v,K)L+\frac12g(v,L)K$ belongs to $E$. This gives the orthogonal direct sum $V=P\oplus E$, since a vector $bL+cK$ orthogonal to both $L$ and $K$ has $b=c=0$. Thus $E$ has dimension two. Diagonalizing $g|_E$ by [F6] and adjoining the displayed diagonal basis of $P$, uniqueness of inertia and the signature of $g$ show that $g|_E$ has two positive directions and no negative or zero directions. In particular it is positive definite. If $v\in L^\perp$, its $K$ coefficient in this decomposition vanishes, so $L^\perp=\mathbb RL\oplus E$. The form $\bar\gamma([v],[w])=g(v,w)$ is well-defined on $L^\perp/\mathbb RL$, since adding multiples of $L$ to either representative leaves it unchanged. The map $E\to L^\perp/\mathbb RL$, $e\mapsto[e]$, is consequently a linear isometry and bijection. This proves the positive two-dimensional screen assertion for every nonzero null $L$ without any congruence hypothesis. [F1, F6, step 1.2, construct, algebra]

2.2 By trace-freeness, the strong condition gives $Q(v,v)\ge0$ for future timelike $v$. A past timelike or null vector changes to a future vector under negation, while its quadratic contraction is unchanged. Hence $\operatorname{Ric}(n,n)=2Q(n,n)\ge0$ for every unit timelike $n$ and $\operatorname{Ric}(L,L)=2Q(L,L)\ge0$ for every nonzero null $L$. [F1, F4, step 1.1, algebra]

3.1 By [F6], the positive form on $E$ has an orthonormal basis, hence so does the screen by step 2.1. Given any representatives $e_1,e_2$ of an orthonormal screen basis, replace each $e_A$ by $e_A+\frac12g(e_A,K)L$. The replacements preserve the classes and lie in $E$, so are an orthonormal basis of $E$. For these representatives the basis $L,K,e_1,e_2$ therefore has inverse metric $g^{-1}=-\frac12(L\otimes K+K\otimes L)+\sum_Ae_A\otimes e_A$. [F6, step 1.2, step 2.1, construct, algebra]

4.1 Since $F(L,L)=0$, contraction of the inverse metric in step 3.1 gives $F_{ac}L^aF_b{}^cL^b=\sum_AF(L,e_A)^2$. The trace term in $Q(L,L)$ vanishes because $g(L,L)=0$. Therefore $\operatorname{Ric}(L,L)=2\sum_AF(L,e_A)^2$. Replacing any representative by $e_A+tL$ leaves $F(L,e_A)$ unchanged by alternation, proving the claimed representative independence. [F1, step 3.1, algebra] ∎



## The Killing derivative is an exact closed two-form

[Open item](item-lem-author-cea8e61dc3c6-killing-exact-two-form) · level 1


### Statement

For the stationary Lorentzian data, put $\alpha=T^\flat$ and $F_{ab}=\nabla_aT_b$. Then $F_{ab}=-F_{ba}$, $F=\tfrac12d\alpha$ and $dF=0$. Here a two-form has coordinate expansion $F=\tfrac12F_{ab}dx^a\wedge dx^b$.

### Facts & Assumptions

[F1] The metric, Killing field, local flow and torsion-free metric connection are those of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] Exterior differentiation has its coordinate formula and satisfies $d^2=0$. [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove all asserted identities under these hypotheses.

1.1 In a coordinate chart, the derivative of the flow pullback is $(\mathcal L_Tg)_{ab}=T^c\partial_cg_{ab}+g_{cb}\partial_aT^c+g_{ac}\partial_bT^c$. Metric compatibility and symmetry of the Christoffel symbols rewrite this as $\nabla_aT_b+\nabla_bT_a$. The Killing condition makes this sum zero, so $F$ is alternating. [F1, algebra]

2.1 Torsion freedom gives $(d\alpha)_{ab}=\partial_aT_b-\partial_bT_a=\nabla_aT_b-\nabla_bT_a=2F_{ab}$. Applying $d$ once more gives $dF=\tfrac12d^2\alpha=0$. [step 1.1, F1, F2, algebra] ∎

### External input

The cited Killing equation supplies background for the local exactness calculation.


## Vanishing divergence implies closed Hodge dual

[Open item](item-lem-author-cea8e61dc3c6-divergence-hodge-closure) · level 1


### Statement

For the stationary Lorentzian data and a smooth real two-form $U$, $\nabla^aU_{ab}=0$ implies $d(\star_gU)=0$. Thus the word co-closed here means precisely the vanishing-divergence condition, equivalently the displayed Hodge-closure equation.

### Facts & Assumptions

[F1] Use the metric connection and index conventions of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] The real Hodge star and its complex extension are those of [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data).

[F3] The Hodge formula is $(\star_gU)_{ab}=\tfrac12\epsilon_{abcd}U^{cd}$, and exterior differentiation is alternating differentiation. [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[F4] At each point one may choose coordinates with $g_{ab}=\operatorname{diag}(-1,1,1,1)$ and first metric derivatives zero. [physics:thm-gr-point-normal-and-exponential-coordinate-charts](https://alphabetamath.cc/physics/item/thm-gr-point-normal-and-exponential-coordinate-charts)

[F5] In a positively oriented chart the metric volume form is $\epsilon=\sqrt{|\det(g_{ab})|}\,dx^0\wedge dx^1\wedge dx^2\wedge dx^3$; its component array is the positive density times the alternating symbol. [physics:def-gr-metric-volume-form-and-current-flux](https://alphabetamath.cc/physics/item/def-gr-metric-volume-form-and-current-flux)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove all asserted identities under these hypotheses.

1.1 Fix a point $p$ and use [F4], making the chart positively oriented by reversing one spatial coordinate if necessary. The Christoffel symbols and first metric derivatives vanish at $p$. Write $\epsilon$ for the metric volume form of [F5]. Its components are $\sqrt{|\det g|}$ times the alternating symbol. Since the determinant is a polynomial in the metric entries and the square-root function is smooth at $|\det g(p)|=1$, the vanishing of their first derivatives gives $\partial\epsilon(p)=0$. For distinct indices $a,b,c$ let $j$ be the missing fourth index. The Hodge formula gives $(\star_gU)_{bc}=\epsilon_{bcaj}U^{aj}$, with no sum over $a,j$, since the two complementary terms in the half-sum agree. [F1, F2, F3, F4, F5, algebra]

2.1 At $p$, cyclically adding derivatives and using $\partial\epsilon(p)=0$ gives $(d\star_gU)_{abc}=\epsilon_{abcj}(\partial_aU^{aj}+\partial_bU^{bj}+\partial_cU^{cj})=\epsilon_{abcj}\nabla_kU^{kj}$ for distinct $a,b,c$, with only $k$ summed in the last expression; the missing $k=j$ term is zero by antisymmetry. Put $V^j=\nabla_kU^{kj}$. Metric compatibility gives $V^j=g^{jb}\nabla^aU_{ab}$, with $a,b$ summed. Thus vanishing divergence implies $V=0$, and the displayed identity makes every distinct-index component of $d\star_gU$ zero. Repeated-index components vanish by alternation. Since $p$ was arbitrary, $d\star_gU=0$ globally. [step 1.1, F1, F3, F4, algebra]

3.1 Conversely, suppose $d\star_gU=0$. For each $j$ at $p$, choose the other three indices as $a,b,c$. The identity in step 2.1 gives $0=\epsilon_{abcj}V^j$, with no summation here. By [F5] and the normal metric at $p$, $\epsilon_{abcj}=\pm1$, so $V^j=0$ for each $j$. Lowering the free index in $V^j=g^{jb}\nabla^aU_{ab}$ using the nondegenerate metric yields $\nabla^aU_{ab}=g_{bj}V^j=0$, with the contracted indices summed. The point was arbitrary, proving the converse globally and hence the asserted equivalence. [step 1.1, step 2.1, F1, F5, algebra] ∎



## Equivariant homotopy and forced contraction constant

[Open item](item-lem-author-9e1b6fa65528-equivariant-cartan-normalization) · level 1


### Statement

In the relative homotopy construction on $U$, supply a smooth symmetric covariant two-tensor $g$ that is nondegenerate at each point: if $g_q(v,w)=0$ for every $w\in T_qU$, then $v=0$. No dimension or signature restriction is imposed. Suppose commuting isometries of $g$ generated by $K,Z$ preserve $S$ and $\Theta$, $K$ vanishes on $S$, and $Z$ generates a $2\pi$-periodic action. For either flow, the isometry condition for every defined flow map $F$ is $F^*g=g$, equivalently $g_{F(q)}(dF_qv,dF_qw)=g_q(v,w)$ for all $q$ in its domain and $v,w\in T_qU$. Suppose the bundle identification is equivariant for these isometries. Let $T=K-\Omega Z$ for a constant $\Omega$, and let $D$ be smooth with $i_T\Theta=dD$. If the neighborhood is connected and contains $p\in S$ with $T_p=0$, circle averaging of $\beta$ followed by the homotopy gives $\mathcal L_KW=\mathcal L_ZW=\mathcal L_TW=0$ and $W(T)+D=D(p)$. Invariance here means pullback invariance under each defined local flow.

### Facts & Assumptions

[F1] Use the full relative homotopy data, including its ZFC convention, dilation-stable normal-bundle neighborhood, smooth closed two-form $\Theta$, and smooth base one-form $\beta$ with $d\beta=\iota^*\Theta$. Its homotopy formula gives a smooth primitive for every such base form. [lem-author-9e1b6fa65528-relative-normal-homotopy](item-lem-author-9e1b6fa65528-relative-normal-homotopy)

[F2] Here a $2\pi$-periodic action means a smooth global flow $\phi$ of $Z$ on the manifold carrying the supplied action, with $\phi_0=\mathrm{id}$, $\phi_{s+t}=\phi_s\circ\phi_t$, and $\phi_{s+2\pi}=\phi_s$; no least-period condition is imposed. Write $\phi_s$ also for its restriction to the invariant submanifold $S$ when acting on base forms. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) Componentwise integration in a fixed finite-dimensional fibre commutes with fixed linear maps; translation and splitting of scalar integrals make a full-period integral invariant under shifts. Only these general integration properties from the circle-action item's Justification are used here, independently of its normalized Lorentzian action definition. [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[F3] For a smooth vector field $X$ and smooth $k$-form $\omega$ with $k\geq1$, contraction means $(i_X\omega)_q(v_1,\ldots,v_{k-1})=\omega_q(X_q,v_1,\ldots,v_{k-1})$; it is smooth, and for a one-form $W$ it is the scalar $i_XW=W(X)$. Cartan's identity is $\mathcal L_X=d i_X+i_Xd$. Lie derivative means differentiation of pullback by the local flow at parameter zero. [math:def-interior-product-of-a-form-by-a-vector-field](https://alphabetamath.cc/item/def-interior-product-of-a-form-by-a-vector-field) [math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula) [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)

[F4] Pullback evaluates a form on the differential of the map, is smooth and functorial, and satisfies $d(F^*\omega)=F^*(d\omega)$ for smooth maps $F$. [math:def-pullback-of-a-differential-form](https://alphabetamath.cc/item/def-pullback-of-a-differential-form) [math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges](https://alphabetamath.cc/item/prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges) [math:thm-the-exterior-derivative-commutes-with-pullback](https://alphabetamath.cc/item/thm-the-exterior-derivative-commutes-with-pullback)

[F5] For continuous scalar functions on a compact rectangle with a continuous parameter derivative, that derivative passes through the integral. Apply this repeatedly to smooth coefficients in each coordinate variable. The coordinate formula $d(\sum_I a_I dx^I)=\sum_I da_I\wedge dx^I$ then permits exterior differentiation under the parameter integral. [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle) [math:thm-local-coordinate-formula-for-the-exterior-derivative](https://alphabetamath.cc/item/thm-local-coordinate-formula-for-the-exterior-derivative)

[F6] A smooth real function whose differential vanishes is constant on each connected component. [math:prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component](https://alphabetamath.cc/item/prop-a-smooth-function-with-zero-differential-is-constant-on-each-connected-component)

[F7] A smooth vector field has locally unique integral curves through each initial point, depending smoothly on the initial point. Local flows follow these integral curves and satisfy their flow law. Write $\psi_t$ for the local flow of $K$; the commuting-flow hypothesis means $\psi_t\circ\phi_s=\phi_s\circ\psi_t$ wherever both sides are defined. For smooth maps, $d(G\circ F)_q=dG_{F(q)}\circ dF_q$. [math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves](https://alphabetamath.cc/item/thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[F8] A smooth covariant two-tensor is a smooth section of the type $(0,2)$ tensor bundle. For a smooth map $F$, tensor pullback is $(F^*g)_q(v,w)=g_{F(q)}(dF_qv,dF_qw)$. The supplied symmetric nondegenerate tensor in the Statement is the metric preserved by both flows; their isometry condition is exactly this pullback equality, on each defined flow domain. [math:def-smooth-tensor-field](https://alphabetamath.cc/item/def-smooth-tensor-field) [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

### Proof

**Given:** The data and hypotheses in the Statement, with the full relative homotopy data in [F1].

**Goal:** Establish the stated invariant primitive and forced contraction constant.

1.1 Define $\bar\beta=(2\pi)^{-1}\int_0^{2\pi}\phi_s^*\beta\,ds$ as a one-form on $S$, integrating in each fixed cotangent fibre. The pullback definition gives coefficients smooth jointly in $s$ and the base point. On a compact base-coordinate rectangle, [F5] applies successively to every coordinate derivative; their integrals are continuous by uniform continuity on the compact product and the integral bound by interval length times the supremum. Thus $\bar\beta$ is smooth. Commutation with fixed linear coordinate changes makes this a globally defined one-form. Since $\phi_s$ preserves $S$ and $\Theta$, functoriality and commutation of exterior derivative with pullback give $d(\phi_s^*\beta)=\phi_s^*\iota^*\Theta=\iota^*\Theta$. Exterior differentiation under the integral therefore yields $d\bar\beta=\iota^*\Theta$. [F1, F2, F4, F5, given]

2.1 The flow law and functoriality give $\phi_t^*\bar\beta=(2\pi)^{-1}\int_0^{2\pi}\phi_{s+t}^*\beta\,ds=\bar\beta$, since the integrand is periodic and a full-period integral is unchanged by a shift. For each $q\in S$, the constant curve at $q$ is an integral curve of $K$, since $K_q=0$. Uniqueness in [F7], continued on overlapping local time intervals, identifies $\psi_t(q)$ with this curve throughout its defined time interval. Thus the $K$ flow restricts to the identity on $S$ and also preserves $\bar\beta$. Apply [F1] with this averaged base form to obtain the smooth one-form $W=\pi^*\bar\beta+\int_0^1\lambda^{-1}\delta_\lambda^*(i_{\mathcal R}\Theta)\,d\lambda$ with $dW=\Theta$. [F1, F2, F4, F7, step 1.1, given]

3.1 Let $F$ be either symmetry flow map on a domain where it is defined, and let $F_S$ be its restriction to $S$. Equivariance of the supplied bundle identification means that $F$ acts by its induced fibre-linear normal-bundle map: $\pi\circ F=F_S\circ\pi$, $F\circ\delta_\lambda=\delta_\lambda\circ F$, and $dF(\mathcal R)=\mathcal R\circ F$. The pullback definition consequently gives $F^*(i_{\mathcal R}\Theta)=i_{\mathcal R}(F^*\Theta)=i_{\mathcal R}\Theta$. Since $F_S^*\bar\beta=\bar\beta$, functoriality and linearity of the fibre integrals show $F^*W=W$; the smooth extension at $\lambda=0$ is supplied by [F1]. Hence $\mathcal L_KW=\mathcal L_ZW=0$. Differentiating $\psi_t\circ\phi_s=\phi_s\circ\psi_t$ in $s$ at zero using [F7] gives $d\psi_t|_x(Z_x)=Z_{\psi_t(x)}$. For any initial point $q$, set $q(t)=\psi_t(\phi_{-\Omega t}(q))$ on a sufficiently small time interval about zero. The chain rule and the defining integral-curve equations give $q'(t)=K_{q(t)}-\Omega\,d\psi_t|_{\phi_{-\Omega t}(q)}(Z_{\phi_{-\Omega t}(q)})=T_{q(t)}$ at every such $t$, and $q(0)=q$. Uniqueness in [F7] identifies these maps with the local $T$ flow. Both factors preserve $W$, so functoriality gives pullback invariance under that flow; uniqueness continues this invariance throughout each defined local flow, and $\mathcal L_TW=0$. [F1, F2, F3, F4, F7, step 2.1, given]

4.1 Cartan applied to $W$ gives $d(W(T)+D)=\mathcal L_TW-i_TdW+dD=0$, using $dW=\Theta$ and $i_T\Theta=dD$. The scalar $W(T)+D$ is smooth on the connected neighborhood, so [F6] makes it constant there. At the supplied point $p$, $T_p=0$ implies $W_p(T_p)=0$, and its value is therefore $D(p)$. This proves $W(T)+D=D(p)$ together with the asserted invariances. [F3, F6, step 2.1, step 3.1, given] ∎


## Radial primitive and five differentiated decay bounds

[Open item](item-lem-author-9e1b6fa65528-radial-exterior-primitive) · level 1


### Statement

Let $B=\tfrac12B_{ij}\,dx^i\wedge dx^j$ be a closed $C^5$ two-form on $\{|x|>R\}\subset\mathbb R^3$, with $R>0$ and $B_{ij}=O_5(r^{-4})$, $r=|x|$, in the differentiated convention. Define $A_i(x)=-\int_1^\infty sx^jB_{ji}(sx)\,ds$ and $A=A_i\,dx^i$, with repeated spatial indices summed. Then $A$ is $C^5$, $dA=B$, $x^iA_i=0$, and $A_i=O_5(r^{-3})$. If the same differentiated estimates hold at every finite order, the same formula is smooth. The finite-order hypothesis alone is used only for the $C^5$ conclusion.

### Statement references

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[physics:def-cm-finite-regularity-canonical-calculus](https://alphabetamath.cc/physics/item/def-cm-finite-regularity-canonical-calculus)

[math:def-improper-integral-at-infinity](https://alphabetamath.cc/item/def-improper-integral-at-infinity)

### Facts & Assumptions

[F1] The differentiated convention $B_{ij}=O_5(r^{-4})$ supplies a radius $R_1>R$ and constants $C_\beta$ such that $|\partial^\beta B_{ij}(y)|\leq C_\beta|y|^{-4-|\beta|}$ for $|\beta|\leq5$ and $|y|\geq R_1$. It imposes no bound as $|y|$ decreases to $R$. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] A $C^k$ coordinate form has $C^k$ alternating coefficient functions; the exterior derivative is defined by differentiating coefficients and wedging the corresponding coordinate covector. Here closed means $dB=0$, equivalently $\partial_iB_{jk}+\partial_jB_{ki}+\partial_kB_{ij}=0$. These conventions apply on any open Euclidean set, including this three-dimensional exterior. [physics:def-cm-finite-regularity-canonical-calculus](https://alphabetamath.cc/physics/item/def-cm-finite-regularity-canonical-calculus)

[F3] Every integral from $1$ to $\infty$ below denotes the limit of its proper integrals from $1$ to $L$ as $L\to\infty$, when that limit is finite. [math:def-improper-integral-at-infinity](https://alphabetamath.cc/item/def-improper-integral-at-infinity)

[F4] For an open integration domain and one real parameter in an open interval, a continuous integrand with a continuous parameter derivative, an absolutely integrable base slice, and an integrable bound for the derivative uniform on each compact parameter interval has a continuously differentiable integral, with derivative equal to the derivative integral. [math:thm-differentiation-under-dominated-improper-multiple-integrals](https://alphabetamath.cc/item/thm-differentiation-under-dominated-improper-multiple-integrals)

[F5] Continuous real functions on nonempty compact metric spaces are bounded; continuous maps on compact metric spaces are uniformly continuous. [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric) [math:thm-heine-cantor-metric](https://alphabetamath.cc/item/thm-heine-cantor-metric)

[F6] For a function continuous on a closed interval and differentiable inside, a Riemann-integrable extension of its derivative integrates to its endpoint difference. [math:thm-newton-leibniz-with-interior-derivative](https://alphabetamath.cc/item/thm-newton-leibniz-with-interior-derivative)

[F7] A locally Riemann-integrable function dominated in absolute value eventually by a function with a convergent improper integral is absolutely improperly integrable. [math:thm-comparison-test-for-improper-integrals](https://alphabetamath.cc/item/thm-comparison-test-for-improper-integrals)

[F8] For real functions differentiable at a point, sums and products are differentiable there with the sum and product rules. A composition is differentiable when the inner function is differentiable there and the outer function is differentiable at its value, with derivative given by the chain rule. For integers $m\geq1$, $(t^m)'=mt^{m-1}$. [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules)

[F9] A Euclidean map whose partial derivatives exist on a neighborhood and are continuous at a point is totally differentiable there with its Jacobian as derivative. For composable maps totally differentiable at the relevant points, $D(g\circ f)(a)=Dg(f(a))\circ Df(a)$. [math:thm-continuous-partial-derivatives-imply-total-differentiability](https://alphabetamath.cc/item/thm-continuous-partial-derivatives-imply-total-differentiability) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated construction and identities.

1.1 Put $E=\{x:|x|>R\}$ and $h_i(s,x)=sx^jB_{ji}(sx)$. For fixed $s\geq1$, fixing the other two coordinates makes $x^\ell\mapsto B_{ji}(sx)$ a composition of the corresponding one-variable coordinate slice of $B_{ji}$ with $x^\ell\mapsto sx^\ell$. The slice is $C^5$ and the inner map is affine, so [F8] applies successively through five coordinate derivatives, with one factor $s$ per chain-rule differentiation. The product rule also differentiates the factor $x^j$ at most once. Thus, for $|\beta|=k\leq5$, these rules express $\partial_x^\beta h_i$ as a sum of terms of the forms $s^{k+1}x^j(\partial^\beta B_{ji})(sx)$ and, when $k\geq1$, constant multiples of $s^k(\partial^{\beta-e_\ell}B_{\ell i})(sx)$ with $\beta_\ell>0$. Thus, whenever $sr\geq R_1$, each sum is bounded by $C_k r^{-3-k}s^{-3}$. Let $K\subset E$ be nonempty and compact, let $a=\min_K|x|>R$, and choose $S>1$ with $Sa\geq R_1$. On $K\times[1,S]$ the same derivatives are continuous and hence bounded. Enlarging a constant to absorb this finite interval gives $|\partial_x^\beta h_i(s,x)|\leq C_{K,\beta}s^{-3}$ for all $s\geq1$ and $x\in K$. This is a local uniform majorant, not a bound uniform up to the inner boundary. [given, F1, F2, F5, F8]

2.1 Since $\int_1^L s^{-3}\,ds=(1-L^{-2})/2$, the majorant in step 1.1 is integrable. Comparison gives absolute convergence of every integral of $\partial_x^\beta h_i$ for $|\beta|\leq5$. These integrals are jointly continuous in $x$: on a compact neighborhood $K$ the tails beyond $L$ are bounded uniformly by $C_{K,\beta}/(2L^2)$, while the integral over $[1,L]$ is continuous by uniform continuity of its integrand on $K\times[1,L]$ and the estimate of an integral by interval length times the uniform bound. Choose an open rectangular neighborhood with compact closure $K\subset E$. For each $|\beta|\leq4$, fix the other two coordinates and apply [F4] to $\partial_x^\beta h_i$ with each remaining coordinate as the real parameter and integration domain $(1,\infty)$. The integrand and its parameter derivative are continuous, every base slice is absolutely integrable, and step 1.1 supplies an integrable derivative bound on every compact parameter interval. The endpoint $s=1$ is regular and has no effect on the integral. Successively applying this argument gives $\partial_x^\beta A_i(x)=-\int_1^\infty\partial_x^\beta h_i(s,x)\,ds$ for every $|\beta|\leq5$; their joint continuity proves $A\in C^5(E)$. [F3, F4, F5, F6, F7, step 1.1]

3.1 For $r\geq R_1$ the asymptotic estimate in step 1.1 holds for every $s\geq1$, so $|\partial_x^\beta A_i(x)|\leq C_k r^{-3-k}\int_1^\infty s^{-3}\,ds=(C_k/2)r^{-3-k}$. Hence $A_i=O_5(r^{-3})$ in exactly the convention of [F1]. If the hypotheses hold at every finite order, repeat steps 1.1 and 2.1 at each such order, with constants and radii allowed to depend on the order; this yields smoothness of the same integral without an all-order conclusion from the finite-order hypothesis alone. [F1, step 1.1, step 2.1]

4.1 Closedness and antisymmetry give $\partial_iB_{kj}-\partial_jB_{ki}=\partial_kB_{ij}$. The first derivative formula from step 2.1 therefore yields $\partial_iA_j-\partial_jA_i=-\int_1^\infty[2sB_{ij}(sx)+s^2x^k\partial_kB_{ij}(sx)]\,ds$. For fixed $x\in E$, the ray $\gamma_x(s)=sx$ lies in $E$ on the open interval $(R/r,\infty)$ containing $[1,L]$. Its derivative is the vector $x$. The $C^5$ coefficients of $B$ have continuous first partial derivatives, so [F9] makes them totally differentiable and gives $\frac{d}{ds}B_{ij}(sx)=x^k\partial_kB_{ij}(sx)$. The product and power rules in [F8] now identify the integrand as the continuous derivative of the $C^1$ function $s\mapsto s^2B_{ij}(sx)$. On $[1,L]$, [F6] evaluates its integral as $L^2B_{ij}(Lx)-B_{ij}(x)$. The first term tends to zero by [F1], since it is $O(L^{-2}r^{-4})$ as $L\to\infty$ for fixed $x$. Passing to the improper limit gives $\partial_iA_j-\partial_jA_i=B_{ij}(x)$, which is $dA=B$ by [F2]. Finally $x^iA_i=-\int_1^\infty s x^ix^jB_{ji}(sx)\,ds=0$ by antisymmetry and convergence. [F1, F2, F3, F6, F8, F9, step 2.1] ∎


## Stationary exact corrections preserve two prescribed gauges

[Open item](item-lem-author-9e1b6fa65528-stationary-exact-gluing) · level 1


### Statement

Let $(M,g,T)$ be stationary Lorentzian data and let $E\subset M$ be open, equipped with the restricted smooth charts of $M$. Only the smooth manifold and field $T$ enter the construction. A stationary region in $E$ means an open subset invariant under the local flow of $T|_E$ wherever that flow is defined. A smooth differential form $\alpha$ is stationary when $\mathcal L_T\alpha=0$, and a smooth function $h$ is stationary when $Th=0$. Closed and exact mean respectively $d\alpha=0$ and $\alpha=d\beta$ for a smooth form $\beta$ of one lower degree.

On $E$ let $\Theta$ be a smooth closed two-form, $D$ a smooth function, $c\in\mathbb R$, and $V$ a smooth stationary one-form with $dV=\Theta$ and $V(T)+D=c$. For $j\in\{H,\infty\}$ let $U_j\subset E$ be disjoint stationary regions, and let $V_j$ be smooth stationary one-forms on $U_j$ with $dV_j=\Theta|_{U_j}$ and $V_j(T)+D=c$. Assume that every smooth closed one-form on each $U_j$ is exact. Supply smooth stationary functions $\eta_j:E\to[0,1]$ with $\operatorname{supp}_E\eta_j\subset U_j$ and $\eta_j=1$ on prescribed open subsets $P_j\subset U_j$, where $\operatorname{supp}_E\eta_j$ is the closure in $E$ of $\{\eta_j\ne0\}$. Then there exist smooth stationary functions $h_H,h_\infty$ on $E$ such that $W=V+dh_H+dh_\infty$ is stationary, $dW=\Theta$, $W(T)+D=c$, and $W|_{P_j}=V_j|_{P_j}$. Thus the corrections are globally exact stationary one-forms and both prescribed gauges are retained.

For the boundary-extension conclusion, let $S\subset\partial_M E$ be a smooth embedded two-sphere in $M$, with $\partial_M E$ the topological boundary. Suppose there is an open neighborhood $O\subset M$ of $S$ with $O\cap E\subset P_H$ and a smooth one-form $\overline V_H$ on $O$ agreeing with $V_H$ on $O\cap E$. Then $W$ extends smoothly to $E\cup O$ by $\overline V_H$ on $O$. Every specified local symmetry $\mathcal L_X\overline V_H=0$ for a smooth field $X$ on $O$ is inherited by the extension on $O$. This includes stationarity on $O$ if $X=T|_O$ is among these fields; no symmetry in the cutoff transition regions is asserted.

### Facts & Assumptions

[F1] The stationary Lorentzian interface supplies the ambient smooth manifold $M$ and smooth field $T$. Open subsets carry canonical restricted smooth structures, independently of the presenting atlas; these are used for $E$, $U_j$, $P_j$, $O$, $O\cap E$ and $E\cup O$. Regions use the local-flow convention, without a completeness assumption. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure](https://alphabetamath.cc/item/prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F2] Smooth forms and their Lie derivatives have the usual alternating-tensor meanings; stationarity of forms is explicitly defined in the Statement by vanishing Lie derivative. [math:def-smooth-differential-k-form](https://alphabetamath.cc/item/def-smooth-differential-k-form) [math:def-lie-derivative-of-a-differential-form](https://alphabetamath.cc/item/def-lie-derivative-of-a-differential-form)

[F3] Closed means exterior derivative zero and exact means an exterior derivative of a smooth form. Exactness of every closed one-form on each $U_j$ is an explicit hypothesis, not inferred from stationarity. [math:def-closed-and-exact-differential-forms](https://alphabetamath.cc/item/def-closed-and-exact-differential-forms)

[F4] Support is the closure of the nonzero locus, as in the smooth partition-of-unity convention. The supplied cutoffs are required to be stationary; neither their existence nor this extra property is deduced from a partition-of-unity definition. [math:def-smooth-partition-of-unity-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-partition-of-unity-on-a-manifold-with-boundary) [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

[F5] For a smooth scalar $a$ and field $Y$, $da(Y)=Ya$. [math:prop-exterior-derivative-of-a-function-is-its-differential](https://alphabetamath.cc/item/prop-exterior-derivative-of-a-function-is-its-differential)

[F6] The exterior derivative is local and satisfies $d^2=0$. [math:prop-the-exterior-derivative-is-local](https://alphabetamath.cc/item/prop-the-exterior-derivative-is-local) [math:thm-the-exterior-derivative-squares-to-zero](https://alphabetamath.cc/item/thm-the-exterior-derivative-squares-to-zero)

[F7] Cartan's formula is $\mathcal L_Y\alpha=d(\iota_Y\alpha)+\iota_Y(d\alpha)$. [math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula)

[F8] The boundary in the extension clause is the topological boundary in $M$, and $S$ is an embedded smooth submanifold that is a two-sphere with its usual smooth structure. These hypotheses do not identify all of $\partial_M E$ with $S$ or assert that $E\cup S$ is a manifold with boundary. [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top) [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart) [math:ex-the-n-sphere-with-its-standard-smooth-atlas](https://alphabetamath.cc/item/ex-the-n-sphere-with-its-standard-smooth-atlas)

[F9] A smooth vector field $X$ acts on smooth functions by the product rule $X(ab)=aXb+bXa$. [math:prop-a-vector-field-acts-as-a-derivation-of-smooth-functions](https://alphabetamath.cc/item/prop-a-vector-field-acts-as-a-derivation-of-smooth-functions)

### Proof

**Given:** The smooth data, exactness assumptions, cutoffs and, for the last conclusion, the ambient neighborhood and extension in the Statement.

**Goal:** Construct the exact corrections, retain both gauges and normalization, and glue the asserted local extension.

1.1 For each $j\in\{H,\infty\}$, the one-form $V_j-V|_{U_j}$ is closed because its exterior derivative is $\Theta|_{U_j}-\Theta|_{U_j}=0$. Exactness on $U_j$ supplies a smooth scalar $\chi_j$ with $d\chi_j=V_j-V|_{U_j}$. The equal contraction constants give $T\chi_j=d\chi_j(T)=V_j(T)-V(T)=0$ on $U_j$. This requires no choice of a normalization for $\chi_j$ and no completeness of $T$. [given, F1, F3, F5]

2.1 Define $h_j=\eta_j\chi_j$ on $U_j$ and $h_j=0$ on $E\setminus U_j$. Every point of $E\setminus U_j$ lies outside the closed set $\operatorname{supp}_E\eta_j$, so it has an open neighborhood in $E$ on which $\eta_j=0$. On that neighborhood the two definitions of $h_j$ agree identically with zero, proving smoothness across the edge of $U_j$. On $U_j$, the directional product rule gives $Th_j=(T\eta_j)\chi_j+\eta_jT\chi_j=0$; elsewhere it follows from the same local zero description. Thus $dh_j(T)=0$ globally. Also $d(dh_j)=0$, and Cartan's formula yields $\mathcal L_T(dh_j)=d(dh_j(T))+\iota_Td(dh_j)=0$. Hence each correction is exact and stationary. [given, F1, F2, F4, F5, F6, F7, F9, step 1.1]

3.1 Put $W=V+dh_H+dh_\infty$. By step 2.1 it is smooth and stationary, $dW=dV=\Theta$, and $W(T)+D=V(T)+D=c$. On $P_j$ the function $h_j$ equals $\chi_j$ on an open set, so locality gives $dh_j=d\chi_j$ there. The other correction vanishes on $U_j$, since its support lies in the disjoint region. Consequently $W=V+d\chi_j=V_j$ on $P_j$. This proves both prescribed gauge identities without altering the normalization. [given, F1, F2, F4, F6, step 1.1, step 2.1]

4.1 In the boundary-extension setting, $O\cap E\subset P_H$, so step 3.1 gives $W=V_H=\overline V_H$ on the entire open overlap $O\cap E$. Define $\widetilde W=W$ on $E$ and $\widetilde W=\overline V_H$ on $O$. The overlap equality makes this well-defined. Every point has an open neighborhood on which it is one of these smooth forms, so it is smooth on $E\cup O$. On $O$ it is exactly $\overline V_H$, and therefore has every stipulated symmetry $\mathcal L_X\overline V_H=0$ there. This proves the extension and symmetry conclusion on an actual neighborhood of the sphere. [given, F1, F2, F8, step 3.1] ∎


## Regular bifurcate null horizon data before rigidity

[Open item](item-def-author-254b7c4bab6d-regular-null-horizon-pair) · level 1


### Definition

Use the smooth Lorentzian metric, time orientation and Levi–Civita connection conventions of the stationary Lorentzian data, but supply no stationary Killing field for the horizon construction. Work in their inherited ZFC conventions. Let $S$ be an embedded spacelike surface diffeomorphic to the unit sphere in $\mathbb R^3$. Its induced positive metric is denoted $\gamma$. Use the null-screen conventions for null normals, spacelike sections and expansions.

Curves and reachability use the causal-curve interface: curves are continuous and locally absolutely continuous in smooth charts, with nonzero future or past causal, respectively timelike, velocity almost everywhere. For a chosen open neighborhood $O$ of $S$, let $J_O^+(S)$ consist of $S$ and all endpoints of future causal curves from $S$ on compact parameter intervals, with the entire curve contained in $O$; let $I_O^+(S)$ use future timelike curves with distinct parameter endpoints and without adjoining $S$. Define $J_O^-(S)$ and $I_O^-(S)$ by past-directed curves. Thus $S$ is included in each causal set by the reflexive endpoint convention. An affinely parametrized geodesic is a smooth curve $c$ satisfying $D_\lambda c'=0$ for the supplied connection; a null generator has nonzero null velocity. Included parameter endpoints have the one-sided derivative convention.

A regular bifurcate null horizon pair near $S$ consists of $O$ and two smooth embedded null hypersurfaces $H_1,H_2\subset O$ without boundary in $O$, intersecting transversely exactly in $S$ and generated by null geodesics orthogonal to $S$. Transverse means $T_pH_1+T_pH_2=T_pM$ for $p\in S$; null means that the restriction of $g$ to each hypersurface tangent space has a one-dimensional radical, the tangent vectors orthogonal to every vector of that tangent space. Each generator meets $S$ exactly once in this neighborhood and is taken on a connected affine-parameter interval with that intersection in its interior. Choose parameter zero there and increasing to the future. Define $H_i^+$ and $H_i^-$ as the unions of the nonnegative and nonpositive parameter portions of these generators, respectively. Each includes $S$, and $H_i=H_i^+\cup H_i^-$ with $H_i^+\cap H_i^-=S$. Only the signs, not any affine scale, enter these subsets.

The local causal-boundary requirement is the following pair of set identities, with all causal curves confined to $O$:

$$\partial_O J_O^+(S)=J_O^+(S)\setminus I_O^+(S)=H_1^+\cup H_2^+.$$

$$\partial_O J_O^-(S)=J_O^-(S)\setminus I_O^-(S)=H_1^-\cup H_2^-.$$

Here $\partial_O A$ is the boundary relative to $O$: every neighborhood in $O$ of such a point meets both $A$ and $O\setminus A$. These are the future and past half-branches, joined along $S$; each $H_i$ itself is a full smooth sheet through $S$. Require each full $H_i$ to be achronal in $O$, meaning that no two of its points are joined by a timelike curve contained in $O$. These conditions are hypotheses on the supplied branches, not assertions that an arbitrary sphere has such extensions. They concern the causal sets computed in $O$, without asserting equalities for causal sets computed in the ambient $M$.

For a smooth nonzero null generator $L_i$ on a branch and tangent vectors $X,Y$ to a transverse spacelike section $Q$, put $\chi_i(X,Y)=g(\nabla_XL_i,Y)$ and $\theta_i=\operatorname{tr}_{\gamma_Q}\chi_i$, where $\gamma_Q=g|_{TQ}$ is the section metric (equal to $\gamma$ on $S$). Call the pair non-expanding when $\theta_i=0$ everywhere on each full branch, including both half-branches and $S$. When generator fields are only locally chosen this means the condition in each such chart. No Killing generator, periodic symmetry, surface gravity, or rigidity conclusion is assumed.

### Definition references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[math:def-geodesic-of-an-affine-connection](https://alphabetamath.cc/item/def-geodesic-of-an-affine-connection)

[physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[Alexakis–Ionescu–Klainerman, local horizon setup, §§1–2](https://arxiv.org/pdf/0902.1173v1)

### Facts & Assumptions

[F1] The Lorentzian supplier fixes the ambient metric, time orientation and connection; the null-screen supplier defines spacelike sections, null normals, null second fundamental forms and their traces. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F2] The causal-curve supplier fixes locally absolutely continuous causal and timelike curves, their time direction, and the reachability endpoint conventions. Apply it to the open submanifold $O$ with the restricted metric and time orientation. [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[F3] The geodesic supplier defines affine geodesics by vanishing covariant acceleration, including the one-sided convention at an included endpoint. The generator hypothesis additionally requires a nonzero null velocity. [math:def-geodesic-of-an-affine-connection](https://alphabetamath.cc/item/def-geodesic-of-an-affine-connection)

[F4] The independent AIK setup uses full sheets with signed affine parameters and local future/past quadrants. The exact source passage and the limits of this definitional use are recorded in the External input section and the source reference.

### Justification

**Given:** The supplied sphere, branches and ambient data in the Definition.

**Goal:** Explain the conditional data and their relative causal-boundary meaning without assuming a Killing generator.

1.1 Embeddedness, transversality and the radical condition are conditions on the indicated tangent spaces. The positive section metric permits its inverse and the trace in the definition of expansion. The affine generator condition uses the supplied connection and geodesic equation. Thus each derivative and contraction has the supplied Lorentzian and null-screen meaning. [given, F1, F3]

2.1 The causal sets use the curve class on the restricted spacetime $O$, including the stated endpoint convention. Future-directed affine parameters based at $S$ define the two halves of each supplied generator; positive affine rescaling preserves their signs. The displayed relative-boundary identities are explicit hypotheses on these subsets, not a theorem deduced from smoothness and transversality. Achronality uses the same curve class in $O$. [given, F2, F3, step 1.1]

3.1 The full-sheet convention matches the geometric setup recorded in F4, while the displayed identities specify exactly which future and past pieces are required. The expansion condition is a pointwise trace equation on both halves and at $S$. Neither these equations nor the set conditions assert existence of a Killing field. This supplies the pre-rigidity data without using a rigidity conclusion as a premise or claiming that arbitrary supplied sheets satisfy the boundary identities. [given, F1, F2, F3, F4, step 1.1, step 2.1] ∎

### External input

Only the geometric sheet/parameter convention is taken from [AIK, §§1–2, especially (2.11)](https://arxiv.org/pdf/0902.1173v1). The displayed boundary equalities specify that convention as conditional data here. The justification is local definitional bookkeeping; no existence or rigidity theorem is imported by this item.


## Positive Harrison denominator and its parameter identity

[Open item](item-lem-author-7a3c9628f105-denominator-positivity) · level 1


### Statement

On an open domain $U$ in stationary Lorentzian data, let $\sigma=f+i\psi$ be a smooth complex scalar, where $f=-g(T,T)$ and $\psi:U\to\mathbb R$ is real-valued and smooth. Assume stationarity: both $f$ and $\psi$ are constant along each local integral curve of $T$ contained in $U$. Let $0\le q\le1$ and set $D_q=|1+q-(1-q)\sigma|^2$. If $f<1$ on a region $E\subseteq U$, then $D_q>0$ there for every $q$; in particular this applies when $E$ is an exterior region. If $S\subseteq U$ is a compact embedded surface with $f\le0$ on $S$, there is an open neighborhood $O\subseteq U$ of $S$, independent of $q$, with $D_q>0$ on $O$. Moreover $D_q=(1-q)^2D_0+4q(1-(1-q)f)$, and at a point $p\in U$ with $T(p)=0$, $D_q(p)=(1-q)^2D_0(p)+4q>0$.

### Facts & Assumptions

[F1] The smooth metric, Killing field, local flow and real scalar $f=-g(T,T)$ use [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). The local integral curves in the stationarity assumption are the trajectories of that local flow.

[F2] A scalar value $z=a+ib$ has real coordinates $a,b$ and squared modulus $|z|^2=a^2+b^2$. These scalar operations, including real and imaginary parts, use [math:def-complex-conjugate-real-imaginary-part-and-modulus](https://alphabetamath.cc/item/def-complex-conjugate-real-imaginary-part-and-modulus).

[F3] An embedded surface means an embedded two-dimensional smooth submanifold, with the subspace topology inherited from the ambient manifold, as in [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart).

[F4] Smooth real scalar functions on $U$ are smooth maps to $\mathbb R$; the smooth-map definition includes continuity on $U$. [math:def-c-r-and-smooth-maps-between-smooth-manifolds](https://alphabetamath.cc/item/def-c-r-and-smooth-maps-between-smooth-manifolds)

[F5] For a continuous map and an open neighborhood $V$ of its value at a point, there is an open neighborhood of the point mapped into $V$. [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)

### Proof

**Given:** The hypotheses in the Statement and the mathematical interfaces in [F1]–[F5].

**Goal:** Establish both positivity claims and the parameter identity, including positivity at a zero of $T$.

1.1 Write $a_q=\operatorname{Re}(1+q-(1-q)\sigma)=1+q-(1-q)f=2q+(1-q)(1-f)$. At any point with $f<1$, this is positive: at $q=0$ it is $1-f>0$, and at $q>0$ its first summand is positive and its second is nonnegative. Since $\psi$ is real-valued, $D_q=a_q^2+(1-q)^2\psi^2\ge a_q^2>0$. This proves positivity on $E$. [given, F1, F2, algebra]

1.2 Using the squared-modulus formula, subtract $(1-q)^2D_0$ from $D_q$. The $\psi^2$ terms cancel, leaving $(1+q-(1-q)f)^2-(1-q)^2(1-f)^2$. Its factorization is $2q\cdot 2(1-(1-q)f)=4q(1-(1-q)f)$, which proves the stated identity for every $q$. [given, F2, algebra]

2.1 Set $O=\{x\in U:f(x)<1\}$. Continuity of $f$ shows that $O$ is open: for each $x\in O$, apply [F5] to the open real interval $(-\infty,1)$ to obtain an open neighborhood of $x$ in $U$ contained in $O$. Because $U$ is open in the ambient manifold, these neighborhoods are also ambient open. The inequality $f\le0$ on $S$ gives $S\subseteq O$. This $O$ is independent of $q$, and step 1.1 gives $D_q>0$ throughout $O$ for every $q\in[0,1]$. In particular the asserted neighborhood exists for the compact embedded surface with its inherited topology; compactness is not needed by this explicit construction. [given, F3, F4, F5, step 1.1]

3.1 If $T(p)=0$, then $f(p)=0$. Step 1.2 gives $D_q(p)=(1-q)^2D_0(p)+4q$, while [F2] gives $D_0(p)=1+\psi(p)^2$ and $D_q(p)=(1+q)^2+(1-q)^2\psi(p)^2\ge1$. This establishes positivity also at both parameter endpoints and completes all the claims. [given, F1, F2, algebra, step 1.2] ∎

### Source notes

The denominator and parameter formulas are attributed to Radu, Section 3.1 (3.5), (3.7), and Section 3.2 (3.17). The proof here is a local calculation; the explicit neighborhood in step 2.1 replaces the source's compactness argument. No existence of a stationary primitive or Einstein–Maxwell solution is inferred from this calculation.


## Scope of smooth field equations at an exterior horizon boundary

[Open item](item-lem-author-7a3c9628f105-exterior-boundary-scope) · level 1


### Statement

Work in ZFC. Let $M$ be an oriented smooth Hausdorff second-countable four-manifold without boundary, let $E,O\subset M$ be open, and put $U=E\cup O$. Let $g_q$ be smooth time-oriented Lorentzian metrics of signature $(-,+,+,+)$ on $U$, with specified smooth timelike time-orientation fields $N_q$, and let $F_q$ be smooth real two-forms on $U$. Use the restricted orientation of $M$ for every Hodge star, and take $\overline E$ in $M$. If for fixed $q$ the source-free geometric electrovacuum equations hold on $E$, their tensor residuals vanish at every point of $O\cap\overline E$. Smooth extension alone does not imply those equations on $O\setminus\overline E$.

### Facts & Assumptions

[F1] Smooth Lorentzian metrics, their connections and Ricci tensors use [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). Only those tensor conventions are needed; no stationary symmetry is required.

[F2] The source-free geometric electrovacuum equations, their oriented Hodge star and stress tensor are those of [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data). The orientation and the time-orientation fields specified in the Statement supply that interface's geometric data. Its choice convention is included in ZFC; the equations are mathematical conditions, not adopted physical laws here.

[F3] The closure $\overline E$ is the intersection of the closed subsets of $M$ containing $E$, hence is contained in each such closed set. Its complement is open. [math:def-interior-closure-boundary-top](https://alphabetamath.cc/item/def-interior-closure-boundary-top)

[F4] The standard flat function is $\beta(s)=\exp(-1/s)$ for $s>0$ and $\beta(s)=0$ for $s\le0$. It is smooth on $\mathbb R$, positive for $s>0$, and all its derivatives vanish at zero. [math:def-the-standard-flat-function](https://alphabetamath.cc/item/def-the-standard-flat-function) [math:thm-the-standard-flat-function-is-smooth-and-flat-at-zero](https://alphabetamath.cc/item/thm-the-standard-flat-function-is-smooth-and-flat-at-zero)

### Proof

**Given:** The hypotheses in the Statement and the tensor conventions in [F1] and [F2].

**Goal:** Prove vanishing on $O\cap\overline E$ and establish the stated non-implication on its open complement.

1.1 Fix $q$. The residuals are $dF_q$, $d(\star_{g_q}F_q)$, and the covariant two-tensor with components $R_{ab}=\operatorname{Ric}(g_q)_{ab}-2((F_q)_{ac}(F_q)_b{}^c-\tfrac14(g_q)_{ab}(F_q)_{cd}(F_q)^{cd})$. Their components are continuous in every smooth chart in $U$. Indeed the inverse of the smooth nondegenerate matrix $g_q$ is smooth, its oriented volume density and Hodge map are smooth, and the Christoffel and Ricci formulas use at most two derivatives of $g_q$. All contractions and exterior derivatives therefore produce smooth tensor components. [given, F1, F2]

1.2 To establish non-implication, use $M=\mathbb R^4$ with coordinates $(t,x,y,z)$ and orientation $dt\wedge dx\wedge dy\wedge dz$, take $E=\{x<0\}$ and $O=M$, and choose the constant family $g_q=-dt\otimes dt+dx\otimes dx+dy\otimes dy+dz\otimes dz$, $N_q=\partial_t$, $F_q=\beta(x)\,dx\wedge dy$. By [F4] the two-forms are smooth across $x=0$, and the metrics are smooth, nondegenerate and Lorentzian everywhere. Their coefficients are constant, so their Christoffel symbols and Ricci tensors vanish. On $E$, $F_q=0$ and all the electrovacuum equations hold. [F1, F2, F4]

2.1 Let $p\in O\cap\overline E$. If a residual were nonzero at $p$, some component $r$ in a chart in $U$ containing $p$ would satisfy $r(p)\ne0$. Continuity gives an open neighborhood $W$ of $p$ in that chart with $|r|>|r(p)|/2$. Since $U$ is open in $M$, $W$ is open in $M$. The equations on $E$ imply $W\cap E=\varnothing$, so the closed set $M\setminus W$ contains $E$. By [F3] it contains $\overline E$, contradicting $p\in W\cap\overline E$. Thus every residual vanishes at $p$. This proof uses the defining closed-set property of closure directly. [given, F3, step 1.1]

3.1 In this example $\overline E=\{x\le0\}$: this closed set contains $E$, and every neighborhood of a point with $x=0$ intersects $E$, since its coordinate image is open. At a point with $x>0$ put $b=\beta(x)>0$. The only independent nonzero field component is $(F_q)_{xy}=b$, and raising spatial indices leaves it unchanged. Hence $(F_q)_{cd}(F_q)^{cd}=2b^2$ and $(F_q)_{tc}=0$, so the prescribed right-hand side of the $tt$ Ricci equation is $2(0-\tfrac14(-1)2b^2)=b^2>0$, whereas $\operatorname{Ric}(g_q)_{tt}=0$. Thus the Einstein equation fails throughout the nonempty open complement $O\setminus\overline E=\{x>0\}$ despite smooth extension across the boundary and validity on $E$. This supplies the asserted non-implication without weakening the boundary conclusion. [F1, F2, F3, F4, step 1.2] ∎

### Source notes

The cited independent source supplies construction context only: Proposition 3.1 states exterior equations, and Appendix A.2 treats null stationary-field points. Neither passage is used to prove the general boundary statement or the counterexample above; both arguments here are locally authored.


## Ernst sublevels and the Mars–Simon tensor interface

[Open item](item-def-author-9f9c6144aed8-ernst-mars-simon) · level 1


### Definition

Use the stationary Lorentzian data, metric connection and index conventions, together with the complex self-dual-form conventions. Let $F_{ab}=\nabla_aT_b$, $\mathcal F=F+i\star F$, and $\mathcal F^2=\mathcal F_{ab}\mathcal F^{ab}$ without conjugation. For a complex two-form $U+iV$ with real $U,V$, use the interior product extended complex linearly: $\iota_T(U+iV)=\iota_TU+i\iota_TV$, so $(\iota_T\mathcal F)_b=T^a\mathcal F_{ab}$.

As normalization data, choose $R_0>0$ and a smooth embedding $e:\{x\in\mathbb R^3:|x|>R_0\}\to M$. Its image is the chosen parametrized spatial end, with radial coordinate $r(e(x))=|x|$. This end datum specifies where the limit is taken and imposes no metric decay conditions. For this interface an **Ernst potential** is a supplied smooth complex scalar $\sigma$ satisfying $d\sigma=2\iota_T\mathcal F$, normalized by $\sigma\to1$ along this end. Precisely, for every $\varepsilon>0$ there is $R>R_0$ such that $|\sigma(e(x))-1|<\varepsilon$ for all $|x|>R$, uniformly in angular direction. Existence of the end datum and of such a potential is supplied, not proved here.

On the open set $N=\{1-\sigma\ne0\}$ define $P=(1-\sigma)^{-1}$ and $y=\operatorname{Re}P$. Write $\epsilon=\mathrm{vol}_g$ for the oriented metric volume tensor: in every positively oriented coordinate chart, $\mathrm{vol}_g=\sqrt{|\det(g_{ab})|}\,dx^0\wedge dx^1\wedge dx^2\wedge dx^3$. Use the same orientation for this tensor and the Hodge star. Write $R_{ab cd}$ for the curvature convention used in the cited source; let $\mathcal R_{ab cd}=R_{ab cd}+\frac i2\epsilon_{cd}{}^{ef}R_{ab ef}$ and $\mathcal I_{ab cd}=(g_{ac}g_{bd}-g_{ad}g_{bc}+i\epsilon_{ab cd})/4$. The **Mars–Simon tensor in the IK convention** is $\mathcal S_{ab cd}=\mathcal R_{ab cd}+6(1-\sigma)^{-1}(\mathcal F_{ab}\mathcal F_{cd}-\mathcal F^2\mathcal I_{ab cd}/3)$. Curvature and orientation conventions must be transported together when applying this formula.

### Definition references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[math:def-interior-product-of-a-form-by-a-vector-field](https://alphabetamath.cc/item/def-interior-product-of-a-form-by-a-vector-field)

[physics:def-gr-metric-volume-form-and-current-flux](https://alphabetamath.cc/physics/item/def-gr-metric-volume-form-and-current-flux)

[math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding)

### Justification

The Killing equation makes $F$ alternating, using [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). The supplied self-dual-form interface [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data) defines the complex contractions. The real interior product in [math:def-interior-product-of-a-form-by-a-vector-field](https://alphabetamath.cc/item/def-interior-product-of-a-form-by-a-vector-field) is smooth and inserts $T$ into the first slot; its complex-linear extension is well defined because the real and imaginary parts are unique. The end embedding, in the sense of [math:def-smooth-embedding](https://alphabetamath.cc/item/def-smooth-embedding), makes $\sigma\circ e$ a specified function on a Euclidean exterior; the quantified limit is therefore a predicate on the supplied data, rather than an assertion that stationary geometry provides an end or a normalized potential.

Clause (a) of [physics:def-gr-metric-volume-form-and-current-flux](https://alphabetamath.cc/physics/item/def-gr-metric-volume-form-and-current-flux) supplies the smooth normalized metric volume form on an oriented Lorentzian four-manifold. Raising its indices uses the given inverse metric. On $N$ the smooth nonzero denominator permits the reciprocal and tensor formula, so they define smooth fields there. This construction does not assert a wave equation, vanishing or a Kerr characterization.

Appendix A.3 of Ionescu–Klainerman, printed p. 54, fixes $R_{ab cd}=g(e_a,\nabla_{e_c}\nabla_{e_d}e_b-\nabla_{e_d}\nabla_{e_c}e_b-\nabla_{[e_c,e_d]}e_b)$. This is the curvature operator of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) with its output index lowered: in a coordinate frame $R_{ab cd}=g_{ae}R^e{}_{bcd}$. Thus the imported convention agrees with that supplier without a sign reversal or slot permutation.

### External input

Ionescu–Klainerman supplies the displayed definition formulas in §4.2–§4.3, printed pp. 22–24, and the reciprocal potential in §7, equation (7.3), printed p. 35. Appendix A.3, printed p. 54, supplies the curvature convention compared above. Its normalization is at infinity along the chosen section. The embedding and quantified angularly uniform limit above specify that convention locally. Only definitions are adopted from the source's vacuum setting; no potential-existence or analytic theorem is inferred.


## Differentiated stationary end bounds imply the weighted Hölder interface

[Open item](item-lem-author-9e5789a3d617-end-holder-interface) · level 1


### Statement

Fix a stationary chart with $X=\partial_t$ on $r=|x|>R$, metric components $g_{\mu\nu}=\eta_{\mu\nu}+O_{k+1}(r^{-\alpha})$, $k\geq2$, $0<\alpha\leq1$, and Minkowski matrix $\eta=\operatorname{diag}(-1,1,1,1)$. Here the asymptotic coefficient of $X$ means the constant $A$ in an expansion $X=(A+a)\partial_t+\sum_{i=1}^3 b^i\partial_{x^i}$ with $a,b^i=O_0(r^{-\alpha})$. Then after increasing $R$, $g_{00}<-1/2$, $g_{ij}v^iv^j\geq|v|^2/2$, $X$ is uniformly timelike and its asymptotic coefficient is $A=1$. Moreover for any $0<\lambda\leq1$, every order-$k$ coordinate derivative $q$ of a metric component satisfies $|q(t,x)-q(\tau,y)|\leq C r^{-\alpha-k-\lambda}(|t-\tau|^\lambda+|x-y|^\lambda)$ when $|x-y|\leq r/2$ and $|t-\tau|\leq1$, where $r=|x|$. These are the local quantitative end inequalities; end gluing and global causality remain separate conditions.

### Facts & Assumptions

[F1] Stationary fields, charts and metric components have the specified geometric meanings. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] Differentiated decay controls Cartesian derivatives uniformly in angle. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F3] If $f:[a,b]\to\mathbb R$ is continuous on $[a,b]$, differentiable on $(a,b)$, $a<b$, and $|f'|\leq M$ there for a finite $M\geq0$, then $|f(b)-f(a)|\leq M(b-a)$. [math:thm-mean-value-inequality](https://alphabetamath.cc/item/thm-mean-value-inequality)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated quantitative end inequalities and coefficient.

1.1 Fix a common radius $R_1$ beyond which the differentiated decay bounds hold, and increase the final $R$ so that $R>2R_1$ and every component of $g-\eta$ has absolute value at most $1/6$ for $r>R$. Then $g_{00}\leq-5/6<-1/2$ and $|\sum_{ij}(g_{ij}-\delta_{ij})v^iv^j|\leq\tfrac16(\sum_i|v^i|)^2\leq|v|^2/2$. Thus $g_{ij}v^iv^j\geq|v|^2/2$. Since $X=\partial_t$, its squared norm is $g_{00}$, so it is uniformly timelike. [given, F1, F2]

1.2 The local flow of $X=\partial_t$ translates $t$ and fixes $x$. Its preservation of $g$ makes the metric components independent of $t$; hence derivatives containing a time derivative vanish, and purely spatial derivatives are independent of $t$. The identity $X=\partial_t$ gives the defined expansion with $A=1$ and $a=b^i=0$. In any such expansion, its time component gives $1-A=a=O_0(r^{-\alpha})$; since $\alpha>0$, the right side tends to zero as $r\to\infty$, so the constant $A$ is uniquely $1$. [given, F1, F2]

2.1 Let $q$ be a purely spatial order-$k$ derivative of a metric component. Join $x$ to $y$ by changing their three coordinates one at a time. Every point $z$ on these coordinate segments satisfies $|z-x|\leq|y-x|\leq r/2$, so $|z|\geq r/2>R_1$. The next differentiated bound gives $|\partial_iq(z)|\leq C r^{-\alpha-k-1}$ on all three segments. On each nondegenerate coordinate interval the restriction of $q$ is $C^1$, and its one-variable derivative is the corresponding partial derivative. Apply [F3] on that interval; zero-length intervals contribute zero. Telescoping the three differences yields $|q(x)-q(y)|\leq C r^{-\alpha-k-1}\sum_{i=1}^3|y^i-x^i|\leq\sqrt3 C r^{-\alpha-k-1}|x-y|$. [given, F2, F3, step 1.1]

3.1 If $x\ne y$, then for $0<\lambda\leq1$ one has $|x-y|^{1-\lambda}\leq(r/2)^{1-\lambda}$, and the preceding bound is at most $C' r^{-\alpha-k-\lambda}|x-y|^\lambda$. For $x=y$ the difference is zero. Purely spatial derivatives have no time dependence, and derivatives containing a time derivative are zero. Adding the nonnegative term $C' r^{-\alpha-k-\lambda}|t-\tau|^\lambda$ therefore gives the claimed estimate for every order-$k$ coordinate derivative when $|t-\tau|\leq1$. [given, step 1.2, step 2.1] ∎


## A complete stationary flow preserves its compact tangent boundary

[Open item](item-lem-author-9e5789a3d617-compact-boundary-flow) · level 1


### Statement

Let $X$ have a complete smooth flow $\phi_t$ on $M$, and let $S\subset M$ be a compact embedded submanifold without boundary with $X_p\in T_pS$ for every $p\in S$. Then $\phi_t(S)=S$ for every real $t$. This requires tangency, not vanishing of $X$ on $S$, and does not assert that $S$ is a Killing bifurcation surface.

### Facts & Assumptions

[F1] A global flow has integral curves through each initial point and satisfies $\phi_0=\operatorname{id}$ and $\phi_t\circ\phi_s=\phi_{t+s}$; hence $\phi_{-t}$ is its inverse. An integral curve solves $\gamma\prime(t)=X_{\gamma(t)}$. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:def-integral-curve-of-a-vector-field](https://alphabetamath.cc/item/def-integral-curve-of-a-vector-field)

[F2] A stationary field is a smooth Killing field; its completeness is an additional hypothesis. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F3] An embedded submanifold has slice charts and the subspace topology. Compactness of $S$ means that every cover by open subsets of $S$ has a finite subcover. [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart) [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[F4] A smooth ambient vector field tangent to an embedded submanifold restricts to a smooth vector field on that submanifold. [math:prop-a-vector-field-tangent-to-an-embedded-submanifold-restricts-to-a-vector-field](https://alphabetamath.cc/item/prop-a-vector-field-tangent-to-an-embedded-submanifold-restricts-to-a-vector-field)

[F5] For a smooth vector field on a manifold, every point has an open neighborhood $U$ and a number $h>0$ with a smooth solution map on $(-h,h)\times U$, giving the unique integral curve for each initial point in $U$. [math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves](https://alphabetamath.cc/item/thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves)

[F6] Through each point of a manifold, a smooth vector field has a unique maximal integral curve. [math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove $\phi_t(S)=S$ for every real $t$.

1.1 If $S$ is empty the conclusion holds immediately. Otherwise tangency and [F4] give a smooth vector field $Y=X|_S$ on the boundaryless manifold $S$. By [F5], the open subsets of $S$ admitting a solution map on some interval $(-h,h)$ form an open cover of $S$. Use intrinsic compactness in [F3] to take a finite subcover $U_1,\ldots,U_N$, with corresponding maps $\Psi_j:(-h_j,h_j)\times U_j\to S$ and $h_j>0$, and put $h=\min_j h_j>0$. Every point of $S$ therefore has a solution for $Y$ on $(-h,h)$. [given, F3, F4, F5]

2.1 Fix $p\in S$ and let $\gamma:(a,b)\to S$ be its maximal integral curve for $Y$, with $\gamma(0)=p$, supplied by [F6]. If $b<\infty$, choose $t_0\in(a,b)$ with $b-t_0<h$ and a $U_j$ containing $\gamma(t_0)$. The curve $t\mapsto\Psi_j(t-t_0,\gamma(t_0))$ is defined on $(t_0-h_j,t_0+h_j)$ and agrees with $\gamma$ on the overlap by uniqueness in [F5], applied at their common time $t_0$. Gluing extends $\gamma$ beyond $b$, contradicting maximality. If $a>-\infty$, choose $t_0$ with $t_0-a<h$ and use the same map for negative time to extend past $a$. Thus $a=-\infty$ and $b=\infty$. [F5, F6, step 1.1]

3.1 Viewed in $M$, each such restricted curve solves the ambient equation: in a slice chart its tangential derivatives are the components of $Y$, while its normal coordinates are zero, and tangency makes these derivatives exactly the components of $X$. It is therefore an ambient integral curve through $p$ by [F1]. Ambient uniqueness in [F5] and [F6] identifies it with $t\mapsto\phi_t(p)$ for every real $t$. Hence $\phi_t(S)\subseteq S$. Applying the same inclusion to $-t$ and using the inverse identity in [F1] gives $S\subseteq\phi_t(S)$, and consequently $\phi_t(S)=S$. [given, F1, F3, F4, F5, F6, step 2.1] ∎


## Isometries preserve maximality and transported boundary

[Open item](item-lem-author-9e5789a3d617-maximal-isometry-covariance) · level 1


### Statement

Let $\phi:M\to M$ be a time-orientation-preserving isometry of $(M,g)$, meaning a diffeomorphism satisfying $\phi^*g=g$ whose differential maps future timelike vectors to future timelike vectors, and let $\widehat\Sigma$ be a smooth embedded spacelike hypersurface with boundary $S$. With the future unit normal and convention $k(U,V)=-g(\nabla_U n,V)$, the induced metric and second fundamental form on $\phi(\widehat\Sigma)$ pull back to those of $\widehat\Sigma$. Consequently maximality $\operatorname{tr}_h k=0$ is preserved, and the transported boundary is $\phi(S)$. In particular a complete stationary flow preserving $S$ preserves the boundary and maximality of every translate.

### Facts & Assumptions

[F1] Stationary Lorentzian data supply the smooth metric $g$, time-orientation field $N$, Killing condition $\mathcal L_Tg=0$, and the unique torsion-free metric-compatible Levi–Civita connection. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] The future unit normal, induced metric, second fundamental form and maximality use the stated hypersurface convention. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) An embedded smooth hypersurface with boundary is supplied with a manifold-with-boundary smooth structure for which its inclusion into the ambient manifold is a smooth embedding. [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)

[F3] Diffeomorphism pushforward preserves Lie brackets of smooth vector fields. [math:cor-diffeomorphism-pushforward-preserves-lie-brackets](https://alphabetamath.cc/item/cor-diffeomorphism-pushforward-preserves-lie-brackets)

[F4] A diffeomorphism between smooth manifolds with boundary maps their intrinsic boundaries onto one another. [math:cor-diffeomorphisms-preserve-interior-and-boundary](https://alphabetamath.cc/item/cor-diffeomorphisms-preserve-interior-and-boundary)

[F5] A smooth vector field has a unique smooth maximal flow satisfying the flow composition law; completeness makes its domain all of $\mathbb R\times M$. [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows) [math:prop-a-vector-field-is-complete-if-and-only-if-its-flow-is-global](https://alphabetamath.cc/item/prop-a-vector-field-is-complete-if-and-only-if-its-flow-is-global)

[F6] The mean value theorem implies that a smooth real function with zero derivative on an interval is constant. [math:cor-mean-value-theorem](https://alphabetamath.cc/item/cor-mean-value-theorem)

[F7] In each Lorentzian tangent space the timelike vectors have exactly two connected components, both convex, with the orthonormal-coordinate descriptions independent of basis up to interchange. Thus a linear Lorentzian isometry permutes these components, and a continuous timelike path stays in one component. [physics:lem-timelike-cone-has-two-convex-components](https://alphabetamath.cc/physics/item/lem-timelike-cone-has-two-convex-components)

[F8] For a smooth map $F:P\to Q$ and a covariant two-tensor $A$ on $Q$, the pullback is defined by $(F^*A)_p(u,v)=A_{F(p)}(dF_pu,dF_pv)$. [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

[F9] A smooth map between manifolds with boundary is an immersion when its differential on each full tangent space is injective, and an embedding when it is also a homeomorphism onto its image. No neatness, properness, closed-image or boundary-preservation condition is included. [math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-immersion-and-embedding-for-manifolds-with-boundary)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish covariance of the induced data, boundary transport and the stationary-flow specialization.

1.1 Write $\phi_*U=d\phi\circ U\circ\phi^{-1}$ and define the pulled-back connection by $D_UV=\phi_*^{-1}(\nabla_{\phi_*U}\phi_*V)$. The connection rules and metric compatibility pull back through the isometry, so $D$ is a metric-compatible connection for $g$. By bracket preservation its torsion is $D_UV-D_VU-[U,V]=\phi_*^{-1}(\nabla_{\phi_*U}\phi_*V-\nabla_{\phi_*V}\phi_*U-[\phi_*U,\phi_*V])=0$. Uniqueness therefore gives $D=\nabla$. [given, F1, F3, F8]

1.2 Give $\phi(\widehat\Sigma)$ the transported smooth structure: if $x$ is a boundary or interior chart on $\widehat\Sigma$, its image chart is $x\circ\phi^{-1}$. Its inclusion into $M$ is the original embedding followed by the ambient diffeomorphism $\phi$, so it is a smooth embedding, and the restriction $\phi:\widehat\Sigma\to\phi(\widehat\Sigma)$ is a diffeomorphism of manifolds with boundary. Intrinsic boundary preservation now gives $\partial(\phi(\widehat\Sigma))=\phi(\partial\widehat\Sigma)=\phi(S)$. [given, F2, F4, F9]

1.3 For the specialization let $\Phi_t$ be the flow of the complete stationary field $T$. It is global and smooth, and $\Phi_{t+h}=\Phi_h\circ\Phi_t$ with $\Phi_t^{-1}=\Phi_{-t}$, so each $\Phi_t$ is a diffeomorphism. Differentiating $\Phi_{t+h}^*g=\Phi_t^*(\Phi_h^*g)$ at $h=0$ gives $\frac{d}{dt}\Phi_t^*g=\Phi_t^*(\mathcal L_Tg)=0$. For fixed $p,U,V$ each evaluation $(\Phi_t^*g)_p(U,V)$ is a smooth real function of $t$. The mean value theorem on the interval joining $0$ and $t$ makes it constant, hence $\Phi_t^*g=g$ for every $t$. This calculation does not require $T$ to be nonzero. [given, F1, F5, F6, F8]

2.1 Put $\Sigma^{\prime}=\phi(\widehat\Sigma)$. The differential takes each tangent space onto that of the image, and metric invariance makes the image spacelike. Since $\phi$ preserves time orientation, $d\phi(n)$ is its future unit normal $n^{\prime}$. Consequently $h^{\prime}(d\phi U,d\phi V)=h(U,V)$ and $k^{\prime}(d\phi U,d\phi V)=-g(\nabla_{d\phi U}n^{\prime},d\phi V)=-g(\nabla_U n,V)=k(U,V)$. Tracing in an $h$-orthonormal basis and its $d\phi$ image gives equal metric traces, so maximality is preserved. These identities hold up to the boundary with the supplied smooth structure. [given, F1, F2, F8, step 1.1]

3.1 Fix $p$ and define $w_s=(d\Phi_s|_p)^{-1}N_{\Phi_s(p)}\in T_pM$. Smoothness and the isometry identity make $s\mapsto w_s$ a continuous timelike path, with $w_0=N_p$. It stays in the future component of the timelike set of $T_pM$. The linear isometry $d\Phi_s|_p$ permutes the two timelike components and maps $w_s$ to the future vector $N_{\Phi_s(p)}$; it therefore maps the future component onto the future component. Thus every $\Phi_s$ preserves time orientation. Applying steps 2.1 and 1.2 to $\phi=\Phi_s$, and using the hypothesized setwise invariance $\Phi_s(S)=S$, proves the claimed boundary and maximality assertions for every translate. [given, F1, F5, F7, step 2.1, step 1.2, step 1.3] ∎


## Stationary graph translation preserves source asymptotics

[Open item](item-lem-author-9e5789a3d617-graph-decay-translation) · level 1


### Statement

Let $k$ be a nonnegative integer, $R_0>0$, $E=\{x\in\mathbb R^3:r=|x|>R_0\}$, and $u\in C^{k+1}(E;\mathbb R)$. In a stationary end chart $V\subseteq\mathbb R\times E$, suppose $\Gamma_u=\{(u(x),x):x\in E\}\subseteq V$ is a hypersurface graph. Write $\mathcal D\subseteq\mathbb R\times M$ for the domain of the stationary flow $\phi$, with coordinate law $\phi_a(t,x)=(t+a,x)$ whenever the flow is defined and both points lie in $V$. Fix $s\in\mathbb R$ such that $(s,p)\in\mathcal D$ and $\phi_s(p)\in V$ for every $p\in\Gamma_u$. Then $\phi_s(\Gamma_u)$ is the graph $t=u(x)+s$ over the same $E$.

If $0<\alpha\leq1$ and $|u|+\sum_{j=1}^{k+1}r^j|\partial^j u|\leq Cw_\alpha(r)$ on $E$, where $C\geq0$ is finite, $w_\alpha(r)=(1+r)^{1-\alpha}$ for $\alpha<1$ and $w_1(r)=1+\log(1+r)$, then the fixed translate obeys the same bound with $C+|s|$ in place of $C$. Here $\partial^j u$ denotes the finite array of order-$j$ Cartesian derivatives, with its Euclidean norm. For $1\leq j\leq k+1$ and $0<\lambda\leq1$, any additionally imposed finite weighted Hölder bound on $\partial^j u$ is unchanged: on every annulus $A_R=\{R<|x|<2R\}\subseteq E$, the seminorm $[v]_{\lambda;A_R}=\sup_{x\ne y\in A_R}|v(x)-v(y)|/|x-y|^\lambda$ is identical for $v=\partial^j(u+s)$ and $v=\partial^j u$. Finiteness of the relevant Hölder seminorms is an additional hypothesis, not a consequence of the stated $C^{k+1}$ regularity. These source-type bounds do not force $u\to0$ or even convergence to a finite constant.

### Facts & Assumptions

[F1] Chart derivative bounds and weighted Hölder estimates have their fixed-coordinate meaning. The formula in the Statement also specifies the endpoint exponent $\lambda=1$. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] A local flow has a domain $\mathcal D$; the translation law and the conditions that the chosen $s$ is defined on all of $\Gamma_u$ and its image remains in $V$ are explicit hypotheses here, not consequences of the flow definition. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F3] A hypersurface is an embedded submanifold of codimension one; $\Gamma_u$ is assumed to be such a hypersurface in the chart. [math:def-codimension-and-hypersurface](https://alphabetamath.cc/item/def-codimension-and-hypersurface)

[F4] If $f:[a,b]\to\mathbb R^m$ is continuous on $[a,b]$, differentiable on $(a,b)$, $a<b$, and $|f'(t)|\leq M$ there for a finite $M\geq0$, then $|f(b)-f(a)|\leq M(b-a)$. [math:thm-mean-value-inequality](https://alphabetamath.cc/item/thm-mean-value-inequality)

[F5] For every $\varepsilon>0$, $\log t/t^\varepsilon\to0$ as $t\to+\infty$. [math:thm-logarithm-slower-than-every-positive-power](https://alphabetamath.cc/item/thm-logarithm-slower-than-every-positive-power)

### Proof

**Given:** The chart, graph, flow-domain conditions, regularity and estimates in the Statement.

**Goal:** Establish graph translation, preservation of the estimates and the absence of forced finite limiting height.

1.1 For every $x\in E$, the domain and containment hypotheses permit use of the coordinate law at $(u(x),x)$, giving $\phi_s(u(x),x)=(u(x)+s,x)$. As $x$ ranges over $E$, these are exactly the points of the translated graph. All derivatives of positive order through $k+1$ remain the same, and $|u+s|\leq|u|+|s|$. Since $w_\alpha\geq1$, replacing $C$ by $C+|s|$ proves the claimed bound, while derivative Hölder differences, their seminorms and any fixed radius weights are identical. [F1, F2]

2.1 On $E=\{r>1\}$, the smooth function $u(x)=\log r$ is unbounded, but $r^j|\partial^j u|$ is bounded for every fixed $j\geq1$: the first derivatives are homogeneous of degree $-1$, further differentiation lowers that degree, and their angular factors are smooth on the unit sphere. Also $|u|\leq w_1(r)\leq C_\alpha w_\alpha(r)$ for $\alpha<1$: apply [F5] with $\varepsilon=1-\alpha>0$ and $t=1+r$. Choose $T\geq2$ so that $\log t\leq t^\varepsilon$ for $t\geq T$. There $1+\log t\leq2t^\varepsilon$; for $2<t\leq T$, $1+\log t\leq1+\log T\leq(1+\log T)t^\varepsilon$. Thus $C_\alpha=\max\{2,1+\log T\}$ suffices. For completeness, if $v=\partial^j u$ and $x,y\in A_R$ with $|x-y|\leq R/2$, the connecting segment stays at radius at least $R/2$. For distinct $x,y$, the finite derivative array $f(t)=v(x+t(y-x))$, $0\leq t\leq1$, is smooth and has $|f'(t)|\leq C_jR^{-j-1}|x-y|$ by the next-derivative bound. Applying [F4] on $[0,1]$ gives $|v(x)-v(y)|\leq C_jR^{-j-1}|x-y|$; for $x=y$ the inequality is immediate. If $|x-y|>R/2$, the individual derivative bounds give $|v(x)-v(y)|\leq C_jR^{-j}$. Consequently $[\partial^j u]_{\lambda;A_R}\leq C_{j,\lambda}R^{-j-\lambda}$ for $0<\lambda\leq1$ and $R\geq2$. This supplies the corresponding weighted Hölder control, including that at the highest derivative order. Thus the displayed growth class does not imply zero height or a finite limiting height; this is a statement about the estimate, not a spacetime counterexample. [F1, F4, F5, step 1.1] ∎


## Complete regular static exterior data and its normalized end

[Open item](item-def-author-f247c641a714-regular-static-exterior-data) · level 1


### Definition

Regular static exterior data consist of a connected oriented three-manifold $\overline X$ with nonempty compact smooth boundary $B$, a positive-definite metric $h$ and real function $V$ which are smooth on $X=\overline X\setminus B$ and at least $C^2$ on $\overline X$. Require $V>0$ on $X$, $V=0$ and $dV\ne0$ on $B$. Completeness up to boundary means completeness of the intrinsic $h$-distance on $\overline X$, with boundary included. A single asymptotically Euclidean end means that the complement of a compact subset of $\overline X$ is diffeomorphic to $\{x\in\mathbb R^3:r=|x|>R_0\}$, with no additional ends or deleted interior boundary. In that chart require $h_{ij}-\delta_{ij}=O_2(r^{-1})$ and $V=1-m/r+O_2(r^{-2})$ for a real number $m$ not initially assumed positive.

The associated globally static spacetime exterior is $\mathbb R_t\times X$ with $g=-V^2dt^2+h$, future orientation $\partial_t$ and stationary field $T=\partial_t$. The boundary $B$ is a boundary of the spatial data; this product formula does not define a nondegenerate Lorentzian metric at $V=0$. Write $D$ for the Levi–Civita connection of $h$, $D^2V(A,C)=A(CV)-(D_AC)V$ for its Hessian and $\Delta_hV=\operatorname{tr}_hD^2V$ for its Laplacian.

### Definition references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)

[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)

### Facts & Assumptions

[F1] Stationary Lorentzian data supply the standing ZFC convention, including the axiom of choice, together with the metric, time-orientation, Killing-field and connection conventions for the smooth interior product. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] The differentiated end notation $O_2$ means uniform Cartesian derivative bounds through order two for each fixed datum. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F3] On the smooth interior the Laplace–Beltrami operator is the metric trace of the Levi–Civita Hessian, with sign $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)

[F4] Smooth manifold-with-boundary charts take values in relatively open subsets of a half-space; smooth transitions are understood by local extension. [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)

[F5] Intrinsic distance uses the infimum of lengths of piecewise $C^1$ connecting curves. The same length formula is specified below for the present $C^2$ boundary metric; its metric property is proved locally rather than imported from a smooth-metric theorem. [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)

[F6] Completeness up to boundary means Cauchy completeness of the intrinsic distance with boundary points included. This agrees with the terminology for embedded smooth spacelike sections, but the abstract $C^2$ boundary case here is justified below. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F7] Future causal curves are locally absolutely continuous and have nonzero future causal velocity almost everywhere; consequently they are nonconstant on every nondegenerate parameter subinterval. [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[F8] A smooth function $u$ is temporal when its gradient satisfies $g(\nabla u,\nabla u)<0$ and $du(N)>0$ for the chosen future timelike orientation field $N$. [physics:def-gr-causal-conditions-and-global-hyperbolicity](https://alphabetamath.cc/physics/item/def-gr-causal-conditions-and-global-hyperbolicity)

[F9] Assuming Countable Choice and Dependent Choice, a temporal function composed with any future causal curve in [F7] is locally absolutely continuous, has positive derivative almost everywhere and is strictly increasing between parameter values on every nonconstant subinterval. [physics:lem-gr-temporal-functions-and-time-functions](https://alphabetamath.cc/physics/item/lem-gr-temporal-functions-and-time-functions)

[F10] The axiom of choice implies Dependent Choice and Countable Choice, so the standing ZFC convention in [F1] supplies both choice hypotheses of [F9]. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

### Justification

**Given:** The data in the Definition and the interfaces in [F1]–[F10].

**Goal:** Justify the object and completeness conventions without asserting an extension across a horizon.

1.1 Use the smooth boundary charts of [F4] and their interior counterparts. For a piecewise $C^1$ curve $\gamma:[a,b]\to\overline X$, set $L_h(\gamma)=\int_a^b\sqrt{h_{\gamma(s)}(\dot\gamma(s),\dot\gamma(s))}\,ds$, summed over its finitely many $C^1$ pieces, and define $d_h(p,q)$ as the infimum of these lengths for curves joining $p$ to $q$, as in [F5]. Small coordinate balls or half-balls are convex, so any two points in one such chart neighborhood can be joined by a smooth coordinate segment. For fixed $p$, the set reachable from $p$ by finitely many such segments is open; its complement is open by the same local segment property. Connectedness therefore makes every point reachable. Each finite piece has finite length by continuity of $h$ on its compact trace. Thus each infimum is finite and nonnegative, using only continuity of $h$ up to $B$. [given, F4, F5]

1.2 The compact-core/end-chart requirement is a global topological condition, not a consequence of pointwise estimates. The differentiated $O_2$ notation fixes all Cartesian derivatives up to second order and is uniform in angular directions for each fixed datum. On the smooth interior the trace-of-Hessian definition fixes the sign of $\Delta_h$ and agrees with $\operatorname{div}_h\operatorname{grad}_h$. [given, F2, F3]

2.1 Constant curves give $d_h(p,p)=0$, and reversal preserves length, so $d_h$ is symmetric. Length is additive under concatenation by splitting the defining integrals. Given $\varepsilon>0$, curves from $p$ to $q$ and from $q$ to $r$ with lengths less than the respective infima plus $\varepsilon$ yield $d_h(p,r)\le d_h(p,q)+d_h(q,r)+2\varepsilon$. Letting $\varepsilon$ decrease to zero gives the triangle inequality. [given, step 1.1]

2.2 On $X$ positivity of $V$ gives a smooth nondegenerate product tensor of signature $(-,+,+,+)$; $g(T,T)=-V^2<0$ and its coefficients are independent of $t$. Thus $T$ is Killing, complete on this product, and hypersurface orthogonal since its metric dual is $-V^2dt$. The construction asserts neither regular Lorentzian coordinates at $B$ nor a maximal analytic extension. [given, F1, step 1.2]

3.1 For distinct $p,q$, take a coordinate ball or boundary half-ball centered at $p$, of radius $\rho>0$, whose compact closure lies in the chart and excludes $q$. Continuity and positive definiteness give a positive minimum $c$ of $h_x(v,v)$ over this compact coordinate closure and the Euclidean unit sphere, hence $h_x(v,v)\ge c|v|^2$. Every connecting curve from $p$ to $q$ first exits this relative ball through its spherical boundary; at a boundary chart the flat face lies in the manifold and is not an exit. The coordinate displacement of the initial curve is $\rho$, so integration of its derivative gives $L_h(\gamma)\ge\sqrt c\int|\dot\gamma|\,ds\ge\sqrt c\,\rho$. Taking the infimum proves $d_h(p,q)>0$. Consequently $d_h$ is a metric also at boundary points for the stated $C^2$ data, and completeness means that every $d_h$-Cauchy sequence converges in $\overline X$, with $B$ included, consistently with [F6]. Completeness itself remains a requirement on the data. [given, F4, F6, step 1.1, step 2.1]

4.1 On the smooth interior product take $N=T$. Direct contraction with $g=-V^2dt^2+h$ gives $\nabla t=-V^{-2}T$, hence $g(\nabla t,\nabla t)=-V^{-2}<0$ and $dt(N)=1>0$. Thus $t$ is temporal by [F8]. The standing ZFC convention in [F1] supplies the choice hypotheses of [F9] by [F10]. For every future causal curve $\gamma:I\to\mathbb R_t\times X$ in [F7], the function $t\circ\gamma$ is therefore locally absolutely continuous and has positive derivative almost everywhere by [F9]. Such a curve is nonconstant on every nondegenerate subinterval by [F7], so [F9] gives $t(\gamma(a))<t(\gamma(b))$ whenever $a<b$ in $I$. This proves the claimed strict increase along the declared causal-curve class. [given, F1, F7, F8, F9, F10, step 2.2, algebra] ∎



## Smooth invariant Harrison primitive near the horizon and at infinity

[Open item](item-thm-stationary-harrison-primitive-input) · level 2


### Statement

In the mass-one stationary vacuum construction under the precise Radu GR/SBS and original maximal-slice hypotheses in [F1], define $F=\tfrac12dT^\flat$, $f=-g(T,T)$, $\sigma=f+i\psi$, where $\psi$ is the smooth twist potential on the exterior and a neighborhood of the bifurcation sphere satisfying $d\psi=2i_T\star F$ and $\psi\to0$ as $r\to\infty$, and put $\Theta_0=4((f-1)F+\psi\star F)$ and $D_0=|1-\sigma|^2$. The symbol $\star$ denotes the oriented Lorentzian Hodge star and $T^\flat=g(T,\cdot)$. There exists a smooth stationary real one-form $W_0$ on the exterior and a neighborhood of the bifurcation sphere $S$, with $dW_0=\Theta_0$, locally invariant under the Hawking field $K$ and rotational field $Z$, and satisfying $W_0(T)+D_0=D_0(p)$ at a common zero $p$ of $T,Z$. Here $K=T+\Omega_HZ$, $K|_S=0$ and $Z$ has period $2\pi$. In the fixed stationary end chart, $W_0=(D_0(p)-D_0)dt+(W_0)_i dx^i$ and $(W_0)_i(x)=-\int_1^\infty sx^j(\Theta_0)_{ji}(sx)\,ds=O_5(r^{-3})$. One primitive has both this end gauge and the smooth invariant homotopy gauge near $S$. The local Hawking-field invariance is asserted only where the local field is defined.

### Facts & Assumptions

[F1] Import the exact construction and hypotheses of the sole statement-bearing Radu citation below. In particular, §3.1 (3.2) specifies $d\psi=2i_T\star F$ and $\psi\to0$ as $r\to\infty$; its following paragraph supplies the global smooth potential on $E$ and its smooth extension across the bifurcation sphere. This includes the stationary product $E\simeq\mathbb R\times\Sigma_1$, $\Sigma_1\simeq(1,\infty)\times\mathbb S^2$, the zero-period criterion for exact two-forms, vanishing first cohomology of the end and collar, and the original $q=1$ stationary collar. These are external inputs, not consequences of the definition of a bifurcate Killing horizon.

[F2] Differential forms, stationary fields, bifurcate horizons, self-dual/Hodge conventions, differentiated decay and periodic actions use the declared geometric definitions. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data) [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[F3] Stokes' theorem transfers periods across the compact annulus between homologous spheres. [math:thm-stokes-theorem-for-smooth-singular-chains](https://alphabetamath.cc/item/thm-stokes-theorem-for-smooth-singular-chains)

[F4] The five local intermediate constructions below give the normal homotopy, equivariance and forced normalization, radial finite-order estimate, stationary lifting and exact gauge gluing under their explicit hypotheses. [lem-author-9e1b6fa65528-relative-normal-homotopy](item-lem-author-9e1b6fa65528-relative-normal-homotopy) [lem-author-9e1b6fa65528-equivariant-cartan-normalization](item-lem-author-9e1b6fa65528-equivariant-cartan-normalization) [lem-author-9e1b6fa65528-radial-exterior-primitive](item-lem-author-9e1b6fa65528-radial-exterior-primitive) [lem-author-9e1b6fa65528-stationary-spatial-lifting](item-lem-author-9e1b6fa65528-stationary-spatial-lifting) [lem-author-9e1b6fa65528-stationary-exact-gluing](item-lem-author-9e1b6fa65528-stationary-exact-gluing)

### External input

The smooth Radu construction in [F1] is imported as an established external input with the complete source statement and hypotheses above. Its spatial decay makes the period on $S_r$ tend to zero: the coefficients are $O(r^{-4})$ and the area scales as $r^2$. Closedness and [F3] therefore give zero period on $S$ and on a generator sphere. The source's cohomology criteria provide the base primitive $\beta$ on $S$ and a global spatial primitive. The first two intermediate lemmas then explain the smooth invariant normal-bundle construction and the forced constant at $p$; the fourth lifts the spatial primitive with exactly this constant. The third proves the radial formula and its five derivative bounds. The fifth explains why exact corrections on the end and the original stationary collar preserve the normalization and leave the Hawking symmetry intact near $S$. No global extension of $K$ or $Z$ is required.

### Source notes

The five intermediate lemmas were fully authored before admitting the residual source inputs. This item retains literature-derived proof provenance and is not a claim that all of Radu's geometric or asymptotic analysis has been reconstructed locally. In particular, the radial lemma proves $C^5$ regularity from the recorded $O_5$ bound; smoothness of the chosen radial end form is included in the imported smooth construction, not inferred solely from five derivative bounds. The collar input is the original $q=1$ collar, avoiding dependence on the Harrison electrovacuum construction. Radu's §3.3 derivation of (3.28) uses the original vacuum end and does not require transformed charge formulas. The separate held vacuum Ernst, local rigidity and Harrison electrovacuum items are not logical suppliers here; their applicable inputs are expressly imported from the independently read source. Source reading does not grant Step-7 judgment or establish a defect in the article under study.


## Ricci contraction of the Killing derivative

[Open item](item-lem-author-cea8e61dc3c6-vacuum-killing-divergence) · level 2


### Statement

For stationary Lorentzian data, the Killing two-form obeys $\nabla^aF_{ab}=-\operatorname{Ric}_{bd}T^d$. In particular, if $\operatorname{Ric}=0$, then $\nabla^aF_{ab}=0$. The curvature and Ricci signs are those of the stationary-data definition.

### Facts & Assumptions

[F1] The connection, index conventions, curvature and Ricci contraction are those of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] The Killing derivative is alternating. [lem-author-cea8e61dc3c6-killing-exact-two-form](item-lem-author-cea8e61dc3c6-killing-exact-two-form)

[F3] The curvature has the pair skew-symmetries, pair-exchange symmetry and symmetric Ricci contraction. [physics:thm-gr-curvature-algebraic-symmetries](https://alphabetamath.cc/physics/item/thm-gr-curvature-algebraic-symmetries)

[F4] Import the vector Ricci commutator with the exact convention recorded in the External input; its source is Reall (4.7)–(4.8).

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove all asserted identities under these hypotheses.

1.1 Apply the commutator in [F4] to the scalar pairing $u_cZ^c$ and use the connection product rule. Scalar second derivatives commute by torsion freedom, so the covector formula is $[\nabla_a,\nabla_b]u_c=-R^d{}_{cab}u_d$. Contracting $u=T^\flat$ gives $g^{ac}[\nabla_a,\nabla_b]T_c=\operatorname{Ric}_{bd}T^d$: indeed $g^{ac}R_{ecab}=-g^{ac}R_{ceab}=-\operatorname{Ric}_{eb}$, using the first-pair skew-symmetry and the stated Ricci contraction. [F1, F3, F4, algebra]

2.1 Alternation gives $\nabla^aT_a=0$ and $\nabla^aF_{ab}=-\nabla^a\nabla_bT_a$. Metric compatibility and step 1.1 therefore yield $\nabla^aF_{ab}=-\nabla_b(\nabla^aT_a)-g^{ac}[\nabla_a,\nabla_b]T_c=-\operatorname{Ric}_{bd}T^d$. Under Ricci flatness the right side vanishes. [step 1.1, F1, F2, algebra] ∎

### External input

The vector identity $[\nabla_c,\nabla_d]Z^a=R^a{}_{bcd}Z^b$ and contraction $\operatorname{Ric}_{ab}=R^c{}_{acb}$ are the imported input from Reall (4.7)–(4.8). Its convention matches the stationary-data definition exactly. No sign of a curvature tensor from a different source is transferred implicitly.


## Killing flow preserves its complex two-form

[Open item](item-lem-author-cea8e61dc3c6-killing-flow-invariance) · level 2


### Statement

For stationary Lorentzian data, let $F=\tfrac12dT^\flat$ and $\mathcal F=F+i\star_gF$. Then $\mathcal L_TF=0$ and $\mathcal L_T\mathcal F=0$. These assertions use only local flow maps and do not require a complete flow.

### Facts & Assumptions

[F1] The Killing field and local flow are defined by [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] The complex two-form and complex-linear Hodge convention are those of [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data).

[F3] The Killing derivative equals $\tfrac12dT^\flat$. [lem-author-cea8e61dc3c6-killing-exact-two-form](item-lem-author-cea8e61dc3c6-killing-exact-two-form)

[F4] The Hodge star is uniquely characterized by the wedge pairing and oriented metric volume. [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)

[F5] A local flow satisfies $\Phi_0=\operatorname{id}$ and $\Phi_t\circ\Phi_s=\Phi_{t+s}$ wherever defined, and its time curves have velocity $T$. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F6] For a real covariant tensor $A$, $\mathcal L_TA=\left.\frac{d}{dt}\right|_{t=0}\Phi_t^*A$. For a complex two-form $U+iV$, define pullback and Lie derivative componentwise: $\Phi_t^*(U+iV)=\Phi_t^*U+i\Phi_t^*V$ and $\mathcal L_T(U+iV)=\mathcal L_TU+i\mathcal L_TV$. The unique real and imaginary parts make these extensions well-defined. [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field) [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[F7] On common local flow domains a smooth real tensor is invariant under the flow exactly when its Lie derivative vanishes. [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)

[F8] Exterior differentiation commutes with pullback by every smooth map, in particular by each local flow map. [math:thm-the-exterior-derivative-commutes-with-pullback](https://alphabetamath.cc/item/thm-the-exterior-derivative-commutes-with-pullback)

[F9] Pullback of forms is smooth, functorial and wedge-preserving. [math:prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges](https://alphabetamath.cc/item/prop-pullback-of-forms-is-smooth-functorial-and-preserves-wedges)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove both Lie derivative identities on local flow domains.

1.1 Work on a sufficiently short common local flow domain. The composition law gives $\Phi_{-t}\circ\Phi_t=\operatorname{id}$ and $\Phi_t\circ\Phi_{-t}=\operatorname{id}$ after restriction, so these smooth maps are local diffeomorphisms. Since $\mathcal L_Tg=0$, tensor-flow invariance gives $\Phi_t^*g=g$. Differentiating $\Phi_t(\Phi_s(p))=\Phi_s(\Phi_t(p))$ at $s=0$ gives $d\Phi_t|_p(T_p)=T_{\Phi_t(p)}$. The differential has nonzero determinant and varies continuously from the identity, so these local flow maps preserve orientation. [F1, F5, F7]

2.1 For $v\in T_pM$, step 1.1 gives $(\Phi_t^*T^\flat)_p(v)=g_{\Phi_t(p)}(T_{\Phi_t(p)},d\Phi_t|_p v)=g_p(T_p,v)$. Thus $\Phi_t^*T^\flat=T^\flat$. By naturality of exterior differentiation, $\Phi_t^*F=\tfrac12\Phi_t^*dT^\flat=\tfrac12d(\Phi_t^*T^\flat)=F$, with the same $F$ as the Killing derivative. [step 1.1, F1, F3, F8, algebra]

2.2 An orientation-preserving local isometry preserves the inverse metric pairing on covectors, hence its determinant pairing on exterior powers. It also preserves oriented metric volume: it takes every positive orthonormal frame to a positive orthonormal frame, on which both volume forms have value one. Pull back $\alpha\wedge\star_g\beta=\langle\alpha,\beta\rangle_g\operatorname{vol}_g$. Wedge preservation and these metric identities give $(\Phi_t^*\alpha)\wedge\Phi_t^*(\star_g\beta)=\langle\Phi_t^*\alpha,\Phi_t^*\beta\rangle_g\operatorname{vol}_g$. Since the local diffeomorphism induces an isomorphism on each exterior-power fibre, its pulled-back $\alpha$ range over all forms at each point. Uniqueness in the Hodge characterization therefore gives $\Phi_t^*(\star_g\beta)=\star_g(\Phi_t^*\beta)$. [step 1.1, F4, F9, algebra]

3.1 Apply step 2.2 to $\beta=F$. Step 2.1 and the componentwise complex extension give $\Phi_t^*\mathcal F=\Phi_t^*F+i\Phi_t^*(\star_gF)=F+i\star_gF=\mathcal F$. Differentiating this identity and $\Phi_t^*F=F$ at $t=0$ gives $\mathcal L_T\mathcal F=0$ and $\mathcal L_TF=0$ by the tensor Lie derivative definition and its complex-linear extension. All maps used were local, so no completeness of the flow is assumed. [step 2.1, step 2.2, F2, F6, algebra] ∎



## Rescaling a null generator preserves zero expansion

[Open item](item-lem-author-254b7c4bab6d-null-expansion-rescaling) · level 2


### Statement

For the horizon data of [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair), let $L$ be a local null generator and let $a$ be a smooth positive function on the branch. On any spacelike section the generator $L'=aL$ has $\chi'=a\chi$ and $\theta'=a\theta$. Consequently the zero-expansion condition does not depend on positive normalization. Use the expansion conventions of [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data).

### Facts & Assumptions

[F1] A null generator is orthogonal to every tangent vector of its null hypersurface; the null form and its trace are computed with the unchanged section metric. [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data)

[F2] An affine connection obeys $\nabla_X(fV)=X(f)V+f\nabla_XV$ for smooth $f$ and vector fields $X,V$. Apply this defining rule to the supplied Levi–Civita connection with $f=a$ and $V=L$, restricting the resulting identity to the section. [math:def-affine-connection-on-a-smooth-manifold](https://alphabetamath.cc/item/def-affine-connection-on-a-smooth-manifold)

### Proof

**Given:**The branch, section, $L$ and $a$ in the Statement.

**Goal:** Compute the two rescaled quantities.

1.1 For section tangent vectors $X,Y$, the connection product rule gives $g(\nabla_X(aL),Y)=X(a)g(L,Y)+a g(\nabla_XL,Y)=a\chi(X,Y)$, since $g(L,Y)=0$. [given, F1, F2]

2.1 The section metric has not changed. Taking its trace gives $\theta'=a\theta$; because $a>0$, either expansion vanishes exactly when the other does. [given, F1, step 1.1] ∎


## Null second fundamental form descends to the screen quotient

[Open item](item-lem-author-254b7c4bab6d-null-form-screen-descent) · level 2


### Statement

For a branch in [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair), suppose its smooth generator $L$ is geodesic up to reparametrization, $\nabla_LL=\kappa L$ for a smooth scalar $\kappa$. Then $B(X,Y)=g(\nabla_XL,Y)$ on $TH$ defines a symmetric bilinear form on $TH/\mathbb RL$. Its trace in the positive quotient metric agrees with the expansion computed on every spacelike section transverse to $L$. Thus the expansion uses no preferred section. The quotient and metric conventions are those of [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data), and the connection is as in [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

### Facts & Assumptions

[F1] The null generator spans the radical of the hypersurface tangent metric. Its quotient metric is positive definite, and a transverse spacelike section identifies isometrically with the quotient. The connection is torsion-free and metric-compatible. [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair) [def-null-screen-expansion-and-focal-data](item-def-null-screen-expansion-and-focal-data) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

### Proof

**Given:**The null hypersurface and pregeodesic generator in the Statement.

**Goal:** Establish descent, symmetry and section independence.

1.1 Metric compatibility gives $B(X,L)=\frac12Xg(L,L)=0$. The pregeodesic equation gives $B(L,Y)=\kappa g(L,Y)=0$. For tangent extensions $X,Y$, metric compatibility and $g(L,X)=g(L,Y)=0$ give $B(X,Y)-B(Y,X)=-g(L,\nabla_XY-\nabla_YX)=-g(L,[X,Y])=0$, since $[X,Y]$ is tangent to the hypersurface. Thus $B$ annihilates the kernel in both slots and is symmetric. [given, F1]

2.1 Changing a tangent representative by a multiple of $L$ therefore leaves $B$ unchanged. By the quotient metric and section identification in F1, its trace on the quotient equals its trace in any section representative. The definition of expansion is exactly that trace. [F1, step 1.1] ∎



## A branch-tangent Killing field restricts to the bifurcation sphere

[Open item](item-lem-author-254b7c4bab6d-tangent-killing-restriction) · level 2


### Statement

For the transverse branch pair in [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair), let $T$ be a smooth ambient Killing field tangent to each branch. Then $T|_S$ is tangent to $S$ and is Killing for the Riemannian induced metric $\gamma=g|_{TS}$. Nontriviality on $S$ means $T|_S\not\equiv0$ and allows isolated zeroes. Use the Killing and metric conventions in [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

### Facts & Assumptions

[F1] The horizon pair supplies smooth embedded transverse branches $H_1,H_2$ with intersection the embedded spacelike sphere $S$ and induced positive metric $\gamma=g|_{TS}$. The stationary-data conventions define the ambient Killing equation $\mathcal L_Tg=0$ using the local-flow Lie derivative. [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] For transverse embedded submanifolds, the tangent space of their intersection is the intersection of their tangent spaces. Applied to these branches, $T_pS=T_pH_1\cap T_pH_2$. [math:cor-transverse-intersection-theorem](https://alphabetamath.cc/item/cor-transverse-intersection-theorem)

[F3] A smooth ambient vector field tangent to an embedded submanifold restricts to a smooth vector field on it. [math:prop-a-vector-field-tangent-to-an-embedded-submanifold-restricts-to-a-vector-field](https://alphabetamath.cc/item/prop-a-vector-field-tangent-to-an-embedded-submanifold-restricts-to-a-vector-field)

[F4] An embedded submanifold admits slice charts in which it is the coordinate slice with all normal coordinates zero. [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

[F5] For a smooth covariant two-tensor $h$ and vector field $V$, the local-flow Lie derivative has components $(\mathcal L_Vh)_{ij}=V^k\partial_kh_{ij}+h_{kj}\partial_iV^k+h_{ik}\partial_jV^k$. This formula applies to both $g$ on the ambient manifold and $\gamma$ on $S$; it imposes no signature restriction. [math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor](https://alphabetamath.cc/item/prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor)

### Proof

**Given:** The transverse pair and branch-tangent Killing field.

**Goal:** Establish tangency and the intrinsic Killing equation.

1.1 For $p\in S$, branch tangency gives $T_p\in T_pH_1\cap T_pH_2=T_pS$ by the transverse-intersection theorem. Since $S$ is embedded and $T$ is smooth, the restriction theorem gives a smooth field $A=T|_S$ on $S$. [given, F1, F2, F3]

2.1 Fix $p\in S$ and take a slice chart $(x^1,x^2,x^3,x^4)$ around $p$ with $S$ given by $x^3=x^4=0$. Tangential indices $a,b,c$ range over $1,2$ and normal indices $\mu$ over $3,4$. On the slice, $A^a=T^a|_S$ and $\gamma_{ab}=g_{ab}|_S$. Tangency gives $T^\mu|_S=0$, so differentiating this identically zero function in each tangential coordinate gives $(\partial_aT^\mu)|_S=0$. [F1, F4, step 1.1]

3.1 Apply the covariant two-tensor coordinate formula first on $S$ and then in the ambient chart. With $c$ summed over $1,2$, it gives $(\mathcal L_A\gamma)_{ab}=\left.(T^c\partial_cg_{ab}+g_{cb}\partial_aT^c+g_{ac}\partial_bT^c)\right|_S=\left.(\mathcal L_Tg)_{ab}\right|_S=0$. Indeed, the additional normal-index terms in the ambient formula vanish by $T^\mu|_S=0$ and $(\partial_aT^\mu)|_S=(\partial_bT^\mu)|_S=0$. Thus $\mathcal L_A\gamma=0$ in every such chart, and $A$ is Killing for the induced Riemannian metric. Nontriviality means $A\not\equiv0$ and does not require $A$ to be nowhere zero. [F1, F5, step 1.1, step 2.1] ∎


## Lifting a normalized stationary primitive to the Harrison parameter

[Open item](item-lem-author-7a3c9628f105-primitive-parameter-lift) · level 2


### Statement

Work on an open domain $U$ containing $p$, with $\psi:U\to\mathbb R$ smooth and real-valued, $f=-g(T,T)$, and both $f$ and $\psi$ constant along every local integral curve of $T$ contained in $U$. Assume the stationary Lorentzian and denominator data specified in [F1]–[F2], a real two-form $F=\tfrac12\mathrm dT^\flat$, and a smooth stationary one-form $W_0$ (meaning $\mathcal L_TW_0=0$) with $\mathrm dW_0=4((f-1)F+\psi\star_gF)$ and $W_0(T)=D_0(p)-D_0$, where $T(p)=0$. Define $W_q=(1-q)^2W_0-4q(1-q)T^\flat$ for $q\in[0,1]$. Then $W_q(T)=D_q(p)-D_q$, $\mathrm dW_q=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$, $W_1=0$, and $W_q$ is smooth in spacetime and $q$.

For the decay assertion, take the spatial components in one fixed Cartesian exterior chart $x=(x^1,x^2,x^3)$ with $r=|x|>R_0>0$, and let $T_i$ denote the spatial components of $T^\flat$. Interpret differentiated estimates and parameter uniformity by [F3]. If $(W_0)_i=O_5(r^{-3})$ and $T_i=O_5(r^{-2})$ in this same chart, then $(W_q)_i=O_5(r^{-2})$ uniformly for $q\in[0,1]$.

### Statement references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[lem-author-7a3c9628f105-denominator-positivity](item-lem-author-7a3c9628f105-denominator-positivity)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula)

[math:def-lie-derivative-of-a-differential-form](https://alphabetamath.cc/item/def-lie-derivative-of-a-differential-form)

### Facts & Assumptions

[F1] Stationarity of $(g,T)$ and $T^\flat$ use [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data), and the real two-form and star use [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data). A smooth one-form $\omega$ is called stationary when $\mathcal L_T\omega=0$, with the Lie derivative of a differential form defined in [math:def-lie-derivative-of-a-differential-form](https://alphabetamath.cc/item/def-lie-derivative-of-a-differential-form).

[F2] On the open domain $U$ containing $p$ specified in the Statement, $\sigma=f+i\psi$ is smooth, $f=-g(T,T)$, and $\psi:U\to\mathbb R$ is smooth and real-valued. Both $f$ and $\psi$ are constant along every local integral curve of $T$ contained in $U$. Thus the scalar $D_q=|1+q-(1-q)\sigma|^2$ obeys the polynomial identity of [lem-author-7a3c9628f105-denominator-positivity](item-lem-author-7a3c9628f105-denominator-positivity) on $U$ for $q\in[0,1]$.

[F3] The fixed Cartesian exterior chart, multi-index derivatives, componentwise $O_m(r^{-b})$ bounds and parameter-uniform estimates are those of [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data). Uniformity requires a common radius and derivative constants for every parameter value. Only this fixed-chart notation is used; no existence or coordinate invariance of an end is asserted.

[F4] The operator $\mathrm d$ is the exterior derivative of [math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula). For a smooth real one-form $\omega$ and smooth vector fields $X,Y$, its formula is $(\mathrm d\omega)(X,Y)=X(\omega(Y))-Y(\omega(X))-\omega([X,Y])$.

### Proof

**Given:** The hypotheses in the Statement and the interfaces in [F1]–[F4].

**Goal:** Establish the polynomial identities, smoothness and conditional uniform decay.

1.1 Since $T^\flat(T)=-f$ and $T(p)=0$ gives $f(p)=0$, contraction yields $W_q(T)=(1-q)^2(D_0(p)-D_0)+4q(1-q)f$. Subtract the polynomial identity $D_q=(1-q)^2D_0+4q(1-(1-q)f)$ at the variable point from its value at $p$ to obtain $D_q(p)-D_q$. [given, F1, F2, algebra]

1.2 Expanding the three terms of [F4] for $a\alpha+b\eta$, with real constants $a,b$ and smooth real one-forms $\alpha,\eta$, gives $\mathrm d(a\alpha+b\eta)=a\,\mathrm d\alpha+b\,\mathrm d\eta$: each derivative and evaluation is real-linear in the one-form. With $q$ fixed, the coefficients $(1-q)^2$ and $-4q(1-q)$ are spacetime constants, so this linearity and the given $\mathrm dT^\flat=2F$ give $\mathrm dW_q=4(1-q)^2((f-1)F+\psi\star_gF)-8q(1-q)F$. The coefficient of $F$ simplifies to $4(1-q)((1-q)f-(1+q))$, giving the asserted curl. The defining formula for $W_q$ is polynomial in $q$ with smooth stationary coefficients and gives $W_1=0$. [given, F1, F4, algebra]

2.1 In the chart of the decay assertion, let $\beta$ be any multi-index with $|\beta|\le5$. By [F3] the two input estimates give a common radius $R>\max\{R_0,1\}$ and constants $A_\beta,B_\beta\ge0$ with $|\partial^\beta(W_0)_i|\le A_\beta r^{-3-|\beta|}$ and $|\partial^\beta T_i|\le B_\beta r^{-2-|\beta|}$ for every spatial component and $r\ge R$. These inputs have no $q$ dependence. Since $0\le(1-q)^2\le1$ and $0\le4q(1-q)\le1$ on $[0,1]$, differentiating the defining component formula gives $|\partial^\beta(W_q)_i|\le A_\beta r^{-3-|\beta|}+B_\beta r^{-2-|\beta|}\le(A_\beta+B_\beta)r^{-2-|\beta|}$. The same radius and constants work for all $q\in[0,1]$, precisely the required uniform $O_5(r^{-2})$ estimate. [given, F1, F3, algebra] ∎

### Source notes

The polynomial construction and normalization are attributed to Radu, Section 3.2 (3.12)–(3.18); the fixed-chart differentiated notation is stated in Section 1.1 after (1.1). The proof here is a local conditional calculation, including the explicit uniform derivative bound. Neither existence of the stationary primitive nor the Einstein–Maxwell equations are imported or established here.


## Exact asymptotic and orbit package for the IK criterion

[Open item](item-def-author-9f9c6144aed8-ik-af) · level 2


### Definition

Fix a smooth connected orientable paracompact boundaryless, time-oriented Lorentzian four-manifold $(M,g,N)$ and a smooth Killing field $T$, with the stationary Lorentzian conventions. The **IK AF package** consists of an open end $M^{\mathrm{end}}\cong\mathbb R\times\{x\in\mathbb R^3:|x|>R\}$, with coordinates $(t,x)$, $r=|x|$, $T=\partial_t$, and $g_{00}=-1+2M/r+O(r^{-2})$, $g_{ij}=\delta_{ij}+O(r^{-1})$, $g_{0i}=O(r^{-2})$, where the constant $M>0$ is the mass parameter (distinct from the manifold denoted by the same letter).

Here $u=O(r^{-b})$ means $u(0,\cdot)=O_0(r^{-b})$ in the fixed spatial chart: some $R_1>R$ and finite $C\geq0$ satisfy $|u(0,x)|\leq Cr^{-b}$ for all $r\geq R_1$, componentwise for an array. The metric remainders are independent of $t$ because $T=\partial_t$ is Killing, so the same bounds hold for every $t\in\mathbb R$, uniformly over spatial angular directions and time. No differentiated decay is asserted by this unindexed notation.

Set $E=I^-_M(M^{\mathrm{end}})\cap I^+_M(M^{\mathrm{end}})$, using chronological reachability in $M$. Require an embedded spacelike section $\Sigma_0\cong\{|x|>1/2\}$ agreeing with $t=0$ on the end. Denote its unique smooth future unit normal by $T_0$, so $g(T_0,T_0)=-1$, $g(T_0,N)<0$ and $g(T_0,v)=0$ for $v\in T\Sigma_0$.

For each $p\in E$, let $\gamma_p:I_p\to M$ be the unique maximal integral curve of $T$ with $\gamma_p(0)=p$. Require every such orbit to be complete, meaning $I_p=\mathbb R$, and to meet $\Sigma_0$. Require also $|g(T,T_0)|>0$ on $\Sigma_0\cap E$. These requirements are assumptions, not consequences of mere stationarity or leading asymptotic decay.

### Definition references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)

### Facts & Assumptions

[F1] The stationary Lorentzian data specify the smooth metric, time orientation, Killing equation and local-flow conventions. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] The chronological exterior is the intersection of chronological past and future computed in the specified ambient manifold; a spacelike hypersurface has positive-definite induced metric. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F3] The fixed-chart decay interface with $m=0$ defines $O_0(r^{-b})$ by a common radius and componentwise constants, uniformly over spatial angular directions. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F4] In a smooth time-oriented Lorentzian four-manifold, an embedded spacelike hypersurface has a unique future unit normal, smooth along the hypersurface. Only parts (a)–(b) of the normal lemma are used. [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)

[F5] A smooth vector field has a unique maximal integral curve through each point, normalized at parameter zero. [math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)

### Justification

**Given:** The manifold, field, end chart and spacelike section specified in the Definition.

1.1 The chronological operations determine $E$ in the ambient manifold. The normal lemma applies to the time-oriented Lorentzian manifold and embedded spacelike section, giving the stated unique smooth $T_0$. The maximal-integral-curve theorem applies to the smooth $T$ on $M$, so $I_p=\mathbb R$ and intersection with $\Sigma_0$ are unambiguous additional predicates for each $p\in E$. Nonvanishing of $g(T,T_0)$ is the separately imposed transversality condition; no existence of an AF package or completeness theorem is asserted. [given, F1, F2, F4, F5]

2.1 In the end chart the local flow of $T=\partial_t$ sends $(t,x)$ to $(t+s,x)$. Differentiating its metric pullback at $s=0$ by the Lie-derivative definition gives $0=(\mathcal L_Tg)_{\mu\nu}=\partial_tg_{\mu\nu}$. Thus each metric remainder has the same value at $(t,x)$ as at $(0,x)$. Applying the $m=0$ decay convention to the time-zero remainder gives the same radius and constants for all $t$, exactly the ordinary bounds defined above. The package therefore specifies definite data and predicates without deriving any of its existence or orbit assumptions from the asymptotic estimates. [given, F1, F3, step 1.1] ∎

### External input

The independent Ionescu–Klainerman source supplies the AF predicates in section 1.2, equations (1.4)–(1.5), printed/PDF pp. 6–7. Only that definition package is imported; no vacuum equation, existence theorem or analytic continuation result is inferred here.


## Pathwise exhaustion by anchored Ernst sublevels

[Open item](item-lem-author-9f9c6144aed8-sublevel-path-exhaustion) · level 2


### Statement

Let $X$ be a smooth manifold, $y:X\to\mathbb R$ continuous, $q\in X$, and for $R>y(q)$ let $U_R$ be the connected component containing $q$ of $\{y<R\}$. Every point joined to $q$ by a continuous path in $X$ belongs to some $U_R$. Hence if a tensor field vanishes on every $U_R$, it vanishes on the path component of $q$.

Here all subsets carry the subspace topology. A tensor field may have any fixed type $(r,s)$, with $r,s$ nonnegative integers: at each $p\in X$ it assigns an element of the fibre $T^r_sX$ over $p$. A complex tensor field assigns a pair of real tensors in that fibre, written $A_p+iB_p$; zero means that both parts are zero. No regularity of the tensor field is required.

This applies to the reciprocal potential in the Ernst–Mars–Simon interface on any manifold region where it is defined, using the stationary Lorentzian conventions. It does not prove that this region is the whole exterior, or supply vanishing on a sublevel.

### Statement references

[math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)

[math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)

[math:def-connected-component-and-quasicomponent](https://alphabetamath.cc/item/def-connected-component-and-quasicomponent)

[math:def-path-connected](https://alphabetamath.cc/item/def-path-connected)

[math:def-type-r-s-tensor-bundle](https://alphabetamath.cc/item/def-type-r-s-tensor-bundle)

[math:def-direct-sum-model-of-complexification](https://alphabetamath.cc/item/def-direct-sum-model-of-complexification)

[def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

### Facts & Assumptions

[F1] The Ernst interface supplies a smooth complex scalar $\sigma$, the open set $N=\{1-\sigma\ne0\}$, and the definitions $P=(1-\sigma)^{-1}$ and $y=\operatorname{Re}P$ there. Smoothness of $P,y$ and continuity of $y$ are established below from these data. This supplies no assertion that $N$ is the whole exterior. [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)

[F2] In the stationary application, the ambient smooth manifold and tensor conventions are those of the stationary Lorentzian interface. The general $X$ in the Statement is a smooth manifold of arbitrary dimension. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [math:def-smooth-manifold](https://alphabetamath.cc/item/def-smooth-manifold)

[F3] The type $(r,s)$ tensor bundle has at each point the real multilinear-tensor fibre. Its complexification can be represented by pairs of real tensors, whose zero is the pair of zero tensors. [math:def-type-r-s-tensor-bundle](https://alphabetamath.cc/item/def-type-r-s-tensor-bundle) [math:def-direct-sum-model-of-complexification](https://alphabetamath.cc/item/def-direct-sum-model-of-complexification)

[F4] A composite of continuous maps of topological spaces is continuous. Continuity here is topological continuity, with the usual topology on $\mathbb R$. [math:lem-continuity-is-local-and-pastes](https://alphabetamath.cc/item/lem-continuity-is-local-and-pastes) [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)

[F5] A closed interval $[a,b]$ with $a<b$ in $\mathbb R$ is compact for relative open covers. A real open cover consists of ambient open subsets of $\mathbb R$ covering the set. The real extreme-value theorem applies to a real-variable continuous function on a nonempty compact subset of its real domain and supplies an attained finite maximum. [math:lem-closed-interval-compactness-from-completeness](https://alphabetamath.cc/item/lem-closed-interval-compactness-from-completeness) [math:def-open-cover-r](https://alphabetamath.cc/item/def-open-cover-r) [math:thm-extreme-value-r](https://alphabetamath.cc/item/thm-extreme-value-r)

[F6] An order-convex subset of $\mathbb R$, in particular $[0,1]$, is connected in the real separated-set sense. The topological bridge identifies this with connectedness for the subspace topology inherited from the usual topology on $\mathbb R$. Thus $[0,1]$ with that subspace topology is connected as a topological space. [math:thm-connected-subsets-of-r-are-intervals](https://alphabetamath.cc/item/thm-connected-subsets-of-r-are-intervals) [math:cor-connected-subsets-of-the-line](https://alphabetamath.cc/item/cor-connected-subsets-of-the-line)

[F7] Continuous images of connected spaces are connected. A map whose image lies in a subspace is continuous into that subspace exactly when its composite with the inclusion is continuous. The connected component of a point in that subspace contains every connected subset through that point. [math:thm-continuous-image-of-a-connected-space](https://alphabetamath.cc/item/thm-continuous-image-of-a-connected-space) [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top) [math:def-connected-component-and-quasicomponent](https://alphabetamath.cc/item/def-connected-component-and-quasicomponent)

[F8] A path from $q$ to $p$ is a continuous map $\gamma:[0,1]\to X$ with endpoints $q,p$; the path component of $q$ consists exactly of its path endpoints. [math:def-path-connected](https://alphabetamath.cc/item/def-path-connected)

[F9] The usual topology of $\mathbb R$ has a neighborhood basis $(c-\delta,c+\delta)$, equivalently $\{t:|t-c|<\delta\}$, with $\delta>0$. Real-variable continuity on $A\subseteq\mathbb R$ is the relative epsilon–delta condition at each $c\in A$. [math:lem-real-line-is-a-metric-space](https://alphabetamath.cc/item/lem-real-line-is-a-metric-space) [math:def-continuity-real](https://alphabetamath.cc/item/def-continuity-real)

[F10] Smooth maps are described in smooth charts by componentwise $C^k$ Euclidean maps for every finite $k$. Finite sums, scalar multiples, products and compositions preserve $C^k$ on open Euclidean domains. For $m,n\ge1$, a $C^k$ map from an open subset of $\mathbb R^m$ to real $n\times n$ matrices has a $C^k$ inverse wherever its determinant is nonzero; the case $n=1$ gives scalar reciprocals. [math:def-c-r-and-smooth-maps-between-smooth-manifolds](https://alphabetamath.cc/item/def-c-r-and-smooth-maps-between-smooth-manifolds) [math:thm-ck-euclidean-maps-closed-under-algebra-and-composition](https://alphabetamath.cc/item/thm-ck-euclidean-maps-closed-under-algebra-and-composition) [math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)

[F11] An open subset of a smooth manifold carries the restricted smooth structure, with its subspace topology. A smooth map on an open manifold domain is continuous there. [math:prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure](https://alphabetamath.cc/item/prop-an-open-subset-of-a-smooth-manifold-has-a-canonical-restricted-smooth-structure) [math:prop-smooth-maps-are-continuous](https://alphabetamath.cc/item/prop-smooth-maps-are-continuous)

[F12] Every complex number has unique real and imaginary parts; if $u+iv\ne0$, then $(u+iv)^{-1}=(u-iv)/(u^2+v^2)$ and $u^2+v^2>0$. [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)

### Proof

**Given:** The objects in the Statement and a path $\gamma:[0,1]\to X$ with $\gamma(0)=q$ and $\gamma(1)=p$.

**Goal:** Put $p$ in some $U_R$ and deduce the vanishing assertion.

1.1 Put $h=y\circ\gamma:[0,1]\to\mathbb R$, which is topologically continuous by composition. For $c\in[0,1]$ and $\varepsilon>0$, continuity supplies a relative open neighborhood $W$ of $c$ mapped into $(h(c)-\varepsilon,h(c)+\varepsilon)$. Write $W=O\cap[0,1]$ with $O$ open in $\mathbb R$. Choose $\delta>0$ with $(c-\delta,c+\delta)\subseteq O$. Then $t\in[0,1]$ and $|t-c|<\delta$ imply $|h(t)-h(c)|<\varepsilon$. Thus $h$ satisfies precisely the real-variable continuity hypothesis of the extreme-value theorem. [given, F4, F7, F9, choose]

1.2 In the stationary application, $N$ is an open subset of the supplied smooth four-manifold, so use its restricted smooth structure. Identify a smooth complex scalar with its two real component functions and write $\sigma=a+ib$. On $N$ put $d=(1-a)^2+b^2>0$. The complex inverse formula gives $P=(1-a+ib)/d$ and $y=(1-a)/d$. In every restricted chart, $a,b,d$ are $C^k$ for every finite $k$ by componentwise smoothness and finite algebra. Apply the inverse-regularity result to the $1\times1$ matrix $[d]$ on that open chart domain: its determinant is $d\ne0$, so $1/d$ is $C^k$ for every finite $k$. Finite products give both components of $P$ and $y$ the same regularity. These components are continuous in the charts because order-zero regularity is included in $C^k$; composing with chart homeomorphisms gives continuity locally on $N$, and locality gives continuity on $N$. The smooth-map definition now gives smoothness of $P,y$, and the smooth-continuity result also gives the continuity of $y$ needed by the lemma. [F1, F2, F4, F10, F11, F12, algebra]

2.1 The interval $[0,1]$ is nonempty and compact for relative open covers since $0<1$. Restricting any ambient real open cover to $[0,1]$ gives a relative open cover; its finite subcover supplies a finite selection of the original ambient sets, still covering $[0,1]$. Hence the interval is compact also in the real open-cover convention. Apply the real extreme-value theorem to $A=K=[0,1]$ and $h$ from step 1.1 to obtain a finite maximum $B$. Put $R=B+1$. Then $R>y(q)$ and $\gamma([0,1])\subseteq\{y<R\}$. [given, step 1.1, F5, F7, choose]

3.1 Write $S_R=\{y<R\}$. The same path regarded as a map $[0,1]\to S_R$ is continuous by the characteristic property of the subspace topology. The interval with its usual subspace topology is connected as a topological space by F6, so its image is connected in $S_R$ and contains $q$. [given, step 2.1, F6, F7]

4.1 The connected-component definition in $S_R$ puts this connected image through $q$ inside $U_R$. In particular, $p=\gamma(1)\in U_R$. [step 3.1, F7]

5.1 If the specified tensor field vanishes on every $U_R$, step 4.1 gives its zero value at $p$. This uses only pointwise zero in the tensor fibre, and applies equally to both parts of a complex tensor. Every point in the path component is such an endpoint, so the field vanishes on that component. [given, step 4.1, F3, F8]

6.1 Apply steps 1.1, 2.1, 3.1, 4.1 and 5.1 on $N$, or on any manifold region in $N$ on which the potential is restricted, using the continuity established in step 1.2. The domain restriction and the need to supply sublevel vanishing are retained: this gives neither that $N$ is the whole exterior nor vanishing on a sublevel. [step 1.1, step 2.1, step 3.1, step 4.1, step 5.1, step 1.2, F1, F2] ∎


## Exact asymptotically stationary end contract

[Open item](item-def-author-4cb89398a4ab-asymptotically-stationary-end) · level 2


### Definition

Use the smooth time-oriented Lorentzian data $(M,g,N,T)$ and causal-curve conventions supplied by the Lorentzian and causal interfaces. Here acausal means that no two distinct points are joined by a causal curve. A hypersurface, possibly with boundary, means an embedded smooth three-dimensional submanifold of the four-manifold $M$, with a supplied manifold-with-boundary smooth structure; its codimension is $4-3=1$. A Chruściel–Wald $(k,\alpha)$-asymptotically stationary end consists of such an acausal hypersurface $\Sigma=\Sigma_1\sqcup\Sigma'$ and the following data and requirements. The remainder $\Sigma'$ is supplied as an embedded smooth three-dimensional submanifold with boundary of $\Sigma$; its boundary means its intrinsic manifold boundary, with the induced smooth two-manifold structure, rather than its topological boundary in $M$. Its inclusion in $M$ is also required to be a smooth embedding.

(1) Supply a diffeomorphism $e:E\to\Sigma_1$, where $E=\{z\in\mathbb R^3:|z|>R_1\}=\mathbb R^3\setminus B(R_1)$, $R_1>0$, and $B(R_1)$ is the closed Euclidean ball. Thus $\Sigma_1$ has the smooth structure of an open end of $\Sigma$. A coordinate system $(t,x^1,x^2,x^3)$ on an open neighborhood $O_1$ of $\Sigma_1$ obeys the following estimates for constants $C>0$, integer $k\ge2$, $0<\alpha\le1$ and $0<\lambda\le1$. Put $r=(\sum_i(x^i)^2)^{1/2}$ and require $r>0$ throughout $O_1$. The model coordinate $z$ and the spacetime coordinates $(t,x)$ are separately supplied: no identity $x=e^{-1}$, level-set condition $t|_{\Sigma_1}=0$, or inequality $r>R_1$ on $O_1$ is assumed. Put $\eta=\operatorname{diag}(-1,1,1,1)$; indices $\mu,\nu,\sigma_j$ range from $0$ to $3$, and $i,j$ from $1$ to $3$:

$$g_{00}<-C^{-1},\qquad |g_{\mu\nu}-\eta_{\mu\nu}|\le Cr^{-\alpha},\qquad g_{ij}Z^iZ^j\ge C^{-1}\sum_i(Z^i)^2\quad(Z\in\mathbb R^3).$$

$$|\partial_{\sigma_1}\cdots\partial_{\sigma_m}g_{\mu\nu}|\le Cr^{-\alpha-m}\quad(1\le m\le k).$$

Writing $\partial^k$ for any ordered $k$ coordinate derivatives, require

$$|(\partial^kg_{\mu\nu})(t,x)-(\partial^kg_{\mu\nu})(\tau,y)|\le Cr(x)^{-\alpha-k-\lambda}(|t-\tau|^\lambda+|x-y|^\lambda)$$

whenever both points lie in $O_1$, $|t-\tau|\le1$ and $|x-y|\le r(x)/2$. Absolute values on components are ordinary real absolute values and $|x-y|$ is the Euclidean norm; the estimate holds for each component and derivative choice.

(2) Let $\overline E=\{z\in\mathbb R^3:|z|\ge R_1\}$ have its usual smooth manifold-with-boundary structure, and let $S$ be a connected component of the intrinsic boundary $\partial\Sigma'$. Supply a diffeomorphism $h:\partial\overline E\to S$, meaning a bijective smooth map with smooth inverse. Its realization in the given smooth hypersurface is part of the data: supply a smooth embedding $j:\overline E\to\Sigma$ whose restriction to $E$ is $e$ followed by the inclusion of $\Sigma_1$, and whose restriction to $\partial\overline E$ is $h$ followed by the inclusion of $S$. Require $j(\overline E)\cap\Sigma'=S$ and $j(\overline E)\cup\Sigma'=\Sigma$. These maps specify the smooth boundary identification implicit in the source's disjoint end/remainder notation. No compactness of $\Sigma'$ is imposed, and existence of such a gluing realization is required data, not an asserted gluing theorem.

(3) The smooth Killing field $T$ on all of $M$ has a complete flow $\phi_u$, $u\in\mathbb R$, satisfies $g(T,T)<-C^{-1}$ on $\Sigma_1$, and has asymptotics

$$T=(A+O(r^{-\alpha}))\partial_t+\sum_iO(r^{-\alpha})\partial_{x^i},\qquad A\ne0.$$

Here a complete flow means a smooth global flow of $T$: the map $\phi:\mathbb R\times M\to M$, $\phi(u,p)=\phi_u(p)$, is smooth, $\phi_0=\operatorname{id}_M$, $\frac{d}{du}\phi_u(p)=T_{\phi_u(p)}$, and $\phi_{u+v}=\phi_u\circ\phi_v$ for all real $u,v$. The component $O(r^{-\alpha})$ bounds hold uniformly in the end coordinates as $r\to\infty$. Constants may be enlarged to one common $C$. These are imposed data, not consequences of the word stationary.

### Definition references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)

[math:def-codimension-and-hypersurface](https://alphabetamath.cc/item/def-codimension-and-hypersurface)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[math:thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold](https://alphabetamath.cc/item/thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

### Facts & Assumptions

[F1] The Lorentzian and causal suppliers define the underlying metric, Killing field and causal terminology. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F2] Chruściel–Wald Definition 2.1 supplies the three end conditions: the displayed metric estimates, the boundary identification, and the complete uniformly timelike Killing field with its stated asymptotics. The smooth gluing realization and positive-r estimate domain are made explicit here as supplied data.

[F3] An embedded smooth submanifold with boundary carries a supplied smooth structure for which its inclusion is a smooth embedding. Codimension is ambient dimension minus submanifold dimension. These interfaces apply to $\Sigma\subset M$ and to the remainder and closed-end realization in $\Sigma$. [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary) [math:def-codimension-and-hypersurface](https://alphabetamath.cc/item/def-codimension-and-hypersurface)

[F4] The boundary of a smooth three-manifold with boundary has the induced smooth boundaryless two-manifold structure. A diffeomorphism between boundaryless smooth manifolds is a bijective smooth map with smooth inverse; this applies to $e$ and $h$. [math:thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold](https://alphabetamath.cc/item/thm-the-boundary-is-a-closed-embedded-smooth-n-minus-one-manifold) [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[F5] A global flow of a smooth vector field is a smooth map on $\mathbb R\times M$ with identity at zero, integral curves generated by the field, and the flow composition law. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

### Justification

**Given:** The displayed smooth structures, maps, coordinate domain and conditions.

**Goal:** Define a precise end contract without asserting existence for arbitrary stationary data.

1.1 The Lorentzian and causal conventions give meanings to the metric, Killing condition and acausality. The supplied embeddings make $\Sigma$ a codimension-one smooth submanifold, and give $\Sigma'$ and $j(\overline E)$ their stated manifold-with-boundary structures. These are requirements on the data, so no smooth structure is inferred from an arbitrary set-theoretic remainder. [given, F1, F3]

1.2 In the chosen spacetime chart every derivative and norm in (1) is a derivative or norm of a specified real component. The explicit condition $r>0$ on all of $O_1$ makes each negative radial power defined, including at both points in the Hölder condition. This uses no relation between the model radius $|z|$ and the coordinate radius $r$, and does not infer $r>R_1$ from the topology of $\Sigma_1$. [given, F1, F2]

2.1 The supplied boundary diffeomorphism $h$ is between smooth two-manifolds; the restrictions of $j$ identify its boundary values with that map and its interior values with the end model. Thus (2) is a definite compatibility condition on supplied smooth maps. Clause (3) separately requires the smooth global flow generated by $T$ in [F5] and its component bounds; a local Killing field alone does not supply it. The conjunction retains the cited metric estimates, Hölder condition, boundary identification and uniform timelikeness, with the necessary structural and domain conventions explicit and with no existence conclusion. [given, F1, F2, F3, F4, F5, step 1.1, step 1.2] ∎

### External input

The end estimates, boundary identification and Killing-field conditions are imported from Chruściel–Wald Definition 2.1, printed/PDF pp. 8–9. The preceding paragraph supplies its embedded codimension-one hypersurface convention. The smooth boundary realization and positive-r domain are explicit formulation data here; no coordinate or gluing existence result is imported or proved.


## Black and white exclusion is an ambient reachability condition

[Open item](item-lem-author-9e5789a3d617-exterior-exclusion-interface) · level 2


### Statement

In a time-oriented spacetime $M$, fix a union of stationary end regions $M_{\rm ext}$ and any subset $U\subset M$. Define $B=M\setminus I_M^-(M_{\rm ext})$ and $W=M\setminus I_M^+(M_{\rm ext})$. Then $(B\cup W)\cap U=\varnothing$ if and only if $U\subset I_M^-(M_{\rm ext})\cap I_M^+(M_{\rm ext})$. For any subset $\Sigma\subset M$, define $D(\Sigma)$ here to be the set of points through which every inextendible timelike curve in $M$ meets $\Sigma$. The equivalence applies in particular to $U=\operatorname{int}D(\Sigma)$ with this explicit local convention. The chronological relations are computed in $M$; changing the ambient spacetime requires recomputing them.

### Facts & Assumptions

[F1] Chronological past and future use future timelike curves in the specified ambient manifold. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated construction and identities.

1.1 The equality $(B\cup W)\cap U=\varnothing$ means simultaneously that $U\cap B$ and $U\cap W$ are empty. Taking complements in $M$ gives $U\subset I_M^-(M_{\rm ext})$ and $U\subset I_M^+(M_{\rm ext})$. Their conjunction is precisely the stated inclusion. [F1]

2.1 Conversely the inclusion excludes every point of $U$ from each complement, so it excludes their union. This set argument holds for any $U$, in particular the interior of the domain of dependence defined above; it neither identifies that domain with a desired exterior nor changes timelike-curve domains of dependence to a different convention. [F1, step 1.1] ∎


## Exact AIK global, horizon and quantitative hypotheses

[Open item](item-def-author-0a41d659d5ab-aik-quantitative-package) · level 2


### Definition

The **AIK quantitative stationary package** is the following collection of data and assumptions; it is separate from a generic bifurcate Killing horizon and from other black-hole comparison packages.

Let $(M,g,N,o)$ be a connected oriented, time-oriented, paracompact smooth Lorentzian four-manifold without boundary of signature $(-,+,+,+)$, with $\operatorname{Ric}(g)=0$ and a smooth Killing field $T$. Let $E_r=\{x\in\mathbb R^3:|x|>r\}$ and let $\Phi_0:E_{1/2}\to\Sigma_0\subset M$ be a diffeomorphism onto an embedded spacelike partial Cauchy hypersurface. Here partial Cauchy means acausal and edgeless: no two distinct points are causally related, and there is no $q\in\overline{\Sigma_0}$ such that every neighborhood $U$ of $q$ contains a timelike curve, avoiding $\Sigma_0$, from a point of $I^-_U(q)$ to a point of $I^+_U(q)$. No claim that it is Cauchy for all of $M$ is imposed. Write $\Sigma_r=\Phi_0(E_r)$ and $S_0=\Phi_0(\{|x|=1\})$. Require $\Sigma_1$ to be maximal. Let $\nu$ be the future unit normal to $\Sigma_0$, $h=g|_{T\Sigma_0}$, $n=-g(T,\nu)$, and $X=T-n\nu$.

**GR.** For sufficiently large $R_0$, the map on $E_{R_0}$ extends to a diffeomorphism $\Phi_0:\mathbb R\times E_{R_0}\to M^{\rm end}$ onto an open end, with $T=\partial_0$. Put $r=|x|$. There are $M_0>0$ and $S^1,S^2,S^3\in\mathbb R$, with $J=((S^1)^2+(S^2)^2+(S^3)^2)^{1/2}<M_0^2$, such that $g_{00}=-1+2M_0/r+O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$, and $g_{0i}=-2\epsilon_{ijk}S^jx^k/r^3+O_6(r^{-3})$. The alternating symbol has $\epsilon_{123}=1$. Differentiated bounds count all coordinate derivatives through total order six, including $x^0$ derivatives (which vanish on this stationary end). Set $E=I^-_M(M^{\rm end})\cap I^+_M(M^{\rm end})$. Require $E$ to be globally hyperbolic, $\Sigma_0\cap I^-_M(M^{\rm end})=\Sigma_0\cap I^+_M(M^{\rm end})=\Sigma_1$, $T\ne0$ on $E$, and every $T$-orbit in $E$ to be complete and intersect $\Sigma_1$ transversely.

**SBS.** In a neighborhood $O$ of $S_0$, require $H^+=O\cap\partial_M I^-_M(M^{\rm end})$ and $H^-=O\cap\partial_M I^+_M(M^{\rm end})$ to be smooth embedded null non-expanding hypersurfaces intersecting transversely in $S_0$. Here is the precise non-expansion convention, which applies to either null hypersurface $H=H^\pm$. Let $L_p=T_pH\cap(T_pH)^{\perp_g}$ be its null normal line and $Q_p=T_pH/L_p$ the two-dimensional quotient. Its positive-definite metric is $q_p([U],[V])=g_p(U,V)$, with $[U]$ denoting the class modulo $L_p$. For a smooth nowhere-zero local section $\ell$ of $L$, the **null second fundamental form** is the symmetric form on $Q$ given by $B_\ell([U],[V])=g(\nabla_U\ell,V)$, where $U,V$ are tangent to $H$ and $\nabla$ is the ambient Levi–Civita connection. Tangential covariant differentiation may use any smooth ambient extension of $\ell$. Its **expansion** is $\theta_\ell=\operatorname{tr}_q B_\ell=q^{AB}(B_\ell)_{AB}$, where $A,B=1,2$ label any local frame of $Q$ and $(q^{AB})$ is the inverse quotient metric. The hypersurface is **non-expanding** when $\theta_\ell=0$ on every such local domain. The local justification below proves well-definedness and $\theta_{f\ell}=f\theta_\ell$ for every smooth nowhere-zero real function $f$, so this vanishing condition needs no normal scale or affine parametrization. Require $T$ to be tangent to both and not identically zero on $S_0$. These conditions do not identify $T$ with a horizon-generating Killing field vanishing on $S_0$.

**Quantitative choices.** Fix large $A_1\ge2$ and $R_1\ge\max(R_0,A_1^4,8M_0,2\sqrt{A_1},2)$. On $\Sigma_{3/4}$ require $A_1^{-1}|v|^2\le h_{ij}v^iv^j\le A_1|v|^2$ and $\sum_{i=1}^3|g(\partial_i,T)|+|g(\nu,T)|\le A_1$. On the restricted end $\Phi_0(\mathbb R\times E_{R_1})$ require
$$\sum_{m=0}^6r^{m+1}\sum_{j,k=1}^3|\partial^m(g_{jk}-\delta_{jk})|+\sum_{m=0}^6r^{m+2}|\partial^m(g_{00}+1-2M_0/r)|+\sum_{m=0}^6r^{m+3}\sum_{i=1}^3|\partial^m(g_{0i}+2\epsilon_{ijk}S^jx^kr^{-3})|\le A_1.$$

Here $|\partial^m u|$ is the sum over all four-coordinate derivatives of total order $m$; the displayed decay bound is imposed on $\Phi_0(\mathbb R\times E_{R_1})$, rather than on all of the original $R_0$ end.

As in source §1.2, specify a smooth cutoff $\chi:\mathbb R\to[0,1]$ supported in $(-\infty,2]$ and equal to one on $(-\infty,1]$. Specify a smooth ambient vector field $T'$ in a neighborhood of $\Sigma_{3/4}$ and on $\Phi_0(\mathbb R\times E_{2R_1})$, with $T'=\chi(r/R_1)\nu+(1-\chi(r/R_1))T$ on $\Sigma_{3/4}$ and $T'=T$ on $\Phi_0(\mathbb R\times E_{2R_1})$. For $0<\eta_0<1/4$ sufficiently small, require the local flow of $T'$ to give the diffeomorphism $\Phi_1:(-\eta_0,\eta_0)\times E_{1-\eta_0}\to\widetilde M$, with $\Phi_1(t,x)=\operatorname{Fl}^{T'}_t(\Phi_0(x))$ and $\partial_0=T'$ in these coordinates. Require $\Phi_1(0,x)=\Phi_0(x)$ for $x\in E_{1-\eta_0}$ and $\Phi_1(t,x)=\Phi_0(t,x)$ for $(t,x)\in(-\eta_0,\eta_0)\times E_{2R_1}$. No stationary-coordinate agreement is required for $R_0<r\le2R_1$ away from the slice. Require $\sum_{j=1}^3|g_{0j}|+|g_{00}+1|\le A_1/(R_1+r)$ throughout $\widetilde M$ in the $\Phi_1$ coordinates, and put
$$A_2=\sup_{\widetilde M}\sum_{m=0}^6\left(\sum_{\alpha,\beta=0}^3|\partial^mg_{\alpha\beta}|+\sum_{\alpha=0}^3|\partial^mT^\alpha|\right),\qquad A=\max(R_1,A_2,\eta_0^{-1},(M_0^2-J)^{-1})<\infty.$$

The source uses $\epsilon_0$ for $\eta_0$ and $\epsilon$ for the independent horizon-smallness parameter. The extra lower bounds $R_1\ge8M_0,2\sqrt{A_1},2$ are a choice of a sufficiently large end radius, permitted before fixing $A$; they impose no smallness assumption on a spacetime. One can enlarge the end radius and redo the source's cutoff construction before fixing the quantitative constants.

### Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The Lorentzian, stationary-field, curvature and index conventions, including the inverse metric and the torsion-free metric-compatible Levi–Civita connection, are those of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] The horizon vocabulary distinguishes the stationary field from a Killing generator and defines nullness, the radical null normal line and bifurcation transversality. The quotient metric, null second fundamental form and expansion are defined locally in the present Definition and justified below. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[F3] Spacelike sections, the future unit normal, maximality, lapse and shift use [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data).

[F4] Fixed-chart differentiated decay uses [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data); the present Definition explicitly extends its derivative counting to the four source coordinates.

[F5] Exterior chronological sets, completeness, transversality and global hyperbolicity have the domain-relative meanings of [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data).

[F6] The independent source assumption contract is recorded in External input.

[F7] The local-flow notation for $T'$ uses [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) on the open neighborhood where $T'$ is smooth. Its domain and integral-curve laws require neither a Killing field nor completeness; the uniform time interval, chart diffeomorphism and agreement properties remain imposed hypotheses.

### Justification

**Given:** The data and hypotheses in the Definition, with the set-theoretic convention [A1].

**Goal:** Verify that the package is a definite collection of hypotheses, without asserting its existence.

1.1 The specified charts and section determine $r$, all component derivatives, the end, the exterior, and the sphere. The geometric interfaces make the smoothness, causal, spacelike-normal and maximality conditions predicates on these data. The flow notation is interpreted on the open neighborhood where $T'$ is specified, in the sense of [F7]. The flow chart uses $E_{1-\eta_0}\subset E_{3/4}$, and its agreement sets are the slice and $(-\eta_0,\eta_0)\times E_{2R_1}$; on the latter the interpolating field equals $T$. The decay sum uses only the restricted $R_1$ end. These charts, interpolation and inequalities are supplied hypotheses, not conclusions of generic stationarity. The SBS tangencies concern $T$, whereas a Killing generator in [F2] is separately specified; the two are not equated. [given, F1, F2, F3, F4, F5, F6, F7]

1.2 For a local defining function $u$ of the embedded null hypersurface $H$, $du\ne0$ and $H=\{u=0\}$ locally. Nondegeneracy gives a smooth nonzero normal $g^{-1}(du)$ spanning $(TH)^{\perp_g}$, which is one-dimensional and contained in $TH$ by nullness. Thus $L$ is a smooth line bundle with local nonzero sections. At any point, normalize the supplied timelike orientation vector to $e_0$, with $g(e_0,e_0)=-1$. A nonzero null vector can be written $\ell=a(e_0+e_1)$, with $a\ne0$ and $e_1\in e_0^\perp$ of length one. The space $e_0^\perp$ is positive definite by signature $(-,+,+,+)$. Every $U\in TH=\ell^\perp$ then has the unique form $U=b(e_0+e_1)+v$ with $v\in e_0^\perp\cap e_1^\perp$. For $V=c(e_0+e_1)+w$, $g(U,V)=g(v,w)$. This proves that $q$ is well-defined and positive definite on the two-dimensional quotient $Q$; smoothness follows in local quotient frames from smoothness of $g$ and $L$. [given, F1, F2, algebra]

2.1 For tangent fields $U,V$, metric compatibility gives $g(\nabla_U\ell,V)=-g(\ell,\nabla_UV)$. Torsion freedom and tangency of $[U,V]$ give $B_\ell(U,V)-B_\ell(V,U)=-g(\ell,[U,V])=0$. Also $g(\nabla_U\ell,\ell)=\tfrac12U(g(\ell,\ell))=0$, so symmetry makes both slots vanish on $L$. The expression is bilinear over smooth functions in $U,V$, descends to $Q$, and is independent of representatives. Any two ambient extensions of $\ell$ differ by a field vanishing along $H$, whose covariant derivative in a tangent direction vanishes there; hence the formula is extension-independent and defines a smooth symmetric form. [step 1.2, F1, F2, algebra]

3.1 The positive-definite quotient metric has an inverse, so the contraction defining $\theta_\ell$ is independent of the quotient frame. For any smooth nowhere-zero $f$, the connection product rule gives $g(\nabla_U(f\ell),V)=f g(\nabla_U\ell,V)+(Uf)g(\ell,V)=f B_\ell([U],[V])$. Consequently $B_{f\ell}=fB_\ell$ and $\theta_{f\ell}=f\theta_\ell$. Every pair of local nonzero sections of $L$ differs by such an $f$ on their overlap. Thus vanishing of the expansion is independent of all local choices and defines the non-expansion predicate used in SBS. [step 1.2, step 2.1, F1, F2, algebra]

4.1 The finite derivative sums and the displayed supremum define $A_2$ as an extended nonnegative number; the explicit finiteness requirement makes $A$ finite. The strict condition $J<M_0^2$ makes its last term positive and finite. Fixing these charts and bounds before choosing a small horizon parameter makes dependence on $A$ unambiguous. Choosing the end radius sufficiently large, and the flow interval sufficiently small, is the source §1.2 convention and does not infer existence of any unassumed geometric object. Together with the local null-form calculation, this makes the entire package a definite collection of hypotheses. [step 1.1, step 3.1, F4, F6, algebra] ∎

### External input

AIK §§1.1–1.2 supplies the GR, SBS, maximal-section and quantitative-coordinate assumption contract (1.1)–(1.4), (1.6)–(1.10), including the restricted end for (1.7) and the slice/far-end agreement for the flow chart. These are imposed assumptions, not conclusions of generic stationarity, an I-plus-regularity equivalence or a local reconstruction of a rigidity theorem. The null quotient metric, second fundamental form and scale-invariant zero-expansion predicate are supplied by the local Definition and Justification, rather than imported as an unstated source theorem. Minguzzi Definitions 2.130 and 3.35 supply the edge and partial-Cauchy conventions.


## Vacuum curvature of a globally static product

[Open item](item-lem-author-f247c641a714-static-vacuum-reduction) · level 2


### Statement

For the static product of the regular exterior data, the equation $\operatorname{Ric}(g)=0$ on $\mathbb R\times X$ is equivalent to
$$\Delta_hV=0,\qquad D^2V=V\operatorname{Ric}(h).$$
When these equivalent conditions hold, the scalar curvature of $h$ is zero. The displayed spatial equations then extend continuously to $B$ when $h,V$ are $C^2$ there, in the multiplication form displayed above.

### Statement references

[def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)

[math:def-scalar-curvature](https://alphabetamath.cc/item/def-scalar-curvature)

[math:def-ricci-curvature](https://alphabetamath.cc/item/def-ricci-curvature)

### Facts & Assumptions

[F1] The formulation and calculations use the following exact object, operator and earlier-result interfaces: [def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)

[F2] On the smooth interior, the Riemannian Christoffel formula applies to the positive-definite metric $h$, and the nondegenerate four-metric Christoffel formula applies to $g=-V^2dt^2+h$ because $V>0$ there. The ZFC convention of [F1] includes the countable choice assumed by the latter supplier. [math:prop-christoffel-formula-for-the-levi-civita-connection](https://alphabetamath.cc/item/prop-christoffel-formula-for-the-levi-civita-connection) [physics:thm-gr-nondegenerate-levi-civita-and-tensor-derivative](https://alphabetamath.cc/physics/item/thm-gr-nondegenerate-levi-civita-and-tensor-derivative)

[F3] For the smooth Riemannian metric $h$ on $X$, scalar curvature is the metric trace of its Ricci tensor: $\operatorname{Scal}(h)=h^{ij}\operatorname{Ric}_{ij}(h)$. The ZFC convention of [F1] includes the countable choice assumed by this definition. [math:def-scalar-curvature](https://alphabetamath.cc/item/def-scalar-curvature)

[F4] On the smooth Riemannian interior, $\operatorname{Ric}(h)(A,C)=\operatorname{tr}(Z\mapsto R_h(Z,A)C)$, with $R_h(A,C)E=D_AD_CE-D_CD_AE-D_{[A,C]}E$. This curvature sign agrees with the Lorentzian convention in [F1]. [math:def-ricci-curvature](https://alphabetamath.cc/item/def-ricci-curvature)

### Proof

**Given:** The static product of [F1], its Levi–Civita curvature conventions and coordinate Hessian formula, the Christoffel formulas in [F2], the scalar-curvature definition in [F3], and the Riemannian Ricci definition in [F4].

**Goal:** Derive the spatial equations, rather than presume a static vacuum reduction.

1.1 In product coordinates, $g_{tt}=-V^2$, $g_{ti}=0$ and $g_{ij}=h_{ij}$. The Christoffel formulas of [F2] give $\Gamma^t{}_{ti}=V^{-1}\partial_iV$, $\Gamma^i{}_{tt}=Vh^{ij}\partial_jV$, $\Gamma^i{}_{jk}=\Gamma^i{}_{jk}(h)$, with all other mixed Christoffel symbols zero. Substituting into $\operatorname{Ric}_{ab}=\partial_c\Gamma^c{}_{ab}-\partial_b\Gamma^c{}_{ac}+\Gamma^c{}_{cd}\Gamma^d{}_{ab}-\Gamma^c{}_{bd}\Gamma^d{}_{ac}$ yields $\operatorname{Ric}_{tt}(g)=V\Delta_hV$, $\operatorname{Ric}_{ti}(g)=0$, and $\operatorname{Ric}_{ij}(g)=\operatorname{Ric}_{ij}(h)-V^{-1}(\partial_i\partial_jV-\Gamma^k{}_{ij}(h)\partial_kV)$. For the last formula, the extra terms are $-\partial_j(V^{-1}\partial_iV)+V^{-1}\Gamma^k{}_{ij}(h)\partial_kV-V^{-2}\partial_iV\partial_jV=-V^{-1}(D^2V)_{ij}$. [given, F1, F2, F4]

2.1 Since $V>0$ in $X$, vanishing of these components is precisely the two equations in the Statement. Their spatial trace, using [F3], is $V\operatorname{Scal}(h)=\Delta_hV=0$, giving zero scalar curvature. At $B$ all quantities in the multiplication form $D^2V=V\operatorname{Ric}(h)$ and in $\Delta_hV=0$ are continuous under the stated $C^2$ hypotheses, so their zero identities have the continuous boundary limits. This extension does not divide by the vanishing lapse. [given, F1, F3, step 1.1] ∎


## The pointwise static end bounds imply the original weighted hypotheses

[Open item](item-lem-author-f247c641a714-static-end-weighted-integrability) · level 2


### Statement

Assume the Axiom of Countable Choice. Let $H_{ij}=h_{ij}-\delta_{ij}$ and $v=V-1+m/r$ in the end of the regular static exterior data, and fix an end cutoff $R>R_0$. For $4<q<\infty$ and $0<\lambda<1$, define $L^q_\alpha$ on $r>R$ by finiteness of $\int_{r>R}|f|^q r^{-\alpha q-3}\,dx$. Then
$$\partial_k\partial_\ell H_{ij}\in L^q_{-\lambda-2},\qquad \partial_k\partial_\ell v\in L^q_{-\lambda-3}.$$
Thus the differentiated pointwise falloff supplies the weighted second-derivative hypotheses in Bunting–Masood-ul-Alam's Assumption 1 (p.148), for example with $q=6$ and $\lambda=1/2$. The compact-core end topology and the zeroth- and first-derivative falloff in that asymptotic contract are also supplied by the regular static exterior data. This comparison concerns the end conditions; positivity of $m$, the static vacuum equations and boundary conditions require their separate arguments.

### Statement references

[def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)

[math:thm-polar-coordinates-formula-for-lebesgue-measure](https://alphabetamath.cc/item/thm-polar-coordinates-formula-for-lebesgue-measure)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

### Facts & Assumptions

[F1] The regular static exterior data have a single Cartesian end outside a compact core, with $H=O_2(r^{-1})$ and $v=O_2(r^{-2})$; the $O_2$ convention gives uniform Cartesian derivative bounds through order two. [def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)

[F2] In dimension three the polar integration formula applies to every nonnegative Borel function on $\mathbb R^3$, with volume element $r^2\,dr\,d\sigma$ and finite Borel measure $\sigma$ on $S^2$. The cited theorem assumes Countable Choice. [math:thm-polar-coordinates-formula-for-lebesgue-measure](https://alphabetamath.cc/item/thm-polar-coordinates-formula-for-lebesgue-measure)

[A1] Adopt the Axiom of Countable Choice to meet precisely the choice hypothesis of [F2]. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F3] The imported asymptotic contract is Bunting–Masood-ul-Alam, p.148, Assumption 1 and its weighted-space definition, as recorded in the External input section and the source reference.

### External input

Only the end-data formulation is imported here: outside a compact core the end is Euclidean in topology, $H=O(r^{-1})$, $\partial H=O(r^{-2})$, $V=1-m/r+v$, $v=O(r^{-2})$, $\partial v=O(r^{-3})$, and for some $\lambda>0$ and $4<q<\infty$ one requires $\partial^2H\in L^q_{-\lambda-2}$ and $\partial^2v\in L^q_{-\lambda-3}$. The weighted convention is $\int |f|^q r^{-\alpha q-3}\,dx<\infty$. These are the conditions read on p.148, Assumption 1, with $H$ here denoting the source's metric perturbation. The local proof below verifies these end conditions from [F1]; no static classification theorem or mass-positivity assertion is imported as a premise of this mathematical lemma.

### Proof

**Given:** The Cartesian end and $O_2$ bounds of [F1], the polar integration theorem [F2] under [A1], and the external formulation [F3].

**Goal:** Verify the two weighted integrability assertions and the stated comparison of end conditions.

1.1 The differentiated bounds give $|\partial^2H|\leq Cr^{-3}$ and $|\partial^2v|\leq Cr^{-4}$ uniformly in angle for $r>R_1$, where $R_1>R$. Extend each nonnegative weighted component integrand by zero off $r>R_1$; smoothness on the end makes this extension Borel measurable. Apply [F2] with $n=3$, using [A1] at this invocation. The first weighted $q$th power is at most $C^q\sigma(S^2)\int_{R_1}^\infty r^{-3q}r^{(\lambda+2)q-3}r^2\,dr=C^q\sigma(S^2)\int_{R_1}^\infty r^{q(\lambda-1)-1}\,dr$. This last integral is $R_1^{q(\lambda-1)}/(q(1-\lambda))<\infty$, since $\lambda<1$. The finite sum of components does not affect convergence. [given, F1, F2, A1]

2.1 For the lapse remainder the same polar formula bounds its weighted $q$th power by $C^q\sigma(S^2)\int_{R_1}^\infty r^{-4q}r^{(\lambda+3)q-3}r^2\,dr=C^q\sigma(S^2)\int_{R_1}^\infty r^{q(\lambda-1)-1}\,dr<\infty$. On the compact annulus $R\leq r\leq R_1$ all component second derivatives and weights are bounded, and its Cartesian volume is finite, also by [F2]. Adding the annular integrals proves both claims on $r>R$. [given, F1, F2, A1, step 1.1]

3.1 The order-zero and order-one parts of [F1] give exactly $H=O(r^{-1})$, $\partial H=O(r^{-2})$, $v=O(r^{-2})$ and $\partial v=O(r^{-3})$, while its compact-core chart gives the required end topology. The weight in [F3] agrees with the Statement, so steps 1.1 and 2.1 verify its second-derivative requirements. Choosing $q=6$ and $\lambda=1/2$ meets $4<q<\infty$ and $\lambda>0$ simultaneously. Enlarging the compact cutoff only discards a compact annulus, whose finite integral was checked in step 2.1. This establishes the asserted end comparison without claiming that a borderline $O(r^{-2})$ second derivative would suffice. [given, F1, F3, step 1.1, step 2.1] ∎



## Stationary maximal hypersurface existence with a horizon boundary

[Open item](item-thm-stationary-maximal-slice-existence-input) · level 3


### Statement

Under the exact class-(b) hypotheses and exclusion condition [F1], There is a family $\widehat\Sigma_s$ of smooth spacelike maximal asymptotically flat hypersurfaces, $s\in\mathbb R$, with $\partial\widehat\Sigma_s=S$, $\widehat\Sigma_s$ diffeomorphic to $\Sigma$, $\phi_t(\widehat\Sigma_s)=\widehat\Sigma_{s+t}$ and interiors covering $U$ and Cauchy there in the source convention. If $X$ is timelike on $U$, or if $\operatorname{Ric}(Z,Z)\geq0$ for every timelike $Z$, their interiors foliate $U$. The source's asymptotic flatness means end graphs obeying Definition 2.4: $|u|+\sum_{j=1}^{k+1}r^j|\partial^ju|\leq Cw_\alpha(r)$, with $w_\alpha$ as in the graph-translation lemma, together with the corresponding weighted Hölder condition on the highest derivatives. In particular at $\alpha=1$ logarithmic height growth is allowed.

### Facts & Assumptions

[F1] The complete class-(b) hypotheses and exclusion condition are as follows. Let $(M,g)$ be a smooth connected time-oriented strongly causal spacetime and $\Sigma$ a connected closed acausal hypersurface with boundary $S$. Closed means closed as a subset of $M$; acausal means that no causal curve connects distinct points of $\Sigma$. Suppose $\Sigma$ is the union of finitely many exterior ends $\Sigma_i$ and a compact interior $\Sigma_{\rm int}$ with boundary, glued along their boundary components. Each $\Sigma_i$ is diffeomorphic to $\mathbb R^3\setminus\overline B(R_i)$. For some $k\geq2$, $0<\alpha\leq1$, $0<\lambda\leq1$ and end-dependent $C$, each has a neighborhood chart with $r=|x|$, $g_{00}<-C^{-1}$, $|g_{\mu\nu}-\eta_{\mu\nu}|\leq Cr^{-\alpha}$, $g_{ij}v^iv^j\geq C^{-1}|v|^2$ and $|\partial^j g_{\mu\nu}|\leq Cr^{-\alpha-j}$ for $1\leq j\leq k$. Order-$k$ derivatives have difference bound $Cr^{-\alpha-k-\lambda}(|t-\tau|^\lambda+|x-y|^\lambda)$ for $|t-\tau|\leq1$ and $|x-y|\leq r(x)/2$. The sphere bounding each end is identified diffeomorphically with a connected boundary component of its complementary portion. A Killing field $X$ is complete on $M$, uniformly timelike on each end, tangent to $S$, and in each chart is $(A_i+O(r^{-\alpha}))\partial_t+O(r^{-\alpha})\partial_{x^i}$ with $A_i\ne0$. These are Definitions 2.1 and 2.3, called class (b); the definition does not require $X=0$ on $S$ or a bifurcate Killing horizon. Set $M_i=\bigcup_{t\in\mathbb R}\phi_t(\Sigma_i)$, $M_{\rm ext}=\bigcup_iM_i$, $B=M\setminus I_M^-(M_{\rm ext})$, $W=M\setminus I_M^+(M_{\rm ext})$. Let $D(\Sigma)$ use the source's inextendible-timelike-curve convention and put $U=\operatorname{int}D(\Sigma)$. Require $(B\cup W)\cap U=\varnothing$.

[F2] The declared definitions supply stationary Lorentzian geometry, ambient chronological relations, spacelike maximality and differentiated end bounds. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F3] The five intermediate lemmas explain the quantitative end interface, invariant compact boundary, precise exclusion test, isometry covariance and graph decay limitations. [lem-author-9e5789a3d617-end-holder-interface](item-lem-author-9e5789a3d617-end-holder-interface) [lem-author-9e5789a3d617-compact-boundary-flow](item-lem-author-9e5789a3d617-compact-boundary-flow) [lem-author-9e5789a3d617-exterior-exclusion-interface](item-lem-author-9e5789a3d617-exterior-exclusion-interface) [lem-author-9e5789a3d617-maximal-isometry-covariance](item-lem-author-9e5789a3d617-maximal-isometry-covariance) [lem-author-9e5789a3d617-graph-decay-translation](item-lem-author-9e5789a3d617-graph-decay-translation)

### External input

Import Chruściel–Wald Theorem 4.2 under exactly [F1], with asymptotic flatness in their Definition 2.4 and source domain-of-dependence/Cauchy convention. This is an existence and covariance input; its nonlinear elliptic existence argument is not reconstructed here. The five authored local lemmas establish the indicated interfaces and consequences but are not represented as a proof of the existence theorem. For an application with the explicit additional mathematical hypothesis $\operatorname{Ric}(g)=0$, one has $\operatorname{Ric}(Z,Z)=0\geq0$ for every timelike $Z$. Thus the timelike-convergence alternative applies once the class-(b) and exclusion hypotheses have been established.

### Source notes

Neither the imported existence theorem nor the local graph estimate supplies stronger differentiated decay, a zero-height end gauge, or an identification of $U$ with a separately specified exterior. Consumers must establish these additional application obligations. Strong causality here is an ambient hypothesis, not merely a property of a smaller exterior. No source bifurcation-surface hypothesis has been inserted into class (b). The source defines $D$ using inextendible timelike curves (p.8); this item retains that convention rather than silently substituting the local causal-curve formulation.


## Closed Ernst contraction and the real potential

[Open item](item-lem-author-cea8e61dc3c6-closed-ernst-contraction) · level 3


### Statement

For Ricci-flat stationary Lorentzian data, put $F_{ab}=\nabla_aT_b$, $\mathcal F=F+i\star_gF$, and $\eta=2\iota_T\mathcal F$, where $(\iota_T\mathcal F)_b=T^a\mathcal F_{ab}$. Then $d\eta=0$ and $\operatorname{Re}\eta=d(-g(T,T))$. There are smooth complex potentials locally. On an open set where $\eta=d\sigma$, $\operatorname{Re}\sigma=-g(T,T)$ up to one real constant on each connected component.

### Facts & Assumptions

[F1] The fields, metric connection, and scalar $f=-g(T,T)$ are defined in [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] Use $\mathcal F=F+i\star_gF$ with complex-linear Hodge star. [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)

[F3] The real Killing two-form satisfies $dF=0$. [lem-author-cea8e61dc3c6-killing-exact-two-form](item-lem-author-cea8e61dc3c6-killing-exact-two-form)

[F4] Ricci flatness implies $\nabla^aF_{ab}=0$. [lem-author-cea8e61dc3c6-vacuum-killing-divergence](item-lem-author-cea8e61dc3c6-vacuum-killing-divergence)

[F5] Vanishing divergence of a two-form implies closedness of its Hodge dual. [lem-author-cea8e61dc3c6-divergence-hodge-closure](item-lem-author-cea8e61dc3c6-divergence-hodge-closure)

[F6] The complex Killing two-form satisfies $\mathcal L_T\mathcal F=0$. [lem-author-cea8e61dc3c6-killing-flow-invariance](item-lem-author-cea8e61dc3c6-killing-flow-invariance)

[F7] The Cartan identity is $\mathcal L_T\omega=d\iota_T\omega+\iota_Td\omega$, and is extended complex linearly. [math:thm-cartans-magic-formula](https://alphabetamath.cc/item/thm-cartans-magic-formula)

[F8] Every closed smooth real one-form on a star-shaped coordinate domain has a potential by the Poincare lemma. [math:thm-poincare-lemma-for-star-shaped-domains](https://alphabetamath.cc/item/thm-poincare-lemma-for-star-shaped-domains)

[F9] Use real exterior differentiation defined by the invariant vector-field formula. For a complex form written in its unique real and imaginary parts as $U+iV$, define $d(U+iV)=dU+i\,dV$ and $\iota_T(U+iV)=\iota_TU+i\iota_TV$, including degree zero for $d$. These are componentwise extensions, with $T$ real. [math:def-exterior-derivative-by-the-invariant-vector-field-formula](https://alphabetamath.cc/item/def-exterior-derivative-by-the-invariant-vector-field-formula)

[F10] On a smooth real function $h$, exterior differentiation is the ordinary differential: $dh(X)=Xh$. [math:prop-exterior-derivative-of-a-function-is-its-differential](https://alphabetamath.cc/item/prop-exterior-derivative-of-a-function-is-its-differential)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove all asserted identities under these hypotheses.

1.1 Each term in the invariant formula [F9] is real-linear in the form, so $d(aU+bV)=a\,dU+b\,dV$ for real constants $a,b$. Consequently the componentwise extension in [F9] is complex-linear and commutes with taking real and imaginary parts. Applying the real Cartan identity separately to those parts gives [F7] for complex forms. By [F3]–[F5], $d\mathcal F=dF+i\,d\star_gF=0$. Applying [F7] and then [F6] gives $d\eta=2(\mathcal L_T\mathcal F-\iota_Td\mathcal F)=0$. By [F10], metric compatibility and the antisymmetry of $F$ give $(df)_b=-2T^a\nabla_bT_a=2T^aF_{ab}=\operatorname{Re}\eta_b$. [F1, F2, F3, F4, F5, F6, F7, F9, F10, algebra]

2.1 Restrict to a coordinate ball; its image is star-shaped. By step 1.1, both real and imaginary parts of $\eta$ are closed smooth real one-forms. Evaluating the invariant formula [F9] on commuting coordinate vector fields identifies closedness of either real one-form with $\partial_jA_k=\partial_kA_j$ for its real coefficient field $A$. Thus their coefficient fields meet the closed $C^1$ hypotheses of [F8], which supplies real potentials whose complex combination is a local $\sigma$. Their first partial derivatives are smooth components of $\eta$, so these potentials are smooth. Wherever a global primitive is assumed, step 1.1 and [F9]–[F10] give $d(\operatorname{Re}\sigma-f)=0$. This difference is constant on each coordinate ball by integrating its zero derivative along segments, and hence locally constant. On each connected component it is constant, since every nonempty fiber of a locally constant function is open and closed. No assertion that all periods vanish is used. [step 1.1, F1, F8, F9, F10, algebra] ∎

## Metric transport along a null generator

[Open item](item-lem-author-254b7c4bab6d-null-metric-transport) · level 3


### Statement

On the null branch with generator $L$ in [lem-author-254b7c4bab6d-null-form-screen-descent](item-lem-author-254b7c4bab6d-null-form-screen-descent), write $q=g|_{TH}$. For tangent fields $X,Y$, $(\mathcal L_Lq)(X,Y)=2B(X,Y)$. Thus vanishing $B$ means preservation of the degenerate tangent metric along the local generator flow. The zero-trace condition remains invariant under the rescalings in [lem-author-254b7c4bab6d-null-expansion-rescaling](item-lem-author-254b7c4bab6d-null-expansion-rescaling); no implication from zero trace to vanishing $B$ is asserted here. The Lie derivative and connection conventions are those of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

### Facts & Assumptions

[F1] The descended null form is symmetric; the ambient connection is torsion-free and metric-compatible. Positive rescaling multiplies the expansion. [lem-author-254b7c4bab6d-null-form-screen-descent](item-lem-author-254b7c4bab6d-null-form-screen-descent) [lem-author-254b7c4bab6d-null-expansion-rescaling](item-lem-author-254b7c4bab6d-null-expansion-rescaling) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] For any smooth tensor on a smooth manifold, its Lie derivative along a smooth vector field is the derivative at zero of pullback by its local flow. It obeys the tensor-product rule, commutes with contractions, acts on functions by directional differentiation, and acts on vector fields by the Lie bracket. Apply these facts on $H$ to the smooth covariant two-tensor $q$ and the tangent generator $L$; no nondegeneracy of $q$ is required. [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field) [math:thm-lie-derivative-is-a-derivation-of-the-tensor-algebra](https://alphabetamath.cc/item/thm-lie-derivative-is-a-derivation-of-the-tensor-algebra) [math:prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields](https://alphabetamath.cc/item/prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields)

[F3] On every common local flow domain, a smooth tensor has zero Lie derivative if and only if its pullback by each defined flow map equals the tensor. Apply this to $q$ and the local flow of $L$ on $H$; completeness of $L$ is not assumed. [math:prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes](https://alphabetamath.cc/item/prop-a-tensor-field-is-invariant-under-a-flow-if-and-only-if-its-lie-derivative-vanishes)

### Proof

**Given:** The branch, tangent metric and generator in the Statement.

**Goal:** Compute the Lie derivative and its stated consequence.

1.1 Regard $q(X,Y)$ as the contraction of $q\otimes X\otimes Y$. The derivation and contraction rules in F2 give $L(q(X,Y))=(\mathcal L_Lq)(X,Y)+q([L,X],Y)+q(X,[L,Y])$. Thus $(\mathcal L_Lq)(X,Y)=L(g(X,Y))-g([L,X],Y)-g(X,[L,Y])$. The brackets here are intrinsic to $H$; ambient extensions of tangent fields give the same brackets on $H$. Replacing each bracket by its torsion-free connection expression and expanding the first term by metric compatibility leaves $g(\nabla_XL,Y)+g(X,\nabla_YL)$. [given, F1, F2]

2.1 Symmetry of $B$ makes this sum $2B(X,Y)$. Hence $B=0$ gives $\mathcal L_Lq=0$. By F3, for the local generator flow $\Phi_t$ this implies $\Phi_t^*q=q$ on every common local flow domain, proving preservation of the degenerate tangent metric. The rescaling statement follows from F1 and asserts only invariance of zero trace. [F1, F3, step 1.1] ∎


## Regular Lorentzian metric from the normalized rank-one map

[Open item](item-lem-author-7a3c9628f105-rank-one-metric) · level 3


### Statement

Assume the normalized family in [lem-author-7a3c9628f105-primitive-parameter-lift](item-lem-author-7a3c9628f105-primitive-parameter-lift), with $D_q>0$ and $D_q(p)>0$. Define $A_qv=v+D_q^{-1}W_q(v)T$ and $g_q=(D_q/4)A_q^*g$. Then $A_q$ is orientation preserving and invertible, $g_q$ is Lorentzian and smooth through $f=0$, and $g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-(f/D_q)W_q\otimes W_q)$. Also $g_1=g$ and $g_q(T,T)=D_q(p)^2g(T,T)/(4D_q)$; in particular its sign is unchanged.

### Facts & Assumptions

[F1] Metric duals and $f$ use [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data), and fiberwise algebraic pullbacks use [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data).

[F2] The one-forms and their contraction normalization are supplied by [lem-author-7a3c9628f105-primitive-parameter-lift](item-lem-author-7a3c9628f105-primitive-parameter-lift).

[F3] The smooth denominator is $D_q=|1+q-(1-q)\sigma|^2$ for the smooth scalar $\sigma=f+i\psi$ and $q\in[0,1]$, as in [lem-author-7a3c9628f105-denominator-positivity](item-lem-author-7a3c9628f105-denominator-positivity). In particular, evaluating its defining formula at $q=1$ gives $D_1=|2|^2=4$.

### Proof

**Given:**The hypotheses in the Statement and the Facts below.

**Goal:** Establish the stated conclusions.

1.1 Write $D=D_q$, $C=D_q(p)$ and $W=W_q$. Since $D+W(T)=C$, direct multiplication gives $(I+T\otimes W/D)^{-1}=I-T\otimes W/C$. If $T\ne0$, a basis starting with $T$ makes this rank-one map triangular with diagonal $(C/D,1,1,1)$; if $T=0$, it is the identity and $C=D$. Thus its determinant is $C/D>0$. Invertible algebraic pullback and positive rescaling preserve Lorentz signature. [given, F1, F2]

2.1 Expanding $g(A_qu,A_qv)$ gives the stated tensor formula because $g(T,T)=-f$. Its only denominator is the positive $D_q$, so it is smooth through $f=0$. The identity $W_1=0$ from [F2] and the evaluation $D_1=4$ in [F3] give $g_1=g$. Finally $A_qT=(C/D)T$, hence the asserted contraction and sign identity. All coefficients are smooth in $q$ and spacetime wherever $D_q>0$. [given, F1, F2, F3, algebra, step 1.1] ∎

### Source notes

This conditional calculation follows §3.2 (3.11), (3.20)–(3.23) of the cited independent source. No existence of the stationary primitive or Einstein–Maxwell solution is inferred from this calculation alone.


## Exact bifurcate-sphere package for the IK criterion

[Open item](item-def-author-9f9c6144aed8-ik-sbs) · level 3


### Definition

For the end, section and exterior in [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af), set $S_0=\partial I^-(M^{\mathrm{end}})\cap\partial I^+(M^{\mathrm{end}})$. The **IK SBS package** requires $S_0\subset\Sigma_0$ to be an embedded two-sphere equal to $|x|=1$ under the chosen identification of $\Sigma_0$ with $\{|x|>1/2\}$. In a neighborhood $O$ of $S_0$, require $H^+=O\cap\partial I^-(M^{\mathrm{end}})$ and $H^-=O\cap\partial I^+(M^{\mathrm{end}})$ to be smooth embedded null hypersurfaces, each diffeomorphic to $S_0\times(-1,1)$, intersecting transversely in $S_0$. Require both to be non-expanding, meaning their null second fundamental forms have zero trace. Here the null second fundamental form is $\chi_L(X,Y)=g(\nabla_X L,Y)$ on the two-dimensional spacelike quotient of a null hypersurface by its null normal line, for a smooth nonzero null normal $L$; its trace uses the quotient's induced positive metric. Finally $T$ is tangent to both branches and is not identically zero on $S_0$. Nullness and transversality follow the conventions in [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data); this package does not require $T$ itself to be a null generator.

### Facts & Assumptions

[F1] The AF package fixes the ambient smooth time-oriented Lorentzian four-manifold, end, section, exterior and stationary field, with the inherited ZFC conventions. [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af)

[F2] A smooth null hypersurface has a tangent metric with nonzero radical; its null normal line is that radical. The embeddedness and transversality conventions are those of [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data). No Killing generator is assumed for either branch here.

[F3] The ambient metric has signature $(-,+,+,+)$, and its Levi–Civita connection is torsion-free and metric-compatible: $Xg(U,V)=g(\nabla_XU,V)+g(U,\nabla_XV)$ and $\nabla_XY-\nabla_YX=[X,Y]$. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F4] For a smooth null hypersurface whose tangent metric is positive semidefinite of rank two, the normal-screen supplier gives the smooth positive quotient $L^\perp/\mathbb RL$ and its identification with a transverse spacelike section. Derivatives of fields along the hypersurface use the pullback connection. Its Countable Choice assumption is supplied by the inherited ZFC convention. Only these clauses of [physics:lem-gr-fx-null-normal-plane-and-screen](https://alphabetamath.cc/physics/item/lem-gr-fx-null-normal-plane-and-screen) are used; its affine-generator descent clause is replaced by the local argument below.

[F5] A smooth vector bundle map over the identity of a smooth base with constant fibre rank has a smooth kernel subbundle. In particular, a rank-two map from a rank-three bundle has a smooth rank-one kernel, with smooth nonzero local sections. [math:prop-constant-rank-kernels-and-images-of-bundle-maps-over-one-base-are-subbundles](https://alphabetamath.cc/item/prop-constant-rank-kernels-and-images-of-bundle-maps-over-one-base-are-subbundles)

### Justification

**Given:** Either smooth null branch $H$ in the Definition, with its ambient Lorentzian metric and Levi–Civita connection. Work locally on $H$; the smooth nonzero null normal $L$ used below will be obtained in step 1.1.

1.1 At a point $p$, nondegeneracy of the ambient metric and codimension one give $\dim (T_pH)^\perp=1$. Choose a nonzero vector $L_p$ in the radical. Then $(T_pH)^\perp=\mathbb RL_p$ and $T_pH=L_p^\perp$. In a basis with metric $-(dx^0)^2+|dx|^2$, write $L_p=a(1,u)$ with $a\ne0$ and $|u|=1$. Every vector of $L_p^\perp$ is uniquely $(b,bu+v)$ with $u\cdot v=0$, and its squared norm is $|v|^2$. Thus the tangent metric is positive semidefinite of rank two with radical exactly $\mathbb RL_p$. View the induced metric as the smooth bundle map $b_H:TH\to T^*H$, $b_H(v)=g(v,\cdot)|_{TH}$. Its fibre rank is two by the preceding calculation, and its kernel is the radical. By F5 this kernel is a smooth line subbundle; choose a smooth nowhere-zero local section $L$. The quotient and its positive metric are therefore those in F4, reversing the sign of a local normal if needed for that supplier's future convention. In particular $\bar\gamma([X],[Y])=g(X,Y)$ is independent of representatives and positive definite. [given, F1, F2, F3, F4, F5, algebra]

2.1 For smooth tangent fields $X$ on $H$, the bracket $[L,X]$ is tangent to $H$. Metric compatibility and torsion freedom give $g(\nabla_LL,X)=-g(L,\nabla_LX)=-g(L,\nabla_XL+[L,X])=-\frac12Xg(L,L)=0$. Hence $\nabla_LL$ lies in $(TH)^\perp=\mathbb RL$: there is a smooth local scalar $\kappa$ with $\nabla_LL=\kappa L$. Smoothness follows by dividing a nonvanishing component of $L$ into the corresponding smooth component of $\nabla_LL$. This derives the required pregeodesic property for every such normal; it imposes no affine parametrization or Killing assumption. [given, F2, F3, step 1.1]

3.1 The pullback derivative $\nabla_XL$ depends only on $L$ along $H$: two smooth ambient extensions differ by a field vanishing on $H$, whose derivative in each tangent direction also vanishes there. The expression $\chi_L(X,Y)=g(\nabla_XL,Y)$ is bilinear in the tangent vectors. Metric compatibility gives $\chi_L(X,L)=\frac12Xg(L,L)=0$, while step 2.1 gives $\chi_L(L,Y)=\kappa g(L,Y)=0$. Changing either representative by a multiple of $L$ therefore leaves $\chi_L$ unchanged. It is symmetric because $\chi_L(X,Y)-\chi_L(Y,X)=-g(L,\nabla_XY-\nabla_YX)=-g(L,[X,Y])=0$. Thus it defines a smooth symmetric form on $TH/\mathbb RL$, and its trace uses the inverse of the positive quotient metric established in step 1.1. [given, F2, F3, F4, step 1.1, step 2.1]

4.1 Any other nonzero local normal is $fL$ for a smooth nowhere-zero function $f$. The connection product rule gives $\chi_{fL}(X,Y)=f\chi_L(X,Y)+X(f)g(L,Y)=f\chi_L(X,Y)$. The quotient metric is unchanged, so the trace is multiplied by $f$ and its vanishing is independent of the chosen local normal. This makes the non-expansion predicate well-defined on both branches. The remaining clauses prescribe embedded sets and tangencies without asserting existence of a horizon generator Killing field. [given, F1, F2, F3, step 1.1, step 3.1] ∎

### External input

The independent [Ionescu–Klainerman source](https://arxiv.org/pdf/0711.0040) supplies the SBS predicates in section 1.2, SBS and footnotes 5–6, printed/PDF p. 7. Only this geometric definition package is imported. The quotient well-definedness and normal-rescaling argument above are local; no existence, vacuum field equation or analytic theorem is inferred from recording these predicates.


## Stationary transport of vanishing from a section

[Open item](item-lem-author-9f9c6144aed8-stationary-zero-transport) · level 3


### Statement

Use the IK AF package, with exterior $E$ and section $\Sigma_0$, and let $\Phi:\mathbb R\times E\to E$ be the complete stationary flow. Let $S$ be a smooth tensor field on $E$ of any fixed type $(r,s)$, where $r,s$ are nonnegative integers, with real or complex values. Use the diffeomorphism pullback specified below, extended to complex values by applying it to the real and imaginary parts. If $\Phi_t^*S=S$ for every real $t$ and $S=0$ on $\Sigma_0\cap E$, then $S=0$ on $E$.

For application to the Mars–Simon tensor, additionally establish or import $E\subseteq N=\{1-\sigma\ne0\}$, where $\sigma$ is the supplied Ernst potential, and establish or import flow invariance of that tensor. Its definition supplies a complex covariant four-tensor only on $N$. Neither domain inclusion nor preservation follows merely from vanishing on the section.

### Statement references

[def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af)

[def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)

[math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains](https://alphabetamath.cc/item/prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains)

[math:def-smooth-tensor-field](https://alphabetamath.cc/item/def-smooth-tensor-field)

[math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space)

[math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

[math:prop-a-diffeomorphism-pulls-back-tensor-fields-and-forms-isomorphically](https://alphabetamath.cc/item/prop-a-diffeomorphism-pulls-back-tensor-fields-and-forms-isomorphically)

[math:cor-the-differential-of-a-diffeomorphism-is-an-isomorphism](https://alphabetamath.cc/item/cor-the-differential-of-a-diffeomorphism-is-an-isomorphism)

### Facts & Assumptions

[F1] Every stationary orbit through $E$ is complete and meets the section. The flow in the Statement is on $E$, so its section intersection lies in $\Sigma_0\cap E$. [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af)

[F2] Each time-$t$ map of a smooth maximal flow is a diffeomorphism between its open domains, with inverse the time-$(-t)$ map. Applied to the complete flow on $E$, these domains are both $E$. [math:prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains](https://alphabetamath.cc/item/prop-time-t-flow-maps-are-diffeomorphisms-between-open-domains)

[F3] A smooth type-$(r,s)$ tensor field is a smooth section of its tensor bundle; each real fiber tensor is a multilinear map on $r$ cotangent and $s$ tangent arguments. Complex values mean a pair of real tensors, with all constructions applied componentwise. [math:def-smooth-tensor-field](https://alphabetamath.cc/item/def-smooth-tensor-field) [math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space)

[F4] For covariant fields, $(f^*S)_q(v_1,\ldots,v_s)=S_{f(q)}(df_qv_1,\ldots,df_qv_s)$. If $f$ is a diffeomorphism, this pullback has inverse $(f^{-1})^*$. [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field) [math:prop-a-diffeomorphism-pulls-back-tensor-fields-and-forms-isomorphically](https://alphabetamath.cc/item/prop-a-diffeomorphism-pulls-back-tensor-fields-and-forms-isomorphically)

[F5] For a diffeomorphism $f$ the differential $A=df_q$ is a linear isomorphism. The mixed-tensor pullback convention used here is $(f^*S)_q(\alpha_1,\ldots,\alpha_r,v_1,\ldots,v_s)=S_{f(q)}(\alpha_1\circ A^{-1},\ldots,\alpha_r\circ A^{-1},Av_1,\ldots,Av_s)$, where $\alpha_i\in T_q^*E$ and $v_j\in T_qE$. This defines a multilinear tensor and agrees with the covariant construction when $r=0$. [math:cor-the-differential-of-a-diffeomorphism-is-an-isomorphism](https://alphabetamath.cc/item/cor-the-differential-of-a-diffeomorphism-is-an-isomorphism) [math:def-type-r-s-tensor-on-a-finite-dimensional-vector-space](https://alphabetamath.cc/item/def-type-r-s-tensor-on-a-finite-dimensional-vector-space)

[F6] The Mars–Simon tensor formula defines a smooth complex covariant four-tensor on the open set $N=\{1-\sigma\ne0\}$; its restriction to all of $E$ therefore requires $E\subseteq N$. [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon)

### Proof

**Given:** The flow-invariant real or complex type-$(r,s)$ tensor on $E$ and its vanishing on $\Sigma_0\cap E$.

**Goal:** Show $S_p=0$ for every $p\in E$.

1.1 Each $\Phi_t:E\to E$ is a diffeomorphism with inverse $\Phi_{-t}$. In particular $d\Phi_t|_q:T_qE\to T_{\Phi_t(q)}E$ is a linear isomorphism at every $q\in E$. [given, F2, F5]

1.2 Fix $p\in E$. By the orbit-section assumption, choose $q\in\Sigma_0\cap E$ and $t\in\mathbb R$ such that $p=\Phi_t(q)$. Invariance and section vanishing give $(\Phi_t^*S)_q=S_q=0$. [given, F1, choose]

2.1 Set $A=d\Phi_t|_q$. For arbitrary $\beta_i\in T_p^*E$ and $w_j\in T_pE$, insert $\alpha_i=\beta_i\circ A$ and $v_j=A^{-1}w_j$ into the mixed-pullback formula. It gives $S_p(\beta_1,\ldots,\beta_r,w_1,\ldots,w_s)=(\Phi_t^*S)_q(\beta_1\circ A,\ldots,\beta_r\circ A,A^{-1}w_1,\ldots,A^{-1}w_s)=0$. Thus every evaluation is zero, so $S_p=0$. This also covers $r=0$ with the covariant pullback and its inverse, and $r=s=0$ with empty argument lists. Applying the same argument to the real and imaginary parts proves the complex case. Since $p$ was arbitrary, $S=0$ on $E$. [F3, F4, F5, step 1.1, step 1.2, algebra] ∎


## Coordinate cones and the separate stationary generator

[Open item](item-lem-author-4cb89398a4ab-end-coordinate-cones) · level 3


### Statement

For an end satisfying the exact asymptotically stationary end contract, the coordinate vector $\partial_t$ is uniformly timelike on $O_1$, and every nonzero vector tangent to a coordinate level set of $t$ in $O_1$ is spacelike. The separate hypothesis $g(T,T)<-C^{-1}$ on $\Sigma_1$ concerns the complete stationary generator $T$, not merely $\partial_t$. If a second Killing field $K$ and a Killing horizon $H$ for $K$ are supplied, meaning that $H$ is a smooth embedded null hypersurface and $K$ is tangent and normal on its nonempty dense nonzero part, the end conditions do not imply that $K$ is timelike on $\Sigma_1$ or $O_1$. This non-implication holds even if $K$ is complete.

### Statement references

[def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end)

[def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

### Facts & Assumptions

[F1] The end contract supplies $g_{00}<-C^{-1}$, $g_{ij}Z^iZ^j\ge C^{-1}|Z|^2$ and the separate uniform timelikeness condition for $T$ on $\Sigma_1$. It also supplies the smooth time-oriented Lorentzian and causal conventions, the acausal hypersurface and its smooth end/remainder realization, the remaining coordinate estimates on $O_1$, and the completeness and asymptotics of $T$. [def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end)

[F2] A Killing horizon for a specified Killing field $K$ is a smooth embedded null hypersurface on whose nonempty dense nonzero-generator part $K$ is tangent and normal. The null normal line is the radical of the induced metric. This definition asserts no relation between $K$ and the stationary field $T$, and imposes no field equation. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

### Proof

**Given:** An end and coordinates satisfying [F1]; any additional horizon and field use [F2].

**Goal:** Prove the coordinate-cone conclusions and exhibit an end with a complete horizon-normal field that is not timelike on that end.

1.1 Since $g(\partial_t,\partial_t)=g_{00}<-C^{-1}$ on $O_1$, the coordinate time vector is uniformly timelike there. [F1]

1.2 A nonzero tangent vector to $t=\mathrm{constant}$ has the form $v=\sum_iZ^i\partial_{x^i}$ with $Z\ne0$, so $g(v,v)=g_{ij}Z^iZ^j\ge C^{-1}|Z|^2>0$. The bound on $g(T,T)$ is separately imposed in end clause (3), on $\Sigma_1$. [F1]

1.3 For the countermodel take $M=\mathbb R^4$ with its standard smooth structure and orientation, $g=-dt^2+(dx^1)^2+(dx^2)^2+(dx^3)^2$, time orientation $N=\partial_t$, and $T=\partial_t$. Set $\Sigma=\{t=0\}$, $\Sigma_1=\{t=0,\ |x|>1\}$, $\Sigma'=\{t=0,\ |x|\le1\}$ and $O_1=\{(t,x):|x|>1\}$. These are the standard embedded hyperplane, open exterior and closed ball, with their usual smooth structures. For a future causal vector $(a,b)$, the metric and orientation give $a\ge|b|$ and $a>0$. Thus along every nonconstant future causal curve the locally absolutely continuous coordinate $t$ is strictly increasing, by integrating its positive almost-everywhere derivative on any compact parameter subinterval. Consequently $\Sigma$ is acausal. [F1, construct]

2.1 Take $R_1=1$, $E=\{z:|z|>1\}$, $\overline E=\{z:|z|\ge1\}$, $e(z)=(0,z)$, $j(z)=(0,z)$ and $h=j|_{\partial\overline E}$. The sphere $S=\partial\Sigma'=\{t=0,|x|=1\}$ is connected; $h$ is a diffeomorphism onto $S$, $j(\overline E)\cap\Sigma'=S$ and $j(\overline E)\cup\Sigma'=\Sigma$. With $C=2$, $k=2$, $\alpha=\lambda=1$, all metric differences, positive-order derivatives and Hölder differences in end clause (1) vanish. Its remaining bounds are $-1<-1/2$ and $|Z|^2\ge|Z|^2/2$, and $r>1$ throughout $O_1$. The complete flow $\phi_u(t,x)=(t+u,x)$ preserves $g$, so $T$ is Killing, $g(T,T)=-1<-1/2$, and the asymptotics hold with $A=1$ and zero error. This verifies all three end clauses. [F1, step 1.3, construct]

3.1 Define $K=\partial_t+\partial_{x^1}$ and $H=\{t=x^1\}$. Its flow $\psi_u(t,x^1,x^2,x^3)=(t+u,x^1+u,x^2,x^3)$ is defined for all real $u$ and preserves the constant metric, so $K$ is a complete Killing field distinct from $T$. The map $(s,y,z)\mapsto(s,s,y,z)$ smoothly embeds $\mathbb R^3$ onto $H$; the induced form is $dy^2+dz^2$, with radical spanned by the everywhere nonzero tangent vector $K$. Equivalently, $g(K,\cdot)=-dt+dx^1$ annihilates $TH$. Thus $H$ is a Killing horizon for $K$ under [F2]. But $g(K,K)=-1+1=0$ everywhere, including on $\Sigma_1$ and $O_1$. The fully verified end therefore does not force even pointwise timelikeness of a separate complete horizon-normal field, while retaining all coordinate and stationary bounds. [F1, F2, step 1.1, step 1.2, step 1.3, step 2.1] ∎



## Complete stationary saturation of the end

[Open item](item-lem-author-4cb89398a4ab-complete-end-saturation) · level 3


### Statement

For the complete stationary action $\phi_u$ of [def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end), define the saturated end by $M_{\mathrm{end}}=\bigcup_{u\in\mathbb R}\phi_u(\Sigma_1)$. Then $\phi_v(M_{\mathrm{end}})=M_{\mathrm{end}}$ for every $v\in\mathbb R$, and $T$ is timelike everywhere on $M_{\mathrm{end}}$. The saturation uses $T$ and need not be defined using a different horizon generator.

### Facts & Assumptions

[F1] The end contract supplies a complete group of isometries generated by $T$, with $g(T,T)<-C^{-1}$ on $\Sigma_1$. [def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end)

### Proof

**Given:** The complete action and saturated end in the Statement.

**Goal:** Establish saturation invariance and timelikeness on the saturation.

1.1 The group law gives $\phi_v(M_{\mathrm{end}})=\bigcup_{u\in\mathbb R}\phi_{v+u}(\Sigma_1)=M_{\mathrm{end}}$, since translation by $v$ is a bijection of $\mathbb R$. Completeness supplies every parameter used here. [F1]

2.1 Differentiating $\phi_v(\phi_u(p))=\phi_{v+u}(p)$ at $u=0$ gives $(d\phi_v)_pT_p=T_{\phi_v(p)}$. Since $\phi_v$ is an isometry, $g(T,T)(\phi_v(p))=g(T,T)(p)$. For $p\in\Sigma_1$ this is negative, proving timelikeness on its full saturation. Both assertions concern the specified stationary action only. [F1, step 1.1] ∎


## Horizon smallness is the induced norm of the tangential stationary field

[Open item](item-lem-author-0a41d659d5ab-horizon-field-norm) · level 3


### Statement

For the AIK quantitative package, $g(T,T)=-n^2+h(X,X)$ on $\Sigma_0$. On $S_0$ the stationary field is tangent to $S_0$, $n=0$ and $X=T$. Consequently $g(T,T)=|T|_h^2\ge0$ there and $\sup_{S_0}|g(T,T)|<\epsilon^2$ is exactly $\sup_{S_0}|T|_h<\epsilon$ for $\epsilon>0$. The norm is the induced Riemannian norm on the spacelike sphere, not an unspecified Lorentzian vector norm.

### Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The GR/SBS package fixes the transverse horizon intersection and the tangencies of $T$. [def-author-0a41d659d5ab-aik-quantitative-package](item-def-author-0a41d659d5ab-aik-quantitative-package)

[F2] The unique normal/shift decomposition is $T=n\nu+X$, with $g(\nu,\nu)=-1$ and $g(X,\nu)=0$. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F3] For transverse embedded submanifolds, the tangent space of their intersection is the intersection of their tangent spaces. [math:cor-transverse-intersection-theorem](https://alphabetamath.cc/item/cor-transverse-intersection-theorem)

[F4] The Euclidean unit sphere in $\mathbb R^3$ is compact. [math:cor-euclidean-closed-balls-and-spheres-are-compact](https://alphabetamath.cc/item/cor-euclidean-closed-balls-and-spheres-are-compact)

[F5] Continuous images of compact spaces are compact, and a continuous real-valued function on a nonempty compact space attains its maximum and minimum. [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conditional conclusion.

1.1 The decomposition in [F2] gives $g(T,T)=n^2g(\nu,\nu)+2ng(\nu,X)+g(X,X)=-n^2+h(X,X)$. At a point $p\in S_0$, [F1] supplies $T_p\in T_pH^+\cap T_pH^-$, and transversality allows [F3] to identify this intersection with $T_pS_0$. Since $S_0\subset\Sigma_0$, it follows that $g(T,\nu)=0$, hence $n=0$ and $X=T$. [F1, F2, F3, algebra]

2.1 The package identifies $S_0$ as the image of the nonempty unit sphere $\{x\in\mathbb R^3:|x|=1\}$ under the smooth map $\Phi_0$. The unit sphere is compact by [F4], so its continuous image $S_0$ is nonempty and compact by [F5]. The induced metric is positive definite, and the function $f(p)=|T_p|_h=\sqrt{h_p(T_p,T_p)}$ is continuous: in local coordinates its square is a finite sum of products of smooth metric and field components, and the nonnegative square root is continuous. Thus [F5] gives a maximum $m=\max_{S_0}f\ge0$. [step 1.1, F1, F2, F4, F5]

3.1 By step 1.1, $g(T,T)=h(T,T)=f^2\ge0$ on $S_0$. Since $0\le f\le m$ and $f$ attains $m$, the increasing square function gives $\sup_{S_0}|g(T,T)|=m^2$ and $\sup_{S_0}|T|_h=m$. For $\epsilon>0$, $m^2<\epsilon^2$ holds exactly when $m<\epsilon$, proving the two strict smallness conditions equivalent. It does not identify either with ADM angular-momentum smallness. [step 1.1, step 2.1, algebra] ∎



## The quantitative asymptotic end is uniformly timelike

[Open item](item-lem-author-0a41d659d5ab-asymptotic-timelike-gap) · level 3


### Statement

For the AIK quantitative package, $g(T,T)\le-1/2$ on $\Sigma_{R_1}$. In particular the stationary field is timelike throughout that end, independently of the horizon-smallness parameter.

### Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The source end coordinates have $T=\partial_0$, $|g_{00}+1-2M_0/r|\le A_1r^{-2}$ and the chosen radius satisfies $R_1\ge8M_0$ and $R_1\ge2\sqrt{A_1}$. [def-author-0a41d659d5ab-aik-quantitative-package](item-def-author-0a41d659d5ab-aik-quantitative-package)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conditional conclusion.

1.1 On the end the stationary field is the coordinate vector $\partial_0$, so $g(T,T)=g_{00}$. The zeroth-order term of the quantitative end bound gives $g_{00}\le-1+2M_0/r+A_1/r^2$. [F1, given, algebra]

2.1 For $r\ge R_1$, the two positive terms are at most $1/4$ each by the chosen lower bounds on $R_1$. Hence $g(T,T)\le-1+1/4+1/4=-1/2$, as asserted. No horizon estimate enters this calculation. [step 1.1, F1, algebra] ∎


## Regular static boundary geometry and positivity of the end coefficient

[Open item](item-lem-author-f247c641a714-static-boundary-and-positive-mass) · level 3


### Statement

Assume the spatial static vacuum equations for the regular exterior data. Every boundary component is totally geodesic in $h$, and $|DV|_h$ is a positive constant on each component. Moreover
$$4\pi m=\int_X |DV|_h^2\,d\mu_h>0,$$
so $m>0$ follows from the original hypotheses and need not be added as a new assumption.

### Statement references

[def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)

[lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction)

[math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)

[math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)

[math:def-induced-connection-and-second-fundamental-form](https://alphabetamath.cc/item/def-induced-connection-and-second-fundamental-form)

[math:def-totally-geodesic-submanifold](https://alphabetamath.cc/item/def-totally-geodesic-submanifold)

[math:thm-collar-neighborhood-theorem](https://alphabetamath.cc/item/thm-collar-neighborhood-theorem)

[math:thm-monotone-convergence-for-the-integral](https://alphabetamath.cc/item/thm-monotone-convergence-for-the-integral)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)

[math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing)

[math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)

### Facts & Assumptions

[F1] The regular exterior data supply the connected oriented manifold with compact smooth boundary, the $C^2$ boundary metric and lapse, the single normalized end, and the inherited ZFC convention. The static reduction supplies $\Delta_hV=0$ and $D^2V=V\operatorname{Ric}(h)$, including their continuous boundary limits. The gradient, Hessian and divergence formulas fix the differential operators. [def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data) [lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction) [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)

[F2] Countable choice $\mathrm{AC}_\omega$ is included in the ZFC convention inherited in [F1]; it is used for the declared geometric and density-integration suppliers. Concretely, full choice applied to the family of values of a sequence of nonempty sets, followed by composition with that sequence, gives countable choice. [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F3] The normal-valued second fundamental form is $\mathrm{II}(A,C)=(D_AC)^\perp$, and total geodesicity means $\mathrm{II}=0$. The smooth definitions assume countable choice. At the present $C^2$ boundary their pointwise formulas are used with the $C^1$ Levi–Civita coefficients; their extension independence and the normal-form identification are checked in step 1.1, without assuming that $h$ is smooth at $B$. [math:def-induced-connection-and-second-fundamental-form](https://alphabetamath.cc/item/def-induced-connection-and-second-fundamental-form) [math:def-totally-geodesic-submanifold](https://alphabetamath.cc/item/def-totally-geodesic-submanifold)

[F4] Under countable choice a smooth manifold with boundary admits a smooth collar $c:B\times[0,1)\to\overline X$, a diffeomorphism onto a relative neighborhood of $B$ with $c(p,0)=p$. This is a smooth-manifold assertion, independent of boundary regularity of $h$. [math:thm-collar-neighborhood-theorem](https://alphabetamath.cc/item/thm-collar-neighborhood-theorem)

[F5] The divergence theorem under countable choice applies to every smooth vector field on a compact oriented smooth Riemannian manifold with smooth boundary, with its outward normal. Our applications are on domains contained in $X$, where $h,V$ are smooth; compactness makes the support condition automatic. [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)

[F6] On the smooth interior, $d\mu_h$ is the intrinsic Borel measure of the positive smooth density $\sqrt{\det h}\,|dx^1dx^2dx^3|$. Under countable choice the density measure has its coordinate integral formula, and its integration agrees with smooth density integration on compact smooth domains. In oriented coordinates this is also the volume-form integral used by [F5], since both have coefficient $\sqrt{\det h}$. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing) [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)

[F7] For any measure space, nonnegative measurable $f_j$ increasing pointwise to $f$ satisfy $\int f_j\,d\mu\uparrow\int f\,d\mu$, with no prior finiteness assumption. [math:thm-monotone-convergence-for-the-integral](https://alphabetamath.cc/item/thm-monotone-convergence-for-the-integral)

### Proof

**Given:** The regular static data and reduced equations of [F1], their inherited countable choice in [F2], the geometric interfaces [F3]–[F5], and the integration interfaces [F6]–[F7].

**Goal:** Prove the regular boundary geometry and the positive energy identity without assuming a positive end coefficient.

1.1 The boundary limit in [F1] is $D^2V=0$. Because $V|_B=0$ and $dV\ne0$ there, $DV$ is nonzero and normal to $B$. If $n$ is the inward unit normal, positivity of $V$ inside implies $n(V)>0$, so $DV=n(V)n$ on $B$. For tangent fields $A,C$, the Hessian formula gives $D^2V(A,C)=n(V)h(D_A n,C)$. Metric compatibility gives $h(D_AC,n)=-h(C,D_A n)$, and hence $\mathrm{II}(A,C)=-h(D_A n,C)n$. These identities remain valid for the stated boundary regularity: the inverse metric is $C^2$, its Christoffel coefficients are $C^1$, and $n=DV/|DV|$ on $B$ is $C^1$. In a boundary chart, two extensions of a tangent field differ by coefficients vanishing on $B$; their tangential derivatives also vanish there. The formula $D_AW=A(W^i)\partial_i+\Gamma^i{}_{jk}A^jW^k\partial_i$ therefore proves extension independence along $B$. Orthogonal projection onto the line spanned by $n$ gives exactly the normal-valued form in [F3]. Since $n(V)>0$ and $D^2V(A,C)=0$, this form vanishes, proving total geodesicity in the pointwise sense of [F3]. [given, F1, F2, F3]

1.2 Take the collar $c$ from [F4] and fix $0<t_0<1$. The strip $c(B\times[0,t_0])$ is compact. Choose $R_*$ so large that it and the compact core lie inside the region bounded by the end sphere $S_{R_*}$. For $R\ge R_*$ let $K_R$ be the complement in $\overline X$ of the end region $r>R$; it is compact by the compact-core hypothesis. Set $R_j=R_*+j$, $\varepsilon_j=t_0/(j+1)$ and $D_j=K_{R_j}\setminus c(B\times[0,\varepsilon_j))$. These are compact smooth domains entirely in $X$, with disjoint boundary faces $S_{R_j}$ and $B_{\varepsilon_j}=c(B\times\{\varepsilon_j\})$. They satisfy $D_j\subset D_{j+1}$ and $\bigcup_jD_j=X$: the end cutoff eventually includes each point, and the shrinking collar eventually excludes no fixed interior point. The product rule gives $\operatorname{div}_h(VDV)=|DV|_h^2+V\Delta_hV=|DV|_h^2$. Applying [F5] on $D_j$ therefore expresses its energy integral as the sum of its outer and inner fluxes. [given, F1, F2, F4, F5, F6]

2.1 For tangent $A$, metric compatibility and the Hessian formula give $A(|DV|_h^2)=2D^2V(A,DV)=0$ on $B$. Thus $|DV|_h^2$ is locally constant on $B$, and is constant on each connected component. Its value is positive there because $dV\ne0$. [given, F1, step 1.1]

2.2 The pullback metrics $c_s^*h$ on the compact $B$, for $0\le s\le t_0$, depend continuously on $(p,s)$ and are positive definite. Relative to $c_0^*h$ their area ratios are uniformly bounded by compactness. The latter has finite area by a finite boundary atlas and bounded continuous coordinate densities. Hence $\operatorname{Area}_h(B_s)\le C$. Also $V(c(p,s))=\int_0^s\partial_t(V\circ c)(p,t)\,dt=O(s)$ uniformly, and $|DV|_h$ is uniformly bounded on the strip by the $C^2$ data. With either unit normal on $B_s$, the absolute flux of $VDV$ is consequently at most $Cs$, so the inner flux for $D_j$ tends to zero. These estimates use the smooth collar and continuity on its compact strip, not a smooth-metric theorem at $B$. [given, F1, F4, step 1.2]

3.1 The differentiated end conditions give $\partial_rV=m/R^2+O(R^{-3})$, $DV=O(R^{-2})$ in the end Cartesian frame, the outward unit normal $\nu_h=\partial_r+O(R^{-1})$ in that frame, and $dA_h=(1+O(R^{-1}))R^2d\omega$. Since $V=1+O(R^{-1})$, the outer flux is $\int_{S_R}Vh(DV,\nu_h)\,dA_h=4\pi m+O(R^{-1})$. Combining this with the vanishing inner flux yields $\lim_j\int_{D_j}|DV|_h^2\,d\mu_h=4\pi m$. [given, F1, F5, F6, step 1.2, step 2.2]

4.1 The sets $D_j$ are Borel, and $f_j=\mathbf1_{D_j}|DV|_h^2$ are nonnegative measurable functions on the measure space $(X,\mathcal B(X),\mu_h)$ of [F6]. They increase pointwise to $|DV|_h^2$ by step 1.2. Monotone convergence [F7] and step 3.1 give $\int_X|DV|_h^2\,d\mu_h=4\pi m$, in particular a finite integral. To see strict positivity, fix a boundary point, where $|DV|_h>0$. Continuity supplies an interior coordinate ball on which $|DV|_h^2$ is bounded below by a positive constant. A smaller ball has positive $\mu_h$-measure by the positive continuous coordinate density in [F6]. The energy is therefore strictly positive, and $m>0$ follows. [given, F1, F6, F7, step 1.1, step 2.1, step 1.2, step 3.1] ∎



## Vacuum Killing and Ernst differential identities

[Open item](item-thm-vacuum-killing-ernst-input) · level 4


### Statement

For the stationary Lorentzian data with $\operatorname{Ric}(g)=0$, let $F_{ab}=\nabla_aT_b$ and $\mathcal F=F+i\star_gF$. Then $F=\tfrac12dT^\flat$, $\nabla^aF_{ab}=0$, $dF=d\star_gF=0$, and the complex one-form $\eta=2\iota_T\mathcal F$ is closed. It has smooth local potentials. On any domain where $\eta=d\sigma$, $\operatorname{Re}\sigma=-g(T,T)$ up to an additive real constant on each connected component. A single constant suffices on a connected domain. Global existence and normalization of a potential require a separate period or topology argument.

### Facts & Assumptions

[F1] The smooth oriented, time-oriented four-manifold, metric of signature $(-,+,+,+)$, Killing field, connection and curvature convention are those of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] The complex-linear Hodge star and complex self-dual form convention are those of [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data).

[F3] The Killing derivative is an exact closed two-form. [lem-author-cea8e61dc3c6-killing-exact-two-form](item-lem-author-cea8e61dc3c6-killing-exact-two-form)

[F4] Its divergence is $-\operatorname{Ric}_{bd}T^d$. [lem-author-cea8e61dc3c6-vacuum-killing-divergence](item-lem-author-cea8e61dc3c6-vacuum-killing-divergence)

[F5] A vanishing-divergence two-form has closed Hodge dual. [lem-author-cea8e61dc3c6-divergence-hodge-closure](item-lem-author-cea8e61dc3c6-divergence-hodge-closure)

[F6] The Killing flow preserves the complex two-form. [lem-author-cea8e61dc3c6-killing-flow-invariance](item-lem-author-cea8e61dc3c6-killing-flow-invariance)

[F7] In vacuum the Ernst contraction is closed, has real part $df$, and has local potentials; a primitive has real part $f$ plus componentwise constants. [lem-author-cea8e61dc3c6-closed-ernst-contraction](item-lem-author-cea8e61dc3c6-closed-ernst-contraction)

### Proof

**Given:**The data and hypotheses in the Statement.

**Goal:** Prove all asserted identities under these hypotheses.

1.1 The hypotheses give the geometric data required by [F3]–[F6]. By [F3], $F=\tfrac12dT^\flat$ and $dF=0$. Ricci flatness and [F4] give $\nabla^aF_{ab}=0$, and [F5] gives $d\star_gF=0$. The complex Hodge convention is exactly the one in [F2]. [given, F1, F2, F3, F4, F5, F6]

2.1 Apply [F7] with this same $T$, $F$ and $\star_g$: it gives all claims about $\eta$ and local or assumed global primitives. On a connected domain the componentwise constant is a single constant. None of these inputs asserts a global primitive from closedness alone, so the stated separate global obligation remains. [step 1.1, F7] ∎

### Source notes

Independently retrieved and read Ionescu–Klainerman, §4.1 opening and §4.2 (4.11)–(4.18), including the vacuum, Killing and Hodge conventions and the separate simply-connectedness sentence. The differential identities agree with the formulation here. That passage states the Ernst identities and refers elsewhere for their verification; its full cited proof was not read. The proof above instead composes the five locally authored prerequisites, whose only explicit external differential input is the convention-matched Ricci commutator from Reall. No global black-hole hypothesis or complete flow is needed for these local differential identities. No source proof review or native mathematical acceptance is claimed.


## Hawking and rotational fields near a bifurcate sphere

[Open item](item-thm-local-bifurcate-rigidity-input) · level 4


### Statement

Let $(O,g)$ be a connected oriented smooth four-dimensional Ricci-flat spacetime, with the metric and Killing-field conventions of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). Let $(S,H_1,H_2)$ be a regular bifurcate non-expanding null horizon pair in the precise pre-rigidity sense of [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair). There is an open neighborhood $O'\subseteq O$ of $S$ and a nontrivial smooth Killing field $K$ tangent to the null generators of both branches. This conclusion assumes no previously existing Killing generator.

If additionally a smooth Killing field $T$ is tangent to both branches and $T|_S\not\equiv0$, one may shrink $O'$ so that $[T,K]=0$ and there is a constant $\lambda_0$ for which $Z=T+\lambda_0K$ is a nontrivial rotational Killing field commuting with $T$. Rotational means that its local flow has a common positive period on the chosen neighborhood; after constant rescaling it has the normalized circle-action convention of [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data). The conclusions concern a full neighborhood of $S$, not extension over the entire exterior.

### Facts & Assumptions

[F1] The regular null-horizon pair defines the pre-rigidity sphere, causal branches and zero-expansion conditions without positing a Killing generator. [def-author-254b7c4bab6d-regular-null-horizon-pair](item-def-author-254b7c4bab6d-regular-null-horizon-pair)

[F2] Positive generator rescaling preserves zero expansion; the null second fundamental form and its trace are defined on the screen independently of a transverse section. [lem-author-254b7c4bab6d-null-expansion-rescaling](item-lem-author-254b7c4bab6d-null-expansion-rescaling) [lem-author-254b7c4bab6d-null-form-screen-descent](item-lem-author-254b7c4bab6d-null-form-screen-descent)

[F3] The null-metric transport identity identifies the geometric meaning of the null form, without using a rigidity conclusion or deriving shear-freeness from trace alone. [lem-author-254b7c4bab6d-null-metric-transport](item-lem-author-254b7c4bab6d-null-metric-transport)

[F4] A Killing field tangent to both branches restricts to a Killing field of the bifurcation sphere; the additional nontriviality condition means not identically zero there. [lem-author-254b7c4bab6d-tangent-killing-restriction](item-lem-author-254b7c4bab6d-tangent-killing-restriction)

[F5] Ambient Killing fields use the Lorentzian convention and normalized rotational fields use the circle-action convention. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

### External input

Theorem 1.1 of Alexakis–Ionescu–Klainerman supplies the full-neighborhood Hawking field under the stated regular non-expanding bifurcate-horizon hypotheses. Their Theorem 1.2 and §5 Propositions 5.1–5.2 supply the commuting field and the linear combination $Z=T+\lambda_0K$ with a common positive period under the additional branch-tangent symmetry hypothesis. These conclusions are imported inputs, not proofs reconstructed here. The five preceding local items formulate and relate the pre-rigidity data; they do not claim to replace the characteristic existence and unique-continuation arguments of the cited source. The exact source statement, hypotheses and actual reading limits are recorded in the citation metadata.



## Ionescu–Klainerman local Kerr criterion with full interface

[Open item](item-pthm-ik-local-kerr-criterion-input) · level 4


### Statement

Work in a smooth time-oriented vacuum Einstein spacetime $(M,g)$ of dimension $3+1$, with $M$ connected, orientable, paracompact and without boundary, and a smooth Killing field $T$. Impose the exact IK AF package [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af) and exact IK SBS package [def-author-9f9c6144aed8-ik-sbs](item-def-author-9f9c6144aed8-ik-sbs). Use the forms, contraction and supplied normalized Ernst potential of [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon). Require this same supplied potential to satisfy $\sigma(0,x)\to1$ as $|x|\to\infty$ on the $t=0$ spatial end of the IK AF chart, in the angularly uniform sense of that interface. Let $M>0$ be the AF mass. Assume $-4M^2\mathcal F^2=(1-\sigma)^4$ on all of $S_0$ and $\operatorname{Re}(1/(1-\sigma))>1/2$ at some point of $S_0$. Then $E$ is locally isometric to the domain of outer communication of a Kerr spacetime of mass $M$ with $0<a<M$, in the Kerr exterior convention [physics:def-gr-fx-kerr-exterior](https://alphabetamath.cc/physics/item/def-gr-fx-kerr-exterior). Here locally isometric means every point has a neighborhood with a metric-preserving diffeomorphism onto an open subset of that Kerr exterior. A single global isometry, injective global matching, or a matching of the whole extensions is not supplied by this conclusion.

### Facts & Assumptions

[F1] The formulation uses [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) under its stated hypotheses.

[F2] The formulation uses [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) under its stated hypotheses.

[F3] The formulation uses [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data) under its stated hypotheses.

[F4] The formulation uses [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data) under its stated hypotheses.

[F5] The formulation uses [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) under its stated hypotheses.

[F6] The formulation uses [physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law) under its stated hypotheses.

[F7] The formulation uses [physics:def-gr-fx-kerr-exterior](https://alphabetamath.cc/physics/item/def-gr-fx-kerr-exterior) under its stated hypotheses.

[F8] The formulation uses [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) under its stated hypotheses.

[F9] The formulation uses [def-author-9f9c6144aed8-ik-af](item-def-author-9f9c6144aed8-ik-af) under its stated hypotheses.

[F10] The formulation uses [def-author-9f9c6144aed8-ik-sbs](item-def-author-9f9c6144aed8-ik-sbs) under its stated hypotheses.

[F11] The formulation uses [def-author-9f9c6144aed8-ernst-mars-simon](item-def-author-9f9c6144aed8-ernst-mars-simon) under its stated hypotheses.

### External input

Imported input 1 is the Main Theorem of Ionescu–Klainerman at the exact locator in source 0, with all AF, SBS and T hypotheses above, including $\sigma\to1$ along the specified AF section. Both imported inputs use this same supplied potential; no additive renormalization is made between the horizon hypotheses and either invocation. It supplies the local Kerr conclusion directly; this item claims no local proof of that theorem.

Imported input 2 is Proposition 8.3 and its §8.2 completion at source 1. Put $\Sigma'_0=\{p\in\Sigma_0\cap E:\sigma(p)\ne1\}$ and $y=\operatorname{Re}(1-\sigma)^{-1}$ there. Let $y_{S_0}$ denote the constant value of $y$ on $S_0$ supplied by Lemma 8.1. For $R>y_{S_0}$ the source defines $U_R$ as the unique component of $\{p\in\Sigma'_0:y(p)<R\}$ whose closure in $\Sigma_0$ contains $S_0$. Proposition 8.2 supplies $R_1>y_{S_0}$, and under the full theorem setting Proposition 8.3 proves $\mathcal S=0$ on every $U_R$ with $R\ge R_1$. The completion then excludes the missing denominator-zero points and obtains (8.1). This analytic input, including the conditional Carleman estimate and bootstrap, is imported rather than reconstructed. The elementary path-exhaustion lemma [lem-author-9f9c6144aed8-sublevel-path-exhaustion](item-lem-author-9f9c6144aed8-sublevel-path-exhaustion) explains the exhaustion step only where its path hypotheses hold; it does not replace the source's boundary continuation, quantitative bounds, or exclusion of $\sigma=1$. The transport lemma [lem-author-9f9c6144aed8-stationary-zero-transport](item-lem-author-9f9c6144aed8-stationary-zero-transport) explains how invariant tensor vanishing extends from a section when its explicit invariance hypothesis is met; it supplies no analytic continuation estimate.


## Smooth Maxwell tensor formula without division by the stationary norm

[Open item](item-lem-author-7a3c9628f105-regular-maxwell-form) · level 4


### Statement

Assume the family and orientation in [lem-author-7a3c9628f105-rank-one-metric](item-lem-author-7a3c9628f105-rank-one-metric). Let $\mathcal F=F+i\star_gF$ satisfy $i_T\mathcal F=\tfrac12\mathrm d\sigma$ and $\mathrm d\sigma(T)=0$. Put $H_q=1+q-(1-q)\sigma$, $D_q=|H_q|^2$, and $Z_q=-\sqrt{1-q^2}(\overline{H_q}/H_q)(\mathcal F+(2D_q)^{-1}W_q\wedge\mathrm d\sigma)$. Then $Z_q$ is self-dual for $g_q$ and equals $F_q+i\star_{g_q}F_q$ for the real two-form $F_q=\operatorname{Re}Z_q$. It is spacetime smooth, continuous in $q\in[0,1]$, and $F_1=0$. Moreover $i_{4T/D_q(p)}Z_q=\mathrm d\Phi_q$ where $\Phi_q=-\sqrt{1-q^2}(1+\sigma)/H_q$.

### Facts & Assumptions

[F1] The metric, metric index contraction and stationary scalar conventions use [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] Self-duality and fiberwise pullback use [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data).

[F3] The orientation-preserving map and metric are those of [lem-author-7a3c9628f105-rank-one-metric](item-lem-author-7a3c9628f105-rank-one-metric).

[F4] The smooth family $W_q$ and the contraction normalization $W_q(T)=D_q(p)-D_q$ are supplied by [lem-author-7a3c9628f105-primitive-parameter-lift](item-lem-author-7a3c9628f105-primitive-parameter-lift).

[F5] The Hodge star is the unique smooth map characterized on real two-forms by $\alpha\wedge\star_g\beta=\langle\alpha,\beta\rangle_g\,\mathrm{vol}_g$, where $\langle\alpha,\beta\rangle_g=\tfrac12\alpha_{ab}\beta^{ab}$; it satisfies $\star_g^2=-\operatorname{id}$. These are mathematical conclusions of [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus).

[F6] Interior product of a smooth form by a smooth vector field is the pointwise operation of [math:def-interior-product-of-a-form-by-a-vector-field](https://alphabetamath.cc/item/def-interior-product-of-a-form-by-a-vector-field): $(i_X\omega)_x(v_2,\ldots,v_k)=\omega_x(X_x,v_2,\ldots,v_k)$ for $k\ge1$. On the complex forms of [F2], extend it by $i_X(U+iV)=i_XU+i\,i_XV$.

[F7] The exterior derivative and its local coordinate formula and graded product rule are supplied by [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus). For a smooth real function $u$, $(\mathrm du)(X)=X(u)$. For a smooth complex function $u+iv$ with real $u,v$, use the componentwise extension $\mathrm d(u+iv)=\mathrm du+i\,\mathrm dv$; the product rule extends by complex bilinearity. All derivatives here are in spacetime at fixed $q$.

### Proof

**Given:** The hypotheses in the Statement and the Facts above.

**Goal:** Establish the stated conclusions.

1.1 Expanding the alternating form gives $A_q^*\mathcal F=\mathcal F+D_q^{-1}W_q\wedge i_T\mathcal F=\mathcal F+(2D_q)^{-1}W_q\wedge\mathrm d\sigma$. The defining metric-and-volume identity for the Hodge star is preserved by an orientation-preserving invertible linear map; in dimension four a positive conformal factor cancels on two-forms. Consequently $A_q^*\mathcal F$ is self-dual for $(D_q/4)A_q^*g$. Complex scalar multiplication preserves this eigenspace. Writing $Z_q=U+iV$ and comparing real parts in $\star_{g_q}Z_q=-iZ_q$ gives $V=\star_{g_q}U$. [given, F1, F2, F3, F5, F6]

2.1 Put $C=D_q(p)$. Using $W_q(T)=C-D_q$ from [F4] and $\mathrm d\sigma(T)=0$, contraction with $T$ gives $i_T(A_q^*\mathcal F)=\tfrac12(1+W_q(T)/D_q)\mathrm d\sigma=C\,\mathrm d\sigma/(2D_q)$. Multiplication by the displayed factor and $4/C$ yields $-2\sqrt{1-q^2}\,\mathrm d\sigma/H_q^2$, using $D_q=H_q\overline H_q$. Using the scalar exterior derivative and its componentwise complex extension in [F7], differentiating $\Phi_q$ gives exactly this expression. Positivity of $D_q$ removes every spacetime singular denominator, and the only endpoint factor $\sqrt{1-q^2}$ is continuous and vanishes at one. This proves the regularity and endpoint claims, without asserting differentiability in $q$ at one. [given, F1, F3, F4, F6, F7, algebra, step 1.1] ∎

### Source notes

This conditional calculation follows §3.2 (3.24)–(3.25) of the cited independent source. No existence of the stationary primitive or Einstein–Maxwell solution is inferred from this calculation alone.


## Chronological equivariance and the no-white-hole condition

[Open item](item-lem-author-4cb89398a4ab-chronological-equivariance) · level 4


### Statement

Use the chronological relations of [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data). If a time-orientation-preserving isometry $\psi$ satisfies $\psi(E)=E$, then $\psi(I^\pm(E))=I^\pm(E)$ and $\psi(\partial I^\pm(E))=\partial I^\pm(E)$. In particular this applies to every $\phi_v$ and $E=M_{\mathrm{end}}$ of [lem-author-4cb89398a4ab-complete-end-saturation](item-lem-author-4cb89398a4ab-complete-end-saturation). Thus $B=M\setminus I^-(M_{\mathrm{end}})$, $W=M\setminus I^+(M_{\mathrm{end}})$ and $N=\partial I^-(M_{\mathrm{end}})$ are stationary-invariant, and $W=\varnothing$ is exactly $M=I^+(M_{\mathrm{end}})$. Chronological sets here are defined by the same curve formulas for any subset $E$, without requiring $E$ open.

### Facts & Assumptions

[F1] Chronological futures and pasts are defined by existence of future timelike curves, and boundaries are closure minus interior. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[F2] Every $\phi_v$ is an isometry and the saturated end is invariant under it. [lem-author-4cb89398a4ab-complete-end-saturation](item-lem-author-4cb89398a4ab-complete-end-saturation)

### Proof

**Given:** The action, set and causal conventions in the Statement.

**Goal:** Prove the chronological and boundary invariance and the no-white-hole identity.

1.1 A time-orientation-preserving isometry maps future timelike curves to future timelike curves. Applying it to a curve from $E$ to $p$ gives $\psi(I^+(E))\subset I^+(E)$; applying its inverse gives the reverse inclusion. The identical argument with the curve direction reversed proves the past identity. As a diffeomorphism, $\psi$ maps open sets to open sets, and it and its inverse preserve limits, so it preserves interiors and closures and hence the displayed boundaries. [F1]

2.1 The connected one-parameter action preserves time orientation: along $v\mapsto(d\phi_v)_pV$, for a fixed future timelike $V$, timelikeness is preserved and the sign relative to a continuous future time-orientation field cannot change without becoming zero. At $v=0$ the vector is future. Apply step 1.1 and [F2]. Complements are preserved by a bijection, and $M\setminus I^+(M_{\mathrm{end}})=\varnothing$ is equivalent to $M=I^+(M_{\mathrm{end}})$ by elementary set complementation. This proves all assertions. [F1, F2, step 1.1] ∎


## Quantitative lapse and shift bounds force annular timelikeness

[Open item](item-lem-author-0a41d659d5ab-annular-timelike-gap) · level 4


### Statement

For the AIK quantitative package and $\sup_{S_0}|g(T,T)|<\epsilon^2$, let $C_1=C_1(A)$ be the lapse constant from the explicit external estimate. For all sufficiently small $0<\epsilon<1$ depending only on $A$, the stationary field is strictly timelike on $1+\epsilon^{1/100}\le r\le R_1$ in $\Sigma_0$. More explicitly, once the imported estimates hold, $\epsilon^{7/150}<(8A_1C_1^2)^{-1}$ suffices for this assertion.

### Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The quantitative package includes $A_1^{-1}I\le(h_{ij})\le A_1I$ and the source section coordinates. [def-author-0a41d659d5ab-aik-quantitative-package](item-def-author-0a41d659d5ab-aik-quantitative-package)

[F2] The norm identity and exact horizon-smallness translation are those of [lem-author-0a41d659d5ab-horizon-field-norm](item-lem-author-0a41d659d5ab-horizon-field-norm).

[F3] Lapse and shift components use the hypersurface definitions in [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data).

[F4] The explicit External input supplies $n\ge C_1^{-1}(r-1)/r$ and $\sum_j|X_j|\le\epsilon^{1/30}$ on the bounded annulus, for the covariant shift components $X_j=h_{ji}X^i$.

[F5] A self-adjoint endomorphism of a finite-dimensional real inner product space admits an orthonormal eigenbasis. [math:cor-real-spectral-theorem-for-self-adjoint-endomorphisms](https://alphabetamath.cc/item/cor-real-spectral-theorem-for-self-adjoint-endomorphisms)

[F6] In signature $(-,+,+,+)$, a tangent vector is timelike exactly when its squared Lorentzian norm is negative. [physics:def-causal-classification-of-lorentz-vectors](https://alphabetamath.cc/physics/item/def-causal-classification-of-lorentz-vectors)

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conditional conclusion.

1.1 Put $\delta=\epsilon^{1/100}<1$. For $r\ge1+\delta$, monotonicity of $(r-1)/r$ gives $n\ge C_1^{-1}\delta/(1+\delta)\ge\delta/(2C_1)$. Since $h^{-1}\le A_1I$, the covariant-component estimate gives $h(X,X)=h^{ij}X_iX_j\le A_1\sum_jX_j^2\le A_1\epsilon^{1/15}$. The symmetric matrix $H=(h_{ij})$ defines a self-adjoint endomorphism of Euclidean $\mathbb R^3$, since $u^{\mathsf T}Hv=(Hu)^{\mathsf T}v$. By [F5] it has an orthonormal eigenbasis. Applying [F1] to each unit eigenvector puts its eigenvalue in $[A_1^{-1},A_1]$, so the eigenvalues of $H^{-1}$ are the reciprocals of those of $H$ and are therefore at most $A_1$, proving the inverse-metric bound. [F1, F3, F4, F5, algebra]

2.1 The norm identity now yields $g(T,T)\le-(4C_1^2)^{-1}\epsilon^{1/50}+A_1\epsilon^{1/15}$. Since $1/15-1/50=7/150$, the threshold in the Statement bounds the second term by $(8C_1^2)^{-1}\epsilon^{1/50}$, and hence $g(T,T)\le-(8C_1^2)^{-1}\epsilon^{1/50}<0$. By [F6], this strict negativity makes $T$ timelike throughout the stated annulus. All constants in this condition depend only on the fixed source bounds. [step 1.1, F1, F2, F6, algebra] ∎

### External input

Import the source lapse lower bound (2.10) and shift estimate (2.15), with exactly the GR/SBS/maximal and quantitative assumptions stated in the package and the source horizon bound. Only these inequalities are used here; their elliptic, integral, interpolation and transport proofs remain external. The norm estimate uses covariant shift components and the inverse induced metric, avoiding an implicit identification with contravariant components.


## From a Schwarzschild spatial isometry to the normalized spacetime exterior

[Open item](item-lem-author-f247c641a714-schwarzschild-static-data-lift) · level 4


### Statement

Suppose the regular static exterior data satisfy the reduced equations and their spatial metric is isometric, with its boundary and asymptotic end, to
$$h_{\rm S}=\left(1+\frac{\mu}{2s}\right)^4(ds^2+s^2d\omega^2),\qquad s>\mu/2,\quad \mu>0.$$
Then the normalized lapse is $V_{\rm S}=(1-\mu/(2s))/(1+\mu/(2s))$, the lapse coefficient is $m=\mu$, and the full static product is isometric to the Schwarzschild spacetime exterior. No assumption about maximal analytic extension of the spacetime is needed for this lifting step.

### Statement references

[def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)

[lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction)

[math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)

[lem-author-f247c641a714-static-boundary-and-positive-mass](item-lem-author-f247c641a714-static-boundary-and-positive-mass)

[physics:def-gr-schwarzschild-exterior-model](https://alphabetamath.cc/physics/item/def-gr-schwarzschild-exterior-model)

[math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### Facts & Assumptions

[F1] The regular static exterior data supply the global product, its future field $\partial_t$, the boundary and normalized end, and the inherited ZFC convention. The static reduction supplies $\Delta_hV=0$. [def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data) [lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction)

[F2] The inherited ZFC convention includes full choice and hence countable choice $\mathrm{AC}_\omega$, as required by the divergence theorem and the Schwarzschild model definition. Explicitly, for a sequence of nonempty sets, apply full choice to its set of values and compose that choice function with the sequence. No new choice hypothesis is being imposed. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)

[F3] Under countable choice the divergence theorem applies to smooth fields on compact oriented smooth Riemannian domains, with outward unit normals; compactness makes the support condition automatic. The boundary-and-mass lemma supplies $\int_X|DV|_h^2\,d\mu_h=4\pi m$. Only that energy identity is imported from this lemma. All divergence applications below take place inside $X$, where the metric is smooth. [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem) [lem-author-f247c641a714-static-boundary-and-positive-mass](item-lem-author-f247c641a714-static-boundary-and-positive-mass)

[F4] The Schwarzschild exterior model is the product $\mathbb R_{x^0}\times(s_{\rm Sch},\infty)\times S^2$ with metric $-(1-s_{\rm Sch}/r)d(x^0)^2+(1-s_{\rm Sch}/r)^{-1}dr^2+r^2\gamma_{S^2}$, future field $\partial_{x^0}$, and $s_{\rm Sch}=2G_Nm_*/c^2$. Here use the purely mathematical parameters $c=G_N=1$, $m_*=\mu$, $x^0=t$, $r=\mathcal R$ and $s_{\rm Sch}=2\mu$; $d\omega^2=\gamma_{S^2}$ is the unit round sphere metric. The symbol $s_{\rm Sch}$ is distinct from the isotropic radius $s$ in the Statement. No physical law or measured constant is imported by these parameter choices. [physics:def-gr-schwarzschild-exterior-model](https://alphabetamath.cc/physics/item/def-gr-schwarzschild-exterior-model)

[F5] On the smooth interior, $d\mu_h$ is the intrinsic Borel measure of the positive smooth Riemannian density $\sqrt{\det h}\,|dx^1dx^2dx^3|$. Under countable choice this measure has the coordinate integral formula, and integration against it agrees with smooth density integration on compact smooth domains. With the inherited orientation this also equals the volume-form integral in [F3], since both have coefficient $\sqrt{\det h}$. These interfaces apply to the compact annuli below, without any boundary regularity requirement at $B$, which is outside each annulus. [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:thm-density-measure-is-independent-of-the-chart-gluing](https://alphabetamath.cc/item/thm-density-measure-is-independent-of-the-chart-gluing) [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)

[F6] On any measure space, an increasing sequence of nonnegative measurable functions with pointwise limit $f$ has integrals increasing to $\int f$, without a prior finiteness assumption. [math:thm-monotone-convergence-for-the-integral](https://alphabetamath.cc/item/thm-monotone-convergence-for-the-integral)

[F7] On the smooth Riemannian interior, $Df=(df)^\sharp$, $D^2f(A,C)=h(D_ADf,C)$ and $\operatorname{div}_hY=\operatorname{tr}(A\mapsto D_AY)$. Tracing the connection product rule gives $\operatorname{div}_h(fDf)=|Df|_h^2+f\Delta_hf$. In coordinates the divergence is $(\det h)^{-1/2}\partial_i((\det h)^{1/2}Y^i)$. [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)

### Proof

**Given:** The boundary-preserving spatial isometry in the Statement, the regular static data and harmonic lapse equation of [F1], their inherited countable choice in [F2], the divergence, energy and model interfaces in [F3]–[F4], and the integration and differential-operator interfaces in [F5]–[F7].

**Goal:** Recover the lapse and global product, rather than infer a global spacetime result from a merely local isometry.

1.1 Pull back the radial function $U=(1-\mu/(2s))/(1+\mu/(2s))$ through the spatial isometry, and write $a=\mu/2$ and $\phi(s)=1+a/s$. By the coordinate divergence formula in [F7], its radial Laplacian is $(\phi^6s^2)^{-1}\partial_s(s^2\phi^2\partial_sU)=0$, since $s^2\phi^2\partial_sU=\mu$. Thus $U$ is harmonic, zero at $B$, and tends to one. The difference $w=V-U$ is harmonic and zero on $B$. Outside compact cores both asymptotically Euclidean metrics are uniformly comparable to their Euclidean metrics, so distance from a fixed compact set is bounded above and below by positive multiples of the corresponding radius. The isometry preserves those distances, hence the original end radius and $s$ are comparable. The given end estimates and preservation of gradient norms consequently give $w=O(s^{-1})$ and $|Dw|_h=O(s^{-2})$. [given, F1, F7]

2.1 Use the spatial isometry to identify $X$ with $(a,\infty)\times S^2$. For integers $j\ge1$, put $\varepsilon_j=1/(j+1)$, $R_j=a+j+1$ and $D_j=\{a+\varepsilon_j\le s\le R_j\}$. These are compact oriented smooth Riemannian domains entirely in $X$, with two disjoint smooth boundary spheres; they increase and their union is $X$. On a sphere $s=b$, the unit normals are $\pm\phi(b)^{-2}\partial_s$ and the area density is $\phi(b)^4b^2d\omega$. In a fixed compact strip adjacent to $B$, the $C^2$ regular data give a uniform bound for $|DV|_h$, and the explicit $U$ has bounded gradient, hence $|Dw|_h\le C$. The radial segments from $s=a$ to $a+\varepsilon$ have length $\int_a^{a+\varepsilon}\phi(s)^2ds=O(\varepsilon)$. The zero boundary value of $w$ then gives $w=O(\varepsilon)$ on the inner face, whose area is uniformly bounded by the displayed formula. Thus the absolute inner flux of $wDw$ is $O(\varepsilon_j)$. The outer area is $O(R_j^2)$, and the bounds in step 1.1 make its absolute outer flux $O(R_j^{-1})$. This constructs the exhaustion and both estimates directly for $w$. [given, F1, step 1.1]

3.1 By [F7], $\operatorname{div}_h(wDw)=|Dw|_h^2$. Apply the divergence theorem [F3] on each $D_j$, using countable choice [F2] and the integration convention [F5]. Step 2.1 bounds the nonnegative energy by $\int_{D_j}|Dw|_h^2\,d\mu_h\le C(\varepsilon_j+R_j^{-1})\to0$. The compact domains are Borel and $\mathbf1_{D_j}|Dw|_h^2$ are nonnegative Borel functions increasing pointwise to $|Dw|_h^2$. Monotone convergence [F6] therefore gives $\int_X|Dw|_h^2\,d\mu_h=0$. A nonzero value of $|Dw|_h$ would, by continuity, give an interior coordinate ball with the integrand bounded below by a positive constant, and the positive continuous coordinate density in [F5] gives that ball positive measure. Hence $Dw=0$ everywhere. Connectedness makes $w$ constant, and its zero limit at infinity makes it zero. [F1, F2, F3, F5, F6, F7, step 1.1, step 2.1]

4.1 Set $\mathcal R=s(1+\mu/(2s))^2$. This is strictly increasing from $2\mu$ to infinity on $s>\mu/2$, and direct differentiation gives $h_{\rm S}=(1-2\mu/\mathcal R)^{-1}d\mathcal R^2+\mathcal R^2d\omega^2$ and $U^2=1-2\mu/\mathcal R$. Taking the product of the spatial isometry with the identity on all $t\in\mathbb R$ therefore gives a global isometry of the full static exterior to $-(1-2\mu/\mathcal R)dt^2+(1-2\mu/\mathcal R)^{-1}d\mathcal R^2+\mathcal R^2d\omega^2$. With the parameter and unit-round-metric identifications in [F4], this is precisely the Schwarzschild exterior model, and the map sends $\partial_t$ to $\partial_{x^0}$, preserving the time orientation. [given, F1, F4, step 3.1]

5.1 On the same $D_j$, the product identity [F7] and the harmonicity of $U$ give $\operatorname{div}_h(UDU)=|DU|_h^2$. Apply [F3] with [F2] and [F5]. The sphere normal and area formula of step 2.1 give the flux of $UDU$ through $s=b$, oriented toward increasing $s$, as $4\pi U(b)b^2\phi(b)^2\partial_sU(b)=4\pi\mu U(b)$. The inner outward normal has the opposite sign, so $\int_{D_j}|DU|_h^2\,d\mu_h=4\pi\mu\bigl(U(R_j)-U(a+\varepsilon_j)\bigr)\to4\pi\mu$. Apply [F6] to $\mathbf1_{D_j}|DU|_h^2$ as in step 3.1 to obtain $\int_X|DU|_h^2\,d\mu_h=4\pi\mu$. These computations on the model are also computations on $X$: an isometry preserves gradient norms, and its metric pullback identity gives $\sqrt{\det(F^*h_{\rm S})}=|\det dF|\sqrt{\det h_{\rm S}}\circ F$ in coordinates, exactly the transformation law of the intrinsic density in [F5]. Since $V=U$ on $X$ by step 3.1, comparison with the independently supplied identity $\int_X|DV|_h^2\,d\mu_h=4\pi m$ in [F3] gives $\mu=m$, without presuming invariance of an end-coordinate coefficient. [F2, F3, F5, F6, F7, step 1.1, step 2.1, step 3.1, step 4.1] ∎


## Regular Harrison Einstein–Maxwell family

[Open item](item-thm-harrison-electrovacuum-construction-input) · level 5


### Statement

Assume exactly Radu's mass-one GR/SBS and original maximal-slice hypotheses, detailed in Facts below. For $0\le q\le1$, the regular Harrison formulas define Lorentz metrics $g_q$ and real two-forms $F_q$ on $E\cup O$, for one neighborhood $O$ of the bifurcation sphere $S_0$. They satisfy $(g_1,F_1)=(g,0)$ and $\mathcal L_Tg_q=\mathcal L_TF_q=0$. On $E$ they satisfy the source-free geometric electrovacuum equations, and on outward oriented end spheres $S_r$ their electric and magnetic fluxes $(4\pi)^{-1}\int_{S_r}\star_{g_q}F_q$ and $(4\pi)^{-1}\int_{S_r}F_q$ are $\sqrt{1-q^2}$ and zero. The metrics depend smoothly on $q$ on compact subsets; the fields are spacetime smooth and continuous in $q$. Near $S_0$ the local commuting Killing fields $K,Z$ remain Killing, and the two horizon branches retain generator $K$ and its surface gravity. The sign of $g_q(T,T)$ equals the sign of $g(T,T)$. The tensors extend smoothly across $S_0$; equations there follow on $O\cap\overline E$ by continuity, without asserting equations throughout $O\setminus\overline E$. No small-angular-momentum bound is assumed.

### Facts & Assumptions

[A1] Work in ZFC, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice). The stationary, hypersurface, asymptotic, form, electrovacuum and circle-action interfaces are [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data), [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data), [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data), [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data), [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data), [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data) and [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data).

[A2] The precise imported GR data are a connected oriented time-oriented smooth vacuum four-spacetime, a spacelike acausal edgeless partial Cauchy hypersurface $\Sigma^0=\Phi_0(\{|x|>1/2\})$, $\Sigma_1=\Phi_0(\{|x|>1\})$, and $S_0=\Phi_0(\{|x|=1\})$. The stationary end has $T=\partial_t$ and $g_{00}=-1+2/r+O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$, $g_{0i}=-2\epsilon_{ijk}S^jx^kr^{-3}+O_6(r^{-3})$. The spacetime orientation is fixed by $\mathrm dt\wedge\mathrm dx^1\wedge\mathrm dx^2\wedge\mathrm dx^3$ in this chart and is used for every $\star_g$ and $\star_{g_q}$. Here $S_r=\{t=0,\ |x|=r\}$ has the outward boundary orientation induced by $\mathrm dx^1\wedge\mathrm dx^2\wedge\mathrm dx^3$ on the zero-time end slice. Its exterior $E=I^-(M^{\mathrm{end}})\cap I^+(M^{\mathrm{end}})$ is globally hyperbolic; $\Sigma^0\cap I^-(M^{\mathrm{end}})=\Sigma^0\cap I^+(M^{\mathrm{end}})=\Sigma_1$; $T$ is nowhere zero on $E$, with complete orbits meeting $\Sigma_1$ transversally. SBS requires the two chronological boundary hypersurfaces $H^\pm$ near $S_0$ to be smooth, null, transverse and nonexpanding, intersecting in $S_0$, with $T$ tangent to both and not identically zero on $S_0$. The induced geometry extends smoothly to $S_0$ and $\operatorname{tr}_h k=0$ on $\Sigma_1$. These are §1.1 GR, SBS and maximality of the independent external source, with mass rescaled to one; they are additional hypotheses rather than consequences of the interface definitions in [A1].

[F1] Use the normalized vacuum Ernst data of the source: $f=-g(T,T)$, $F=\tfrac12\mathrm dT^\flat$, $\mathcal F=F+i\star_gF$, $\sigma=f+i\psi$ with $\psi(\infty)=0$, $i_T\mathcal F=\tfrac12\mathrm d\sigma$, $f<1$ on $E$, and $f\le0$ on $S_0$. The local source fields obey $[K,Z]=0$, $T=K+\Omega Z$ with constant $\Omega\ne0$, $K|_{S_0}=0$, and the periodic field $Z$ has a pole $p$ where $T(p)=0$.

[F2] The shared stationary primitive supplier [thm-stationary-harrison-primitive-input](item-thm-stationary-harrison-primitive-input) gives $\mathrm dW_0=4((f-1)F+\psi\star_gF)$, $W_0(T)=D_0(p)-D_0$, smooth extension across $S_0$, local $K,Z$ invariance and the radial end choice $W_{0i}=O_5(r^{-3})$. Its normalization, decay and extension are existence inputs, not consequences of the following polynomial calculations.

[F3] The denominator, primitive lift, metric, electromagnetic tensor and boundary-scope arguments are [lem-author-7a3c9628f105-denominator-positivity](item-lem-author-7a3c9628f105-denominator-positivity), [lem-author-7a3c9628f105-primitive-parameter-lift](item-lem-author-7a3c9628f105-primitive-parameter-lift), [lem-author-7a3c9628f105-rank-one-metric](item-lem-author-7a3c9628f105-rank-one-metric), [lem-author-7a3c9628f105-regular-maxwell-form](item-lem-author-7a3c9628f105-regular-maxwell-form) and [lem-author-7a3c9628f105-exterior-boundary-scope](item-lem-author-7a3c9628f105-exterior-boundary-scope).

[F4] Radu Proposition 3.1, §3.1–3.3 and Appendix A are imported for the normalized vacuum inputs in [F1], the exterior Einstein–Maxwell equations (including exterior $f=0$), fluxes, and local horizon Killing-field and surface-gravity preservation, under [A2].

### Proof

**Given:**The hypotheses in the Statement and the Facts below.

**Goal:** Establish the stated conclusions.

1.1 Apply [F2] to fix one $W_0$; set $D_q=|1+q-(1-q)\sigma|^2$ and $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. The denominator lemma gives positivity on $E$ and a common neighborhood $O$ of $S_0$. The primitive-lift lemma gives $W_q(T)=D_q(p)-D_q$ and the curl identity. In particular no time-coordinate normalization is chosen independently of the contraction constant fixed at $p$. [A1, A2, F1, F2, F3]

2.1 The rank-one metric lemma gives $g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-(f/D_q)W_q\otimes W_q)$, its Lorentz signature, smoothness and sign identity. The regular-Maxwell lemma gives $F_q$ as the real part of its self-dual tensor formula, endpoint values and the stated distinct parameter regularities. Stationarity follows because every coefficient is formed algebraically from stationary fields. [A1, F1, F2, F3, step 1.1]

3.1 Apply the precisely scoped external construction input [F4] under [A2] for the Einstein–Maxwell equations on $E$, the two charge integrals, and preservation of $K,Z$ and the horizon surface gravity near $S_0$. These differential-equation, flux and horizon claims are imported; the preceding algebra alone does not establish them. The boundary-scope lemma extends the equations to $O\cap\overline E$ by continuity but supplies no equation on the open opposite side. Thus smooth horizon extension and exterior field equations have distinct scopes exactly as asserted. The imported construction assumes GR, SBS and maximality, with no global smallness hypothesis. [A1, A2, F3, F4, step 2.1] ∎



Radu Proposition 3.1 is imported for the exterior Einstein–Maxwell equations, the charge integrals, and preservation of the local horizon Killing fields and surface gravity, under precisely the GR/SBS and maximality hypotheses specified above. Appendix A.2 covers exterior points with $f=0$; its scope is not all of the horizon neighborhood.

### External input

Radu Proposition 3.1 is imported for the exterior Einstein–Maxwell equations, the charge integrals, and preservation of the local horizon Killing fields and surface gravity, under precisely the GR/SBS and maximality hypotheses specified above. Appendix A.2 covers exterior points with $f=0$; its scope is not all of the horizon neighborhood.


## Static vacuum Schwarzschild classification contract

[Open item](item-pthm-static-vacuum-uniqueness-input) · level 5


### Statement

In the zero-cosmological-constant vacuum Einstein model, let the spacetime exterior be the globally static product $g=-V^2dt^2+h$ on $\mathbb R_t\times X$. Assume the regular static exterior data: $\overline X$ is a connected oriented three-dimensional exterior complete up to nonempty compact smooth boundary $B$, $V>0$ inside and $V=0$ on $B$, the interior data are smooth and extend at least $C^2$ to $B$, and $dV\ne0$ there. The single asymptotically Euclidean end is the complement of a compact core, with $h-\delta=O_2(r^{-1})$ and $V=1-m/r+O_2(r^{-2})$, and there is no other end or deleted interior boundary. No connectedness of $B$ is assumed.

Then the exterior is globally isometric to the Schwarzschild exterior of mass $m>0$, and $B$ is a connected two-sphere. Staticity and this global static product must already have been established; this theorem does not turn an arbitrary non-rotating stationary spacetime into a static one. The classification is of the given exterior; it does not assert a maximal analytic extension beyond its horizon.

### Statement references

[def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data)

[lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction)

[lem-author-f247c641a714-static-end-weighted-integrability](item-lem-author-f247c641a714-static-end-weighted-integrability)

[lem-author-f247c641a714-static-boundary-and-positive-mass](item-lem-author-f247c641a714-static-boundary-and-positive-mass)

[lem-author-f247c641a714-schwarzschild-static-data-lift](item-lem-author-f247c641a714-schwarzschild-static-data-lift)

[physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)

### Facts & Assumptions

[A1] The classical field law is adopted on the smooth spacetime interior with zero stress-energy and zero cosmological constant. Tracing $\operatorname{Ric}(g)-\tfrac12\operatorname{Scal}(g)g=0$ in dimension four gives $\operatorname{Ric}(g)=0$. [physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)

[F1] The regular static data, their reduced spatial equations, original weighted-end conditions, boundary geometry, positive mass coefficient, and lifting from Schwarzschild spatial data are the following locally authored application suppliers: [def-author-f247c641a714-regular-static-exterior-data](item-def-author-f247c641a714-regular-static-exterior-data) [lem-author-f247c641a714-static-vacuum-reduction](item-lem-author-f247c641a714-static-vacuum-reduction) [lem-author-f247c641a714-static-end-weighted-integrability](item-lem-author-f247c641a714-static-end-weighted-integrability) [lem-author-f247c641a714-static-boundary-and-positive-mass](item-lem-author-f247c641a714-static-boundary-and-positive-mass) [lem-author-f247c641a714-schwarzschild-static-data-lift](item-lem-author-f247c641a714-schwarzschild-static-data-lift)

[F2] The complete static-data Schwarzschild classification is an established external input: Bunting–Masood-ul-Alam, p.148 hypotheses and Assumption 1, p.150 Theorem 2, and p.153 Riemannian conclusion, with Miao pp.1–2 giving its explicit spatial-data formulation.

### External input

The classification theorem, including connectedness and the Schwarzschild spatial geometry, is imported from the two independent-source records. The five local prerequisites supply the application chain: the adopted vacuum law gives the spatial static equations, the differentiated pointwise decay implies Assumption 1 with $q=6$ and $\lambda=1/2$, the boundary and energy identity give regular boundary data and $m>0$, and the global product lifts the spatial Schwarzschild classification to the stated spacetime exterior. The spatial classification is used on complete data, as explicitly restated by Miao; the “maximally extended” spacetime wording of the original Theorem 2 is not used to infer that an arbitrary ambient spacetime has such an extension. No local proof of the imported classification or of the positive-mass theorem is claimed.

### Source notes

The original theorem’s weighted second derivatives were resolved by reading its source image, not by guessing from corrupted OCR. Miao’s later minimal-boundary theorem with a C3 metric is not substituted for the original C2 zero-lapse-boundary result.


## Precise Rácz–Wald global collapse class

[Open item](item-def-author-4cb89398a4ab-racz-wald-collapse-class) · level 5


### Definition

A **Rácz–Wald collapse-class datum** is a smooth globally hyperbolic spacetime $(M,g)$ with a smooth spacelike Cauchy surface $\Sigma=\Sigma_{\mathrm{end}}\cup\Sigma'$, satisfying the full end contract [def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end) for this single asymptotically flat end. Global hyperbolicity, spacelike and Cauchy are used as in [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data). In particular the coordinate-cone conclusions [lem-author-4cb89398a4ab-end-coordinate-cones](item-lem-author-4cb89398a4ab-end-coordinate-cones) hold, while the stationary generator $T$ has the complete action $\phi_u$ of [lem-author-4cb89398a4ab-complete-end-saturation](item-lem-author-4cb89398a4ab-complete-end-saturation). The remainder $\Sigma'$ is not assumed compact by this definition.

Using that stationary saturation, set $B=M\setminus I^-(M_{\mathrm{end}})$, $W=M\setminus I^+(M_{\mathrm{end}})$ and $N=\partial I^-(M_{\mathrm{end}})$ as in [lem-author-4cb89398a4ab-chronological-equivariance](item-lem-author-4cb89398a4ab-chronological-equivariance). Require $B\ne\varnothing$ and $W=\varnothing$ (equivalently $M=I^+(M_{\mathrm{end}})$).

Require $N$ to be a connected Killing horizon, with $N\cap\Sigma$ compact. More explicitly a second one-parameter group of isometries $\chi_u$ is defined on all of $M$ for every $u\in\mathbb R$, with Killing generator $\xi$ normal to $N$ and chosen future directed on its nonzero-generator part; use the horizon and signed-surface-gravity conventions of [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data). The groups $\chi$ and $\phi$ may differ. Completeness of $T$ never substitutes for the asserted completeness of $\xi$. No numerical normalization of $\xi$ and no nonzero or constant value of its surface gravity are imposed until a theorem requires them.

### Facts & Assumptions

[F1] The exact end contract and its cone and saturation consequences apply. [def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end) [lem-author-4cb89398a4ab-end-coordinate-cones](item-lem-author-4cb89398a4ab-end-coordinate-cones) [lem-author-4cb89398a4ab-complete-end-saturation](item-lem-author-4cb89398a4ab-complete-end-saturation)

[F2] The causal definitions and the chronological equivariance result give the stated meanings and the no-white-hole equivalence. [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [lem-author-4cb89398a4ab-chronological-equivariance](item-lem-author-4cb89398a4ab-chronological-equivariance)

[F3] The horizon supplier defines normal Killing generators and their signed surface gravity. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[F4] The independent source specifies this conjunction at the end of §2; the distinct global group $\chi_u$ is expressly part of that contract.

### Justification

**Given:** The displayed metric, surface, end and actions satisfying the listed conditions.

**Goal:** Specify the complete input class used in the global extension theorem.

1.1 The end contract supplies coordinate and complete stationary-action data; its two local consequences distinguish the coordinate time direction from $T$ and define the invariant saturated end. The causal definitions then define $B,W,N$, and the no-white-hole identity is the set equality proved in the chronological lemma. [F1, F2]

2.1 The horizon supplier gives the meaning of the separate normal generator and scalar. Connectedness, compactness and existence of the second complete group are further hypotheses on the data; none is inferred from local stationarity. The conjunction therefore gives a precise, well-defined input class matching the source, without asserting that an arbitrary stationary horizon belongs to it. [F3, F4, step 1.1] ∎

### External input

The collapse-class restrictions are transcribed from Rácz–Wald, end of §2, pp. 8–9. Its observation that the asymptotic conditions could be weakened is not used to remove any of the stated hypotheses.


## Smooth global data for the axisymmetric comparison

[Open item](item-def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data) · level 5


### Definition

Work in ZFC, including choice. Use the supplied stationary Lorentzian and causal conventions. The global comparison data consist of a smooth connected time-oriented four-dimensional spacetime $(M,g,N)$ with a specified asymptotically flat spacelike end $S_{\rm ext}$ and a complete stationary Killing flow $\phi_t$ generated by $T$, future timelike on that end, together with a smooth effective axial circle action $\psi_s$ of period $2\pi$ by isometries. Require these actions to commute. End decay, $M_{\rm ext}$, $D=I_M^+(M_{\rm ext})\cap I_M^-(M_{\rm ext})$, $I^+$-regularity and regular axis have exactly the predicates of the supplied black-hole comparison-hypothesis interface. Use the supplied normalized circle-action convention. Require the future event horizon to be connected.

When retaining the original item's mean-nondegeneracy assumption, supply a smooth compact horizon section $S$ without boundary and compatible Gaussian-null coordinate patches near it of the form $g=r\varphi\,dv^2+2\,dv\,dr+2rh_a\,dx^a dv+h_{ab}\,dx^a dx^b$, with horizon $r=0$ and section $v=r=0$ in these patches. Require their section restrictions to define a single global smooth scalar $\varphi_S:S\to\mathbb R$ and a smooth positive-definite metric $h$ on $S$: on overlapping section charts the coefficients $\varphi|_S$ agree as scalar values and $h_{ab}|_S$ obey the metric tensor transition law. Let $d\mu_h$ be the intrinsic Riemannian density and interpret $\int_S\varphi_S\,d\mu_h$ by the supplied compactly supported smooth-density integration interface. The relevant mean condition is $\int_S\varphi_S\,d\mu_h\ne0$ in that supplied normalization. This is a nonvanishing predicate; no numerical surface-gravity normalization or implication to a Killing horizon is asserted. It is an optional additional hypothesis for the imported smooth axisymmetric classification, whose source theorem does not need it.

For a specified comparison spacetime, supply separate stationary Lorentzian data $(\widetilde M,\widetilde g,\widetilde N,\widetilde T)$ with a selected asymptotically flat spacelike end $\widetilde S_{\rm ext}$ and complete stationary Killing flow $\widetilde\phi_t$, future timelike on that end. Apply the same end and causal-exterior conventions to these data, setting $\widetilde M_{\rm ext}=\bigcup_{t\in\mathbb R}\widetilde\phi_t(\widetilde S_{\rm ext})$ and $\widetilde D=I_{\widetilde M}^+(\widetilde M_{\rm ext})\cap I_{\widetilde M}^-(\widetilde M_{\rm ext})$. A global metric classification of the exterior by this comparison spacetime means that there exists a diffeomorphism $F:D\to\widetilde D$ satisfying $F^*(\widetilde g|_{\widetilde D})=g|_D$. Diffeomorphism and tensor pullback use their supplied mathematical definitions. This does not mean an isometry of all extensions beyond the horizons.

### Definition references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:def-riemannian-volume-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-riemannian-volume-of-a-compactly-supported-smooth-density)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

### Facts & Assumptions

[F1] ZFC and the supplied geometric interfaces define the ambient objects, causal exterior, complete stationary flow, regular axis and normalized circle action, for the original and separately supplied comparison data. The global regularity predicates are imposed in full. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[F2] On a Riemannian manifold, a smooth compactly supported real function times the intrinsic Riemannian density has a finite intrinsic integral, without an orientation; countable choice suffices for the chart-partition selection and is available in ZFC. [math:def-riemannian-volume-of-a-compactly-supported-smooth-density](https://alphabetamath.cc/item/def-riemannian-volume-of-a-compactly-supported-smooth-density) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F3] A diffeomorphism is a bijective smooth map with smooth inverse. Pullback of a covariant tensor is defined using the differential of its smooth map. [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds) [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

[F4] The independent source supplies the Gaussian-null mean nonvanishing criterion for supplied smooth compact-section data, as recorded in External input. Compatible global section coefficients are explicitly required here rather than inferred from compactness.

### Justification

**Given:** The supplied end, global flows, causal data, optional compatible Gaussian-null section data and, when a comparison is specified, its separate spacetime data.

**Goal:** Verify that these define precise conditional comparison data.

1.1 Complete flow and circle-action predicates specify maps for all real parameters, while the causal interface and the comparison-hypothesis supplier determine $M_{\rm ext}$, $D$ and the full $I^+$-regularity predicate. Commutation, regular-axis and horizon-connectedness are separate stated conditions; none is inferred from a local Killing field. [given, F1]

1.2 For the optional mean condition, the required overlap compatibility supplies a global smooth $\varphi_S$ and Riemannian metric $h$. The support of $\varphi_S$ is a closed subset of compact $S$, hence compact. Thus the density-integration interface applies under ZFC and makes its scalar integral finite and the nonzero test meaningful in the supplied normalization. Multiplication by a nonzero fixed normalization factor does not change whether the integral vanishes. No existence or gauge-independence of these Gaussian-null data is deduced. [given, F1, F2, F4]

2.1 Applying the same exterior construction to the separate comparison data fixes $\widetilde M_{\rm ext}$ and $\widetilde D$ in the ambient $\widetilde M$. The diffeomorphism and tensor-pullback interfaces then make the displayed condition on $F$ a definite predicate, exactly the stipulated isometry between the entire exteriors. No such map or comparison spacetime is asserted to exist by this definition. These definitions require no rigidity, nondegeneracy bridge or classification result. [given, F1, F3, step 1.1, step 1.2] ∎

### External input

Chruściel–Costa–Heusler supplies the end, stationarity, exterior and $I^+$-regularity definitions, axial terminology and the Gaussian-null mean criterion under the recorded hypotheses and reading limits. Theorem 3.2 omits mean-nondegeneracy. Only that omission is noted here; its classification is not proved or applied in this definition. No numerical surface-gravity identity is used.


## The non-timelike region is confined to the local-rigidity collar

[Open item](item-lem-author-0a41d659d5ab-ergoregion-collar) · level 5


### Statement

For the AIK quantitative package there is an open local-rigidity neighborhood $\Omega$ of $S_0$ carrying a rotational Killing field $Z$ commuting with $T$. For sufficiently small $\epsilon>0$ depending only on $A$, the bound $\sup_{S_0}|g(T,T)|<\epsilon^2$ implies $\{p\in\Sigma_1:g(T,T)(p)\ge0\}\subset\Omega$. This set includes the stationary-limit points and uses the source Proposition 1.3 non-strict convention. Here **rotational** means $Z\not\equiv0$ and there is a common $t_0>0$ such that its local flow $\phi^Z$ is defined through time $t_0$ on $\Omega$ and $\phi^Z_{t_0}(p)=p$ for every $p\in\Omega$. Individual orbits may have shorter periods or be fixed; no normalization of $t_0$ or completeness on all of $M$ is asserted.

### Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The stationary package and its fixed quantitative constant are those of [def-author-0a41d659d5ab-aik-quantitative-package](item-def-author-0a41d659d5ab-aik-quantitative-package).

[F2] The source estimates imply timelikeness on $1+\epsilon^{1/100}\le r\le R_1$ for sufficiently small $\epsilon(A)$. [lem-author-0a41d659d5ab-annular-timelike-gap](item-lem-author-0a41d659d5ab-annular-timelike-gap)

[F3] The asymptotic end $r>R_1$ is timelike. [lem-author-0a41d659d5ab-asymptotic-timelike-gap](item-lem-author-0a41d659d5ab-asymptotic-timelike-gap)

[F4] The explicit External input gives $\Omega$, a nontrivial rotational Killing field $Z$ commuting with $T$, its common local period $t_0>0$, and $\rho(A)>0$ such that $\Sigma_1\setminus\Sigma_{1+\rho}\subset\Omega$.

[F5] Local flows and their time maps use [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow). The period condition is local to the rigidity neighborhood; no global flow on $M$ is assumed.

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conditional conclusion.

1.1 Choose the horizon parameter below the threshold for [F2] and also so that $\epsilon^{1/100}<\rho$. This is possible because $\rho>0$ is fixed by the source geometric bounds, independently of the subsequently chosen small parameter. By [F2] and [F3], every point with $r\ge1+\epsilon^{1/100}$ has $g(T,T)<0$. [F1, F2, F3, F4, given]

2.1 Therefore a point of $\Sigma_1$ with $g(T,T)\ge0$ must satisfy $1<r<1+\epsilon^{1/100}<1+\rho$, so lies in $\Sigma_1\setminus\Sigma_{1+\rho}\subset\Omega$. The Killing-field existence, commutation and common-period assertions are exactly [F4], with the local-flow meaning in [F5]; this local application asserts no extension of $Z$ outside $\Omega$. [step 1.1, F1, F4, F5, algebra] ∎

### External input

Import the local rotational-rigidity conclusion of AIK Theorem 1.2 and the quantitative collar inclusion stated in its final proof of Proposition 1.3. The common local period in the rotational conclusion is specified by Proposition 5.2 of the separately cited local-rigidity paper: the time-$t_0$ map is the identity on a neighborhood of $S_0$. Both existence and periodicity remain imported premises. Combining them with the separately imported estimates and the local norm/asymptotic calculations proves the stated confinement, without claiming a reconstruction of the local Carleman construction.


## Connected rotating degenerate vacuum comparison data

[Open item](item-def-author-abbd1939ec07-connected-degenerate-comparison-data) · level 5


### Definition

Work in ZFC. A connected rotating degenerate vacuum comparison datum consists of the time-oriented stationary four-dimensional Lorentzian data $(M,g,T)$ of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data), an asymptotically flat selected end, and the $I^+$-regularity, analyticity and causal-exterior conventions of [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data) and [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data). Require $\operatorname{Ric}(g)=0$. Require that the future event horizon $H^+=I_M^+(M_{\rm ext})\cap\partial_M D$ be nonempty and connected, and that it be a smooth Killing horizon for a specified nonzero generator $K$ with $d(g(K,K))=-2\kappa K^\flat$ on its nonzero-generator part and $\kappa=0$ there. Require that $T$ fail to be tangent to the null normal line somewhere on $H^+$; this is rotation relative to $T$. No bifurcation surface is part of these data.

Here $D$ is the domain of outer communications and $M_{\rm ext}$ the flow-saturated selected end. $I^+$-regularity requires completeness of $T$, global hyperbolicity of $D$, and the finite-end acausal section and once-only horizon-generator cross-section specified by the comparison definition. Connectedness is imposed on the horizon, not merely on that section. These are predicates on supplied data, not assertions that the data exist.

### Facts & Assumptions

[F1] Stationary geometry, causal sets, $I^+$-regularity and analytic charts are [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data), [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data) and [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data).

[F2] Surface gravity, null normal line, the nonzero-generator qualification and rotation are [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data). The inherited choice convention is [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice).

### Justification

**Given:** The supplied geometric objects and the displayed requirements.

**Goal:** Verify that the comparison class is a well-defined predicate without assuming a bifurcation surface or deriving axial symmetry.

1.1 The causal and comparison interfaces determine $M_{\rm ext}$, $D$ and $H^+$, so nonemptiness and connectedness are definite topological predicates. The stated completeness, regularity and analyticity requirements are likewise the explicit predicates in [F1]. [given, F1]

2.1 The horizon interface fixes the surface-gravity equation and rotation condition for the supplied fields. It therefore makes $\kappa=0$ and failure of stationary tangency unambiguous. Adding the tensor equation $\operatorname{Ric}(g)=0$ selects vacuum geometries. None of these operations produces an axial field or a bifurcation surface; those would be further results. [given, F1, F2] ∎


## Ordered horizon rods and twist-jump labels

[Open item](item-def-author-abbd1939ec07-ordered-vacuum-rods) · level 5


### Definition

An ordered finite vacuum rod datum consists of an integer $N\ge1$, real numbers $z_i^-\le z_i^+$ for $1\le i\le N$ and $z_i^+<z_{i+1}^-$ for $1\le i<N$, and intervals $\mathcal H_i=[z_i^-,z_i^+]$. A strict interval is called a nondegenerate horizon rod and an interval with equal endpoints a degenerate puncture $p_i=(0,0,z_i^-)$. In this abstract rod datum these names label the intervals; their identification with geometric event horizons is a separate theorem.

The complementary axis intervals are $\Gamma_1=(-\infty,z_1^-)$, $\Gamma_{j+1}=(z_j^+,z_{j+1}^-)$ for $1\le j<N$, and $\Gamma_{N+1}=(z_N^+,\infty)$. Supply real constants $c_1,\ldots,c_{N+1}$. The labels $\mathcal J_i=(c_{i+1}-c_i)/4$ are the angular-momentum parameters in the HKWX convention. A shift of every $c_j$ by the same constant is a twist gauge change and leaves these labels unchanged. Their identification with Komar integrals of a geometric spacetime is not asserted by this definition.

### Facts & Assumptions

[F1] The stationary axial-action terminology, when a geometric realization is supplied, is [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data). Work in ZFC, [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice). The ordered intervals and real constants themselves are finite numerical data.

[F2] Open, closed and unbounded real intervals, their nonemptiness conditions, and the singleton case $[a,a]=\{a\}$ use [math:def-interval](https://alphabetamath.cc/item/def-interval).

### Justification

**Given:** The integer, ordered endpoints and constants.

**Goal:** Verify the interval decomposition and gauge-invariant labels.

1.1 By the supplied interval definitions, every intervening interval is nonempty: its endpoints satisfy $z_j^+<z_{j+1}^-$ and their midpoint lies strictly between them. The two exterior intervals are semi-infinite. All complementary axis intervals together with the horizon intervals exhaust the real axis: $\mathbb R=(\bigcup_{i=1}^N\mathcal H_i)\cup(\bigcup_{j=1}^{N+1}\Gamma_j)$. Indeed, a real number below $z_1^-$ or above $z_N^+$ lies in an exterior interval; otherwise, if it belongs to no horizon interval, the ordered finite endpoints place it strictly between two consecutive horizon intervals. Equal endpoints give singletons and do not collapse either neighboring open interval because the adjacent strict inequalities remain. [given, F1, F2, algebra]

2.1 Each difference $c_{i+1}-c_i$ is a definite real number, and a common additive shift cancels in the difference. Division by four defines the stated labels without a choice of primitive. Their geometric interpretation requires reconstruction data in addition to these finite labels. [given, step 1.1, algebra] ∎


## Smooth rigidity from a quantitatively small horizon field

[Open item](item-pthm-small-horizon-field-rigidity-input) · level 6


### Statement

In the four-dimensional classical vacuum Einstein model with zero cosmological constant, impose the exact AIK quantitative stationary package, including GR, SBS and the asymptotically flat maximal section. Once $A$ is fixed there is $\epsilon_*(A)>0$ such that $\sup_{S_0}|g(T,T)|<\epsilon_*^2$ implies that the exterior $E$ is isometric to a subextremal Kerr exterior, with the source stationary and axial symmetries. Here the horizon bound is equivalently $\sup_{S_0}|T|_h<\epsilon_*$, using the induced positive metric on $S_0$. The source SBS hypothesis retains $T|_{S_0}\not\equiv0$. The non-timelike subset of the maximal section is then contained in the local rotational-rigidity neighborhood. Smallness of ADM angular momentum is not substituted for this horizon-field condition.

### Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The full GR, SBS, maximality and quantitative assumptions, including the exact constant $A$, are given in [def-author-0a41d659d5ab-aik-quantitative-package](item-def-author-0a41d659d5ab-aik-quantitative-package).

[F2] Horizon tangency makes the source scalar smallness exactly the induced-metric norm smallness. [lem-author-0a41d659d5ab-horizon-field-norm](item-lem-author-0a41d659d5ab-horizon-field-norm)

[F3] The explicit quantitative estimates give confinement of the non-timelike region to the local rotational-rigidity neighborhood. [lem-author-0a41d659d5ab-ergoregion-collar](item-lem-author-0a41d659d5ab-ergoregion-collar)

[A2] Adopt the direct-equation Einstein model, including the model assumptions specified by the field-law supplier, on its matter domain $U\subseteq M$, with vanishing stress-energy on $U$ and $\Lambda=0$. [physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)

[F4] The subextremal Kerr exterior means the standard tensor on $\mathbb R\times(r_+,\infty)\times S^2$ with $M_0>0$, $|a|<M_0$, and $r_+=M_0+\sqrt{M_0^2-a^2}$. [physics:def-gr-fx-kerr-exterior](https://alphabetamath.cc/physics/item/def-gr-fx-kerr-exterior)

[F5] The independently sourced AIK Theorem 1.1, under its full GR/SBS/maximal and quantitative hypotheses, is the imported main theorem recorded in External input and the source reference.

### Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conditional conclusion.

1.1 On the matter domain $U$ specified in [A2], with vanishing stress-energy and $\Lambda=0$, [A2] gives $\operatorname{Ric}_{ab}-\tfrac12Rg_{ab}=0$. Its four-dimensional trace is $R-2R=0$, hence $R=0$ and $\operatorname{Ric}=0$ on $U$. For the rigidity theorem, use the independently assumed $\operatorname{Ric}(g)=0$ on all of $M$ in [F1]; no extension of the field-law deduction beyond $U$ is required. By [F2] the stated horizon norm condition and the source scalar condition are equivalent. Choose $\epsilon_*(A)$ below the threshold in [F5] and that for [F3]; both depend only on the fixed source bounds. [A2, F1, F2, F3, F5, algebra]

2.1 Apply the imported main theorem [F5] with exactly the GR/SBS/maximal and quantitative package [F1]. It gives the asserted stationary axisymmetric Kerr exterior, with the small-angular-momentum range in the source and the subextremal tensor meaning in [F4]. Independently [F3] gives the recorded confinement. The global extension and Kerr-classification steps are part of the imported theorem, not conclusions reconstructed from confinement alone. No inference from a small ADM angular momentum assumption is made. [step 1.1, F1, F3, F4, F5] ∎

### External input

Import AIK Theorem 1.1 in its complete GR/SBS/maximal and quantitative setting. The source condition is $\|g(T,T)\|_{L^\infty(S_0)}<\epsilon^2$, with $\epsilon$ sufficiently small depending only on $A$ from (1.10). The source abstract identifies the isometry conclusion as one about the domains of outer communications. This contract imports the full rigidity theorem, including the global extension and classification it invokes; it does not assert a locally reconstructed rigidity proof.

### Source notes

The exact AIK package retains its own stronger coordinate decay, its GR/SBS assumptions and its nonzero-horizon-field clause; it is separate from a generic black-hole regularity package. AIK uses the non-strict set $g(T,T)\ge0$ in Proposition 1.3, while some terminology calls only $g(T,T)>0$ the ergoregion; the explicit inequality here avoids that convention ambiguity. No source defect or independent mathematical acceptance is asserted.


## Nonzero constant surface gravity and global bifurcate extension

[Open item](item-thm-nondegenerate-bifurcate-extension-input) · level 6


### Statement

Let $(M,g,\Sigma,T,\phi,\xi,\chi,N)$ satisfy the complete Rácz–Wald collapse-class contract [def-author-4cb89398a4ab-racz-wald-collapse-class](item-def-author-4cb89398a4ab-racz-wald-collapse-class), including the exact single-end asymptotic conditions, global hyperbolicity, absence of a white hole and both specified complete actions. Suppose the signed surface gravity of the future horizon-normal generator $\xi$ is a nonzero constant on $N$, with the conventions of [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data).

Then there is a smooth spacetime $(M^*,g^*)$ and an isometric embedding of the **whole** $(M,g)$ into it such that the image of $N$ is a proper subset of a bifurcate Killing horizon. The original group $\chi_u$ extends to $(M^*,g^*)$, and the extension can be chosen with a wedge-reflection isometry about its bifurcation surface. In the local horizon coordinates this reflection sends $(U,V,x^1,x^2)$ to $(-U,-V,x^1,x^2)$.

This is a global embedding conclusion, not a claim that $M^*$ is globally hyperbolic. Extension of additional tensor fields is a separate question, as stated at the start of §5 of the source. No Einstein equation or matter-field extension is asserted. The completeness and horizon-normal property of $\xi$ are hypotheses even if $\xi\ne T$.

### Facts & Assumptions

[F1] The collapse-class definition records every end-of-§2 hypothesis and its supporting end and causal chain. [def-author-4cb89398a4ab-racz-wald-collapse-class](item-def-author-4cb89398a4ab-racz-wald-collapse-class)

[F2] The signed scalar belongs to the specified horizon-normal Killing field; nonzero constant surface gravity is an additional hypothesis. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[F3] Rácz–Wald Theorem 4.2 is the imported global-extension input under precisely these hypotheses.

### External input

Apply Rácz–Wald Theorem 4.2 to [F1] and the nonzero-constant hypothesis [F2]. It supplies the isometric extension of the whole spacetime, the proper-subset bifurcate horizon, the extended group $\chi_u$, and wedge reflection. The source construction identifies the reflection as $(U,V)\mapsto(-U,-V)$. This is an external theorem input, not a locally reconstructed proof. Its §5 separates the further problem of extending invariant tensor fields; no tensor extension follows from this item alone.


## Commuting complete flows give the global product action

[Open item](item-lem-author-64ac0bd1fcc4-commuting-global-symmetry-action) · level 6


### Statement

For the supplied global flows, the map $\alpha((t,[s]),p)=\phi_t(\psi_s(p))$ defines a smooth isometric action of $\mathbb R\times(\mathbb R/2\pi\mathbb Z)$. Here $[s]$ denotes the class of $s$ modulo $2\pi$. This uses the supplied global action convention; it asserts no extension of a locally defined symmetry.

### Statement references

[def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data](item-def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data)

[def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[math:def-lie-group](https://alphabetamath.cc/item/def-lie-group)

[math:thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group](https://alphabetamath.cc/item/thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group)

[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[math:def-smooth-left-action-of-a-lie-group](https://alphabetamath.cc/item/def-smooth-left-action-of-a-lie-group)

### Facts & Assumptions

[F1] Work in the ZFC convention of the global comparison data. Both supplied flows are global isometries, the axial flow is $2\pi$-periodic, and the flows commute. The circle-action convention fixes that period. [def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data](item-def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data) [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[F2] A global flow is jointly smooth in parameter and point, has value the identity at parameter zero, and satisfies the flow law for all real parameters. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F3] Smooth multiplication and inversion define a finite-dimensional real Lie group. Under countable choice, the quotient by a closed normal subgroup is a Lie group; the quotient-manifold theorem makes its projection a smooth surjective submersion. The constant-rank theorem gives local projection coordinates for a submersion. [math:def-lie-group](https://alphabetamath.cc/item/def-lie-group) [math:thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group](https://alphabetamath.cc/item/thm-quotient-by-a-closed-normal-subgroup-is-a-lie-group) [math:thm-quotient-manifold-by-a-closed-lie-subgroup](https://alphabetamath.cc/item/thm-quotient-manifold-by-a-closed-lie-subgroup) [math:thm-constant-rank-theorem-for-manifolds](https://alphabetamath.cc/item/thm-constant-rank-theorem-for-manifolds)

[F4] Products carry their canonical product smooth structures. Maps into a product are smooth exactly when their components are smooth, and composites of smooth maps are smooth. [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure) [math:prop-a-map-into-a-product-is-smooth-iff-its-components-are-smooth](https://alphabetamath.cc/item/prop-a-map-into-a-product-is-smooth-iff-its-components-are-smooth) [math:prop-identity-maps-and-composites-of-smooth-maps-are-smooth](https://alphabetamath.cc/item/prop-identity-maps-and-composites-of-smooth-maps-are-smooth)

[F5] A smooth left action is a jointly smooth map satisfying the identity and action laws. [math:def-smooth-left-action-of-a-lie-group](https://alphabetamath.cc/item/def-smooth-left-action-of-a-lie-group)

[F6] Full choice implies countable choice, so the quotient theorems' choice hypothesis is available in the inherited ZFC convention. [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

### Proof

**Given:** The supplied global commuting isometric flows with their inherited ZFC convention.

**Goal:** Verify the smooth product-group action, including joint smoothness on the quotient parameters.

1.1 The usual smooth real line is a Lie group under addition: addition and negation have polynomial coordinate formulas. Put $\Lambda=2\pi\mathbb Z$. This is a subgroup, and it is normal because addition is abelian. It is closed: for $x\notin\Lambda$, choose a bounded open interval about $x$. Only finitely many integer multiples of the positive number $2\pi$ lie in that interval, and a smaller interval about $x$ avoids those finitely many points. Thus the complement of $\Lambda$ is open. Countable choice follows from the supplied ZFC convention. [F1, F3, F6]

2.1 Apply the quotient theorems to obtain the quotient Lie group $C=\mathbb R/\Lambda$, with addition $[s]+[v]=[s+v]$, and the smooth surjective submersion $q:\mathbb R\to C$. Near each $c\in C$, the constant-rank coordinates express $q$ as a projection; fixing the discarded coordinates gives a smooth section $\sigma:U\to\mathbb R$ with $q\circ\sigma=\mathrm{id}_U$. Give $G=\mathbb R\times C$ the product smooth structure and componentwise addition. Its multiplication and inversion are smooth by the component and composition rules, so it is a Lie group with identity $(0,[0])$. [F3, F4, step 1.1]

3.1 Periodicity gives $\psi_{s+2\pi n}=\psi_s$ for every integer $n$, so the formula for $\alpha$ is independent of the representative of $[s]$. On $\mathbb R\times U\times M$, using a section from step 2.1, it is $\alpha((t,c),p)=\phi_t(\psi_{\sigma(c)}(p))$. The two flows are jointly smooth, and the component and composition rules make this local expression jointly smooth in all three variables. Such neighborhoods cover $G\times M$, proving joint smoothness of $\alpha$. [F1, F2, F4, step 2.1]

4.1 The zero-parameter flow identities give $\alpha((0,[0]),p)=p$. For $a=(t,[s])$ and $b=(u,[v])$, commutation and the flow laws give $\phi_t\psi_s\phi_u\psi_v=\phi_{t+u}\psi_{s+v}$, hence $\alpha(a,\alpha(b,p))=\alpha(a+b,p)$ for every $p$. Together with joint smoothness, these are precisely the smooth left-action axioms. Each action map is an isometry: applying the metric-preservation identity successively to the differentials of $\psi_s$ and $\phi_t$ preserves $g$ under their composite. Thus the claimed global smooth isometric action is obtained from the supplied global flows. [F1, F2, F5, step 2.1, step 3.1] ∎



## Harmonic-map and Weyl reconstruction comparison data

[Open item](item-def-author-abbd1939ec07-reconstructed-harmonic-map-data) · level 6


### Definition

Let $\Gamma=\{\rho=0\}\subset\mathbb R^3$ be the rotation axis in cylindrical coordinates $(\rho,z,\phi)$, with $\phi$ of period $2\pi$. A reconstructed vacuum-map datum consists of the ordered rods of the ordered finite vacuum rod datum, two smooth real axisymmetric functions $u,v$ on $\mathbb R^3\setminus\Gamma$, and smooth functions $w,\alpha$ there, satisfying $\Delta u=2e^{4u}|\nabla v|^2$ and $\Delta v+4\nabla u\cdot\nabla v=0$. Derivatives and norms here are Euclidean. Equivalently these are the harmonic-map equations for the explicitly specified target metric $du^2+e^{4u}dv^2$; only the displayed equations are used in this contract.

Put $U=u+\log\rho$. Require the reconstruction equations $w_\rho=2\rho e^{4u}v_z$, $w_z=-2\rho e^{4u}v_\rho$, $\alpha_\rho=\rho[U_\rho^2-U_z^2+e^{4u}(v_\rho^2-v_z^2)]$, and $\alpha_z=2\rho[U_\rho U_z+e^{4u}v_\rho v_z]$, together with $w\to0$ and $\alpha\to0$ at infinity. Define the reconstructed metric by $\mathbf g=-e^{2U}d\tau^2+\rho^2e^{-2U}(d\phi+w\,d\tau)^2+e^{-2U+2\alpha}(d\rho^2+dz^2)$ on $\mathbb R_\tau\times(\mathbb R^3\setminus\Gamma)$. The datum supplies $w,\alpha$; their global existence or a reduction of arbitrary stationary geometries is not part of the definition.

### Definition references

[def-author-abbd1939ec07-ordered-vacuum-rods](item-def-author-abbd1939ec07-ordered-vacuum-rods)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

### Facts & Assumptions

[F1] The supplied rods and twist labels are [def-author-abbd1939ec07-ordered-vacuum-rods](item-def-author-abbd1939ec07-ordered-vacuum-rods). Lorentzian tensor and stationary-field conventions are [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). Axisymmetry means independence of $\phi$.

[F2] A totally differentiable real function with zero derivative on a nonempty connected open Euclidean set is constant, by [math:thm-zero-derivative-on-connected-open-euclidean-set-iff-constant](https://alphabetamath.cc/item/thm-zero-derivative-on-connected-open-euclidean-set-iff-constant). The orbit half-plane $H=(0,\infty)\times\mathbb R$ is nonempty, open and convex, hence connected.

[F3] The harmonic-map interpretation and the displayed reconstruction formulas use the precise HKWX input recorded in External input and in the source contract; the supplied functions and their normalization are the hypotheses for the local argument.

### Justification

**Given:** Functions satisfying the stated equations and normalization, with the inputs in [F1]–[F3].

**Goal:** Verify that their reconstructed tensor is a well-defined stationary Lorentzian metric off the axis, and that the normalized reconstruction is unique conditional on existence.

1.1 Let $f$ be either $w$ or $\alpha$, and fix any two angular values $\phi_1,\phi_2$. On $H$, put $q(\rho,z)=f(\rho,z,\phi_1)-f(\rho,z,\phi_2)$. The right sides of the reconstruction equations are independent of $\phi$, because $u,v,U$ are axisymmetric. Thus $q$ is smooth with $q_\rho=q_z=0$. By [F2], $q$ is constant on $H$. Along $(\rho,z)=(R,0)$ with $R\to\infty$, both terms tend to zero by the normalization, so this constant is zero. As the angles were arbitrary, $w$ and $\alpha$ are axisymmetric. [given, F1, F2, algebra]

2.1 On $\rho>0$, all exponential coefficients are smooth and positive. The angular one-form $d\phi$ is globally defined off the axis: local angular coordinates differ by constant multiples of $2\pi$, so their differentials agree. The coframe $d\tau$, $d\phi+w\,d\tau$, $d\rho$, $dz$ is linearly independent, and the displayed tensor is diagonal in it with exactly one negative coefficient. Thus it is a smooth nondegenerate Lorentzian metric globally off the axis. Its coefficients are independent of $\tau$ by construction and of $\phi$ by step 1.1, so time translations and rotations preserve it; in particular $\partial_\tau$ is Killing in the stationary-field convention. [given, F1, step 1.1, algebra]

3.1 For fixed $u,v$ and two supplied normalized reconstruction pairs $(w,\alpha)$ and $(\widetilde w,\widetilde\alpha)$, fix $\phi$ and restrict each difference to $H$. The reconstruction equations give zero $\rho,z$ derivatives, so [F2] makes each difference constant on $H$. Along $(R,0)$ the zero limits of both pairs force each constant to vanish. This holds for every $\phi$, giving equality on the full off-axis domain. The reconstruction equalities are definite scalar predicates, and this argument establishes uniqueness conditional on existence without an integrability, global-existence or geometric-reduction assertion. [given, F2, step 2.1, algebra] ∎

### External input

HKWX §1 equation (1.2) and its following target-metric display identify the two stated PDEs as the axisymmetric harmonic-map equations from Euclidean $\mathbb R^3\setminus\Gamma$ into the target with metric $du^2+e^{4u}dv^2$. Equations (1.1), (1.3) and (1.4), and the paragraph after (1.4), supply the metric ansatz, reconstruction quadratures and zero normalization adopted here. This is an imported identification of the displayed equations, not a claimed local proof of a stationary-vacuum reduction or a global reconstruction theorem. The Lorentzian-signature, symmetry and conditional-uniqueness arguments above are local.


## Gram determinant for the two symmetry directions

[Open item](item-lem-author-64ac0bd1fcc4-orbit-gram-determinant) · level 7


### Statement

Let $X_1=T$ and $X_2=Z$ be the generators of the action in [lem-author-64ac0bd1fcc4-commuting-global-symmetry-action](item-lem-author-64ac0bd1fcc4-commuting-global-symmetry-action). Define their Gram matrix by $H_{ij}=g(X_i,X_j)$ and their signed orbit-area square by $W=-\det H$. Under an invertible real change of basis $X'_i=A_i{}^jX_j$, one has $H'=AHA^{\mathsf T}$ and $W'=(\det A)^2W$. Consequently invertibility of the orbit Gram matrix and the sign of $W$ do not depend on that basis. Use the metric conventions in [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). This algebra does not prove that $W$ is positive anywhere.

### Facts & Assumptions

[F1] The stationary flow $\phi_t$ is generated by $T$, and the normalized axial flow $\psi_s$ is generated by $Z$. The generators are smooth ambient vector fields and the metric is symmetric and bilinear. A basis change here is an invertible two-by-two real matrix at the point under consideration. [lem-author-64ac0bd1fcc4-commuting-global-symmetry-action](item-lem-author-64ac0bd1fcc4-commuting-global-symmetry-action) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data](item-def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data) [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[F2] The determinant of a real square matrix is its finite Leibniz sum over permutations. We use this definition for each real two-by-two matrix here. [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)

[F3] Matrix multiplication is given by $(BC)_{ij}=\sum_k B_{ik}C_{kj}$, and transpose by $(B^{\mathsf T})_{ij}=B_{ji}$. These definitions apply to the real two-by-two matrices here. [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)

[F4] For square matrices $B,C$ of the same positive finite size over a commutative ring, $\det(BC)=\det(B)\det(C)$ and $\det(B^{\mathsf T})=\det B$. Apply these results over $\mathbb R$ at size two. [math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative) [math:thm-determinant-of-transpose](https://alphabetamath.cc/item/thm-determinant-of-transpose)

[F5] A real square matrix of positive finite size is invertible if and only if its determinant is nonzero. [math:thm-real-square-matrix-invertible-iff-determinant-nonzero](https://alphabetamath.cc/item/thm-real-square-matrix-invertible-iff-determinant-nonzero)

### Proof

**Given:**The generators, metric and change of basis at one point.

**Goal:** Compute the transformed matrix and signed determinant.

1.1 Bilinearity gives $g(X'_i,X'_j)=A_i{}^kA_j{}^\ell H_{k\ell}$. By the definitions of matrix product and transpose this is exactly $H'=AHA^{\mathsf T}$. [given, F1, F3]

2.1 Apply determinant multiplicativity twice and transpose invariance to obtain $\det H'=\det(A)\det(H)\det(A^{\mathsf T})=(\det A)^2\det H$. Negating this equality gives $W'=(\det A)^2W$. [F2, F4, step 1.1]

3.1 Since $A$ is invertible, $\det A\ne0$ by the real-matrix criterion; hence $(\det A)^2>0$. The determinant identity therefore gives $\det H'\ne0$ if and only if $\det H\ne0$. Applying the same criterion to $H'$ and $H$ proves invertibility invariance, and the positive multiplier preserves the sign of $W$, including its zero value. [given, F5, step 2.1, algebra] ∎


## Exact mixed-rod boundary class for the balance theorem

[Open item](item-def-author-abbd1939ec07-mixed-rod-asymptotic-class) · level 7


### Definition

An admissible HKWX mixed-rod datum is a reconstructed vacuum-map datum with its supplied ordered rods satisfying all the conditions below. Write $\Phi=(u,v)$, $e(u,v)=|\nabla u|^2+e^{4u}|\nabla v|^2$ and $e'(U,v)=|\nabla U|^2+e^{4u}|\nabla v|^2$. Locally integrable means integrable on every compact subset of the specified neighborhood, with Euclidean volume. In the trace conditions below, use a continuous extension of $v$ to each compact subinterval of the indicated open axis rod, equal there to $c_j$; the source provides such representatives in Proposition 2.1(i).

(V) Require local minimality of renormalized energy under competitors preserving the specified singularity data and rod traces, in the variational class of HKWX §2.1. Adopt this source hypothesis independently of the harmonic-map equations; no implication from those equations alone is asserted here.

(A1a) Near each compact subinterval $I$ of an open axis rod, $U,v$ are bounded, $e'(U,v)$ is integrable on a neighborhood of $I$, and $v=c_j$ in trace on $I$.

(A1b) Near every compact subinterval inside a nondegenerate horizon rod, $u,v$ are bounded and $e(u,v)$ is integrable.

(A1c) At the lower and upper pole of a nondegenerate rod, respectively put $\zeta=z-z_i^\pm$ and $r=\sqrt{\rho^2+\zeta^2}$. The renormalized functions are $\widehat U_i^-=U-\tfrac12\log(r-\zeta)$ and $\widehat U_i^+=U-\tfrac12\log(r+\zeta)$. Require $\widehat U_i^\pm,v$ bounded and $|\nabla\widehat U_i^\pm|^2+e^{4u}|\nabla v|^2$ integrable near the pole.

(A2) At each degenerate puncture use centered polar coordinates $(r_i,\theta_i,\phi)$. For some $\epsilon_i,\Lambda_i>0$, require $|u+\log\sin\theta_i|\le\Lambda_i$ off the axis in $B_{\epsilon_i}(p_i)$ and $e'(U,v)$ locally integrable on $B_{\epsilon_i}(p_i)\setminus\{p_i\}$. The adjacent axis traces are $c_i,c_{i+1}$ and satisfy $c_{i+1}-c_i=4\mathcal J_i\ne0$.

(A3) Outside a sufficiently large ball, $U,v$ are bounded, $e'(U,v)$ is locally integrable including across the ordinary axis, $v$ has traces $c_1,c_{N+1}$ on the two semi-infinite rods, and $U\to0$ at infinity. These are explicit input conditions; calling a spacetime regular does not, by this definition alone, verify them.

(H) For every compact subinterval $I\subset\operatorname{Int}\mathcal H_i$ of a nondegenerate rod, $u,v$ extend smoothly and axisymmetrically to a neighborhood of $I$ in $\mathbb R^3$. For a real constant $\kappa_i$ common to that rod, require $\alpha=\log\rho+2u+\kappa_i+O(\rho^2)$, uniformly near each such $I$. Here $O(\rho^2)$ means that the remainder has absolute value at most $C_I\rho^2$ on a sufficiently small neighborhood off the axis. This specifies the horizon-interior behavior using Proposition 2.1(iii), equation (2.23).

### Definition references

[def-author-abbd1939ec07-ordered-vacuum-rods](item-def-author-abbd1939ec07-ordered-vacuum-rods)

[def-author-abbd1939ec07-reconstructed-harmonic-map-data](item-def-author-abbd1939ec07-reconstructed-harmonic-map-data)

### Facts & Assumptions

[F1] All functions, rods, reconstruction equations and normalizations are [def-author-abbd1939ec07-ordered-vacuum-rods](item-def-author-abbd1939ec07-ordered-vacuum-rods) and [def-author-abbd1939ec07-reconstructed-harmonic-map-data](item-def-author-abbd1939ec07-reconstructed-harmonic-map-data).

[F2] The source contract below supplies (V), (A1)–(A3), the continuous axis representative, and (H). The local-minimization premise is retained explicitly: (A1)–(A3) alone are not advertised as the full source framework. These are mathematical conditions on supplied functions, not physical regularity postulates or a theorem placing generic spacetimes in the class.

### Justification

**Given:** The reconstructed functions, neighborhoods and finite rod labels in [F1], with the independently adopted source predicates in [F2].

**Goal:** Check the elementary renormalizations and interval cases, while retaining the imported variational and boundary requirements as inputs.

1.1 All logarithms are evaluated where their arguments are positive off the axis. Indeed $r>|\zeta|$ there, and $\sin\theta_i>0$. Each displayed renormalization therefore defines a smooth function on the punctured off-axis domain; its boundedness and the specified energy integrals are definite scalar conditions. [given, F1, algebra]

2.1 The interval classification determines which conditions apply: poles and interior-rod conditions apply only to strict intervals, and puncture conditions only to singletons. The trace constants and nonzero differences are finite numerical requirements. The horizon condition specifies smooth extensions and an explicit uniform remainder bound on each compact interior interval. Conjoin these scalar and extension requirements with the separately adopted variational predicate [F2]; none is proved merely by naming a horizon regular. This checks the elementary formulation and does not prove existence, local minimality, or geometric spacetime membership. [given, F1, F2, step 1.1] ∎

### External input

HKWX §2.1 supplies the variational predicate (V) and the boundary/energy conditions (A1)–(A3). Proposition 2.1(i),(iii) supplies the axis representative and the explicit horizon-interior regularity used above, under the full §2.1 hypotheses. These premises are imported; the Justification checks only the local formulation.


## A regular weight-one axis has zero logarithmic angle defect

[Open item](item-lem-author-abbd1939ec07-regular-axis-angle-ratio) · level 7


### Statement

Suppose a reconstructed-map metric from [def-author-abbd1939ec07-reconstructed-harmonic-map-data](item-def-author-abbd1939ec07-reconstructed-harmonic-map-data) extends to a regular axis in the weight-one sense of [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data), and on an open axis interval $U$ and $\alpha$ extend continuously as finite functions. Then the logarithmic angle defect $\mathbf b(z):=\log\lim_{\rho\downarrow0} L(\rho,z)/(C(\rho,z)/(2\pi))$ is zero. Here $L(\rho,z)=\int_0^\rho e^{\alpha(s,z)-U(s,z)}ds$ is radial proper length in the orthogonal meridian and $C(\rho,z)=2\pi\rho e^{-U(\rho,z)}$ is axial orbit circumference. In this representation $\mathbf b(z)=\alpha(0,z)$.

Precisely, the extension hypothesis is an extension of this reconstructed metric together with its specified angular action. Locally at each interior axis value, take intervals $J$ in $\tau$ and $I$ in $z$ and $\delta>0$. There is a smooth isometric identification $\iota$ of $J\times(0,\delta)\times I\times S^1$ with an open subset of $M\setminus A$, where $(M,g)$ has the regular weight-one axis $A$ and smooth circle action $\psi_s$. It obeys $\iota(\tau,\rho,z,\phi+s)=\psi_s(\iota(\tau,\rho,z,\phi))$ and $\iota^*g=\mathbf g$. It has a continuous extension $\bar\iota$ to $J\times[0,\delta)\times I\times S^1$ with $\bar\iota(\tau,0,z,\phi)=p(\tau,z)\in A$, independently of $\phi$. This specifies what extension across the coordinate axis means here; no differentiability of $\bar\iota$ at the axis is required, and existence of such an extension is not inferred from the off-axis reconstruction equations.

### Facts & Assumptions

[F1] The metric and period $2\pi$ are [def-author-abbd1939ec07-reconstructed-harmonic-map-data](item-def-author-abbd1939ec07-reconstructed-harmonic-map-data). Smooth extension and the weight-one differential circle action on a spacelike normal plane are the regular-axis conditions of [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data). All limits in the statement are taken at a fixed interior point of the open axis interval. The identification $\iota$, its equivariance and its continuous boundary extension are the explicit meaning of the extension hypothesis in the Statement; the two suppliers alone do not assert that an off-axis reconstruction admits this extension.

[F2] An embedded smooth axis has local slice charts by [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart). An invertible differential gives a smooth local coordinate change by [math:thm-smooth-inverse-function-theorem-on-manifolds](https://alphabetamath.cc/item/thm-smooth-inverse-function-theorem-on-manifolds). Derivatives of the smooth action can be interchanged by [math:thm-clairaut-schwarz-mixed-partials](https://alphabetamath.cc/item/thm-clairaut-schwarz-mixed-partials). Taylor expansion with bounded remainders on smaller coordinate neighborhoods is supplied by [math:thm-multivariable-taylor-formula-with-lagrange-remainder](https://alphabetamath.cc/item/thm-multivariable-taylor-formula-with-lagrange-remainder), applied also to derivatives.

[F3] The invariant inverse-metric pairing and its matrix formula are [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms); its smoothness is [physics:lem-gr-inverse-metric-is-smooth](https://alphabetamath.cc/physics/item/lem-gr-inverse-metric-is-smooth). Both suppliers have domain mathematics. Euclidean differentiation of compositions and rescalings uses [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives).

[F4] Closed Euclidean balls and boxes are compact by [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn), so continuous real functions on them attain their extrema by [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric). A differentiable function at an interior local extremum has zero gradient by [math:thm-fermat-for-euclidean-local-extrema](https://alphabetamath.cc/item/thm-fermat-for-euclidean-local-extrema).

### Proof

**Given:** The reconstructed metric, its continuous meridian coefficients and its regular weight-one extension, realized by the specified equivariant isometric identification $\iota$ with continuous boundary extension $\bar\iota$.

**Goal:** Compute the angle ratio and prove that its logarithm vanishes, without assuming a limiting tangent for the coordinate meridian.

1.1 Fix an interior axis value $z_0$. Restricting the metric to the fixed-$\tau,z,\phi$ meridian and the axial orbit gives exactly $L$ and $C$. Continuity gives $L(\rho,z_0)/\rho\to e^{\alpha(0,z_0)-U(0,z_0)}$: the difference between this average integral and its limiting integrand is bounded by the supremum of the integrand's difference on $[0,\rho]$. Also $C(\rho,z_0)/(2\pi\rho)\to e^{-U(0,z_0)}>0$. Thus the ratio in the statement tends to $e^{\alpha(0,z_0)}$. It remains to show this is one. [given, F1, algebra]

1.2 Write $Z$ for the smooth axial generator and $A$ for the fixed axis. Near the axis point under consideration choose coordinates $(x^0,x^1,y^1,y^2)$ with $A=\{y=0\}$ and with $\partial_{y^1},\partial_{y^2}$ an orthonormal normal pair along $A$. Here is a local construction of the latter refinement of a slice chart. The tangential metric block along $A$ is invertible, because the normal plane is nondegenerate and $g$ is nondegenerate. Subtract the tangential projections of the two transverse coordinate vectors to obtain a normal basis $V_1,V_2$. Put $e_1=V_1/\sqrt{g(V_1,V_1)}$, $W_2=V_2-g(V_2,e_1)e_1$, and $e_2=W_2/\sqrt{g(W_2,W_2)}$. All denominators are smooth and positive. In the original chart map $(x,y)$ to $(x,0)+y^1 e_1(x)+y^2 e_2(x)$, where the vectors are expressed in that chart. Its differential at $y=0$ maps to a tangential basis and this normal pair, hence is invertible; [F2] makes this a local chart. In these refined coordinates $g_{ab}(x,0)=\delta_{ab}$ and $g_{ia}(x,0)=0$ for normal indices $a,b$ and tangential indices $i$. [given, F1, F2, F3, construct, algebra]

2.1 At $y=0$ the generator vanishes. Differentiating the action in its parameter and in the coordinates, with the derivative interchange in [F2], shows that its linearization is zero tangentially and is the generator $J$ of the weight-one rotation on the normal plane; $J^{\mathsf T}J=I$. The sign of $J$ can be fixed locally and does not affect the calculation. With $r=|y|$, Taylor expansion gives tangential components $Z^i=O(r^2)$ and normal components $Z^a=(Jy)^a+O(r^2)$. Consequently, for $f=g(Z,Z)$, Taylor expansion of $f$ and its first derivatives gives $f=r^2+O(r^3)$, $\partial_{y^a}f=2y^a+O(r^2)$ and $\partial_{x^i}f=O(r^2)$. These estimates are uniform on a smaller chart: bound the finitely many required smooth derivatives on a closed coordinate box using [F4]. For the positive orbit radius $R=\sqrt{f}$ off the axis, it follows that $R=r+O(r^2)$, $\partial_{y^a}R=y^a/r+O(r)$ and $\partial_{x^i}R=O(r)$. The smooth inverse metric has normal block $I+O(r)$, mixed block $O(r)$ and bounded tangential block. Thus the invariant scalar $Q:=g^{-1}(dR,dR)=1+O(r)$ tends to one, uniformly in a local axis neighborhood. This uses smooth axis geometry, without asserting that the Weyl meridian has a smooth limiting tangent. [F1, F2, F3, F4, step 1.2, algebra]

3.1 The axial generator used above is the one measured by the reconstructed angular coordinate: differentiating the equivariance identity in $s$ at zero, off the axis, gives $d\iota(\partial_\phi)=Z\circ\iota$. Therefore $g(Z,Z)\circ\iota=\mathbf g(\partial_\phi,\partial_\phi)=\rho^2e^{-2U}$. The isometric identification and the chain rule also identify the inverse-metric norm of the differential of this orbit radius on the two open manifolds: in local charts, put $P=D\iota$, let $G$ be the matrix of $g$, and let $\lambda$ be the column of components of $dR$. The pulled-back metric matrix and covector column are $P^{\mathsf T}GP$ and $P^{\mathsf T}\lambda$; since $P$ is invertible, $(P^{\mathsf T}\lambda)^{\mathsf T}(P^{\mathsf T}GP)^{-1}(P^{\mathsf T}\lambda)=\lambda^{\mathsf T}G^{-1}\lambda$. To check the approach to the axis, fix $\tau_0\in J$, $\phi_0\in S^1$, $z_0\in I$, and put $p_0=p(\tau_0,z_0)$. For $K=\{\xi\in\mathbb R^2:|\xi-(1,0)|\le1/4\}$, define $q_\epsilon(\xi)=\iota(\tau_0,\epsilon\xi_1,z_0+\epsilon\xi_2,\phi_0)$. The parameter points defining $q_\epsilon$ are at Euclidean $(\rho,z)$ distance at most $5\epsilon/4$ from $(0,z_0)$, since $|\xi|\le5/4$ on $K$. By continuity of $\bar\iota$ at $(\tau_0,0,z_0,\phi_0)$, every neighborhood of $p_0$ therefore contains all $q_\epsilon(K)$ for sufficiently small $\epsilon$. In the smaller smooth chart of step 2.1, the normal coordinates of these points consequently tend to zero uniformly, and the uniform estimate $Q=1+O(r)$ there yields $Q(q_\epsilon(\xi))\to1$ uniformly on $K$. This establishes the needed coordinate-to-extension limit without differentiating the boundary extension. [given, F1, F3, step 2.1, algebra]

4.1 By the generator identification in step 3.1, in the reconstructed coordinates $R=\rho e^{-U}=C/(2\pi)$, independently of $\tau,\phi$. Inverting the meridian block of the displayed reconstructed metric therefore gives $Q=e^{2U-2\alpha}(R_\rho^2+R_z^2)$. In particular $|D R|=e^{\alpha-U}\sqrt{Q}$, where $D$ and its norm are Euclidean in $(\rho,z)$. Set $B=e^{-U(0,z_0)}>0$ and $H=e^{\alpha(0,z_0)-U(0,z_0)}>0$. On the closed Euclidean disk $K=\{\xi\in\mathbb R^2:|\xi-(1,0)|\le1/4\}$ define $F_\epsilon(\xi)=R(\epsilon\xi_1,z_0+\epsilon\xi_2)/\epsilon$ for positive sufficiently small $\epsilon$. This disk stays off the axis. Continuity of $U,\alpha$ at $(0,z_0)$ gives $F_\epsilon\to B\xi_1$ uniformly on $K$. Step 3.1 gives $Q\to1$ uniformly on these shrinking coordinate disks. The chain rule and the inverse-block identity then give $|D F_\epsilon|\to H$ uniformly on $K$. No convergence of derivatives of $U$ or $\alpha$ has been assumed. [given, F1, F3, step 3.1, algebra]

5.1 To compare these two limits, fix $\eta>0$ and set $h_\epsilon(\xi)=F_\epsilon(\xi)-B\xi_1$ and $\xi_*=(1,0)$. The continuous function $h_\epsilon(\xi)-\eta|\xi-\xi_*|^2$ attains a maximum on $K$ by [F4]. For small $\epsilon$ it is smaller on the boundary than at $\xi_*$: the boundary penalty is $\eta/16$, while $2\sup_K|h_\epsilon|\to0$. Hence a maximizer $\xi_\epsilon$ is interior, and Fermat's theorem gives $D F_\epsilon(\xi_\epsilon)=B(1,0)+2\eta(\xi_\epsilon-\xi_*)$. The reverse triangle inequality implies $\bigl||D F_\epsilon(\xi_\epsilon)|-B\bigr|\le\eta/2$. Uniform gradient-norm convergence in step 4.1 now implies $|H-B|\le\eta/2$. Since $\eta>0$ was arbitrary, $H=B$. [F4, step 4.1, choose, algebra]

6.1 The equality $H=B$ is $e^{\alpha(0,z_0)-U(0,z_0)}=e^{-U(0,z_0)}$, so $e^{\alpha(0,z_0)}=1$ and $\alpha(0,z_0)=0$. Step 1.1 then gives $\mathbf b(z_0)=\alpha(0,z_0)=0$. As $z_0$ was arbitrary in the open interval, this proves the full statement. [step 1.1, step 4.1, step 5.1, algebra] ∎


## Analytic extremal and multiple-horizon comparison contracts

[Open item](item-pthm-analytic-connectedness-and-extremal-input) · level 8


### Statement

Two independent source comparison results are retained with separate hypotheses.

(1) A four-dimensional stationary rotating asymptotically flat analytic vacuum black hole with one degenerate horizon is extremal Kerr under the source's global black-hole regularity conditions. The precise connected $I^+$-regular comparison data are [def-author-abbd1939ec07-connected-degenerate-comparison-data](item-def-author-abbd1939ec07-connected-degenerate-comparison-data). No bifurcation sphere is assumed for a degenerate generator.

(2) The stationary axisymmetric vacuum balance theorem excludes a regular configuration with $N>1$ horizons when its singular harmonic map belongs to the explicit admissible mixed-rod class [def-author-abbd1939ec07-mixed-rod-asymptotic-class](item-def-author-abbd1939ec07-mixed-rod-asymptotic-class) and every degenerate component has nonzero angular momentum. In fact each finite inter-horizon axis interval has strictly negative logarithmic angle defect. This allows arbitrary mixtures of nondegenerate rods and degenerate punctures and puts no angular-momentum condition on the nondegenerate rods.

Neither contract by itself treats non-rotating degenerate vacuum horizons outside its stated class or proves smooth nonanalytic uniqueness. To apply (2) to a geometric spacetime one must verify its membership in that class; regularity and axisymmetry are not substituted for the class's energy, trace and puncture requirements.

### Facts & Assumptions

[A1] Work in ZFC, [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice). Vacuum general relativity means the source-free zero-cosmological-constant specialization of [physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law), so the geometric field equation is $\operatorname{Ric}(g)=0$.

[F1] The connected rotating degenerate comparison hypotheses are [def-author-abbd1939ec07-connected-degenerate-comparison-data](item-def-author-abbd1939ec07-connected-degenerate-comparison-data). The finite rod labels, twist gauge, reconstruction and complete admissibility conditions are [def-author-abbd1939ec07-ordered-vacuum-rods](item-def-author-abbd1939ec07-ordered-vacuum-rods), [def-author-abbd1939ec07-reconstructed-harmonic-map-data](item-def-author-abbd1939ec07-reconstructed-harmonic-map-data) and [def-author-abbd1939ec07-mixed-rod-asymptotic-class](item-def-author-abbd1939ec07-mixed-rod-asymptotic-class). A regular weight-one axis has zero logarithmic angle defect by [lem-author-abbd1939ec07-regular-axis-angle-ratio](item-lem-author-abbd1939ec07-regular-axis-angle-ratio).

[F2] The exact uniqueness and balance results, and the more limited global-representation and degenerate-local-control inputs, are imported below with their separate hypotheses. The latter inputs are recorded without claiming that a generic geometric spacetime has passed the full HKWX admissibility test.

[F3] The variational premise (V) and conditions (A1)–(A3) in the mixed-rod definition are the hypotheses of HKWX §2.1. Proposition 2.1(i)–(iv) supplies the asymptotic estimates needed by Theorem 1.1; (H) records the regular horizon-interior behavior. This regularity result is an imported premise, not an inference from harmonicity alone.

### External input

The only four-dimensional stationary, rotating, asymptotically flat analytic vacuum black hole with a single degenerate horizon, under the source black-hole regularity assumptions, is the extremal Kerr black hole.

For $N>1$, let a stationary vacuum singular harmonic map with ordered black-hole rod data locally minimize renormalized energy with fixed rod traces and singularity data, and satisfy the source's ordinary-axis, nondegenerate-pole, regular horizon-interior, degenerate-puncture and infinity conditions. Reconstruct the Weyl–Papapetrou metric with $w\to0$ and $\alpha\to0$ at infinity. If every degenerate component has $\mathcal J_i\ne0$, every bounded axis rod has $\mathbf b_j<0$ for $2\le j\le N$. There is no regular asymptotically flat stationary axisymmetric multi-black-hole configuration in this class. No angular-momentum condition is imposed on nondegenerate rods.

HKWX Proposition 2.1 applies to harmonic maps satisfying all the hypotheses of §2.1, including local minimization of renormalized energy. Its parts (i)–(iv) provide ordinary-axis regularity and the puncture, nondegenerate-pole/interior and infinity estimates, with (2.12)–(2.26). These are the estimates identified just before Theorem 1.1. The current mixed-rod definition explicitly supplies those hypotheses and regular horizon-interior behavior; no additional asymptotic assumption is inferred from harmonicity alone.

A stationary, $I^+$-regular, analytic electrovacuum spacetime with connected nonempty rotating degenerate future event horizon has a domain of outer communications isometrically diffeomorphic to that of a Kerr–Newman spacetime. Independently, in the stationary axisymmetric asymptotically flat $I^+$-regular vacuum setting, near every degenerate horizon component the Ernst map is at bounded hyperbolic-plane distance from that of extreme Kerr with the same positive horizon cross-section area; its two adjacent axial twist constants differ in absolute value by $4r_0^2$, where $r_0$ is the positive area radius.

A stationary, axisymmetric, asymptotically flat, $I^+$-regular, electrovacuum four-dimensional spacetime has a domain of outer communications isometric to one of the Weinstein solutions. If the event horizon is connected, that domain is a Kerr–Newman domain of outer communications. The preceding reduction discussion states that global isothermal coordinates and controlled boundary conditions extend to configurations with degenerate components.

### Source notes

The uniqueness and balance contracts retain separate source hypotheses. The current mixed-rod definition supplies the variational and boundary hypotheses used by HKWX Proposition 2.1, which supplies the asymptotics used by its balance theorem. A geometric consumer must still establish that its spacetime yields data in this class and must justify nonzero degenerate angular momenta. Chruściel–Nguyen's local twist jump and the Weinstein representation input are retained for their stated purposes; they do not by themselves establish full HKWX class membership for an arbitrary geometric spacetime.


## Orthogonal projection away from the symmetry plane

[Open item](item-lem-author-64ac0bd1fcc4-orthogonal-orbit-projection) · level 8


### Statement

At a point where the matrix $H$ of [lem-author-64ac0bd1fcc4-orbit-gram-determinant](item-lem-author-64ac0bd1fcc4-orbit-gram-determinant) is invertible, write its inverse as $H^{ij}$ and put $P(V)=V-X_iH^{ij}g(X_j,V)$. Then $P(V)$ is orthogonal to both generators, $P(X_i)=0$, and $P$ is the identity on vectors orthogonal to both. The symmetric form $q(V,W)=g(V,W)-g(V,X_i)H^{ij}g(X_j,W)$ equals $g(PV,PW)$ and annihilates the orbit plane. All conventions are those of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). No global quotient coordinate or positivity theorem is asserted.

### Facts & Assumptions

[F1] The metric is symmetric and the invertible Gram matrix has $H^{ij}H_{jk}=\delta^i_k$; repeated indices $i,j$ are summed over $1,2$. [lem-author-64ac0bd1fcc4-orbit-gram-determinant](item-lem-author-64ac0bd1fcc4-orbit-gram-determinant) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

### Proof

**Given:**The metric, generators and invertible Gram matrix.

**Goal:** Check projection and the displayed form.

1.1 Direct substitution gives $g(X_k,PV)=g(X_k,V)-H_{ki}H^{ij}g(X_j,V)=0$. Substitution of $V=X_k$ gives $P(X_k)=0$. If $g(X_j,V)=0$ for both $j$, the defining formula gives $PV=V$. [given, F1]

2.1 Expand $g(PV,PW)$. The two cross terms are each $-g(V,X_i)H^{ij}g(X_j,W)$, and the quadratic term restores one copy by the inverse identity. The resulting expression is exactly $q(V,W)$; the projection property then shows it annihilates the orbit plane. [F1, step 1.1] ∎



## Algebraic reconstruction from orbit and horizontal metric data

[Open item](item-lem-author-64ac0bd1fcc4-orbit-metric-reconstruction) · level 9


### Statement

For the projection data of [lem-author-64ac0bd1fcc4-orthogonal-orbit-projection](item-lem-author-64ac0bd1fcc4-orthogonal-orbit-projection), define one-forms $\sigma^i(V)=H^{ij}g(X_j,V)$. Then the full metric is $g=H_{ij}\sigma^i\otimes\sigma^j+q$. Thus agreement of $H$, the one-forms $\sigma^i$ and $q$ on a common domain implies agreement of the full metric there. The Gram-matrix and tensor conventions are those of [lem-author-64ac0bd1fcc4-orbit-gram-determinant](item-lem-author-64ac0bd1fcc4-orbit-gram-determinant) and [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data). This is an algebraic reconstruction identity, not an assertion that an Ernst-map uniqueness theorem alone supplies the global one-forms or identifies the domains.

### Facts & Assumptions

[F1] The inverse Gram matrix defines $P$ and $q$ as in the projection lemma, and every vector decomposes as $V=X_i\sigma^i(V)+PV$. [lem-author-64ac0bd1fcc4-orthogonal-orbit-projection](item-lem-author-64ac0bd1fcc4-orthogonal-orbit-projection) [lem-author-64ac0bd1fcc4-orbit-gram-determinant](item-lem-author-64ac0bd1fcc4-orbit-gram-determinant) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] A one-form is a smooth covector field, of type $(0,1)$, and a covariant two-tensor field assigns a bilinear form to each tangent space. Equality of such fields is pointwise equality of these multilinear maps. Smoothness of a covector or covariant two-tensor field is tested by smooth component functions in each chart. [physics:def-gr-tensor-fields-and-components](https://alphabetamath.cc/physics/item/def-gr-tensor-fields-and-components)

[F3] For covectors $\alpha,\beta$ on the same tangent space, the tensor-product definition gives $(\alpha\otimes\beta)(V,W)=\alpha(V)\beta(W)$. We apply this definition pointwise to the one-forms in the Statement. [math:def-tensor-product-of-multilinear-tensors](https://alphabetamath.cc/item/def-tensor-product-of-multilinear-tensors)

[F4] For each finite $r\in\mathbb N$, if a real matrix-valued function on an open Euclidean domain has $C^r$ entries and nonzero determinant everywhere, its inverse has $C^r$ entries. We use this with chart dimension four and matrix size two. [math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)

[F5] For every finite $r\in\mathbb N$, finite componentwise sums and products of $C^r$ Euclidean maps are $C^r$; hence the same finite operations preserve smoothness. [math:thm-ck-euclidean-maps-closed-under-algebra-and-composition](https://alphabetamath.cc/item/thm-ck-euclidean-maps-closed-under-algebra-and-composition)

### Proof

**Given:**The pointwise tensors and decomposition in the Statement.

**Goal:** Recover the full metric from these data.

1.1 Inserting the vector decompositions into $g(V,W)$, both mixed terms vanish because $PV$ and $PW$ are orthogonal to the generators. The orbit term is $H_{ij}\sigma^i(V)\sigma^j(W)$ and the remaining term is $g(PV,PW)=q(V,W)$. [given, F1]

1.2 In a smooth coordinate chart, $H_{ij}=g_{ab}X_i^aX_j^b$ is a finite sum of products of smooth component functions of the metric and generators. Thus $H_{ij}$ and $\det H=H_{11}H_{22}-H_{12}H_{21}$ are smooth. The nonzero determinant locus is open by continuity. On the chart portion of that locus, apply the matrix-inversion result for every finite $r$ to obtain smooth $H^{ij}$. Each $\sigma^i$ is pointwise linear in its vector argument and has components $\sigma^i_a=H^{ij}g_{ba}X_j^b$, smooth by the finite-operation result. The component criterion makes these covectors smooth one-forms. The formula for $q$ in the projection input also has smooth components by the same finite-operation argument. [F1, F2, F4, F5, algebra]

2.1 The tensor-product evaluation rule gives $(H_{ij}\sigma^i\otimes\sigma^j+q)(V,W)=H_{ij}\sigma^i(V)\sigma^j(W)+q(V,W)$. The equality in step 1.1 holds at every point for every pair of tangent vectors, so pointwise equality of bilinear maps gives the asserted covariant-tensor identity. Equal tensors on its right side therefore give equal metrics on a common domain. It gives no mechanism for constructing that domain or controlling boundary conditions, which remain part of the external global classification input. [F1, F2, F3, step 1.1, step 1.2] ∎


## Connected smooth axisymmetric vacuum Kerr classification

[Open item](item-pthm-axisymmetric-vacuum-uniqueness-input) · level 10


### Statement

In the four-dimensional classical vacuum Einstein model with zero cosmological constant, assume the smooth global stationary-axisymmetric comparison data: a selected asymptotically flat end, complete stationary flow, global commuting axial circle action with regular axis, exact $I^+$-regularity and connected event horizon. These are the predicates of the supplied global axisymmetric comparison-data definition and black-hole comparison-hypothesis definition. Retain the mean-nondegeneracy hypothesis in the supplied Gaussian-null sense of the former definition. No additional orbit-space hypothesis is imposed beyond this explicit package. Work in ZFC, including choice. The model equation is $\operatorname{Ric}(g)=0$, the vacuum specialization of the adopted Einstein field law. Metric and causal notation use the stationary Lorentzian and causal-exterior interfaces.

The Kerr comparison object means the following full black-hole exterior family, including the extremal case. For $m>0$ and $|a|\le m$, set $r_+=m+\sqrt{m^2-a^2}$ and $D_{m,a}=\mathbb R_t\times(r_+,\infty)_r\times S^2$, with its product smooth structure. Use the round sphere metric $\gamma$, the rotation-dual one-form $\lambda$ and the height function $\zeta$, pulled back to this product, in the declared Kerr tensor convention; thus away from the poles $\gamma=d\theta^2+\sin^2\theta\,d\phi^2$, $\lambda=\sin^2\theta\,d\phi$ and $\zeta=\cos\theta$. Put $\Sigma=r^2+a^2\zeta^2$ and $\Delta=r^2-2mr+a^2$. The comparison metric is the globally smooth sphere-tensor expression

$$g_{m,a}=-\left(1-\frac{2mr}{\Sigma}\right)dt\otimes dt+\frac{\Sigma}{\Delta}\,dr\otimes dr+\Sigma\gamma+\frac{a^2(\Sigma+2mr)}{\Sigma}\,\lambda\otimes\lambda-\frac{2amr}{\Sigma}\left(dt\otimes\lambda+\lambda\otimes dt\right).$$

The independent Kerr geometry inputs identify $(D_{m,a},g_{m,a})$ as the open domain of outer communications relative to its selected asymptotically flat end, including $|a|=m$, when $r_+=m$ and $\Delta=(r-m)^2$. The rotation axis is included through $S^2$; the event-horizon boundary $r=r_+$ is excluded. For $|a|<m$ this agrees with the supplied subextremal Kerr tensor datum. Reversal of azimuth gives the equivalent convention with $a$ replaced by $-a$.

Then for some such $m,a$ there exists a diffeomorphism $F:D\to D_{m,a}$ with $F^*g_{m,a}=g|_D$. Thus the entire domain of outer communications $D$ is isometric to the domain of outer communications of a Kerr spacetime. The conclusion concerns the whole exterior, not just an Ernst potential or a neighborhood of the horizon, and does not classify arbitrary extensions beyond it.

No independent analyticity assumption is required for this axisymmetric comparison. Axisymmetry is already a global hypothesis; extending a locally constructed axial Killing field to all of $D$ is a separate obligation. The smooth classification source does not require mean-nondegeneracy, so this application retains that hypothesis without inferring pointwise nondegeneracy from it.

### Statement references

[def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data](item-def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data)

[def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)

[physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)

[physics:def-gr-fx-kerr-exterior](https://alphabetamath.cc/physics/item/def-gr-fx-kerr-exterior)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

### Facts & Assumptions

[A1] The adopted vacuum field equation is the zero-matter, zero-cosmological-constant specialization of the Einstein field law. [physics:post-gr-einstein-field-law](https://alphabetamath.cc/physics/item/post-gr-einstein-field-law)

[F1] Global end, causal, symmetry and regularity data use the exact named interfaces, with inherited ZFC conventions. The source's definition of $I^+$-regularity is retained in full. The global comparison-data definition supplies the meaning of a full-exterior isometry by diffeomorphism and metric pullback. [def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data](item-def-author-64ac0bd1fcc4-global-axisymmetric-comparison-data) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-black-hole-comparison-hypothesis-data](item-def-black-hole-comparison-hypothesis-data) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F2] The commuting global flows give an action of $\mathbb R\times S^1$; this is not obtained by continuing a merely local field. [lem-author-64ac0bd1fcc4-commuting-global-symmetry-action](item-lem-author-64ac0bd1fcc4-commuting-global-symmetry-action)

[F3] The signed Gram determinant, conditional orthogonal projection and algebraic metric reconstruction have the explicit local identities in the named suppliers. They introduce the objects relevant to orbit-space reduction without purporting to prove its global topology or boundary regularity. [lem-author-64ac0bd1fcc4-orbit-gram-determinant](item-lem-author-64ac0bd1fcc4-orbit-gram-determinant) [lem-author-64ac0bd1fcc4-orthogonal-orbit-projection](item-lem-author-64ac0bd1fcc4-orthogonal-orbit-projection) [lem-author-64ac0bd1fcc4-orbit-metric-reconstruction](item-lem-author-64ac0bd1fcc4-orbit-metric-reconstruction)

[F4] The published mathematical Kerr interface supplies the sphere-tensor notation and subextremal metric convention. In the notation there, $\lambda=\xi^\flat$ and its mass parameter is denoted here by $m$. Its subextremal restriction is preserved; it is not used to assert an extremal exterior or a domain-of-outer-communications property. Those full-family geometry inputs are imported separately below. [physics:def-gr-fx-kerr-exterior](https://alphabetamath.cc/physics/item/def-gr-fx-kerr-exterior)

### External input

Import the vacuum specialization of Chruściel–Costa–Heusler Theorem 3.2, read with §3.2.4's vacuum Kerr case. Theorem 3.2 gives an isometry of the full domain of outer communications; its electrovacuum conclusion is Kerr–Newman for a connected horizon, and the vacuum specialization is Kerr. Section 3.3.1 expressly distinguishes this theorem, requiring no analyticity, from the rigidity step that derives axisymmetry. Its explicit hypotheses are stationarity, axisymmetry, asymptotic flatness, $I^+$-regularity, dimension four and the electrovacuum equations, specialized here to vacuum; connectedness gives the Kerr conclusion. No unnamed additional orbit-space assumption is retained. Global orbit-space control, harmonic-map uniqueness and reconstruction are parts of this imported classification, not consequences proved by the elementary local suppliers.

Import the Kerr exterior manifold and its identification as the domain of outer communications for both subextremal and extremal parameters from Sbierski §3.2 and the opening of §3.2.1. His convention $0\le a\le m$, $m>0$, covers both regimes; reversing azimuth gives the negative-$a$ convention. This input identifies the full product exterior, including the sphere axis and excluding the horizon boundary; it is not merely a metric formula on a pole-free patch.

Import the metric coefficients and smooth spherical extension from Aretakis §§2.1–2.2, with the existing supplier's sphere-tensor notation. Section 2.1 fixes the Boyer–Lindquist coefficients in the $(-,+,+,+)$ convention; §2.2 supplies the regular Lorentzian metric and explicitly identifies the extremal domain of outer communications as $r>m$. Thus extremality is included without extrapolating the published subextremal interface's hypotheses. The whole-exterior classification and these comparison-family geometry facts are external established inputs; no local proof of them is claimed.

Chruściel–Costa 0806.0016 Theorem 1.3 is not invoked as a smooth theorem, and its Corollary 6.3 alone is not treated as a full metric classification. The five local intermediate items define the exact global hypothesis package and the elementary action, orbit and reconstruction algebra. They do not reconstruct the imported global classification proof or assert a mean-to-pointwise nondegeneracy bridge. Exact source hypotheses and actual reading limits appear in the references.
