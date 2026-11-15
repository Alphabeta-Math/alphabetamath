---
title: The thin-collar flux error is uniform over all smooth comparison regions
status: published
research_item: lem-author-60420990c802-uniform-thin-collar-flux-comparison
dependency_level: 3
---

## Prerequisites

- [lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance](item-lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance)
- [lem-author-60420990c802-bounded-distance-laplacian-and-collar-density](item-lem-author-60420990c802-bounded-distance-laplacian-and-collar-density)
- [lem-thin-collar-divergence-area-input](item-lem-thin-collar-divergence-area-input)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density)
- [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)
- [math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary)
- [math:def-smooth-partition-of-unity-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-partition-of-unity-on-a-manifold-with-boundary)
- [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation)
- [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)
- [math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)
- [math:def-riemannian-volume-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-riemannian-volume-form-on-an-oriented-manifold)



## Statement

Work in ZFC. Let $(\Sigma,h)$ be a smooth Riemannian manifold of dimension $n\ge1$ with compact boundary $S$ and metric smooth and positive up to $S$. Fix the supplied compact inward normal distance collar $F:S\times[0,a_0]\to\Sigma$, where $\rho$ is intrinsic distance from $S$, $\rho\circ F=s$, and $F^*h=ds^2+h_s$. The fixed collar constants satisfy $C\ge0$, $K>0$, $|\nabla_h\rho|=1$, $|\Delta_h\rho|\le C$, and $F^*dV_h=j(p,s)\,dA_S\,ds$ with $0<j\le K$. Use $\Delta_h=\operatorname{div}_h\nabla_h$ and Riemannian density integration; no orientation or connectedness is assumed.

For $0<\eta\le a_0$, let $\Omega\subset\{0\le\rho\le\eta\}$ be a compact smooth $n$-dimensional region with boundary $S\sqcup D$ that contains the inward side of $S$. The outer boundary $D$ may be disconnected. Then
$$|S|=\int_Dh(\nabla_h\rho,\nu)\,dA-\int_\Omega\Delta_h\rho\,dV_h\le|D|+CK\eta|S|,$$
where $\nu$ is the outward unit normal of $\Omega$, $|S|=\int_SdA_S$, and $|D|=\int_DdA$. In particular the error is $O(\eta)$ uniformly in every choice of smooth region or approximation parameter. If $S$ is empty, its supplied collar and every such region are empty and all integrals are zero.

## Facts & Assumptions

[A1] Work in ZFC, retaining the choice assumption of both collar suppliers. The Axiom of Choice implies countable choice, which supplies the foundational hypothesis of the divergence, partition and density-integration theorems used below. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:thm-choice-implies-dependent-implies-countable-choice](https://alphabetamath.cc/item/thm-choice-implies-dependent-implies-countable-choice)

[F1] A Riemannian metric is smooth and positive definite on each tangent space. The normal-distance supplier gives $\rho\circ F=s$, $F^*h=ds^2+h_s$ and $\nabla_h\rho=\partial_s$, smoothly up to $S$. The bounded-collar supplier gives the fixed $C,K,a_0$, the density formula and $\operatorname{Vol}_h(\Omega)\le K\eta|S|$ for every measurable region in this collar; in particular every compact smooth region is Borel. These suppliers allow disconnected manifolds, using extended intrinsic distance between components. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance](item-lem-author-60420990c802-normal-coordinate-is-intrinsic-boundary-distance) [lem-author-60420990c802-bounded-distance-laplacian-and-collar-density](item-lem-author-60420990c802-bounded-distance-laplacian-and-collar-density)

[F2] In dimension three, the thin-collar comparison supplier applies in ZFC to a smooth Riemannian three-manifold with compact boundary, a unit-gradient collar with the stated Laplacian bound, and a compact smooth region containing the inward side of $S$, with boundary $S\sqcup D$. It gives $|S|\le|D|+C\operatorname{Vol}_h(\Omega)$ and, with the density bound, $|S|\le|D|+CK\eta|S|$. Its public statement is an inequality, not the exact flux identity. It is used here only for this three-dimensional comparison. [lem-thin-collar-divergence-area-input](item-lem-thin-collar-divergence-area-input)

[F3] On an oriented Riemannian manifold with boundary of dimension at least one, under countable choice a smooth compactly supported vector field has integral of divergence equal to its outward normal flux. Compact manifolds allow every smooth field. [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)

