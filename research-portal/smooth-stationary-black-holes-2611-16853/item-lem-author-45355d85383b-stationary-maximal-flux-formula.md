---
title: Stationary maximal graphs have an explicit uniformly spacelike flux
status: draft
research_item: lem-author-45355d85383b-stationary-maximal-flux-formula
dependency_level: 2
---

## Prerequisites

- [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)
- [lem-author-db87cb8e0bab-stationary-flux-ellipticity](item-lem-author-db87cb8e0bab-stationary-flux-ellipticity)
- [lem-author-45355d85383b-scaled-decay-holder-upgrade](item-lem-author-45355d85383b-scaled-decay-holder-upgrade)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)
- [physics:lem-gr-metric-divergence-and-density-formula](https://alphabetamath.cc/physics/item/lem-gr-metric-divergence-and-density-formula)
- [math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules)


## Statement

Let $g$ be a smooth time-oriented Lorentzian metric of signature $(-,+,+,+)$ in a stationary chart $(t,x)$, so its coefficients are independent of $t$. For a smooth graph $t=u(x)$, put $Q(x,p)=-g^{00}+2g^{0i}p_i-g^{ij}p_ip_j$, with spatial indices summed from $1$ to $3$, and assume $Q(x,Du)>0$. Then $n_0=-g^{-1}d(t-u)/\sqrt{Q(x,Du)}$ is a unit timelike normal. For any future timelike vector field $T$ along the graph, $n_0$ is future-directed exactly when $d(t-u)(T)>0$. Under this sign condition, the future mean curvature is $H=J^{-1}\partial_{x^i}P^i(x,Du)$, where $J=\sqrt{-\det g}$ and
$$P^i(x,p)=\frac{J(g^{ij}p_j-g^{i0})}{\sqrt{Q(x,p)}}.$$
The derivative in this formula is the total derivative of the composed flux. With the opposite time orientation the future normal and $H$ both change sign, so maximality is still equivalent to $\partial_{x^i}P^i(x,Du)=0$. In particular the displayed $n_0$ is future-directed whenever $\partial_t$ is future timelike.

Fix $0<\alpha<1$. Suppose the chart is a Cartesian end with $r=|x|$ and $g_{00}+1,g_{ij}-\delta_{ij}=O_5(r^{-1})$, $g_{0i}=O_5(r^{-2})$. On the fixed annulus $A=\{y\in\mathbb R^3:1<|y|<2\}$, let $G_R(y)=g(Ry)$ denote the array of metric coefficients evaluated at $Ry$, set $J_R(y)=J(Ry)$, and define $Q_R,P_R$ by the same coefficient formulas using $G_R$. There are $R_*$ and $p_0>0$ such that, for $R\ge R_*$ and $|p|\le p_0$, $Q_R\ge\kappa>0$, $(G_R^{ij})\ge\kappa I$, and $G_R,G_R^{-1},J_R,J_R^{-1}$ have common bounds. The matrices $\partial_pP_R$ are symmetric and satisfy $\lambda I\le\partial_pP_R\le\Lambda I$, and $P_R$ has a common joint $C^{4,\alpha}$ bound on $A\times\{|p|\le p_0\}$. For every fixed finite number of additional slope derivatives, those derivatives of $P_R$ have common joint $C^{4,\alpha}$ bounds as well. With derivatives in $y$ taken at fixed $p$, the zero-slope divergence $s_R(y,0)=\sum_i\partial_{y_i}P_R^i(y,0)$ obeys
$$\|s_R(\cdot,0)\|_{C^{3,\alpha}(A)}\le C R^{-2}.$$
All constants are independent of $R$; the last coefficient constants may depend on the number of slope derivatives. These are explicit flux bounds. For $w(y)=u(Ry)/R$, $D_yw=Du(Ry)$ and the maximal equation rescales to $\operatorname{div}_yP_R(y,D_yw)=0$. Using these flux bounds in a subsequent solution regularity estimate additionally requires a smooth solution with $|Dw|\le p_0$ and any uniform height bound required by that estimate, such as $\|w\|_\infty\le M_0$; metric decay alone supplies no solution or height bound.

## Statement references

[def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[lem-author-db87cb8e0bab-stationary-flux-ellipticity](item-lem-author-db87cb8e0bab-stationary-flux-ellipticity)

[lem-author-45355d85383b-scaled-decay-holder-upgrade](item-lem-author-45355d85383b-scaled-decay-holder-upgrade)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[physics:lem-gr-metric-divergence-and-density-formula](https://alphabetamath.cc/physics/item/lem-gr-metric-divergence-and-density-formula)

[math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)

[math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules)

## Facts & Assumptions

[F1] Mean curvature is the pullback of the divergence of the future unit normal, with the stated Lorentzian and graph conventions. [def-normal-graph-and-mean-curvature-data](item-def-normal-graph-and-mean-curvature-data)

[F2] For the explicit stationary flux, uniform positive bounds on $Q_R$ and $(G_R^{ij})$, together with bounded metric, inverse and density, give symmetric uniform ellipticity. A common background $C^{4,\alpha}$ bound gives a common joint $C^{4,\alpha}$ flux bound. Its separate zero-slope conclusion is only $C^{2,\alpha}$; the stronger estimate here is proved below from the additional differentiated decay. [lem-author-db87cb8e0bab-stationary-flux-ellipticity](item-lem-author-db87cb8e0bab-stationary-flux-ellipticity)

[F3] A differentiated bound $f=O_{m+1}(r^{-b})$ gives uniform $C^{m,\alpha}$ bounds for $R^bf(R\,\cdot)$ on a fixed annulus, also for finite component arrays. [lem-author-45355d85383b-scaled-decay-holder-upgrade](item-lem-author-45355d85383b-scaled-decay-holder-upgrade)

[F4] The notation $O_5(r^{-b})$ uses Cartesian derivatives through order five and a common eventual exterior radius. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F5] Use ordinary componentwise Euclidean Hölder norms; joint flux norms differentiate in both $y$ and $p$, with $R$ a parameter. [math:def-holder-spaces-c-k-alpha-and-their-scaled-norms](https://alphabetamath.cc/item/def-holder-spaces-c-k-alpha-and-their-scaled-norms)

[F6] In these Lorentzian coordinates the metric density is $J=\sqrt{-\det g}$ and $\operatorname{div}_gV=J^{-1}\partial_\mu(JV^\mu)$ for smooth vector fields. This supplier has domain mathematics. [physics:lem-gr-metric-divergence-and-density-formula](https://alphabetamath.cc/physics/item/lem-gr-metric-divergence-and-density-formula)

[F7] Matrix inversion preserves finite differentiability on the invertible locus; its proof uses the cofactor-over-determinant formula. Quantitative bounds below are obtained locally by differentiating the inverse identity. [math:lem-matrix-inversion-preserves-ck-regularity](https://alphabetamath.cc/item/lem-matrix-inversion-preserves-ck-regularity)

[F8] The total derivative of a composite is the composite of its derivatives. Scalar sums, products and quotients with nonzero denominator have their usual derivative rules, iterated on coordinate lines. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives) [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules)

## Proof

**Given:** The hypotheses in the Statement, using the decay assumptions only for the end estimates.

**Goal:** Prove the oriented normal formula, the maximal flux equation and all stated uniform rescaled flux bounds.

1.1 The covector $a=d(t-u)$ annihilates the graph tangents $\partial_{x^i}+u_i\partial_t$ and satisfies $g^{-1}(a,a)=-Q(x,Du)<0$. Thus its kernel is spacelike and $n_0=-g^{-1}a/\sqrt Q$ is a unit timelike normal. The equality $g(n_0,T)=-a(T)/\sqrt Q$ gives precisely the claimed future sign condition. If $T=\partial_t$ is future timelike, then $a(T)=1$. Reversing the normal reverses its divergence and hence the signed mean curvature. [given, F1, algebra]

1.2 The decay hypotheses put $g$ uniformly close to $\eta=\operatorname{diag}(-1,1,1,1)$ sufficiently far out, with determinant bounded away from zero and $g_{00}$ bounded away from zero. The cofactor formula bounds $g^{-1}$ there. Differentiating $g^{-1}g=I$ gives $\partial_k g^{-1}=-g^{-1}(\partial_k g)g^{-1}$; iteration with the product rule through order five gives $g^{-1}-\eta=O_5(r^{-1})$. The mixed entry satisfies the exact identity $g^{i0}=-g^{ij}g_{j0}/g_{00}$, obtained from $g^{i\mu}g_{\mu0}=0$. Each differentiated product therefore has at least one mixed covariant factor of order $r^{-2}$, and the other factors and their derivatives have the inverse bounds just established. Consequently $g^{i0}=O_5(r^{-2})$. The determinant is a finite sum of products of metric entries; the identities $\sqrt{v+h}-\sqrt v=h/(\sqrt{v+h}+\sqrt v)$ and $(\sqrt v)'=1/(2\sqrt v)$ for $v>0$, followed by repeated product and quotient differentiation, similarly show $J-1=O_5(r^{-1})$ and $h-1=O_5(r^{-1})$ for $h=J/\sqrt{-g^{00}}$. All denominators are bounded away from zero on this end. [given, F4, F7, F8, algebra]

2.1 Extend $u$ independently of $t$ and use the same formula for $n_0$ where $Q>0$. This is a smooth unit extension, independent of $t$, with $n_0^i=(g^{ij}u_j-g^{i0})/\sqrt Q$. Stationarity and the density formula give $\operatorname{div}_g n_0=J^{-1}\partial_{x^i}(Jn_0^i)=J^{-1}\partial_{x^i}P^i(x,Du)$. Under the future sign condition this is $H$ by F1; otherwise it is $-H$. Both cases give the same zero-mean-curvature equation. [F1, F6, step 1.1, algebra]

2.2 Apply F3 with $m=4$ to the metric errors and to the inverse, $J$ and $h$ estimates of step 1.2. It gives common $C^{4,\alpha}(A)$ bounds on $G_R$, its inverse and $h_R(y)=h(Ry)$, with $\|d_R\|_{C^{4,\alpha}(A)}\le C R^{-2}$ for $d_R^i(y)=g^{i0}(Ry)$. The same applications for $0\le m<4$ control the lower-derivative Hölder seminorms as needed in products. For example choose $p_0=1/4$. Uniform closeness to $\eta$ implies a common positive lower bound for $Q_R$ and $(G_R^{ij})$ on this slope ball, and common bounds for $G_R,G_R^{-1},J_R,J_R^{-1}$. F2 then gives the claimed ellipticity and joint $C^{4,\alpha}$ bound for $P_R$. To retain any fixed number of extra slope derivatives, differentiate the displayed flux formula in $p$: every term is a finite product of inverse entries, density, slope monomials and negative half-integer powers of $Q_R$. Its derivatives through four further orders in $(y,p)$ involve background derivatives only through order four. The common positive denominator bounds control all smooth scalar factors and their derivatives. For their Hölder estimates use $[fg]_\alpha\le\|f\|_\infty[g]_\alpha+\|g\|_\infty[f]_\alpha$ and, the identities $a^{-1}-b^{-1}=(b-a)/(ab)$ and $\sqrt a-\sqrt b=(a-b)/(\sqrt a+\sqrt b)$, iterated over finite products, bound increments of all the scalar powers when their arguments stay in a fixed positive bounded interval. Combining these identities with the componentwise bounds proves the asserted extra-slope-derivative bounds, with constants allowed to depend on their finite number. [given, F2, F3, F5, F8, step 1.2, algebra]

3.1 At zero slope $P_R^i(y,0)=-h_R(y)d_R^i(y)$. The product rule and Hölder product inequality of step 2.2 give $\|P_R(\cdot,0)\|_{C^{4,\alpha}(A)}\le C\|h_R\|_{C^{4,\alpha}(A)}\|d_R\|_{C^{4,\alpha}(A)}\le C R^{-2}$, using the lower-derivative bounds noted there. One $y$ derivative therefore yields the asserted $C^{3,\alpha}$ zero-slope estimate, rather than only the weaker zero-slope conclusion of F2. Finally $D_yw=Du(Ry)$ and $\operatorname{div}_yP_R(y,Dw)=R(\partial_{x^i}P^i(x,Du))|_{x=Ry}$, so step 2.1 proves the rescaled maximal equation. The coefficient bounds were obtained without a solution estimate. Smoothness and a slope bound must hold for a graph to which one applies such an estimate, and a common bound for $u(Ry)/R$ must be supplied whenever the estimate requires a height bound. [F3, F5, F8, step 2.1, step 2.2, algebra] ∎
