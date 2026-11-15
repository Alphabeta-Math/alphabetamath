---
title: A variable-coefficient annular barrier and inward boundary derivative
status: published
research_item: lem-author-58255dfd955f-annular-hopf-barrier
dependency_level: 2
---

## Prerequisites

- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)
- [lem-author-58255dfd955f-coordinate-schrodinger-form](item-lem-author-58255dfd955f-coordinate-schrodinger-form)
- [lem-author-58255dfd955f-compact-comparison](item-lem-author-58255dfd955f-compact-comparison)
- [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)
- [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)
- [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary)
- [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary)


## Statement

Let $L=\Delta_h-V=a^{ij}\partial_{ij}+b^i\partial_i-V$ be the geometric operator on a relatively compact smooth metric chart, with symmetric uniformly elliptic $a$, bounded $a,b,V$, and $V\ge0$. Let $B_R(z)$ be an interior tangent Euclidean ball at $p$, with its closure in the chart. Suppose $u>0$ in the ball, $u\ge0$ on its closure, $u(p)=0$, $Lu\le0$, and $u$ is $C^2$ inside and $C^1$ at $p$. Then the derivative in direction $(z-p)/R$ at $p$ is strictly positive. This applies to the geometric operator from the coordinate-form lemma.

## Facts & Assumptions

[F1] The smooth metric $h$ is Riemannian in the sense of [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold). The symbol $\Delta_h$ uses the positive-divergence, metric-trace-of-Hessian convention of [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian). For the general metric-chart argument, use the differential expression $\Delta_h=a^{ij}\partial_{ij}+b^i\partial_i$ and coefficient bounds assumed in the Statement. For the smooth-exterior application, [lem-author-58255dfd955f-coordinate-schrodinger-form](item-lem-author-58255dfd955f-coordinate-schrodinger-form) supplies this differential expression for its smooth metric. Subtracting a bounded potential is a pointwise zeroth-order operation; no smoothness of the original $V$ is used below. For this application use the smooth metric on the closed ball, so the stated coefficient bounds and ellipticity hold. Fix $\lambda>0$ with $a^{ij}\xi_i\xi_j\ge\lambda|\xi|^2$, and bounds $\operatorname{tr}a\le T$, $|b|\le B$ and $0\le V\le Q$, where $Q\ge0$ is a constant.

[F2] The supplier [lem-author-58255dfd955f-compact-comparison](item-lem-author-58255dfd955f-compact-comparison) gives comparison for $\Delta_h-W$ on relatively compact smooth domains when $W\ge0$ is smooth and bounded and the difference belongs to $C^2(D)\cap C^1(\overline D)$, with each component closure meeting the boundary. In its stated ZFC setting, $(\Delta_h-W)w\ge0$ and $w\le0$ on the boundary imply $w\le0$ inside. We use this supplier only with the smooth constant $W=Q$ and annuli whose closed outer spheres lie strictly inside $B_R(z)$.

[F3] For every integer $n\ge1$, [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn), part 2, says that a subset of Euclidean $\mathbb R^n$ is compact if and only if it is closed and bounded. We use the Euclidean subspace metric on coordinate spheres and closed annuli. A compact coordinate set is also compact in the manifold: a manifold open cover pulls back under the inverse chart to an open cover of that coordinate set, and a finite subcover transfers back.

[F4] By [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric), a continuous real function on a nonempty compact metric space attains a minimum and a maximum. If it is strictly positive everywhere, its attained minimum is strictly positive.