[F4] Under countable choice there is a smooth partition of unity subordinate to a cover by charts of a manifold with boundary: its nonnegative functions have locally finite supports contained in their charts and sum to one. Compactly supported smooth density integration is local, linear, nonnegative and independent of orientation; in a chart the Riemannian density has coefficient $\sqrt{\det G}$. The oriented Riemannian volume form has this coefficient in positive charts and its absolute density is the Riemannian density, also with the signed zero-form convention in dimension zero. [math:thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary](https://alphabetamath.cc/item/thm-smooth-partitions-of-unity-exist-on-manifolds-with-boundary) [math:def-smooth-partition-of-unity-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-partition-of-unity-on-a-manifold-with-boundary) [math:thm-density-integration-is-defined-without-an-orientation](https://alphabetamath.cc/item/thm-density-integration-is-defined-without-an-orientation) [math:def-riemannian-volume-density](https://alphabetamath.cc/item/def-riemannian-volume-density) [math:def-riemannian-volume-form-on-an-oriented-manifold](https://alphabetamath.cc/item/def-riemannian-volume-form-on-an-oriented-manifold)

[F5] The coordinate formula $\operatorname{div}_hY=(\det G)^{-1/2}\sum_k\partial_k((\det G)^{1/2}Y^k)$ holds also in nonorientable and boundary charts, using smooth extensions at the boundary. [math:prop-coordinate-formula-for-riemannian-divergence](https://alphabetamath.cc/item/prop-coordinate-formula-for-riemannian-divergence)

[F6] Cauchy–Schwarz in each real inner product space $(T_x\Sigma,h_x)$ gives $|h_x(u,v)|\le|u|_h|v|_h$. [math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces](https://alphabetamath.cc/item/thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces)

## Proof

**Given:** The hypotheses in the Statement, in ZFC as in [A1].

**Goal:** Prove the exact flux identity and the uniform area comparison without assuming orientability.

1.1 Assume first that $S\ne\varnothing$. Give $\Omega$ its induced smooth Riemannian metric. Cover this compact manifold with boundary by its boundary and interior charts and choose a subordinate smooth partition $(\chi_i)$. Compactness and local finiteness imply that only finitely many supports meet $\Omega$: finitely many neighborhoods, each meeting only finitely many supports, cover $\Omega$. Each support is closed in compact $\Omega$ and lies in its chart $U_i$, hence is compact in $U_i$. Orient each $U_i$ separately and apply [F3] to the compactly supported field $\chi_iX$, where $X=\nabla_h\rho$ is smooth up to the boundary by [F1]. The only manifold boundary of this relatively open chart is $U_i\cap\partial\Omega$; the field vanishes near its artificial chart edges. In a positive oriented chart the Riemannian volume form integrates as its density, and the same is true of the induced outward-normal-first boundary form. Thus each local divergence identity is an equality of density integrals, without a chosen global orientation. [given, A1, F1, F3, F4]

2.1 For $w=\sqrt{\det G}$, [F5] gives $\operatorname{div}_h(\chi_iX)=w^{-1}\sum_k\partial_k(w\chi_iX^k)=\chi_i\operatorname{div}_hX+X(\chi_i)$. Summing the finitely many local identities from step 1.1, locality and linearity of density integration give $\sum_i\operatorname{div}_h(\chi_iX)=\operatorname{div}_hX$ and $\sum_i h(\chi_iX,\nu)=h(X,\nu)$, since $\sum_i\chi_i=1$ and $\sum_iX(\chi_i)=0$. Consequently $\int_\Omega\Delta_h\rho\,dV_h=\int_{\partial\Omega}h(\nabla_h\rho,\nu)\,dA$. At $S$, the Gaussian metric and inward-side condition imply $\nu=-\partial_s=-\nabla_h\rho$. Its flux is therefore $-|S|$, which yields the stated exact identity. The argument uses only local orientations and includes disconnected $D$. [given, F1, F4, F5, step 1.1]

3.1 On $D$, [F6] and $|\nabla_h\rho|=|\nu|=1$ give $h(\nabla_h\rho,\nu)\le1$. For the other term, the smooth density $(C+\Delta_h\rho)dV_h$ is nonnegative, so positivity and linearity of its integral give $-\int_\Omega\Delta_h\rho\,dV_h\le C\operatorname{Vol}_h(\Omega)\le CK\eta|S|$, using [F1]. All these integrals are finite on the compact smooth region. Inserting these two bounds into step 2.1 proves the displayed inequality in every dimension $n\ge1$. When $n=3$, the region, ZFC, compact boundary, unit gradient, Laplacian bound and collar density supplied in the Statement and [F1] also meet every hypothesis of [F2], which independently gives this same comparison. No three-dimensional comparison is used to obtain the exact identity or to infer the result in other dimensions. [given, A1, F1, F2, F4, F6, step 2.1]

4.1 The coefficient $CK|S|$ depends only on the one fixed compact collar and boundary, not on $\Omega$, any smoothing parameter, or the number of components of $D$. This proves the asserted uniform $O(\eta)$ error. If $S=\varnothing$, [F1] identifies the distance sublevel with the empty collar, so $\Omega=D=\varnothing$ and the same conclusions hold with zero integrals. [given, F1, step 3.1] ∎
