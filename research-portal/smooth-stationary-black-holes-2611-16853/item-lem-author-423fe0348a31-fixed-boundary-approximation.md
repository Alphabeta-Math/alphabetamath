---
title: Boundary-constant-preserving smooth approximation
status: draft
research_item: lem-author-423fe0348a31-fixed-boundary-approximation
dependency_level: 4
---

## Prerequisites

- [lem-author-423fe0348a31-finite-relative-cutoffs](item-lem-author-423fe0348a31-finite-relative-cutoffs)
- [lem-author-423fe0348a31-finite-atlas-smoothing](item-lem-author-423fe0348a31-finite-atlas-smoothing)
- [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)
- [lem-author-423fe0348a31-chart-sobolev-comparison](item-lem-author-423fe0348a31-chart-sobolev-comparison)
- [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold)
- [math:def-extended-riemannian-distance-on-a-disconnected-manifold](https://alphabetamath.cc/item/def-extended-riemannian-distance-on-a-disconnected-manifold)
- [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)
- [math:prop-riemannian-metrics-induce-metrics-on-dual-tensor-and-exterior-bundles](https://alphabetamath.cc/item/prop-riemannian-metrics-induce-metrics-on-dual-tensor-and-exterior-bundles)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)
- [math:prop-chain-rule-for-smooth-half-space-maps](https://alphabetamath.cc/item/prop-chain-rule-for-smooth-half-space-maps)
- [math:thm-ftc-second-part](https://alphabetamath.cc/item/thm-ftc-second-part)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)


## Statement

Work in ZFC. Let $(R,k)$ be a compact smooth Riemannian region (a manifold with boundary) of dimension $n\ge0$ whose boundary is $B_-\sqcup B_+$, with both parts closed and disjoint. Let $u:R\to\mathbb R$ be Lipschitz, equal to constants $c_-$ and $c_+$ respectively on open neighborhoods of these parts. There exist smooth $u_j$ on $R$, all equal to those same constants on fixed smaller boundary neighborhoods, with $u_j\to u$ uniformly and in metric $W^{1,1}(R)$. Here smoothness includes smooth local extension in boundary charts. Lipschitz means a single finite bound with respect to intrinsic Riemannian distance within each connected component; the distance between distinct components is $+\infty$. Metric first-Sobolev convergence here means
$$\int_R\bigl(|u_j-u|+|du_j-du|_k\bigr)\,dV_k\longrightarrow0,$$
where $du$ is the almost-everywhere coordinate weak differential, $|\cdot|_k$ is the dual metric norm, and $dV_k$ is the Riemannian volume density. In dimension zero differentials vanish and each point has volume one; for empty $R$ the supremum error and integral are zero.

## Facts & Assumptions

[F1] Smooth relative cutoffs may equal one near a compact boundary set and have support inside its prescribed open neighborhood. Support is the closure in $R$ of the nonzero locus. [lem-author-423fe0348a31-finite-relative-cutoffs](item-lem-author-423fe0348a31-finite-relative-cutoffs)

[F2] A compactly supported interior Lipschitz function has simultaneous uniform and metric first-Sobolev smooth approximation with all supports in one fixed compact interior set, in every dimension $n\ge0$, under ZFC. Its integral convergence is exactly the one displayed in the Statement. [lem-author-423fe0348a31-finite-atlas-smoothing](item-lem-author-423fe0348a31-finite-atlas-smoothing)

[F3] In dimension three, metric weak gradients and normalized cut areas retain the fixed Riemannian conventions; no cut-area input is needed for the approximation construction. [def-lipschitz-cut-area-data](item-def-lipschitz-cut-area-data)

[F4] Locally Lipschitz functions have coordinate-independent weak differentials on the interior. The metric Sobolev integral uses the dual norm and Riemannian volume density; dimension zero has zero differentials and unit point volumes. These conventions and coordinate norm comparisons are supplied by [lem-author-423fe0348a31-chart-sobolev-comparison](item-lem-author-423fe0348a31-chart-sobolev-comparison).

[F5] The boundary smooth structure uses compatible half-space charts and smooth local Euclidean extensions; $k$ is a smooth positive-definite tensor. Intrinsic distance is the infimum of piecewise $C^1$ curve lengths, with cross-component value $+\infty$; length is the integral of metric speed. [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary) [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold) [math:def-riemannian-distance-on-a-connected-manifold](https://alphabetamath.cc/item/def-riemannian-distance-on-a-connected-manifold) [math:def-extended-riemannian-distance-on-a-disconnected-manifold](https://alphabetamath.cc/item/def-extended-riemannian-distance-on-a-disconnected-manifold) [math:def-riemannian-speed-and-length](https://alphabetamath.cc/item/def-riemannian-speed-and-length)

[F6] The induced dual metric is smooth, so the squared dual norm of a smooth differential is continuous. Continuous real-valued functions on a nonempty compact space attain finite bounds (claim 2). The half-space chain rule holds for local smooth extensions, and the scalar fundamental theorem evaluates a $C^1$ function increment by the integral of its derivative, including one-sided endpoint derivatives. [math:prop-riemannian-metrics-induce-metrics-on-dual-tensor-and-exterior-bundles](https://alphabetamath.cc/item/prop-riemannian-metrics-induce-metrics-on-dual-tensor-and-exterior-bundles) [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps) [math:prop-chain-rule-for-smooth-half-space-maps](https://alphabetamath.cc/item/prop-chain-rule-for-smooth-half-space-maps) [math:thm-ftc-second-part](https://alphabetamath.cc/item/thm-ftc-second-part)

[A1] Work in ZFC, including the Axiom of Choice inherited from the smoothing supplier and sufficient for the chart supplier's Countable Choice assumption. Its use is the approximation in step 3.1 and the weak-differential calculus there. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The hypotheses and conventions in the Statement.

**Goal:** Construct the smooth approximants with exact fixed boundary values and both stated convergences.

1.1 Write $O_-$ and $O_+$ for the open neighborhoods where $u$ has the two prescribed constant values. The set $V=O_+\setminus B_-$ is open and contains the compact set $B_+$. By [F1], take a smooth $\chi_+:R\to[0,1]$ supported in $V$ and equal to one on an open neighborhood $U_+$ of $B_+$, shrinking $U_+$ inside $O_+$. Put $U_-=O_-\setminus\operatorname{supp}\chi_+$; this is an open neighborhood of $B_-$. Set $h=c_-+(c_+-c_-)\chi_+$. Then $h$ is smooth up to the boundary, equals $c_-$ on $U_-$ and $c_+$ on $U_+$, and $v=u-h$ vanishes on $U_-\cup U_+$. [given, F1, F5, construct]

2.1 The smooth dual metric and compactness give a finite $M\ge1$ with $|dh|_k\le M$ on $R$; for empty $R$ take $M=1$. For any piecewise $C^1$ curve $\gamma$ joining $p$ to $q$, refine into finitely many chart pieces. The half-space chain rule, using smooth local extensions also when a piece touches the boundary, gives $|(h\circ\gamma)'|=|dh(\dot\gamma)|\le M|\dot\gamma|_k$. The scalar fundamental theorem on each piece and the triangle inequality therefore give $|h(p)-h(q)|\le M L_k(\gamma)$. Taking the infimum over curves gives $|h(p)-h(q)|\le M d_k(p,q)$ on each component. Distinct components impose no finite-distance constraint. Thus $h$ is Lipschitz under the convention in the Statement, and if $u$ has Lipschitz bound $L$, then $v=u-h$ has bound $L+M$. Its support is closed in compact $R$ and disjoint from the open neighborhood $U_-\cup U_+$ of all of $\partial R$, hence is compactly contained in $R^\circ$. [given, F1, F5, F6, step 1.1, algebra]

3.1 Apply [F2], under [A1], to the Lipschitz $v$ from step 2.1, obtaining smooth $v_j$ supported in a single compact $K\subset R^\circ$, with uniform error tending to zero and $\int_R(|v_j-v|+|dv_j-dv|_k)\,dV_k\to0$. Define $u_j=h+v_j$. On the fixed open neighborhoods $U_-\setminus K$ and $U_+\setminus K$ of the respective boundary parts, every $u_j$ has the exact prescribed constant. Weak differentiation is linear: the coordinate test identities add, so $du_j-du=dv_j-dv$ almost everywhere, while $u_j-u=v_j-v$ pointwise. Thus the uniform errors and the displayed Sobolev errors are exactly those of $v_j-v$ and tend to zero. The sum is smooth up to the boundary because $h$ is, and $v_j$ vanishes near it. The conventions of [F4] include dimension zero and the empty case, completing all assertions. [F2, F4, F5, A1, step 1.1, step 2.1, algebra] ∎
