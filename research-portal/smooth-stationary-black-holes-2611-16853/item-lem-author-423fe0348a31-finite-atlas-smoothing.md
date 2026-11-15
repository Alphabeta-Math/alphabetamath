---
title: Smooth approximation of compactly supported interior heights
status: published
research_item: lem-author-423fe0348a31-finite-atlas-smoothing
dependency_level: 1
---

## Prerequisites

- [lem-author-423fe0348a31-finite-relative-cutoffs](item-lem-author-423fe0348a31-finite-relative-cutoffs)
- [lem-author-423fe0348a31-chart-sobolev-comparison](item-lem-author-423fe0348a31-chart-sobolev-comparison)
- [lem-author-423fe0348a31-compact-chart-mollification](item-lem-author-423fe0348a31-compact-chart-mollification)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction)
- [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)
- [math:def-extended-riemannian-distance-on-a-disconnected-manifold](https://alphabetamath.cc/item/def-extended-riemannian-distance-on-a-disconnected-manifold)
- [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)
- [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)
- [math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)


## Statement

Work in ZFC. Let $(R,k)$ be a compact smooth Riemannian region (a manifold with boundary) of dimension $n\ge0$, and let $v:R\to\mathbb R$ be Lipschitz with support compactly contained in its interior. There exist $v_j\in C_c^\infty(R^\circ)$, all supported in one fixed compact interior set, such that $\|v_j-v\|_\infty+\int_R(|v_j-v|+|dv_j-dv|_k)\,dV_k\to0$. Here $dv$ is the almost-everywhere weak differential, $|\cdot|_k$ is the dual metric norm and $dV_k$ is the Riemannian volume density; for $n=0$, differentials vanish and each point has volume one.

Lipschitz means that there is a single finite $L\ge0$ such that $|v(p)-v(q)|\le Ld_k(p,q)$ for every pair in the same connected component of $R$, with the usual distance on $\mathbb R$. Here $d_k$ is the infimum of the lengths $L_k(\gamma)=\int|\dot\gamma|_k$ of piecewise $C^1$ curves in $R$ joining the two points; distinct components have extended distance $+\infty$ and impose no cross-component inequality.

## Facts & Assumptions

[F1] Finite smooth interior cutoffs form a partition equal to one near the compact support. [lem-author-423fe0348a31-finite-relative-cutoffs](item-lem-author-423fe0348a31-finite-relative-cutoffs)

[F2] Chart and metric first-Sobolev norms are uniformly comparable on each chosen compact chart; locally Lipschitz functions have coordinate-independent weak differentials, with the smooth-cutoff product rule. The supplier also fixes the dimension-zero conventions. [lem-author-423fe0348a31-chart-sobolev-comparison](item-lem-author-423fe0348a31-chart-sobolev-comparison)

[F3] For every dimension $n\ge1$, a compactly supported Lipschitz coordinate function admits mollification converging uniformly and in $W^{1,1}$, with fixed compact support inside its coordinate domain; an admissible kernel exists. [lem-author-423fe0348a31-compact-chart-mollification](item-lem-author-423fe0348a31-compact-chart-mollification)

[F4] The metric is the smooth positive-definite tensor $k$ on $R$. [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)

[F5] Lipschitz continuity is the finite-constant metric inequality, applied on each connected component with one common bound. Intrinsic Riemannian distance is the infimum of piecewise $C^1$ curve lengths; the extended distance is $+\infty$ between distinct components. Length is the integral of metric speed. [math:def-lipschitz-holder-contraction](https://alphabetamath.cc/item/def-lipschitz-holder-contraction) [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold) [math:def-extended-riemannian-distance-on-a-disconnected-manifold](https://alphabetamath.cc/item/def-extended-riemannian-distance-on-a-disconnected-manifold) [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)

[F6] On a compact set contained in a coordinate chart, the Riemannian quadratic form has uniform positive lower and finite upper bounds relative to the Euclidean quadratic form. In particular $k_p(\xi,\xi)\le C|\xi|^2$ there for some finite $C>0$. [math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric](https://alphabetamath.cc/item/lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric)

[F7] Write $R^\circ=\operatorname{Int}R$ for the manifold interior: in positive dimension its points have positive last boundary-chart coordinate; in dimension zero every point is interior and the boundary is empty. [math:def-interior-point-boundary-point-interior-and-boundary-of-a-manifold](https://alphabetamath.cc/item/def-interior-point-boundary-point-interior-and-boundary-of-a-manifold)

[A1] Work in ZFC, carrying the mollification supplier's ZFC hypothesis and the chart-comparison supplier's Countable Choice hypothesis. Choice is inherited through these analytic suppliers, not through the finite partition or the explicit sequence of radii. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:**The hypotheses in the Statement.

**Goal:** Establish the stated construction or identity.

1.1 If $v=0$, take $v_j=0$ with empty support. If $n=0$, every point is interior by [F7], and every chart is a singleton, so $v$ is smooth; take $v_j=v$, whose compact interior support is fixed. The zero-dimensional conventions in [F2] make both errors zero. Henceforth take $n\ge1$ and nonempty support. Cover the support by finitely many interior coordinate balls $x_a:U_a\to B_a$, each with closure contained in a larger interior chart, and choose the cutoffs of [F1]. The identity $v=\sum_a\chi_av$ holds globally, since $v$ vanishes outside its support. By [F6], on $\overline{U_a}$ the coordinate quadratic form satisfies $k_p(\xi,\xi)\le C_a^{\mathrm{met}}|\xi|^2$ for a finite $C_a^{\mathrm{met}}>0$. For $p,q\in U_a$, the inverse-coordinate straight segment stays in $U_a$ and has length at most $\sqrt{C_a^{\mathrm{met}}}|x_a(p)-x_a(q)|$ by [F5]. Thus $d_k(p,q)$ is at most this bound, and the hypothesis gives $|v(p)-v(q)|\le L\sqrt{C_a^{\mathrm{met}}}|x_a(p)-x_a(q)|$. In particular $v$ is locally Lipschitz in smooth coordinates, as required by [F2]. Its coordinate expression is also bounded on the bounded ball $B_a$. Each coordinate cutoff is smooth with compact support in $B_a$, so its derivative is bounded there and the coordinate straight-segment estimate makes it Lipschitz. The product inequality therefore shows that $f_a=(\chi_av)\circ x_a^{-1}$ is Lipschitz and compactly supported in $B_a$. Apply [F3] in dimension $n$, using [A1], and fix for each chart a radius $r_a>0$ such that every mollified support for radius at most $r_a$ stays in one fixed compact subset $K_a$ of that chart. Use the explicit radii $r_a/(j+1)$. [given, F1, F2, F3, F5, F6, F7, A1, construct]

2.1 Pull the finitely many smooth coordinate approximants back to their charts, extend by zero, and sum them to obtain $v_j$. The zero extensions are smooth because their supports stay away from the chart sides, and all sums are supported in the fixed compact interior union $\bigcup_a K_a$. The supremum error is at most the sum of the finitely many coordinate supremum errors. Apply [F2] to each coordinate difference $f_{a,j}-f_a$, with the same fixed compact support set $K_a$ for all $j$; linearity and the cutoff product rule identify the resulting summed weak differential with $dv_j-dv$. The integral error is therefore at most $\sum_a C_a\|f_{a,j}-f_a\|_{W^{1,1}}$, with constants $C_a$ independent of $j$, and tends to zero by [F3]. Both stated convergences follow. [F2, F3, A1, step 1.1, algebra] ∎
