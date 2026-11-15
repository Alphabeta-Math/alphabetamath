---
title: Coordinate and weak forms of the geometric Schrödinger equation
status: published
research_item: lem-author-58255dfd955f-coordinate-schrodinger-form
dependency_level: 1
---

## Prerequisites

- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [math:def-riemannian-gradient](https://alphabetamath.cc/item/def-riemannian-gradient)
- [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)
- [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)
- [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)
- [math:cor-repeated-riemann-integrals-on-rectangles](https://alphabetamath.cc/item/cor-repeated-riemann-integrals-on-rectangles)
- [math:lem-schwartz-cutoffs-from-the-standard-smooth-step](https://alphabetamath.cc/item/lem-schwartz-cutoffs-from-the-standard-smooth-step)


## Statement

Let $(\Sigma,h)$ be the smooth exterior, with real smooth $V$ and real $u\in C^2_{\mathrm{loc}}(\Sigma^\circ)$, where $\Sigma^\circ=\Sigma\setminus\partial\Sigma$. In any relatively compact coordinate chart $U$, including a boundary chart, put $U^\circ=U\cap\Sigma^\circ$, $m=\sqrt{\det(h_{ij})}$, $A^{ij}=mh^{ij}$ and $q=mV$. On $U^\circ$, the classical equation $(\Delta_h-V)u=0$ is equivalent to $-\partial_i(A^{ij}\partial_j u)+qu=0$. For such a $C^2$ function these equations are also equivalent to the weak identity $\int_{U^\circ}(A^{ij}\partial_j u\partial_i\varphi+qu\varphi)\,dx=0$ for every real $\varphi\in C_c^\infty(U^\circ)$, so every test has support compactly contained in the interior, away from the manifold boundary. Here $dx$ and the test functions are understood in chart coordinates. The matrix $A$ is symmetric uniformly positive definite on compact chart subsets, including those meeting $\partial\Sigma$. In nondivergence form the operator is $h^{ij}\partial_{ij}+b^j\partial_j-V$, where $b^j=m^{-1}\partial_i(mh^{ij})$. If $u$ is $C^2$ up to a portion of $U\cap\partial\Sigma$, the pointwise operator formulas and classical equation extend there by continuity.

## Facts & Assumptions

**Given:** The exterior, its smooth metric, boundary-chart conventions and sign convention are those of [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data). Use the regularity and notation in the Statement; repeated indices are summed. At finite regularity, the gradient is the metric dual of the differential, divergence is the trace of the Levi-Civita covariant derivative of a $C^1$ vector field, and the Laplacian is the metric trace of the Hessian of a $C^2$ function. Step 1.1 justifies the smooth supplier formulas at this regularity. A weak solution here means the displayed identity for interior-supported tests, with $u$ and its first derivatives locally square integrable on $U^\circ$; every $C^2$ function has that local integrability.

[F1] For smooth functions the gradient has components $h^{ij}\partial_j u$ by [math:def-riemannian-gradient](https://alphabetamath.cc/item/def-riemannian-gradient). For smooth vector fields the divergence has density formula $m^{-1}\partial_i(mX^i)$ by [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence). For smooth functions the metric trace of the Hessian equals divergence of gradient by [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian). These are smooth-input supplier statements; the needed extension is proved locally below.

[F2] For a real $C^1$ function $g$ on an open interval containing $[a,b]$, $\int_a^b g'(t)\,dt=g(b)-g(a)$, including oriented endpoints, by [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts).

[F3] A continuous real function on a nondegenerate closed rectangle in $\mathbb R^n$, $n\ge1$, has repeated Riemann integrals in every coordinate order, all equal to its multiple integral, by [math:cor-repeated-riemann-integrals-on-rectangles](https://alphabetamath.cc/item/cor-repeated-riemann-integrals-on-rectangles). We use this continuous-input result on enclosing rectangles for the compactly supported coordinate integrands below; no measurable-section or exceptional-section assertion is needed.

[F4] For $n\ge1$, [math:lem-schwartz-cutoffs-from-the-standard-smooth-step](https://alphabetamath.cc/item/lem-schwartz-cutoffs-from-the-standard-smooth-step) supplies $\chi\in C_c^\infty(\mathbb R^n)$ with $0\le\chi\le1$, $\chi=1$ on $|x|\le1$ and $\chi=0$ on $|x|\ge2$, together with smooth rescalings $\chi_R(x)=\chi(x/R)$ for $R>0$. We use $n=3$ and translate a rescaling inside the interior chart image.

## Proof

**Given:** The hypotheses and data in the Statement and Facts & Assumptions.

**Goal:** Establish the coordinate, ellipticity and interior weak-form conclusions of the Statement.

**Proof technique:** direct.

1.1 Fix an interior point $p$ with coordinates $x_0$. The smooth polynomial $P(x)=u(p)+\partial_i u(p)(x^i-x_0^i)+\tfrac12\partial_{ij}u(p)(x^i-x_0^i)(x^j-x_0^j)$ has the same derivatives through order two as $u$ at $p$. Metric duality gives $(\operatorname{grad}_h u)^i=h^{ij}\partial_j u$ directly, and differentiation gives $\partial_k(\operatorname{grad}_h u)^i=(\partial_kh^{ij})\partial_j u+h^{ij}\partial_{kj}u$. Thus $\operatorname{grad}_h u$ and $\operatorname{grad}_h P$ have equal values and first derivatives at $p$, so their covariant derivatives and traces agree there. More generally, the trace of $\nabla X$ for $C^1$ $X$ depends only on $X(p)$ and its first coordinate derivatives: replacing its coefficients by affine polynomials with those same data reduces the divergence density formula to its smooth case in [F1]. Applying [F1] to $P$ therefore proves $\Delta_hu(p)=m^{-1}\partial_i(mh^{ij}\partial_j u)(p)$, since the right side also uses only these derivatives through order two. This proves the required $C^2$ and $C^1$ extensions without assuming extra regularity. [F1, given, algebra]

2.1 Multiply the formula in step 1.1 by $m>0$ and change the sign to obtain the divergence equation. Expanding its derivative gives $\Delta_hu=h^{ij}\partial_{ij}u+m^{-1}\partial_i(mh^{ij})\partial_j u$, proving the nondivergence expression. If $u$ is $C^2$ up to the chart boundary, continuity of all these expressions extends the identities and any classical equation to that boundary. The inverse metric is symmetric positive definite and $m>0$. On any nonempty compact chart subset $K$, the continuous positive function $A^{ij}(x)\xi_i\xi_j$ on $K\times\{\xi\in\mathbb R^3:|\xi|=1\}$ has positive minimum and finite maximum. These are the asserted uniform ellipticity bounds, also when $K$ meets the boundary. [step 1.1, given, algebra]

3.1 Let $\varphi\in C_c^\infty(U^\circ)$ be real. For each $i$, put $G^i=A^{ij}\partial_j u\,\varphi$ on the interior chart image $\Omega$. This is $C^1$ and its support is compactly contained in $\Omega$. Its zero extension $\widehat G^i$ is $C^1$ on $\mathbb R^3$: near every point outside that compact support it is identically zero. Choose a nondegenerate closed rectangle $Q=\prod_{k=1}^3[a_k,b_k]$ with this support in its interior. The derivative $\partial_i\widehat G^i$ is continuous on $Q$, so [F3] computes its multiple integral by integrating first in $x^i$. For every fixed choice of the other coordinates, $t\mapsto\widehat G^i(x^1,\ldots,t,\ldots,x^3)$ is $C^1$ on $\mathbb R$ and vanishes at $a_i,b_i$. Thus [F2] makes its derivative's integral on $[a_i,b_i]$ zero, and [F3] gives $\int_Q\partial_i\widehat G^i\,dx=0$. All coordinate integrands are continuous with compact support, so their integrals are computed on such enclosing rectangles. Summing in $i$, applying the product rule and rearranging yields $\int_{U^\circ}(-\partial_i(A^{ij}\partial_j u)+qu)\varphi\,dx=\int_{U^\circ}(A^{ij}\partial_j u\partial_i\varphi+qu\varphi)\,dx$. If the classical equation holds, step 2.1 makes the left side zero, proving the weak identity. This integration-by-parts identity itself used only the regularity of $u$ and $\varphi$, and the support restriction excludes a manifold-boundary contribution even when $U$ is a boundary chart. [F2, F3, step 2.1, given, algebra]

4.1 Conversely, for the assumed $C^2$ function the residual $f=-\partial_i(A^{ij}\partial_j u)+qu$ is continuous on $U^\circ$. The same integration by parts turns the weak identity into $\int f\varphi\,dx=0$ for every such test. If $f(p)\ne0$, continuity gives $\delta>0$ such that the closed coordinate ball $\overline B_\delta(x_0)$ about the coordinates $x_0$ of $p$ is contained in the interior chart image and $f$ has the sign of $f(p)$ with $|f|\ge |f(p)|/2$ throughout this ball. Use [F4] with $n=3$ and set $\varphi(x)=\chi(2(x-x_0)/\delta)$. Translation of the smooth rescaling with $R=\delta/2$ is smooth; moreover $0\le\varphi\le1$, $\varphi=1$ on $\overline B_{\delta/2}(x_0)$ and $\operatorname{supp}\varphi\subseteq\overline B_\delta(x_0)$. Thus $\varphi\in C_c^\infty(U^\circ)$ is an admissible test, and $f\varphi$ has one sign everywhere and absolute value at least $|f(p)|/2$ on the smaller ball. Its integral is nonzero, contradicting the weak identity. This proves $f=0$, and step 2.1 recovers the classical geometric equation. Thus the weak and classical equations are equivalent at the stated regularity. [F4, step 2.1, step 3.1, given, algebra] ∎
