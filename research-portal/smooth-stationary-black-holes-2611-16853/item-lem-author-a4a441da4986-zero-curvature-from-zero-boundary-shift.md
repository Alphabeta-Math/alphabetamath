---
title: A supplied complete maximal slice has zero extrinsic curvature in the
  zero-shift case
status: draft
research_item: lem-author-a4a441da4986-zero-curvature-from-zero-boundary-shift
dependency_level: 6
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [lem-author-a4a441da4986-stationary-maximal-divergence](item-lem-author-a4a441da4986-stationary-maximal-divergence)
- [thm-maximal-jacobi-lapse-input](item-thm-maximal-jacobi-lapse-input)
- [lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)
- [math:def-induced-orientation-on-a-hypersurface-from-a-coorientation](https://alphabetamath.cc/item/def-induced-orientation-on-a-hypersurface-from-a-coorientation)
- [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-cauchy-schwarz-finite](https://alphabetamath.cc/item/thm-cauchy-schwarz-finite)


## Statement

Suppose a connected smooth complete-up-to-boundary maximal hypersurface $\overline\Sigma$ with nonempty compact smooth boundary $S$ and one asymptotically Euclidean end has already been supplied in the stationary vacuum spacetime. Assume $T|_S=0$, its lapse tends uniformly to one, and in an end chart $h-\delta=O_2(r^{-1})$, $k=O(r^{-2}\log r)$ and $X=O(r^{-1}\log r)$, with tensor norms measured by $h$ or the uniformly equivalent Cartesian metric. Then the lapse satisfies $N>0$ inside and has positive inward normal derivative at $S$, and $k=0$ everywhere on this hypersurface. These are consequences of the supplied slice, not a replacement for its existence and end estimates.

## Statement references

[def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[lem-author-a4a441da4986-stationary-maximal-divergence](item-lem-author-a4a441da4986-stationary-maximal-divergence)

[thm-maximal-jacobi-lapse-input](item-thm-maximal-jacobi-lapse-input)

[lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)

[math:def-induced-orientation-on-a-hypersurface-from-a-coorientation](https://alphabetamath.cc/item/def-induced-orientation-on-a-hypersurface-from-a-coorientation)

[math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[math:thm-cauchy-schwarz-finite](https://alphabetamath.cc/item/thm-cauchy-schwarz-finite)

## Facts & Assumptions

[A1] Work in the inherited ZFC convention, including the Axiom of Choice. Applying a choice function to the family of values of any countable family of nonempty sets and composing with its indexing gives countable choice. This supplies the choice hypothesis of the divergence theorem used in step 2.2, as well as the choice conventions of the other suppliers. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The stationary data supply an oriented smooth time-oriented Lorentzian four-manifold and a smooth Killing field $T$; vacuum here is the geometric hypothesis $\operatorname{Ric}(g)=0$. The supplied spacelike hypersurface has smooth future unit normal $n$, induced metric $h$, symmetric second fundamental form $k(U,V)=-g(\nabla_U n,V)$, and maximality $\operatorname{tr}_h k=0$. Its lapse and shift are $N=-g(T,n)$ and $X=T-Nn$. Complete up to the compact boundary uses the intrinsic distance with the boundary included. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F2] Use the smooth exterior convention: a compact core and a fixed chart onto $\{x\in\mathbb R^3:|x|>r_0\}$, with $r=|x|$, and $\Delta_h=\operatorname{div}_h\operatorname{grad}_h$. The end limit is uniform in this chart. Here $h-\delta=O_2(r^{-1})$ means that each Cartesian component and its coordinate derivatives of orders $j=0,1,2$ are $O(r^{-1-j})$. The displayed $O$ bounds for $k$ and $X$ are pointwise norm bounds. [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)

[F3] On a supplied maximal hypersurface the Killing lapse satisfies $\Delta_hN=(|k|_h^2+\operatorname{Ric}(n,n))N$. On a connected smooth Riemannian exterior, a smooth solution of $(\Delta_h-V)u=0$ with smooth $V\ge0$, zero compact boundary values, and uniform positive end limit is positive inside and has strictly positive inward unit normal derivative at the boundary. [thm-maximal-jacobi-lapse-input](item-thm-maximal-jacobi-lapse-input) [lem-exterior-lapse-maximum-and-boundary-control](item-lem-exterior-lapse-maximum-and-boundary-control)

[F4] With these vacuum and maximal conventions, the smooth tangent field $Y^i=k^{ij}X_j$ satisfies $\operatorname{div}_hY=N|k|_h^2$. [lem-author-a4a441da4986-stationary-maximal-divergence](item-lem-author-a4a441da4986-stationary-maximal-divergence)

[F5] A coorienting normal ray on a hypersurface in an oriented manifold induces its orientation by the normal-first rule. On an oriented Riemannian manifold with smooth boundary, countable choice permits the divergence theorem for smooth compactly supported vector fields, with outward unit normal and outward-normal-first boundary orientation; on a compact manifold every smooth field is compactly supported. [math:def-induced-orientation-on-a-hypersurface-from-a-coorientation](https://alphabetamath.cc/item/def-induced-orientation-on-a-hypersurface-from-a-coorientation) [math:thm-riemannian-divergence-theorem](https://alphabetamath.cc/item/thm-riemannian-divergence-theorem)

[F6] For finite real lists $(a_j)$ and $(b_j)$, $(\sum_j a_jb_j)^2\le(\sum_j a_j^2)(\sum_j b_j^2)$. [math:thm-cauchy-schwarz-finite](https://alphabetamath.cc/item/thm-cauchy-schwarz-finite)

## Proof

**Given:** The conditional slice, geometric vacuum and end hypotheses of the Statement, with [A1] and [F1]–[F6].

**Goal:** Prove the stated lapse properties and the vanishing of $k$.

1.1 At $S$, $T=0$ gives $N=-g(T,n)=0$ and then $X=T-Nn=0$ directly. The smooth normal and orthogonal decomposition extend to the boundary by the supplied smooth spacelike boundary data. No null sheets are needed for these pointwise conclusions. [given, F1]

1.2 Orient $\overline\Sigma$ by the smooth future normal $n$: a tangent basis $(v_1,v_2,v_3)$ is positive precisely when $(n,v_1,v_2,v_3)$ is positive in the oriented ambient spacetime. Since $n$ is everywhere transverse, this is a smooth orientation, including at $S$. For sufficiently large $R$, remove the open tail $\{r>R\}$ to obtain the compact smooth truncation $\Omega_R$ with boundary $S\sqcup S_R$, where $S_R=\{r=R\}$. Compactness follows from the compact-core exterior convention; the end chart makes $S_R$ a smooth boundary disjoint from $S$. Restrict the induced orientation to $\Omega_R$ and give its boundary the outward-normal-first orientation. [given, F1, F2, F5]

2.1 By [F3] and the geometric vacuum hypothesis, $\Delta_hN=|k|_h^2N$. The potential $|k|_h^2$ is smooth and nonnegative. The exterior is connected with smooth compact boundary, $N$ is smooth up to that boundary, step 1.1 supplies its zero boundary values, and its uniform end limit is one. Thus the exterior maximum and boundary-control result gives $N>0$ inside and a strictly positive inward unit normal derivative at every point of $S$. [given, F1, F2, F3, step 1.1]

2.2 The field $Y$ in [F4] is smooth on compact $\Omega_R$, so the divergence theorem applies there with countable choice supplied by [A1]. If $\nu_R$ is its outward unit normal on $S_R$, the identity becomes $\int_{\Omega_R}N|k|_h^2\,d\mu_h=\int_{S_R}h(Y,\nu_R)\,dA_h$, since $X=0$ makes the flux on $S$ zero. In an $h$-orthonormal frame, apply [F6] to each row of $(k_{ij})$ and the components of $X$, then sum: $|Y|_h^2=\sum_i(\sum_j k_{ij}X_j)^2\le(\sum_{i,j}k_{ij}^2)(\sum_jX_j^2)=|k|_h^2|X|_h^2$. Taking nonnegative square roots gives $|Y|_h\le |k|_h|X|_h$. The bound $h-\delta=O(r^{-1})$ makes $h$ uniformly equivalent to the Cartesian metric for large $r$, and its restriction to $S_R$ therefore gives $\operatorname{Area}_h(S_R)\le CR^2$. The end estimates yield $\left|\int_{S_R}h(Y,\nu_R)\,dA_h\right|\le CR^2R^{-2}\log R\,R^{-1}\log R=CR^{-1}(\log R)^2\to0$. [given, A1, F1, F2, F4, F5, F6, step 1.1, step 1.2]

3.1 The integrand $N|k|_h^2$ is continuous and nonnegative by step 2.1. The compact truncations are nested and exhaust the hypersurface. For any fixed sufficiently large $R_0$ and all $R\ge R_0$, $0\le\int_{\Omega_{R_0}}N|k|_h^2\,d\mu_h\le\int_{\Omega_R}N|k|_h^2\,d\mu_h$, and the right side tends to zero by step 2.2. Every such fixed integral is therefore zero. A positive value of the integrand at an interior point would, by continuity and positivity of the Riemannian volume density, give a positive integral on a small coordinate neighborhood, a contradiction. Hence $N|k|_h^2=0$ throughout the interior; its strictly positive lapse factor forces $k=0$ there. Smoothness up to $S$ then gives $k=0$ on the boundary as well. [F1, step 2.1, step 1.2, step 2.2] ∎
