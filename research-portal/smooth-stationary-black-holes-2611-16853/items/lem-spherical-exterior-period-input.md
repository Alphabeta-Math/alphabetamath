---
id: lem-spherical-exterior-period-input
title: Periods and primitives on a spherical exterior
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:def-axiom-of-choice
  - math:def-closed-and-exact-differential-forms
  - math:def-de-rham-cohomology
  - math:def-pullback-of-a-differential-form
  - math:thm-the-exterior-derivative-commutes-with-pullback
  - math:thm-de-rham-cohomology-of-spheres
  - math:thm-de-rham-cohomology-is-smooth-homotopy-invariant
  - math:lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary
  - math:cor-a-closed-oriented-manifold-has-no-top-form-with-nonzero-integral-that-is-exact
  - math:def-smooth-manifold
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure
  - math:ex-the-n-sphere-with-its-standard-smooth-atlas
  - math:def-oriented-smooth-manifold-and-oriented-chart
  - math:def-embedded-submanifold-and-slice-chart
  - math:def-smooth-differential-k-form
  - math:def-wedge-product-of-differential-forms
dependency_roles:
  math:def-axiom-of-choice: mathematical-premise
  math:def-closed-and-exact-differential-forms: mathematical-premise
  math:def-de-rham-cohomology: mathematical-premise
  math:def-pullback-of-a-differential-form: mathematical-premise
  math:thm-the-exterior-derivative-commutes-with-pullback: mathematical-premise
  math:thm-de-rham-cohomology-of-spheres: mathematical-premise
  math:thm-de-rham-cohomology-is-smooth-homotopy-invariant: mathematical-premise
  math:lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary: mathematical-premise
  math:cor-a-closed-oriented-manifold-has-no-top-form-with-nonzero-integral-that-is-exact: mathematical-premise
  math:def-smooth-manifold: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure: mathematical-premise
  math:ex-the-n-sphere-with-its-standard-smooth-atlas: mathematical-premise
  math:def-oriented-smooth-manifold-and-oriented-chart: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  math:def-smooth-differential-k-form: mathematical-premise
  math:def-wedge-product-of-differential-forms: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Work in ZFC. Let $E$ be a smooth manifold with a specified diffeomorphism $\Phi:\mathbb R\times(1,\infty)\times S^2\to E$. A smooth real or complex differential form is closed if its exterior derivative vanishes and exact if it is the exterior derivative of a smooth form of one lower degree. Every smooth closed real or complex one-form on $E$ is exact. A smooth closed real or complex two-form on $E$ is exact if and only if its integral over one sphere $\Phi(\{t\}\times\{r\}\times S^2)$ vanishes, where $r>1$ and the sphere carries the orientation transported from the outward orientation of $S^2$. For a complex form the integral is taken componentwise. Applying this criterion to a particular stationary exterior requires a product diffeomorphism as a separate hypothesis; this result does not establish one.

## Statement references

[[math:def-axiom-of-choice]]

[[math:def-closed-and-exact-differential-forms]]

[[math:def-pullback-of-a-differential-form]]

[[math:lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary]]

[[math:def-smooth-manifold]]

[[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]]

[[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure]]

[[math:ex-the-n-sphere-with-its-standard-smooth-atlas]]

[[math:def-oriented-smooth-manifold-and-oriented-chart]]

[[math:def-embedded-submanifold-and-slice-chart]]

[[math:def-smooth-differential-k-form]]

## Facts & Assumptions

[A1] ZFC supplies the countable choice assumed in the sphere cohomology calculation. [[math:def-axiom-of-choice]]

[F1] The degree-$k$ de Rham cohomology is the real vector space of closed smooth $k$-forms modulo exact forms; a closed form has zero class precisely when it is exact. [[math:def-de-rham-cohomology]] [[math:def-closed-and-exact-differential-forms]]

[F2] Under countable choice, $H^1_{\mathrm{dR}}(S^2)=0$ and $H^2_{\mathrm{dR}}(S^2)$ is one-dimensional over $\mathbb R$. [[math:thm-de-rham-cohomology-of-spheres]]

[F3] A smooth homotopy equivalence induces an isomorphism on de Rham cohomology by pullback. Pullback commutes with exterior differentiation. [[math:thm-de-rham-cohomology-is-smooth-homotopy-invariant]] [[math:thm-the-exterior-derivative-commutes-with-pullback]] [[math:def-pullback-of-a-differential-form]]

[F4] On a compact oriented boundaryless manifold, an exact top form has zero integral. Integration of top forms on such a manifold is real-linear, strictly positive on a nonzero nonnegative form, and invariant under orientation-preserving diffeomorphisms. [[math:cor-a-closed-oriented-manifold-has-no-top-form-with-nonzero-integral-that-is-exact]] [[math:lem-finite-chart-localization-for-compactly-supported-forms-on-manifolds-with-boundary]]

