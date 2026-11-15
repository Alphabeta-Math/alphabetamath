---
title: Surface measure, flux densities and null normal gauge
status: published
research_item: def-surface-area-flux-and-null-variation-data
dependency_level: 5
---

## Prerequisites

- [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)
- [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)
- [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus)
- [math:def-riemannian-volume-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-riemannian-volume-form-on-an-oriented-manifold)
- [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry)
- [math:def-riemann-curvature-four-tensor](https://alphabetamath.cc/item/def-riemann-curvature-four-tensor)
- [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain)
- [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge)
- [lem-author-c50357f4fa9e-expansion-second-jet](item-lem-author-c50357f4fa9e-expansion-second-jet)
- [lem-author-c50357f4fa9e-linear-expansion-variation](item-lem-author-c50357f4fa9e-linear-expansion-variation)
- [lem-author-c50357f4fa9e-mots-boost-variation](item-lem-author-c50357f4fa9e-mots-boost-variation)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-integral-of-a-compactly-supported-top-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-top-form-on-an-oriented-manifold)
- [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density)
- [math:def-integrable-real-and-complex-functions-and-their-integrals](https://alphabetamath.cc/item/def-integrable-real-and-complex-functions-and-their-integrals)
- [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration)


## Definition

Work under $\mathrm{AC}_\omega$ for the normal-graph construction and chart-partition integration. Let $(M,g)$ be a smooth oriented, time-oriented Lorentzian four-manifold with signature $(-,+,+,+)$, let $\Sigma$ be a smooth spacelike hypersurface, and let $S\subset\operatorname{int}\Sigma$ be a smooth oriented embedded spacelike two-surface without boundary with a supplied smooth outward unit normal $\nu$ in $h=g|_{T\Sigma}$. The future unit normal of $\Sigma$ is $n$. The induced metric on $S$ is $q$, and $d\mu_q$ denotes its positive oriented area form (its associated positive density is used in unsigned area integrals). Define
$$L=n+\nu,\qquad \underline L=(n-\nu)/2,\qquad g(L,\underline L)=-1.$$
For $U\in TS$ set $\zeta(U)=-g(\underline L,\nabla_U L)$, where $\nabla$ is the spacetime metric connection. For any supplied smooth real two-form $F$ on $M$, its **magnetic and electric flux densities** are the unique smooth functions $b,e$ on $S$ specified by
$$F|_{TS}=b\,d\mu_q,\qquad (\star_gF)|_{TS}=e\,d\mu_q.$$
Let $V_q$ be the Radon Borel measure determined by the positive Riemannian density $|d\mu_q|$. Here integrable means absolutely integrable for $V_q$: $\int_S|f|\,dV_q<\infty$. When $b$ and $e$, respectively, are integrable, define their magnetic and electric fluxes by $\int_Sb\,dV_q$ and $\int_Se\,dV_q$. For compact $S$ this holds automatically, and these fluxes equal the oriented top-form integrals $\int_SF|_{TS}$ and $\int_S(\star_gF)|_{TS}$. For noncompact $S$, the same notation for an absolutely integrable top form is interpreted by the stated density integral. The orientation of $M$ fixes $\star_g$, and the supplied orientation of $S$ fixes the signs of $b,e$.

All surface derivatives use the Levi–Civita connection $D^q$ of $q$: $q(\operatorname{grad}_q f,X)=df(X)$, $\operatorname{div}_q X=\operatorname{tr}(Y\mapsto D^q_YX)$, and $\Delta_q f=\operatorname{div}_q\operatorname{grad}_q f$. On one-forms, divergence means divergence of the $q$-dual vector field. The **Gauss curvature** is $K_q=q(R^q(e_1,e_2)e_2,e_1)$ for a $q$-orthonormal frame, with $R^q(X,Y)Z=D^q_XD^q_YZ-D^q_YD^q_XZ-D^q_{[X,Y]}Z$; this is the positive-round-sphere convention.

Fix an admissible outward normal-graph tube $T(p,r)=\exp^h_p(r\nu_p)$ as in the graph-domain lemma; on compact $S$ such a uniform tube exists. For every admissible $u$, let $F_u(p)=T(p,u(p))$, let $\nu_u$ be the outward graph unit normal and set $L_u=n|_{F_u(S)}+\nu_u$. Let $\Theta(u)=F_u^*(\theta_{L_u})$, where $\theta_{L_u}=\operatorname{tr}_{q_u}g(\nabla L_u,\cdot)$ is the outgoing expansion and $q_u=F_u^*h$. Define the **normal-graph expansion linearization** by
$$\mathcal L\phi=\left.\frac{d}{d\epsilon}\right|_0\Theta(\epsilon\phi).$$
For closed $S$ (compact without boundary) this acts on every smooth function. On a noncompact $S$ a global variation needs an actual common admissible parameter interval; compactly supported directions in a supplied tube suffice, while the local differential expression is defined on all smooth germs. When $\theta_L=0$ identically, $S$ is a MOTS and $\mathcal L$ in this fixed gauge is called its **outward stability operator in $\Sigma$**. It is a linear differential operator of order at most two. Smooth boosts fixing the base $L$ do not change this variation at a MOTS; changing its base positive scale multiplies it by that scale. The explicit curvature and matter coefficient formula is a separate first-variation result, not part of this definition.

## Facts & Assumptions

[F1] [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form) supplies $h,n$ and the spacetime derivative along $\Sigma$. [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry) supplies null expansion and normal-frame scaling.

[F2] [physics:lem-emg-lorentz-hodge-calculus](https://alphabetamath.cc/physics/item/lem-emg-lorentz-hodge-calculus) supplies the smooth Lorentzian Hodge star on the oriented spacetime; [math:def-riemannian-volume-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-riemannian-volume-form-on-an-oriented-manifold) supplies the nowhere-zero oriented area form of $q$.

[F3] [math:thm-fundamental-theorem-of-riemannian-geometry](https://alphabetamath.cc/item/thm-fundamental-theorem-of-riemannian-geometry) supplies the unique intrinsic surface connection; [math:def-riemann-curvature-four-tensor](https://alphabetamath.cc/item/def-riemann-curvature-four-tensor) fixes the curvature four-tensor convention used for $K_q$.

[F4] [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain) establishes the graph domain, including its compactness qualifications; [lem-author-c50357f4fa9e-outward-graph-null-gauge](item-lem-author-c50357f4fa9e-outward-graph-null-gauge) establishes the smooth outward graph normal and null gauge.

[F5] [lem-author-c50357f4fa9e-expansion-second-jet](item-lem-author-c50357f4fa9e-expansion-second-jet) gives the local second-data expression, [lem-author-c50357f4fa9e-linear-expansion-variation](item-lem-author-c50357f4fa9e-linear-expansion-variation) establishes its linear, path-independent derivative, and [lem-author-c50357f4fa9e-mots-boost-variation](item-lem-author-c50357f4fa9e-mots-boost-variation) gives the exact MOTS boost and reparametrization qualifications.

[F6] [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice) records the assumed $\mathrm{AC}_\omega$. Under that assumption, [math:def-integral-of-a-compactly-supported-top-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-integral-of-a-compactly-supported-top-form-on-an-oriented-manifold) defines the integral of a smooth compactly supported top form using chart partitions.

[F7] [math:prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density](https://alphabetamath.cc/item/prop-riemannian-volume-is-the-radon-measure-of-the-riemannian-density) supplies the compact-finite Radon Borel measure $V_q$ of $|d\mu_q|$. [math:def-integrable-real-and-complex-functions-and-their-integrals](https://alphabetamath.cc/item/def-integrable-real-and-complex-functions-and-their-integrals) defines absolute integrability and the signed integral. [math:thm-density-measure-integration-agrees-with-smooth-density-integration](https://alphabetamath.cc/item/thm-density-measure-integration-agrees-with-smooth-density-integration) gives the absolutely convergent chart formula for $L^1(V_q)$ functions and its agreement with smooth compact-support density integration.

## Justification

The orthogonality and normalization in [F1] give the displayed null pairing, as also calculated in [F4]. Covariant derivatives in directions tangent to $S$ are independent of any ambient extensions by [F1], so $\zeta$ is a smooth one-form. By [F2], every smooth two-form on the oriented two-dimensional $S$ is a unique scalar multiple of $d\mu_q$: in a positive chart the scalar is its coefficient divided by $\sqrt{\det q}$. The nonzero denominator proves existence, uniqueness and smoothness of $b,e$; the top-form transformation law makes these ratios agree on overlaps. The positive density $|d\mu_q|$ gives $V_q$ by [F7], and smooth $b,e$ are Borel functions. Absolute integrability in [F7] defines each finite signed flux even on a noncompact $S$. If $S$ is compact, every smooth function on $S$ has compact support, so the smooth compact-support comparison in [F7] proves its integrability. In a positive chart, the coefficient of $f\,d\mu_q$ and that of the signed density $f|d\mu_q|$ are both $f\sqrt{\det q}$. Their partition-weighted chart integrals therefore coincide by [F6] and [F7]. Taking $f=b,e$ proves the two compact oriented-flux equalities; on noncompact $S$, the $L^1$ chart formula in [F7] gives the declared absolutely convergent extension. Countable choice is used in the inherited chart-partition integration constructions of [F6] and [F7]. The intrinsic connection and tensorial contractions in [F3] define the displayed gradient, divergence and Laplacian independently of coordinates. The curvature definition is antisymmetric in its first two slots. Applying metric compatibility to the commutator $D^q_XD^q_Y-D^q_YD^q_X-D^q_{[X,Y]}$ acting on $q(Z,W)$ gives $q(R^q(X,Y)Z,W)+q(Z,R^q(X,Y)W)=0$, proving antisymmetry in the final two slots. Under a change of orthonormal frame, these two antisymmetries make the displayed value multiply by the square of the frame determinant, which is one in dimension two. Thus $K_q$ is well defined even under an orientation-reversing frame change. Finally [F4] gives actual admissible graph domains and a smooth fixed gauge, and [F5] proves well-definedness, linearity, path independence and the stated restrictions on boost invariance of the derivative. No Einstein equation, compactness without explicit mention, geodesic completeness or arbitrary parameter-dependent null normalization is presumed.
