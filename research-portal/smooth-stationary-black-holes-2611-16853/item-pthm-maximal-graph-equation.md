---
title: Asymptotic maximal graph equation and coefficients
status: published
research_item: pthm-maximal-graph-equation
dependency_level: 13
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 14, §3.2.1, divergence equation and L
      statement: The normalized maximal graph satisfies the displayed divergence
        equation and a second-order equation with coefficients
        a^{ij}=δ^{ij}+O(r_q^{-1}), b^j=O(r_q^{-2}), and f=O(r_q^{-3}), uniformly
        for q bounded below by a positive constant.
      hypotheses: The article's stationary vacuum construction and the candidate
        maximal sections in its continuation argument, with q in a fixed
        positive interval.
      reading_limits: Read the frozen article text at the cited passage. This
        reference attributes the article's claim; the argument below uses the
        stated suppliers and a local calculation.
---

PDF p. 14: ` §3.2.1, divergence equation and L `

## Prerequisites

- [pthm-end-lapse-slope](item-pthm-end-lapse-slope)
- [pthm-transformed-end-geometries](item-pthm-transformed-end-geometries)
- [pthm-harrison-lorentzian-algebra](item-pthm-harrison-lorentzian-algebra)
- [def-stationary-maximal-graph](item-def-stationary-maximal-graph)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [physics:lem-gr-metric-divergence-and-density-formula](https://alphabetamath.cc/physics/item/lem-gr-metric-divergence-and-density-formula)
- [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)
- [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)
- [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle)


## Statement

Fix $\delta\in(0,1)$ and take the family of candidate sections and normalized stationary end coordinates in the uniform asymptotic slope result. In particular, the sections are assumed to exist, are smooth and spacelike and have zero mean curvature; the differentiated end and graph-slope estimates there hold uniformly for $q\in[\delta,1]$. Write $g=g_q$, $u=\widetilde u_q$, $r=r_q$, and let indices $i,j,k$ range over $1,2,3$ in the coordinates $(t_q,x_q)$. Then, on a common sufficiently distant end, $u$ satisfies
$$\partial_i\!\left(\frac{\sqrt{-\det g}\,(g^{ij}u_j-g^{i0})}{\sqrt{-g^{00}+2g^{0j}u_j-g^{jk}u_j u_k}}\right)=0.$$
Moreover this equation can be written $a^{ij}(g,\partial u)u_{ij}+b^j(g,\partial g,\partial u)u_j=f(g,\partial g)$, where $a^{ij}=\delta^{ij}+O(r^{-1})$, $b^j=O(r^{-2})$, and $f=O(r^{-3})$, uniformly for $q\in[\delta,1]$. These estimates mean bounds by constants independent of $q$ on a common end; the constants and radius may depend on $\delta$. The function $f$ in this equation is distinct from the stationary norm $-g(T,T)$.

## Statement references

[pthm-end-lapse-slope](item-pthm-end-lapse-slope)

[pthm-transformed-end-geometries](item-pthm-transformed-end-geometries)

[def-stationary-maximal-graph](item-def-stationary-maximal-graph)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

## Facts & Assumptions

[F1] In the normalized stationary coordinates, the graph is $t_q=u(x_q)$ and the spacelike graph has zero mean curvature. With the supplied sign convention, the mean curvature is $H=-\operatorname{tr}_h k$. [def-stationary-maximal-graph](item-def-stationary-maximal-graph) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F2] Uniformly on a common end, $g_{00}=-1+O_5(r^{-1})$, $g_{0i}=O_5(r^{-2})$, and $g_{ij}=\delta_{ij}+O_5(r^{-1})$; the subscript means that each spatial derivative through order five gains the corresponding inverse power of $r$. [pthm-transformed-end-geometries](item-pthm-transformed-end-geometries)

[F3] Uniformly on a common end, $|\partial u|\le Cr^{-1/2}$ and the graph is spacelike. [pthm-end-lapse-slope](item-pthm-end-lapse-slope)