[F5] A smooth manifold is equipped with a smooth atlas; a diffeomorphism is a smooth bijection with smooth inverse. Finite products carry the smooth structure given by product charts. [[math:def-smooth-manifold]] [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]] [[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure]]

[F6] The unit sphere $S^2$ has its standard stereographic smooth atlas. An orientation is a smooth choice of a ray in each tangent determinant line; an embedded submanifold is locally a coordinate slice and carries the subspace topology. [[math:ex-the-n-sphere-with-its-standard-smooth-atlas]] [[math:def-oriented-smooth-manifold-and-oriented-chart]] [[math:def-embedded-submanifold-and-slice-chart]]

[F7] A smooth real $k$-form is a smooth section of the $k$th exterior power of the cotangent bundle. The wedge of differential forms is defined pointwise by the wedge of alternating covectors; complex forms are pairs of real forms with componentwise linear operations. [[math:def-smooth-differential-k-form]] [[math:def-wedge-product-of-differential-forms]]

## Proof

**Given:** The specified diffeomorphism, $t\in\mathbb R$, and $r>1$. Let $i:S^2\to E$ be $i(x)=\Phi(t,r,x)$, and let $p:E\to S^2$ be projection to the sphere factor after applying $\Phi^{-1}$.

**Goal:** Prove the stated exactness and period criteria.

1.1 Set $S_{t,r}=i(S^2)$. If $z:U\to V\subset\mathbb R^2$ is a sphere chart and $I,J$ are open intervals about $t,r$ with $J\subset(1,\infty)$, the coordinates $(z(x),u-t,v-r)$ on $\Phi(I\times J\times U)$ are smooth charts of $E$. They identify its intersection with $S_{t,r}$ with $V\times\{0\}\times\{0\}$. Thus $S_{t,r}$ is an embedded smooth surface with the subspace topology. In these charts $i$ is $z\mapsto(z,0,0)$, and its inverse on the image is the restriction of $p$; both are smooth, so $i:S^2\to S_{t,r}$ is a diffeomorphism. Give $S^2$ the outward orientation, in which $(v,w)$ is positive when $\det(x,v,w)>0$, and transport it by $i$ to $S_{t,r}$. This is a smooth orientation since the displayed determinant varies smoothly and never vanishes on a tangent basis. For a two-form $\alpha$ on $E$, its integral over $S_{t,r}$ is the integral of its pullback by the inclusion $S_{t,r}\hookrightarrow E$. The orientation-preserving diffeomorphism $i$ and [F4] identify that integral with $\int_{S^2}i^*\alpha$. [given, F3, F4, F5, F6, construct]

2.1 We have $p\circ i=\operatorname{id}_{S^2}$. A smooth homotopy from $\operatorname{id}_E$ to $i\circ p$ is obtained in product coordinates by $(u,v,x)\mapsto((1-s)u+st,(1-s)v+sr,x)$ for $0\leq s\leq1$; the second coordinate remains greater than $1$. Hence $i$ and $p$ are smooth homotopy inverses. Pullback by $i$ is therefore an isomorphism in every de Rham degree. In degree one, [F2] and [F1] imply that every closed real one-form on $E$ is exact. [given, F1, F2, F3, F5, step 1.1]

2.2 On the outward-oriented unit sphere define $\sigma=x_1\,dx_2\wedge dx_3-x_2\,dx_1\wedge dx_3+x_3\,dx_1\wedge dx_2$, restricted to $S^2$. Its value on a tangent basis $(v,w)$ is $\det(x,v,w)$, so it is a positive smooth top form. It is closed because every three-form on the two-dimensional sphere vanishes. By [F4], $\int_{S^2}\sigma>0$ and an exact two-form has zero integral. Thus $[\sigma]$ is nonzero and, by the one-dimensionality in [F2], generates $H^2_{\mathrm{dR}}(S^2)$. For any closed real two-form $\beta$ on $S^2$, write $[\beta]=c[\sigma]$; then $\beta-c\sigma$ is exact, and linearity and [F4] give $\int\beta=c\int\sigma$. Consequently $\beta$ is exact exactly when its integral vanishes. [F1, F2, F4, F6, F7, step 1.1, algebra]

3.1 Let $\alpha$ be a closed real two-form on $E$. Its pullback $i^*\alpha$ is closed, and the integral over the specified oriented sphere is $\int_{S^2}i^*\alpha$. By step 2.2 this integral vanishes exactly when $i^*[\alpha]=0$; the isomorphism in step 2.1 makes that equivalent to $[\alpha]=0$, hence to exactness of $\alpha$. The argument works for every choice of $t$ and $r>1$, so a vanishing period on any one such sphere suffices. [given, F1, F3, F4, step 1.1, step 2.1, step 2.2]

4.1 For complex forms, write the form as its real part plus $i$ times its imaginary part. Exterior differentiation and integration act componentwise, and a complex form is exact precisely when both real components are exact: combine their real primitives into a complex primitive. Applying the real one-form result and the real two-form criterion to both components proves the stated complex cases. [F1, F7, step 2.1, step 3.1] ∎
