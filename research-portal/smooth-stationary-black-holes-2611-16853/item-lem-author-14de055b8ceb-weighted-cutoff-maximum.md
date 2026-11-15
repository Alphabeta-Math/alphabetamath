---
title: Weighted cutoff maximum gives a uniform normal angle
status: published
research_item: lem-author-14de055b8ceb-weighted-cutoff-maximum
dependency_level: 4
---

## Prerequisites

- [math:def-smooth-collar-of-a-manifold-boundary](https://alphabetamath.cc/item/def-smooth-collar-of-a-manifold-boundary)
- [lem-author-14de055b8ceb-gaussian-cutoff-projection](item-lem-author-14de055b8ceb-gaussian-cutoff-projection)
- [lem-author-56ff511785bf-full-range-log-angle](item-lem-author-56ff511785bf-full-range-log-angle)
- [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold)
- [math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function)
- [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)
- [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)
- [math:lem-negative-semidefinite-hessian-at-an-interior-local-maximum](https://alphabetamath.cc/item/lem-negative-semidefinite-hessian-at-an-interior-local-maximum)


## Statement

Let $N$ be a smooth manifold with nonempty compact boundary $S$, and let $c:S\times[0,\varepsilon)\to N$ be a supplied smooth boundary collar: $c$ is a smooth embedding, $c(s,0)=s$, and its image is an open neighborhood of $S$ in $N$. Choose $0<\ell<\varepsilon$, put $K=c(S\times[0,\ell])$, and supply a smooth real function $u$ on $K$, smooth up to its boundary. The compact smooth graph collar in this lemma is $M=\{(x,u(x)):x\in K\}$, identified with $K$ by graph projection. Identify its inner boundary, the graph over $c(S\times\{0\})$, with $S$; its artificial outer edge is the graph over $c(S\times\{\ell\})$. Let $h$ be a smooth Riemannian metric on $M$, smooth up to the boundary. Use its gradient $\nabla=\operatorname{grad}_h$, squared norm $|\cdot|_h^2$ and positive-divergence Laplace–Beltrami operator $\Delta=\operatorname{tr}_h\operatorname{Hess}_h$. Suppose $v\ge1$ is smooth up to the boundary, $\Delta\log v\ge\tfrac14|\nabla\log v|_h^2-Cv^2$, and $v\le B_0$ on $S$. Let $\chi$ be continuous on $M$ and smooth on $\{\chi>0\}$, with the following assumed cutoff properties: $0\le\chi\le1$, $\chi=1$ on $S$, $\chi=0$ on the outer edge, and on $\chi>0$ the bounds $|\nabla\chi|_h^2\ge av^2-b$ and $|\Delta\chi|\le Cv^2$. Here $a>0$, $b\ge0$ and $C\ge0$ are fixed constants; one common $C$ may be obtained by enlarging the constants in the two differential estimates. Then some integer $m>4$, determined only by these constants, satisfies $\sup_{\chi\ge1/2}v\le2^m\max\{B_0,1,\sqrt{2b/a}\}$. No uniform candidate second-derivative estimate is assumed.

## Statement references

[math:def-smooth-collar-of-a-manifold-boundary](https://alphabetamath.cc/item/def-smooth-collar-of-a-manifold-boundary)

## Facts & Assumptions

[F1] The cutoff value, regularity, gradient and Laplacian properties in the Statement are assumptions of this lemma. For geometric applications, [lem-author-14de055b8ceb-gaussian-cutoff-projection](item-lem-author-14de055b8ceb-gaussian-cutoff-projection) supplies these properties under its own hypotheses: a smooth Gaussian tube with compact closure, smooth reference-boundary distance, a smooth spacelike maximal graph in the prescribed cone, the stated tube shrinking and cutoff-width restrictions.

[F2] The logarithmic angle inequality in the Statement is an assumption of this lemma. For geometric applications, [lem-author-56ff511785bf-full-range-log-angle](item-lem-author-56ff511785bf-full-range-log-angle) supplies it for a smooth spacelike maximal hypersurface and a smooth future unit timelike field with the stated uniform observer-metric bounds on its first two covariant derivatives and the ambient Ricci tensor. Compactness here is only that of the chosen closed graph collar with its fixed outer edge.

[F3] The metric is positive definite, including at a smooth boundary, as in [math:def-riemannian-metric-and-riemannian-manifold](https://alphabetamath.cc/item/def-riemannian-metric-and-riemannian-manifold). The gradient is characterized by $h(\nabla f,X)=df(X)$ as in [math:def-riemannian-gradient-of-a-smooth-function](https://alphabetamath.cc/item/def-riemannian-gradient-of-a-smooth-function), and $\Delta f$ is the metric trace of the Levi–Civita Hessian with the positive-divergence sign convention in [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian).

[F4] The Hessian formulas $\operatorname{Hess}_h f(X,Y)=X(Yf)-(\nabla^h_XY)f$ and $(\operatorname{Hess}_h f)_{ij}=\partial_i\partial_jf-\Gamma^k{}_{ij}\partial_kf$ are [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas).

[F5] A continuous real-valued function on a nonempty compact space attains its maximum, by claim 2 of [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps).

[F6] At an interior local maximum of a $C^2$ function on a Euclidean open set, its first derivatives vanish and its Euclidean Hessian is negative semidefinite. [math:lem-negative-semidefinite-hessian-at-an-interior-local-maximum](https://alphabetamath.cc/item/lem-negative-semidefinite-hessian-at-an-interior-local-maximum) The conversion to the metric trace on the collar is given below.

## Proof

**Given:** The compact collar, Riemannian metric, regularity and inequalities in the Statement. **Goal:** Bound the angle on the positive inner part without a uniform candidate second-derivative estimate.

1.1 For any integer $m>4$, $W=\chi^mv$ is continuous on the nonempty compact collar, so [F5] gives a point $p$ where it attains its maximum. On the outer edge $W=0$, and on $S$ it is at most $B_0$. If its maximum is zero the desired bound is immediate. Otherwise, if $p$ is interior, $\chi(p)>0$ and $F=\log W=\log v+m\log\chi$ is smooth in a neighborhood of $p$ and has a local maximum there. Thus no differentiation across $\chi=0$ is needed. [F1, F5, given]

2.1 At that interior positive maximum choose a smooth interior coordinate chart. Apply [F6] to the coordinate representative of $F$ to get $\partial_iF(p)=0$ and a negative semidefinite matrix $(\partial_i\partial_jF)(p)$. By [F4], the Christoffel term vanishes at $p$, so the intrinsic Hessian has that same quadratic form. Its value on each $h$-unit basis vector is nonpositive; tracing as in [F3] gives $\Delta F(p)\le0$. Also [F3] gives $\nabla F(p)=0$, hence $\nabla\log v=-m\nabla\chi/\chi$ at $p$. [F3, F4, F6, step 1.1, algebra]

3.1 For a positive smooth scalar $u$, [F3] and [F4] give $\nabla\log u=u^{-1}\nabla u$ and $\operatorname{Hess}_h\log u=u^{-1}\operatorname{Hess}_h u-u^{-2}du\otimes du$ by differentiating $\log u$ twice. Taking the metric trace gives $\Delta\log u=(\Delta u)/u-|\nabla u|_h^2/u^2$. Apply this identity to $\chi$ near $p$, and insert the assumed logarithmic angle inequality and $\Delta\chi\ge-Cv^2$. With step 2.1 this yields $0\ge\Delta F\ge(m^2/4-m)|\nabla\chi|_h^2/\chi^2-Cv^2(1+m/\chi)$ at $p$. [F1, F2, F3, F4, step 2.1, given, algebra]

4.1 Put $V_0=\max\{1,\sqrt{2b/a}\}$, which is real by $a>0$ and $b\ge0$. If an interior positive maximum has $v(p)>V_0$, then $|\nabla\chi|_h^2\ge av^2-b\ge(a/2)v^2$. Since $m>4$, the coefficient $m^2/4-m$ is positive. Multiplying step 3.1 by $\chi^2/v^2$ and using $0<\chi\le1$ and $C\ge0$ gives $0\ge(a/2)(m^2/4-m)-C(\chi^2+m\chi)\ge(a/2)(m^2/4-m)-C(1+m)$. Choose an integer $m>\max\{8,32C/a\}$. Then $m^2/4-m\ge m^2/8$ and $(a/2)(m^2/4-m)-C(1+m)\ge am^2/16-C(1+m)>0$, a contradiction. This choice depends only on the stated constants. [F1, step 3.1, given, choose, algebra]

5.1 For that fixed $m$, a positive maximum therefore either lies on $S$, where $W\le B_0$, or is interior with $v(p)\le V_0$, where $W(p)\le V_0$ since $\chi\le1$. The zero-maximum case also obeys $\sup_M W\le\max\{B_0,V_0\}$. On $\chi\ge1/2$, division by $\chi^m\ge2^{-m}$ now gives the stated bound. Only individual smoothness at a positive maximum was used, so no uniform candidate second-derivative estimate was assumed. [step 1.1, step 4.1, given, algebra] ∎