[F4] On a smooth time-oriented Lorentzian four-manifold with its Levi–Civita connection, the metric density $w=\sqrt{|\det g|}$ gives $\nabla_\mu J^\mu=w^{-1}\partial_\mu(wJ^\mu)$ for a smooth vector field $J$ in a smooth chart. [physics:lem-gr-metric-divergence-and-density-formula](https://alphabetamath.cc/physics/item/lem-gr-metric-divergence-and-density-formula)

[F5] If $h$ is continuously differentiable on an open interval containing $[0,1]$, then $\int_0^1h'(s)\,ds=h(1)-h(0)$. [math:lem-fundamental-theorem-and-integration-by-parts](https://alphabetamath.cc/item/lem-fundamental-theorem-and-integration-by-parts)

[F6] If $v:U\to V\subseteq\mathbb R^n$ is totally differentiable at $a\in U$ and $w:V\to\mathbb R^m$ is totally differentiable at $v(a)$, then $D(w\circ v)(a)=Dw(v(a))\circ Dv(a)$. [math:thm-chain-rule-for-total-derivatives](https://alphabetamath.cc/item/thm-chain-rule-for-total-derivatives)

[F7] Let $a<b$ and $c<d$. If $v,h:[a,b]\times[c,d]\to\mathbb R$ are continuous and $\partial_yv(y,s)=h(y,s)$ for $a<y<b$ and every $s\in[c,d]$, then $G(y)=\int_c^dv(y,s)\,ds$ satisfies $G\prime(y)=\int_c^dh(y,s)\,ds$ for $a<y<b$. [math:thm-differentiation-under-the-integral-sign-on-a-compact-rectangle](https://alphabetamath.cc/item/thm-differentiation-under-the-integral-sign-on-a-compact-rectangle)

[F8] The inherited stationary graph data supply an original stationary Lorentzian metric $g_{\mathrm{orig}}$, normalized Ernst potential, pole with $T_p=0$, and smooth stationary Harrison one-form with $W_q(T)=d_q-D_q$ on a domain $D_q>0$ containing the exterior; the transformed metric is $g_q=(D_q/4)A_q^*g_{\mathrm{orig}}$. For these data the Harrison Lorentzian-algebra result gives $d_q>0$ and $\mathcal L_Tg_q=0$. The graph coordinates have $T=\partial_t$ and $t_q=d_qt/(4q)$, with $q$ and $d_q$ constant in spacetime. [def-stationary-maximal-graph](item-def-stationary-maximal-graph) [pthm-harrison-lorentzian-algebra](item-pthm-harrison-lorentzian-algebra)

## Proof

**Given:** The candidate family and normalized end coordinates in the Statement.

**Goal:** Derive the divergence equation and the stated uniform coefficient bounds.

1.1 By [F8], the Harrison stationarity result applies to the supplied data on the end and gives $\mathcal L_Tg_q=0$. The local flow of $T=\partial_t$ translates $t$ with the spatial coordinates fixed, so the flow definition of the metric Lie derivative makes every component of $g_q$ independent of $t$. Since $\partial_{t_q}=(4q/d_q)T$, the components in the normalized coordinates are independent of $t_q$ as well. Set $\tau=t_q-u(x_q)$ and $D=-g^{00}+2g^{0j}u_j-g^{jk}u_j u_k$. The spacelike graph has timelike normal covector $d\tau$, so $D>0$. Its future unit normal has components $n^\mu=-g^{\mu\nu}\partial_\nu\tau/\sqrt D$. Extend this normal off the graph using the same formula and the time-independent function $u$. The mean curvature vanishes exactly when $\nabla_\mu n^\mu=0$: differentiating $g(n,n)=-1$ shows the normal-normal contribution to the ambient divergence vanishes. Applying [F4] to the smooth extended normal gives $\nabla_\mu n^\mu=(\sqrt{-\det g})^{-1}\partial_\mu(\sqrt{-\det g}\,n^\mu)$. Time independence removes the time derivative, and $n^i=(g^{ij}u_j-g^{i0})/\sqrt D$. This proves the displayed divergence equation. [given, F1, F3, F4, F8, algebra]

2.1 Write $p=(p_j)$ and define $D(x,p)=-g^{00}+2g^{0j}p_j-g^{jk}p_jp_k$ and $A^i(x,p)=\sqrt{-\det g}(g^{ij}p_j-g^{i0})/\sqrt{D(x,p)}$. The metric estimates and matrix inversion give $g^{00}=-1+O_5(r^{-1})$, $g^{0i}=O_5(r^{-2})$, $g^{ij}=\delta^{ij}+O_5(r^{-1})$, and $\sqrt{-\det g}=1+O_5(r^{-1})$. For $p=s\partial u$, $0\le s\le1$, the slope bound implies $D(x,p)=1+O(r^{-1})$ uniformly; hence it is bounded away from zero on a common larger end. Direct differentiation of the displayed rational expression, holding $p$ fixed for spatial derivatives, gives $\partial_{p_j}A^i(x,p)=\delta^{ij}+O(r^{-1})$ and $\partial_{x_i}\partial_{p_j}A^i(x,p)=O(r^{-2})$ uniformly on this segment. Also $A^i(x,0)=O(r^{-2})$ and $\partial_{x_i}A^i(x,0)=O(r^{-3})$. These estimates use only the first spatial derivatives of the metric bounds and the explicit factors $p$, with $|p|^2=O(r^{-1})$. [F2, F3, F6, step 1.1, algebra]

3.1 Define $B^{ij}(x,p)=\int_0^1\partial_{p_j}A^i(x,sp)\,ds$. By step 2.1, for each fixed $x$ and $p=\partial u(x)$, the curve $s\mapsto A^i(x,sp)$ is smooth on an open interval containing $[0,1]$. The chain rule [F6] gives its derivative as $\partial_{p_j}A^i(x,sp)p_j$. Applying [F5] componentwise gives $A^i(x,p)=A^i(x,0)+B^{ij}(x,p)p_j$. The same identity holds for nearby $(x,p)$ wherever the segment has $D(x,sp)>0$. [F5, F6, step 2.1, algebra]

4.1 Fix $x_0$ on the common end and $p_0=\partial u(x_0)$. For each spatial index $i$, hold the other coordinates and $p=p_0$ fixed. Positivity of $D(x_0,sp_0)$ for $0\le s\le1$ and smoothness give a sufficiently small closed interval $[a,b]$ containing $x_0^i$ in its interior on which $D(x,sp_0)>0$ for every $s\in[0,1]$. On this rectangle the integrand $\partial_{p_j}A^i(x,sp_0)$ and its $x_i$ derivative are continuous, so [F7] applies with integration interval $[0,1]$. Consequently, with $p$ held fixed, $\partial_{x_i}B^{ij}(x_0,p_0)=\int_0^1\partial_{x_i}\partial_{p_j}A^i(x_0,sp_0)\,ds$. The uniform pointwise bound in step 2.1 makes this $O(r^{-2})$ after summing over $i$; the auxiliary interval need not be uniform in $q$. [F7, step 2.1, step 3.1, algebra]

5.1 Apply the chain rule [F6] to $x\mapsto A^i(x,\partial u(x))$. The divergence equation becomes $\partial_{p_j}A^i(x,\partial u)u_{ij}+\partial_{x_i}A^i(x,\partial u)=0$, with the second derivative holding $p$ fixed. Differentiating the identity in step 3.1 at fixed $p$ and using step 4.1 yields $a^{ij}u_{ij}+b^ju_j=f$, with $a^{ij}=\partial_{p_j}A^i(x,\partial u)$, $b^j=\partial_{x_i}B^{ij}(x,\partial u)$ with $p$ held fixed in that derivative, and $f=-\partial_{x_i}A^i(x,0)$. Steps 2.1 and 4.1 give $a^{ij}=\delta^{ij}+O(r^{-1})$, $b^j=O(r^{-2})$ and $f=O(r^{-3})$, uniformly in $q$. This specifies one admissible choice of the coefficients; the divergence equation itself is independent of that choice. [F6, step 1.1, step 2.1, step 3.1, step 4.1, algebra] ∎

## Source notes

The article citation attributes the original equation and estimates. The proof uses the declared end and slope results and the displayed coordinate calculation, without using the article's claim as a premise.
