---
title: A decaying stationary time gauge gives bounded section displacement
status: draft
research_item: lem-author-d20d145f998f-decaying-time-gauge
dependency_level: 0
---

## Prerequisites

- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:def-ck-euclidean-maps-and-diffeomorphisms](https://alphabetamath.cc/item/def-ck-euclidean-maps-and-diffeomorphisms)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-pullback-riemannian-metric](https://alphabetamath.cc/item/def-pullback-riemannian-metric)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)
- [math:thm-real-power-continuity-and-derivatives](https://alphabetamath.cc/item/thm-real-power-continuity-and-derivatives)
- [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)
- [math:thm-monotonicity-of-the-integral](https://alphabetamath.cc/item/thm-monotonicity-of-the-integral)
- [math:thm-cauchy-criterion-for-improper-integrals](https://alphabetamath.cc/item/thm-cauchy-criterion-for-improper-integrals)
- [math:lem-shin-radial-smooth-cutoff](https://alphabetamath.cc/item/lem-shin-radial-smooth-cutoff)
- [math:thm-extreme-value-r](https://alphabetamath.cc/item/thm-extreme-value-r)
- [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)
- [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)
- [physics:lem-lorentz-form-has-orthonormal-basis](https://alphabetamath.cc/physics/item/lem-lorentz-form-has-orthonormal-basis)
- [math:prop-the-graph-of-a-smooth-map-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-graph-of-a-smooth-map-is-an-embedded-submanifold)
- [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)
- [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)


## Statement

Consider two smooth stationary end charts on the same end of a smooth Lorentzian four-manifold of signature $(-,+,+,+)$, with spatial coordinates $x,x^{\prime}\in\mathbb R^3$ and the same timelike Killing field $T=\partial_t=\partial_{t^{\prime}}$. Write $x^{\prime}=f(x)$ and $t^{\prime}=t+F(x)$, where $f$ is a smooth diffeomorphism between complements of sufficiently large compact sets. Suppose the two coordinate representations $h,h^{\prime}$ of the same stationary quotient metric are uniformly comparable to their Euclidean metrics. Put $r=|x|$ and $r^{\prime}=|x^{\prime}|$. Suppose the stationary one-form has representations $g(T,\cdot)/g(T,T)=dt+\varphi_i dx^i=dt^{\prime}+\varphi^{\prime}_j dx^{\prime}{}^j$, where $|\varphi(x)|\le C r^{-2}$ and $|\varphi^{\prime}(x^{\prime})|\le C(r^{\prime})^{-2}$ sufficiently far out, uniformly in angle. All coefficient and derivative norms here are Euclidean.

Then $|Df|$ and $|Df^{-1}|$ are bounded and $r,r^{\prime}$ are comparable sufficiently far out, while $dF=O(r^{-2})$. After subtracting one additive constant from $F$ (equivalently, changing the origin of $t^{\prime}$), $F=O(r^{-1})$ uniformly in angle. There are smooth cutoffs $u_R$ equal to zero on $r\le R$ and to $F$ on $r\ge2R$, extended by zero over any supplied compact interior, with $\sup|u_R|\le C_1/R$ and $\sup|du_R|\le C_2/R^2$. In particular their transition displacements are bounded and their transition derivatives tend uniformly to zero. No existence of either end chart or of an interior stationary product is asserted.

There is also the following conditional spacelike-graph conclusion. Suppose separately that a smooth stationary product $\mathbb R\times C$ with coordinate $t$ extends this end, that $dt$ is timelike everywhere, and that constants $\kappa,K_0>0$ satisfy $g^{00}\le-\kappa$ and $|g^{\mu\nu}|\le K_0$ on its sufficiently far end in the original coordinates, for $\mu,\nu=0,1,2,3$. Then, for sufficiently large $R$, each level of $t+u_R$ is a smooth spacelike graph over $C$, equal to the corresponding original level in $r\le R$ and to the normalized $t^{\prime}$ level in $r\ge2R$. These extra hypotheses hold, for example, for a supplied stationary product with timelike $dt$ whose inverse metric tends uniformly to the Minkowski inverse on the end.

## Statement references

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:def-ck-euclidean-maps-and-diffeomorphisms](https://alphabetamath.cc/item/def-ck-euclidean-maps-and-diffeomorphisms)

[math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[math:def-pullback-riemannian-metric](https://alphabetamath.cc/item/def-pullback-riemannian-metric)

[math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives)

[math:thm-real-power-continuity-and-derivatives](https://alphabetamath.cc/item/thm-real-power-continuity-and-derivatives)

[math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)

[math:thm-monotonicity-of-the-integral](https://alphabetamath.cc/item/thm-monotonicity-of-the-integral)

[math:thm-cauchy-criterion-for-improper-integrals](https://alphabetamath.cc/item/thm-cauchy-criterion-for-improper-integrals)

[math:lem-shin-radial-smooth-cutoff](https://alphabetamath.cc/item/lem-shin-radial-smooth-cutoff)

[math:thm-extreme-value-r](https://alphabetamath.cc/item/thm-extreme-value-r)

[physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms)

[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets)

[physics:lem-lorentz-form-has-orthonormal-basis](https://alphabetamath.cc/physics/item/lem-lorentz-form-has-orthonormal-basis)

[math:prop-the-graph-of-a-smooth-map-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-graph-of-a-smooth-map-is-an-embedded-submanifold)

[math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure)

[math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

## Facts & Assumptions

[F1] Smooth Lorentzian metrics, timelike Killing fields and stationary flow parameters have their mathematical meanings. The quotient metric is represented by the horizontal tensor $h=g-g(T,\cdot)\otimes g(T,\cdot)/g(T,T)$, which annihilates $T$; its coordinate metrics use the Riemannian-metric definition and the pullback formula $(f^*h^{\prime})_x(v,w)=h^{\prime}_{f(x)}(Df_xv,Df_xw)$. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field) [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-pullback-riemannian-metric](https://alphabetamath.cc/item/def-pullback-riemannian-metric)

[F2] Both $f$ and $f^{-1}$ are smooth Euclidean maps. The total chain rule, the sum/product/quotient rules along coordinate lines, and $(s^\alpha)^{\prime}=\alpha s^{\alpha-1}$ for $s>0$ apply. Repeated differentiation of this last formula makes positive powers smooth, including the norm away from the origin. [math:def-ck-euclidean-maps-and-diffeomorphisms](https://alphabetamath.cc/item/def-ck-euclidean-maps-and-diffeomorphisms) [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) [math:thm-algebra-of-derivatives](https://alphabetamath.cc/item/thm-algebra-of-derivatives) [math:thm-real-power-continuity-and-derivatives](https://alphabetamath.cc/item/thm-real-power-continuity-and-derivatives)

[F3] For continuously differentiable real functions on an open interval, integration of the derivative gives the endpoint difference. Proper integration preserves pointwise inequalities. A locally Riemann-integrable function has a convergent improper integral at infinity when its proper tail integrals satisfy the Cauchy criterion. These inputs will be used only for smooth functions and finite piecewise smooth paths. [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts) [math:thm-monotonicity-of-the-integral](https://alphabetamath.cc/item/thm-monotonicity-of-the-integral) [math:thm-cauchy-criterion-for-improper-integrals](https://alphabetamath.cc/item/thm-cauchy-criterion-for-improper-integrals)

[F4] There is a smooth $b:\mathbb R\to[0,1]$ with $b=1$ on $|s|\le1$ and $b=0$ on $|s|\ge2$. The continuous function $|b^{\prime}|$ is bounded on the compact interval $[1,2]$ by the real extreme value theorem. [math:lem-shin-radial-smooth-cutoff](https://alphabetamath.cc/item/lem-shin-radial-smooth-cutoff) [math:thm-extreme-value-r](https://alphabetamath.cc/item/thm-extreme-value-r)

[F5] The inverse metric and the map $\alpha\mapsto\alpha^\sharp$ are defined by $g(\alpha^\sharp,v)=\alpha(v)$ and $g^{-1}(\alpha,\alpha)=g(\alpha^\sharp,\alpha^\sharp)$. A spacelike embedded hypersurface has positive-definite induced metric. A Lorentz form has a basis with matrix $\operatorname{diag}(-1,1,1,1)$; positivity on the orthogonal complement of a timelike vector is proved in step 1.1 rather than imported as an additional assertion. [physics:def-gr-inverse-metric-and-musical-isomorphisms](https://alphabetamath.cc/physics/item/def-gr-inverse-metric-and-musical-isomorphisms) [physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets](https://alphabetamath.cc/physics/item/def-gr-spacelike-hypersurfaces-and-cauchy-sets) [physics:lem-lorentz-form-has-orthonormal-basis](https://alphabetamath.cc/physics/item/lem-lorentz-form-has-orthonormal-basis)

[F6] For a smooth map $H:C\to\mathbb R$, its graph $\Gamma_H=\{(p,H(p)):p\in C\}$ is an embedded submanifold of $C\times\mathbb R$ of dimension $\dim C$. Products carry the canonical smooth structure defined by product charts. Embeddedness means that ambient smooth slice charts identify the subset with a coordinate plane. [math:prop-the-graph-of-a-smooth-map-is-an-embedded-submanifold](https://alphabetamath.cc/item/prop-the-graph-of-a-smooth-map-is-an-embedded-submanifold) [math:prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure](https://alphabetamath.cc/item/prop-products-of-smooth-manifolds-have-a-canonical-product-smooth-structure) [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)

## Proof

**Given:** The end-chart hypotheses in the Statement; for steps 7.1 and 8.1 only, also its additional stationary-product and uniform inverse-metric hypotheses.

**Goal:** Prove the unconditional decay and cutoff estimates and the separately conditional spacelike-graph conclusion.

1.1 First check the needed pointwise linear algebra in an orthonormal Lorentz basis. If $n=(n_0,a)$ is timelike, then $n_0^2>|a|^2$; a vector $v=(v_0,z)$ perpendicular to $n$ has $v_0=(a\cdot z)/n_0$. The elementary identity $|a|^2|z|^2-(a\cdot z)^2=\sum_{i<j}(a_i z_j-a_j z_i)^2\ge0$ gives $g(v,v)\ge(1-|a|^2/n_0^2)|z|^2>0$ for nonzero $v$. For a spatial vector $v$ in either stationary chart, its horizontal lift is $\widehat v=v-g(T,v)T/g(T,T)$, perpendicular to $T$, and $h(v,v)=g(\widehat v,\widehat v)$. The lift is nonzero for nonzero spatial $v$ because $T=\partial_t$. Thus the quotient coordinate metrics are Riemannian. The tensor annihilates $T$, so a change of time section does not change its spatial pullback. [F1, F5, algebra]

2.1 By the pullback formula, $h_x(v,v)=h^{\prime}_{f(x)}(Df_xv,Df_xv)$. Choose common constants $0<\lambda\le\Lambda$ for the two uniform Euclidean comparisons. Then $\lambda|Df_xv|^2\le\Lambda|v|^2$. Applying the same identity to $f^{-1}$ gives the inverse bound. Consequently both derivatives have a uniform bound $L$. [F1, F2, step 1.1]

3.1 Here is an explicit angular path estimate. For unit vectors $a,b$ with $a\cdot b\ge0$, the path $q(s)=((1-s)a+sb)/|(1-s)a+sb|$, $0\le s\le1$, lies on the unit sphere. Its denominator is at least $1/\sqrt2$, and differentiating gives $|q^{\prime}|\le2$. For arbitrary unit $a,b$, take $w=(a+b)/|a+b|$ when $a+b\ne0$; then $a\cdot w,b\cdot w\ge0$. If $b=-a$, take a unit $w$ perpendicular to $a$, obtained by projecting and normalizing a coordinate vector not parallel to $a$. The two normalized segments through $w$ therefore join $a$ to $b$ with total speed integral at most $4$. After scaling they give a path on the radius-$s$ sphere with speed integral at most $4s$. Fix an anchor on a sufficiently large sphere in the $x$ chart, join it angularly to the direction of $x$, and continue radially to $x$. The chain rule, componentwise fundamental theorem and integral inequalities give $|f(x)|\le A+Br$. Apply the identical construction to $f^{-1}$ in the other end chart to obtain $|x|\le A^{\prime}+B^{\prime} r^{\prime}$. On the common far end both radii tend to infinity, since these are charts of the same end; increasing the compact cut removes the additive constants and proves comparability. [F2, F3, step 2.1]

4.1 Equating the two representations of the stationary one-form and using $dt^{\prime}=dt+dF$ gives $dF=\varphi-f^*\varphi^{\prime}$. In components, $(f^*\varphi^{\prime})_i=\varphi^{\prime}_j(f(x))\partial_i f^j$. The derivative bound and radius comparability imply $|dF|\le C r^{-2}$, after increasing a uniform constant. [F1, F2, step 2.1, step 3.1]

5.1 For a fixed unit $\omega$, set $q_\omega(s)=F(s\omega)$. The chain rule gives $|q_\omega^{\prime}(s)|\le C s^{-2}$. The fundamental theorem and order bounds give $|q_\omega(v)-q_\omega(u)|\le C(1/u-1/v)$ for $v>u$ sufficiently large; the integral of $s^{-2}$ is computed from the derivative of $-s^{-1}$. Thus the proper tail integrals of $q_\omega^{\prime}$ satisfy the improper-integral Cauchy criterion. Their convergence and the fundamental theorem give a limit $L(\omega)$ with $|F(r\omega)-L(\omega)|\le C/r$. On the radius-$r$ angular path constructed in step 3.1, integrating $dF$ gives $|F(r\omega_1)-F(r\omega_2)|\le4C/r$. Taking $r$ to infinity shows $L(\omega_1)=L(\omega_2)$ for every pair. Subtract this common constant; the bound $|F(r\omega)|\le C/r$ is uniform in angle. [F2, F3, step 3.1, step 4.1]

6.1 Use the one-dimensional function $b$ of [F4] to set $\chi_R(x)=1-b(r/R)$ and $u_R=\chi_R F$ on the end, extending $u_R$ by zero inside. Choose $R$ so the end formula is defined on a neighborhood of $r\ge R$; the plateau of $b$ makes this extension smooth. The power and chain rules give $|dr|=1$, so $|d\chi_R|\le B_0/R$, with $B_0$ a bound for $|b^{\prime}|$ on $[1,2]$. On $R\le r\le2R$, the product rule gives $|u_R|\le C/R$ and $|du_R|\le|dF|+|F||d\chi_R|\le C(1+B_0)/R^2$. Outside this annulus $u_R$ is either zero or $F$, and the bounds of steps 4.1 and 5.1 give the same global estimates. Every fixed compact interior is unchanged once $R$ is large. [F2, F4, step 4.1, step 5.1]

7.1 Now assume the additional stationary-product and inverse-metric hypotheses of the conditional conclusion. Put $\alpha_s=dt+s\,du_R$ for $0\le s\le1$. On $r\ge R$ write $\varepsilon_R=C_2/R^2$, so $|\partial_i u_R|\le\varepsilon_R$. Expanding in the original coordinates yields $g^{-1}(\alpha_s,\alpha_s)=g^{00}+2s g^{0i}\partial_i u_R+s^2g^{ij}\partial_i u_R\partial_j u_R\le-\kappa+6K_0\varepsilon_R+9K_0\varepsilon_R^2$. For sufficiently large $R$ this is at most $-\kappa/2$, uniformly in $s$ and on the end. On $r\le R$ it equals $g^{-1}(dt,dt)<0$. Hence the entire deformation stays timelike, and its time-cone choice is the one of $dt$. Uniform convergence to the Minkowski inverse supplies the displayed end hypotheses, for example with $g^{00}\le-1/2$ and bounded inverse components beyond a fixed radius. [F5, step 6.1, given, algebra]

8.1 For a level value $c$, set $H(p)=c-u_R(p)$, smooth by step 6.1. By [F6], $\Gamma_H\subset C\times\mathbb R$ is an embedded three-dimensional submanifold. The factor swap $S:C\times\mathbb R\to\mathbb R\times C$, $S(p,t)=(t,p)$, is a diffeomorphism: in the product charts of [F6] it and its inverse are coordinate permutations. If $\psi$ is a slice chart for $\Gamma_H$ on an open set $V$, then $\psi\circ S^{-1}$ on $S(V)$ is a smooth slice chart for $S(\Gamma_H)$, since it has the same coordinate image and sends $S(\Gamma_H)\cap S(V)$ to the same coordinate plane. Thus the level set $S(\Gamma_H)=\{(c-u_R(p),p):p\in C\}$ is embedded in the required order of product factors. Its parametrization is smooth and injective, with smooth inverse the spatial projection; its differential is $v\mapsto(-du_R(v),v)$ and has rank three, so its tangent space is exactly $\ker(dt+du_R)$. The vector $n=(dt+du_R)^\sharp$ is timelike by step 7.1, and this kernel is $n^\perp$ by the musical definition; step 1.1 proves positivity of its induced metric. This is exactly the spacelike-hypersurface definition. The graph agrees with the original level where $u_R=0$ and with the normalized $t^{\prime}$ level where $u_R=F$. The unconditional decay and cutoff conclusions were established before imposing these additional graph hypotheses. [F1, F2, F5, F6, step 1.1, step 6.1, step 7.1] ∎
