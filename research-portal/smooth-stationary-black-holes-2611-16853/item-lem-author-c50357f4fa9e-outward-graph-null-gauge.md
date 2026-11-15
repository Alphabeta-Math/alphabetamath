---
title: Canonical outward normals and null gauge on a graph
status: draft
research_item: lem-author-c50357f4fa9e-outward-graph-null-gauge
dependency_level: 1
---

## Prerequisites

- [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain)
- [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form)
- [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry)
- [math:def-pullback-riemannian-metric](https://alphabetamath.cc/item/def-pullback-riemannian-metric)
- [math:def-musical-isomorphisms](https://alphabetamath.cc/item/def-musical-isomorphisms)


## Statement

Use an admissible normal graph $F_u$ in the tube of the preceding graph-domain lemma, and let $n$ be the smooth future unit normal to the fixed hypersurface $\Sigma$. In tube coordinates $(x^1,x^2,r)$ the covector $\alpha_u=dr-(\partial_a u)dx^a$, evaluated at $(x,u(x))$, annihilates the graph tangent plane. Write $h$ also for its pullback $T^*h$ to the tube. For a tube covector $\alpha$, let $\alpha^{\sharp_h}$ be the unique vector satisfying $h(\alpha^{\sharp_h},V)=\alpha(V)$ for every tube tangent vector $V$, and define $|\alpha|_h=\sqrt{h(\alpha^{\sharp_h},\alpha^{\sharp_h})}$. Set $\nu_u=\alpha_u^{\sharp_h}/|\alpha_u|_h$, and push this vector to $\Sigma$. These definitions agree on overlaps and give the outward smooth $h$-unit normal along the graph, with $\nu_0=\nu$. Here **outward** means positive pairing with $T_*\partial_r$.

The fields $L_u=n+\nu_u$ and $\underline L_u=(n-\nu_u)/2$ along the graph are future null normals satisfying $g(L_u,\underline L_u)=-1$. They depend smoothly on the first graph data $(x,u,\partial u)$ and fix the normal gauge throughout the deformation, rather than choosing a new arbitrary boost at each parameter.

## Facts & Assumptions

[F1] [lem-author-c50357f4fa9e-normal-graph-domain](item-lem-author-c50357f4fa9e-normal-graph-domain) supplies $T$, the admissible graph and its embedding into $\Sigma$.

[F2] [physics:lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form](https://alphabetamath.cc/physics/item/lem-gr-spacelike-hypersurface-normal-and-second-fundamental-form) supplies the smooth future unit normal $n$ of this fixed hypersurface and its smooth induced positive metric $h$.

[F3] [physics:def-gr-fx-null-screen-geometry](https://alphabetamath.cc/physics/item/def-gr-fx-null-screen-geometry) defines null expansion and the effect of changing a null normal's positive scale; its normalized second null normal may be rescaled from pairing $-2$ to pairing $-1$.

[F4] [math:def-pullback-riemannian-metric](https://alphabetamath.cc/item/def-pullback-riemannian-metric) defines $(T^*h)_z(V,W)=h_{T(z)}(dT_zV,dT_zW)$. Since $T$ is the diffeomorphism supplied by [F1], this tensor is a smooth positive definite metric on the tube.

[F5] [math:def-musical-isomorphisms](https://alphabetamath.cc/item/def-musical-isomorphisms) defines $\alpha^{\sharp_h}$ by $h(\alpha^{\sharp_h},V)=\alpha(V)$. The covector norm in the Statement is defined from this vector and the positive metric $h$.

## Proof

**Given:**An admissible graph in the supplied tube, with $h,n,\nu$ as above.

**Goal:** Justify the smooth, normalized outward graph gauge.

1.1 The scalar function $r-u(p)$ is defined on the part of the tube over the domain of $u$, independently of a coordinate chart on $S$. Its differential is $\alpha_u$ and takes value one on $\partial_r$. It is nonzero and annihilates each tangent vector $\partial_a+(\partial_a u)\partial_r$ to the graph. The tube metric is smooth and positive definite by [F4]. The defining identity in [F5] gives $h(\alpha_u^{\sharp_h},V)=\alpha_u(V)$, so $\alpha_u^{\sharp_h}\ne0$ and $|\alpha_u|_h>0$. Dividing by this norm and pushing forward by $T$ gives a unique smooth unit normal with positive pairing with $T_*\partial_r$, since $h(\alpha_u^{\sharp_h}/|\alpha_u|_h,\partial_r)=1/|\alpha_u|_h>0$. At $u=0$, $dT(X,0)=X$ and $T_*\partial_r=\nu$ by [F1], so this normal is $\nu$. The scalar construction makes the local formulas agree. The inverse-matrix and square-root formulas show smooth dependence on $(x,u,\partial u)$. [F1, F2, F4, F5, given, algebra]

2.1 Orthogonality gives $g(n,n)=-1$, $g(\nu_u,\nu_u)=1$, $g(n,\nu_u)=0$. Direct multiplication gives $g(L_u,L_u)=g(\underline L_u,\underline L_u)=0$ and $g(L_u,\underline L_u)=-1$. Both are nonzero and future-directed because their scalar product with the future timelike $n$ is negative. They are normal to the graph. The factors used to normalize the second null vector do not affect the expansion of $L_u$, defined by [F3]. This proves the stated gauge with its smoothness and orientation. [F2, F3, step 1.1, algebra] ∎
