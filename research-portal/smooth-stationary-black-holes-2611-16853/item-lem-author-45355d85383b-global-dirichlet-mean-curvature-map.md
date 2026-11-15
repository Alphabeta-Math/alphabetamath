---
title: The global Dirichlet mean-curvature map is continuously differentiable
status: published
research_item: lem-author-45355d85383b-global-dirichlet-mean-curvature-map
dependency_level: 9
---

## Prerequisites

- [lem-author-45355d85383b-weighted-holder-completeness](item-lem-author-45355d85383b-weighted-holder-completeness)
- [lem-author-45355d85383b-relative-timelike-flow-chart](item-lem-author-45355d85383b-relative-timelike-flow-chart)
- [lem-author-45355d85383b-compact-holder-superposition](item-lem-author-45355d85383b-compact-holder-superposition)
- [lem-author-45355d85383b-weighted-end-superposition](item-lem-author-45355d85383b-weighted-end-superposition)
- [thm-maximal-jacobi-lapse-input](item-thm-maximal-jacobi-lapse-input)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-c-k-map-between-banach-spaces](https://alphabetamath.cc/item/def-c-k-map-between-banach-spaces)
- [math:def-frechet-derivative-between-banach-spaces](https://alphabetamath.cc/item/def-frechet-derivative-between-banach-spaces)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-product-norms-on-finitely-many-normed-spaces](https://alphabetamath.cc/item/def-product-norms-on-finitely-many-normed-spaces)
- [math:thm-finite-products-of-banach-spaces-are-banach](https://alphabetamath.cc/item/thm-finite-products-of-banach-spaces-are-banach)


## Statement

Work in ZFC. Fix $0<\alpha<1$ and $-1<\beta<0$. Let $\Sigma\subset M$ be a supplied smooth embedded three-dimensional exterior with compact smooth boundary $S$, fixed compact-chart data and a fixed spatial end chart $x$. Use the weighted Hölder norms for these fixed data, with derivatives continuous up to the boundary, and put $X_\beta=\{w\in C^{4,\alpha}_\beta(\Sigma):w|_S=0\}$ and $Y_\beta=C^{2,\alpha}_{\beta-2}(\Sigma)$. Equip $\mathbb R\times X_\beta$ with the sum norm $\|(s,v)\|=|s|+\|v\|_{C^{4,\alpha}_\beta}$.

Let $q_*\in I\subset\mathbb R$, where $I$ is open, and let $(M,g_q,N_q,T)$ be stationary Lorentzian data on a common neighborhood of $\Sigma$. The metrics and time orientations are jointly smooth in $q$ and the ambient coordinates, and $T$ is a common stationary field. Assume $\Sigma$ is spacelike and maximal for $g_{q_*}$. All smooth data at $S$ are smooth up to the boundary through local extensions. Supply a common stationary product diffeomorphism $\Psi:\mathbb R_t\times\{x\in\mathbb R^3:r=|x|>R_0\}\to U\subset M$, with $T=\Psi_*\partial_t$ future timelike for every $q$ and $\Sigma\cap U=\{\Psi(u_*(x),x):r>R_0\}$. Its spatial chart agrees with the fixed end chart of $\Sigma$, whose complement is compact, and the metric coefficients are independent of $t$.

In this common chart assume $g_{q,00}=-c(q)^2+e_{q,00}$, $g_{q,ij}=b(q)^2\delta_{ij}+e_{q,ij}$ and $g_{q,0i}=e_{q,0i}$, where $b,c$ are smooth positive functions and $1\le i,j\le3$. On a compact interval $J\subset I$ with $q_*$ in its interior, the errors and their first parameter derivatives satisfy the common differentiated bounds $e_{q,00},e_{q,ij}=O_5(r^{-1})$ and $e_{q,0i}=O_5(r^{-2})$. Require also that $q\mapsto(e_{q,00},e_{q,ij})$ is $C^1$ in the annular $C^{4,\alpha}_{-1}$ norm and $q\mapsto e_{q,0i}$ is $C^1$ in the annular $C^{4,\alpha}_{-2}$ norm. These are explicit uniform end hypotheses. The fixed smooth reference height satisfies $u_*\in C^{5,\alpha}_{-3/4}$ and $\Delta_0u_*\in C^{2,\alpha}_{-3}$ on the end, where $\Delta_0=\sum_{i=1}^3\partial_{x^i}^2$.

Choose the fixed smooth future timelike transverse field $Y$ supplied by the timelike-flow construction: it equals the $g_{q_*}$ future unit normal along a neighborhood of a chosen compact core containing $S$, and equals $T$ on a sufficiently distant product tail. Write $\phi^Y$ for its local flow and $F_w(p)=\phi^Y_{w(p)}(p)$ for its admissible $C^{4,\alpha}$ flow graph. In particular, on that tail $F_w(x)=\Psi(u_*(x)+w(x),x)$. Let $h_*,n_*$ be the induced metric and future unit normal of $\Sigma$ for $g_{q_*}$, and set $k_*(U,V)=-g_{q_*}(\nabla^*_U n_*,V)$, where $\nabla^*$ is the Levi–Civita connection of $g_{q_*}$. Use the mean-curvature convention $H_*=-\operatorname{tr}_{h_*}k_*=0$ and define $V_*=|k_*|_{h_*}^2+\operatorname{Ric}(g_{q_*})(n_*,n_*)$ and $a_*=-g_{q_*}(Y,n_*)$.

After shrinking the parameter interval about $q_*$ and the height ball about zero, the graphs are embedded and spacelike for every parameter and satisfy $F_w|_S=\operatorname{id}_S$. Define $\mathcal H(q,w)=F_w^*(\operatorname{div}_{g_q}n_{q,w})$, where $n_{q,w}$ is the future unit normal of the graph and divergence uses a local unit timelike extension. Then $\mathcal H$ is $C^1$ on this neighborhood of $(q_*,0)$ in $\mathbb R\times X_\beta$ with values in $Y_\beta$, meaning continuous Fréchet differentiability in these norms. Its height derivative is the bounded linear map $D_w\mathcal H(q_*,0)v=(\Delta_{h_*}-V_*)(a_*v)$, with $\Delta_{h_*}=\operatorname{div}_{h_*}\operatorname{grad}_{h_*}$. No boundary condition is imposed on the output. No invertibility or implicit-function conclusion is included.

## Statement references

[lem-author-45355d85383b-weighted-holder-completeness](item-lem-author-45355d85383b-weighted-holder-completeness)

[lem-author-45355d85383b-relative-timelike-flow-chart](item-lem-author-45355d85383b-relative-timelike-flow-chart)

[lem-author-45355d85383b-compact-holder-superposition](item-lem-author-45355d85383b-compact-holder-superposition)

[lem-author-45355d85383b-weighted-end-superposition](item-lem-author-45355d85383b-weighted-end-superposition)

[thm-maximal-jacobi-lapse-input](item-thm-maximal-jacobi-lapse-input)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[math:def-c-k-map-between-banach-spaces](https://alphabetamath.cc/item/def-c-k-map-between-banach-spaces)

[math:def-frechet-derivative-between-banach-spaces](https://alphabetamath.cc/item/def-frechet-derivative-between-banach-spaces)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:def-product-norms-on-finitely-many-normed-spaces](https://alphabetamath.cc/item/def-product-norms-on-finitely-many-normed-spaces)

[math:thm-finite-products-of-banach-spaces-are-banach](https://alphabetamath.cc/item/thm-finite-products-of-banach-spaces-are-banach)

## Facts & Assumptions

[F1] The weighted domain and target, including the closed zero-trace subspace, are real Banach spaces for the fixed exterior and chart data. [lem-author-45355d85383b-weighted-holder-completeness](item-lem-author-45355d85383b-weighted-holder-completeness)

[F2] Under the common product-end bounds and compact parameter smoothness, the timelike-flow construction supplies a fixed transverse field and a parameter-uniform open ball of embedded spacelike zero-trace graphs, fixed pointwise on the boundary. [lem-author-45355d85383b-relative-timelike-flow-chart](item-lem-author-45355d85383b-relative-timelike-flow-chart)

[F3] On a compact truncation, compatible smooth flow charts give a continuously Fréchet differentiable mean-curvature map from the full finite-norm order-four Hölder space to the order-two space, with the explicit local jet derivative and operator-norm continuity. [lem-author-45355d85383b-compact-holder-superposition](item-lem-author-45355d85383b-compact-holder-superposition)

[F4] Under precisely the stationary-family, reference-height and weighted parameter hypotheses stated here, the end mean-curvature map is continuously Fréchet differentiable into weight beta minus two, with a uniform remainder and derivative-continuity modulus over all end annuli; a fixed compact end collar may be included. [lem-author-45355d85383b-weighted-end-superposition](item-lem-author-45355d85383b-weighted-end-superposition)

[F5] The pulled-back mean-curvature variation with velocity $an+X$ is $\Delta_h a-(|k|_h^2+\operatorname{Ric}(n,n))a+X(H)$, with the curvature and second-form conventions used here. In particular the transport term vanishes at a maximal reference slice. [thm-maximal-jacobi-lapse-input](item-thm-maximal-jacobi-lapse-input)

[F6] The stationary data fix the metric, time orientation, connection and Ricci convention; the hypersurface data fix the future normal, induced metric, negative-sign second fundamental form and normal–tangential splitting; the flow-graph definition fixes the pullback and divergence convention. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F7] The exterior definition fixes the compact and annular norms, zero trace and Laplace–Beltrami convention. Differentiated decay and common-parameter bounds are interpreted in the same fixed Cartesian end chart. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F8] A Fréchet derivative is a bounded linear map whose remainder divided by the increment norm tends to zero; class C1 requires continuity of that derivative in operator norm. [math:def-c-k-map-between-banach-spaces](https://alphabetamath.cc/item/def-c-k-map-between-banach-spaces) [math:def-frechet-derivative-between-banach-spaces](https://alphabetamath.cc/item/def-frechet-derivative-between-banach-spaces)

[F9] ZFC includes the Axiom of Choice, retained when invoking the timelike-flow construction and its partition-of-unity input, and the weighted completeness supplier. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F10] The sum norm is a standard finite-product norm, and a finite product of real Banach spaces is Banach in that norm. Apply this to $\mathbb R$ and $X_\beta$. [math:def-product-norms-on-finitely-many-normed-spaces](https://alphabetamath.cc/item/def-product-norms-on-finitely-many-normed-spaces) [math:thm-finite-products-of-banach-spaces-are-banach](https://alphabetamath.cc/item/thm-finite-products-of-banach-spaces-are-banach)

## Proof

**Given:** The fixed exterior, jointly smooth stationary family, uniform end data, maximal reference slice and graph field in the Statement.

**Goal:** Prove the global weighted C1 mapping property and identify its bounded height derivative.

1.1 On a smaller compact parameter interval, positivity of $b,c$ bounds them above and away from zero. The uniform end estimates and $Du_*=O(r^{-7/4})$ imply bounded ambient components and $h_{q,ij}=g_{q,ij}+g_{q,0i}u_{*,j}+g_{q,0j}u_{*,i}+g_{q,00}u_{*,i}u_{*,j}=b(q)^2\delta_{ij}+O(r^{-1})$ uniformly. Thus $h_q\ge m\delta$ on a sufficiently distant common tail for some $m>0$. These are the end hypotheses of [F2], with stationary generator normalization one. On compact subsets, joint smoothness and reference spacelikeness give its remaining family hypotheses after shrinking the interval. Invoke [F2], carrying [F9], to fix $Y$, its flow domain and an open admissible graph ball. On the tail where $Y=T$ the graph is exactly the time translation in the Statement. Hence [F4] applies with all its reference-height and parameter-norm assumptions supplied explicitly; on compact truncations the fixed smooth flow charts and locally extended smooth data meet [F3]. The spaces and their sum-norm product are Banach by [F1] and [F10]. [given, F1, F2, F3, F4, F6, F7, F9, F10, algebra]

2.1 Apply [F3] on a compact truncation containing the nontranslation region and a fixed overlap collar, and [F4] on the translation tail. Their outputs agree on the overlap because both compute the future geometric mean curvature pulled back by the same $F_w$. Their derivatives agree there as well: at each overlap point subtract the two Fréchet remainder identities along a fixed increment direction, divide by its scalar size and let that scalar tend to zero. The compact and end derivatives therefore define one linear operator $L_{q,w}$ on $\mathbb R\times X_\beta$. Restrictions of a height to this fixed truncation are bounded in its finite-chart order-four Hölder norm by its global weighted norm: on the added compact end collar only bounded-radius annuli occur, so their weight factors and all fixed chart-transition coefficients have finite bounds. The same finite-chart comparison for order two shows that the global target norm is bounded by a constant times the sum of the compact target norm and the tail norm. Thus, for $\varepsilon=|s|+\|v\|_{C^{4,\alpha}_\beta}$, the global remainder is bounded by $C(\omega_K(\varepsilon)+\omega_E(\varepsilon))\varepsilon$, where the compact and end moduli tend to zero by [F3] and [F4]. Their derivative bounds also give boundedness of $L_{q,w}$, and the same comparison applied to derivative differences gives operator-norm continuity. By [F8] this proves the asserted global $C^1$ property. Zero trace constrains the height directions only and imposes no output boundary condition. [given, F1, F2, F3, F4, F7, F8, F10, step 1.1, algebra]

3.1 At fixed $q=q_*$, the variation $F_{sv}$ has velocity $vY$. Its normal speed is $-g_{q_*}(vY,n_*)=a_*v$, and its remaining velocity component is tangent. Apply [F5] with the data and conventions in [F6]. Since $H_*=0$ identically, tangential transport contributes zero, leaving $(\Delta_{h_*}-V_*)(a_*v)$. This calculation also applies to every $v\in X_\beta$, without assuming density of smooth functions in its Hölder norm: at any interior point the local jet derivative from [F3] or [F4] depends only on the two-jet of $v$, which can be matched by a smooth local polynomial direction; [F5] identifies that same jet expression for smooth local variations. The identity extends to $S$ by continuity of the derivatives up to the boundary. It is consequently the height restriction of the global Fréchet derivative from step 2.1, so is bounded from $X_\beta$ to $Y_\beta$. Positivity of $a_*$ alone is not used to infer invertibility. [given, F3, F4, F5, F6, F7, F8, step 2.1, algebra] ∎