[F5] Use the half-space chart and smooth-transition conventions of [math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary](https://alphabetamath.cc/item/def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary). By [math:def-embedded-smooth-submanifold-with-boundary](https://alphabetamath.cc/item/def-embedded-smooth-submanifold-with-boundary), an embedded smooth submanifold with boundary is a subset with a manifold-with-boundary smooth structure for which inclusion is a smooth embedding. Step 1.2 constructs these charts and the embedding for the closed annulus; no smooth-domain assertion is imported from the comparison theorem.

## Proof

**Given:** The hypotheses in the Statement and the suppliers and bounds in [F1]–[F5].

**Goal:** Prove that the inward derivative at $p$ is strictly positive.

**Proof technique:** direct.

1.1 Put $L_Q=\Delta_h-Q$. Positivity of $u$ inside the ball gives $L_Qu=Lu-(Q-V)u\le0$. Choose $\alpha>0$ so large that $\alpha^2\lambda R^2-2\alpha T-2\alpha BR-Q\ge0$; this is possible because $\lambda R^2>0$. This choice is independent of the truncated outer radius used below. [F1, given, algebra, choose]

1.2 For $R/2<s<R$, let $r=|x-z|$ and $D_s=\{R/2<r<s\}$. Write $n$ for the chart dimension. Since $|p-z|=R>0$, $n\ge1$. The sets $S_{R/2}=\{|x-z|=R/2\}$ and $N_s=\{R/2\le|x-z|\le s\}$ are closed and bounded in $\mathbb R^n$, hence compact by [F3], and lie inside $B_R(z)$. The sphere is nonempty, containing $z+(R/2)e_1$, where $e_1$ is the first coordinate unit vector. The radial inequalities show that $N_s=\overline{D_s}$ and $N_s\setminus D_s$ consists exactly of the spheres of radii $R/2$ and $s$. Here is an explicit smooth boundary chart near a point $y$ of either sphere. Write its radius as $r_0$ and choose $j$ with $y_j-z_j\ne0$. Set $\sigma=\operatorname{sign}(y_j-z_j)$ and use coordinates $(\widehat x_j,t)$, where $\widehat x_j$ lists all coordinates other than $x_j$, with $t=r-r_0$ on the inner sphere and $t=r_0-r$ on the outer sphere. With $\eta=1$ in the inner case and $\eta=-1$ in the outer case, the inverse is $x_j=z_j+\sigma\sqrt{(r_0+\eta t)^2-\sum_{i\ne j}(x_i-z_i)^2}$, retaining the other coordinates. Near $y$ the radicand is positive and the other radial inequality is strict, so these maps are mutually inverse smooth extensions on open Euclidean neighborhoods, and $N_s$ corresponds exactly to $t\ge0$. Along with ordinary charts in $D_s$, they form compatible half-space charts as in [F5]. The inclusion has the subspace topology and in each chart extends to a local Euclidean diffeomorphism, hence is a smooth embedding. Thus $N_s$ is a compact smooth full-dimensional closure with intrinsic boundary exactly those two spheres. Finally, for any $x$ in a component $C$ of $D_s$, the radial path $z+\tau(x-z)/|x-z|$, $|x-z|\le\tau<s$, lies in $D_s$ and in the same component as $x$; its limit at $\tau=s$ lies in $\overline C\cap\partial D_s$. This also covers $n=1$, when the annulus has two interval components and the boundary-chart list $\widehat x_j$ is empty. All these sets lie in the chart interior, so the same smooth-domain and component-boundary assertions hold on the manifold. [F3, F5, given, construct, algebra]

2.1 For any $R/2<s<R$, on $D_s=\{R/2<r=|x-z|<s\}$ set $\psi_s=e^{-\alpha r^2}-e^{-\alpha s^2}$. Direct differentiation in the coordinates from [F1] gives $L_Q\psi_s=e^{-\alpha r^2}(4\alpha^2a^{ij}(x-z)_i(x-z)_j-2\alpha\operatorname{tr}a-2\alpha b\cdot(x-z)-Q)+Qe^{-\alpha s^2}$. Since $r\ge R/2$ and $r\le R$, the parenthesis is at least $\alpha^2\lambda R^2-2\alpha T-2\alpha BR-Q$. Thus $L_Q\psi_s\ge0$ for every such $s$. [F1, step 1.1, algebra]

3.1 By step 1.2 the sphere $r=R/2$ is nonempty and compactly contained in the ball. The $C^2$ regularity of $u$ there gives continuity, so [F4] and strict positivity give an attained minimum $\mu=\min_{r=R/2}u>0$. Put $M=e^{-\alpha R^2/4}>0$ and fix $\epsilon=\mu/(2M)>0$, independently of $s$. On the inner sphere $0\le\psi_s\le M$, hence $\epsilon\psi_s\le u$; on the outer sphere $r=s$, $\psi_s=0<u$. The closed annulus lies inside the open ball, where $u$ is $C^2$, so $w_s=\epsilon\psi_s-u$ belongs to $C^2(D_s)\cap C^1(\overline D_s)$. Step 1.2 supplies its smooth relatively compact closure and proves that every component closure meets its boundary. Moreover $L_Qw_s\ge0$ by steps 1.1 and 2.1. Apply [F2] with constant potential $Q$ to conclude $u\ge\epsilon\psi_s$ throughout $D_s$. This application uses neither regularity on $r=R$ nor smoothness of $V$. [F2, F4, step 1.1, step 2.1, step 1.2, given, algebra, choose]

4.1 Fix $x$ with $R/2<|x-z|<R$. The comparison in step 3.1 holds for every $s\in(|x-z|,R)$, so taking $s\uparrow R$ yields $u(x)\ge\epsilon\psi_R(x)$, where $\psi_R(x)=e^{-\alpha|x-z|^2}-e^{-\alpha R^2}$. Let $v=(z-p)/R$. For $0<t<R/2$, the point $p+tv$ has radius $R-t$ and lies in this annulus. Since $u(p)=\psi_R(p)=0$, division by $t$ gives $(u(p+tv)-u(p))/t\ge\epsilon(e^{-\alpha(R-t)^2}-e^{-\alpha R^2})/t$. The assumed $C^1$ regularity at $p$ gives the left-hand limit $\partial_vu(p)$, and the right-hand limit is $2\epsilon\alpha R e^{-\alpha R^2}>0$. This proves the asserted inward derivative bound with exactly the stated regularity. [step 3.1, given, algebra] ∎
