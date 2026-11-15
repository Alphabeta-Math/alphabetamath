---
title: Strong minimum principle from the annular barrier
status: draft
research_item: lem-author-58255dfd955f-strong-minimum
dependency_level: 3
---

## Prerequisites

- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)
- [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)
- [math:thm-connectedness-characterisations](https://alphabetamath.cc/item/thm-connectedness-characterisations)
- [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn)
- [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric)
- [lem-author-58255dfd955f-annular-hopf-barrier](item-lem-author-58255dfd955f-annular-hopf-barrier)


## Statement

On a connected smooth Riemannian interior, let $V\ge0$ be locally bounded and smooth. A nonnegative $C^2$ function satisfying $(\Delta_h-V)u\le0$ is either strictly positive everywhere or identically zero.

## Facts & Assumptions

[F1] The interior, denoted by $M$, has the smooth positive-definite metric of [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold). Work in interior charts; all closed coordinate balls used below are compactly contained in such a chart.

[F2] Use the positive-divergence sign convention and metric trace of the Hessian from [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian). For smooth functions the coordinate Hessian is $(\operatorname{Hess}f)_{ij}=\partial_{ij}f-\Gamma^k{}_{ij}\partial_kf$ by [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas). For $C^2$ functions use the same pointwise trace; step 1.1 justifies this extension and its coordinate expression. Repeated indices are summed.

[F3] A connected space has no nonempty proper clopen subset by [math:thm-connectedness-characterisations](https://alphabetamath.cc/item/thm-connectedness-characterisations), part 1(b). Continuity of $u$ makes $P=\{u>0\}$ open and $Z=\{u=0\}$ closed; nonnegativity gives $M=P\cup Z$.

[F4] The general metric-chart interface of [lem-author-58255dfd955f-annular-hopf-barrier](item-lem-author-58255dfd955f-annular-hopf-barrier) gives a strictly positive inward derivative at a zero on an interior tangent Euclidean ball when $u>0$ inside, $u\ge0$ on the closure, $Lu\le0$, and $u$ is $C^2$ inside and $C^1$ at the tangency point, for $L=\Delta_h-V$ with bounded coefficients and uniformly elliptic principal part on that chart and $V\ge0$.

[F5] For Euclidean dimension $m\ge1$, [math:thm-heine-borel-rn](https://alphabetamath.cc/item/thm-heine-borel-rn), part 2, identifies compact subsets of $\mathbb R^m$ with closed bounded subsets. We apply it in dimensions $n$ and $2n$ only after disposing of dimension zero.

[F6] By [math:thm-extreme-value-metric](https://alphabetamath.cc/item/thm-extreme-value-metric), a continuous real-valued function on a nonempty compact metric space is bounded and attains its minimum and maximum. In particular, a strictly positive continuous function on such a space has a strictly positive attained minimum.

## Proof

**Given:** The hypotheses in the Statement and the mathematical inputs [F1]–[F6].

**Goal:** Establish the stated alternative without restricting the Riemannian interior to an exterior.

**Proof technique:** direct.

1.1 If $M$ is empty the alternative is vacuous. If $n=\dim M=0$, each chart is a singleton open set because $\mathbb R^0$ is a singleton; hence $M$ is discrete. Every singleton is then clopen, so connectedness and [F3] force a nonempty $M$ to be a singleton. The alternative follows from nonnegativity at its sole point. In the remaining argument $n\ge1$. At any point $x_0$ of an interior chart, replace $u$ by its quadratic Taylor polynomial with the same value, first derivatives and second derivatives at $x_0$. The smooth Hessian formula in [F2] uses only these data and the metric connection coefficients at $x_0$. Under a smooth change of coordinates, the chain rule transforms the derivatives through order two using only these same data, so the Hessian coefficients defined for $u$ transform as those of the polynomial, hence as a bilinear tensor at $x_0$. This proves that their metric trace is well-defined for $u\in C^2$ and gives $\Delta_hu=h^{ij}\partial_{ij}u-h^{ij}\Gamma^k{}_{ij}\partial_ku$. Thus $a^{ij}=h^{ij}$ and $b^k=-h^{ij}\Gamma^k{}_{ij}$ are smooth on the chart. For any nonempty compact chart subset $K$, its coordinate image is closed and bounded by [F5]. Thus $K\times\{\xi\in\mathbb R^n:|\xi|=1\}$, in coordinates, is a nonempty closed bounded subset of $\mathbb R^{2n}$ and is compact by [F5]. The continuous strictly positive function $(x,\xi)\mapsto h^{ij}(x)\xi_i\xi_j$ has a strictly positive attained minimum there by [F6]. Scaling $\xi$ gives uniform ellipticity on $K$. Applying [F6] on $K$ to the absolute values of each of the finitely many smooth coefficients and of $V$ gives finite coefficient and potential bounds. For empty $K$ these bounds are vacuous. These are exactly the metric-chart coefficient conditions in [F4]. [F1, F2, F3, F4, F5, F6, given, algebra]

1.2 Suppose $P$ and $Z$ are both nonempty. If $\overline P\cap Z$ were empty, then $\overline P\subseteq P$, so the open set $P$ would also be closed. It would be a nonempty proper clopen subset of the connected space $M$, contradicting [F3]. Consequently choose $q\in\overline P\cap Z$. [F3, given, choose]

2.1 Center coordinates at $q$ and choose $\rho>0$ such that the closed Euclidean ball $\overline B_{2\rho}(0)$ is contained in the chart image. Choose $z\in P$ with $|z|<\rho/4$, which is possible since $q\in\overline P$. The set $E=Z\cap\overline B_\rho(0)$ in these coordinates contains $0$ and is closed and bounded in $\mathbb R^n$: it is the zero set of the continuous coordinate function $u$ restricted to the closed ball, which lies in the chart. Thus $E$ is nonempty and compact by [F5]. The continuous function $x\mapsto|x-z|$ on $E$ attains its minimum $R$ at some $p\in E$ by [F6]. Since $p\in Z$ and $z\notin Z$, $R=|p-z|>0$; since $0\in E$, $R\le|z|<\rho/4$. Thus $\overline B_R(z)\subset B_{\rho/2}(0)$, and its open ball contains no point of $Z$, so it lies in $P$. Its closure lies in the interior chart and $p$ is a zero on its sphere. [F1, F3, F5, F6, step 1.2, choose]

3.1 On this ball, step 1.1 verifies the operator hypotheses of [F4]. All its function hypotheses hold because $u$ is nonnegative and $C^2$ throughout the interior, positive in the ball by step 2.1, zero at $p$, and satisfies $(\Delta_h-V)u\le0$. The barrier therefore gives $\partial_vu(p)>0$ for $v=(z-p)/R$. But $p$ is an interior minimum of $u$, so the differentiable function $g(t)=u(p+tv)$ has a minimum at $0$ for both signs of small $t$. For $t>0$ its difference quotient $(g(t)-g(0))/t$ is nonnegative, and for $t<0$ it is nonpositive. Both one-sided limits equal $g'(0)$ by differentiability, so $g'(0)\ge0$ and $g'(0)\le0$, hence $\partial_vu(p)=g'(0)=0$. The contradiction excludes simultaneous nonempty $P,Z$. If $P$ is empty then $u\equiv0$; if $Z$ is empty then $u>0$ everywhere. These alternatives also cover the empty interior. [F4, step 1.1, step 2.1, given] ∎
