---
title: Differential exclusion of a large interior weighted angle maximum
status: published
research_item: lem-author-fd2999663761-cutoff-interior-maximum-exclusion
dependency_level: 4
---

## Prerequisites

- [def-author-fd2999663761-temporal-angle-data](item-def-author-fd2999663761-temporal-angle-data)
- [lem-author-fd2999663761-temporal-tangent-gradient](item-lem-author-fd2999663761-temporal-tangent-gradient)
- [lem-author-fd2999663761-logarithmic-angle-conversion](item-lem-author-fd2999663761-logarithmic-angle-conversion)
- [math:lem-negative-semidefinite-hessian-at-an-interior-local-maximum](https://alphabetamath.cc/item/lem-negative-semidefinite-hessian-at-an-interior-local-maximum)
- [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas)
- [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)
- [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules)
- [math:thm-logarithm-derivative-and-integral](https://alphabetamath.cc/item/thm-logarithm-derivative-and-integral)
- [math:def-real-power](https://alphabetamath.cc/item/def-real-power)
- [math:def-natural-logarithm](https://alphabetamath.cc/item/def-natural-logarithm)
- [math:thm-natural-logarithm-laws](https://alphabetamath.cc/item/thm-natural-logarithm-laws)


## Statement

For the temporal angle data, suppose $\alpha\ge a_0>0$. On $\{\tau>0,v>2\}$ assume $\Delta_\Sigma\log v\ge\tfrac14|\nabla_\Sigma\log v|^2-Cv^2$ and $|\Delta_\Sigma\tau|\le Cv^2$ with $C\ge1$. If $T>0$, choose $\mu>4$ so that $(\mu^2/4-\mu)a_0^2\ge2C(T^2+\mu T)$. Then $\tau^\mu v$ has no local maximum in the interior positive-height region where $v>2$. The logarithmic inequality may be obtained from the hyperbolic-angle inequality by the conversion lemma.

## Facts & Assumptions

[F1] The tangential gradient identity gives $|\nabla_\Sigma\tau|^2\ge a_0^2(v^2-1)$. [lem-author-fd2999663761-temporal-tangent-gradient](item-lem-author-fd2999663761-temporal-tangent-gradient)

[F2] The operators and height bound $\tau\le T$ are those in [def-author-fd2999663761-temporal-angle-data](item-def-author-fd2999663761-temporal-angle-data); the conversion from $\eta=\operatorname{arcosh}v$ to $\log v$ is [lem-author-fd2999663761-logarithmic-angle-conversion](item-lem-author-fd2999663761-logarithmic-angle-conversion). The two differential inequalities are assumptions of this lemma.

[F3] In an open Euclidean coordinate domain, a $C^2$ function at an interior local maximum has zero differential and a negative semidefinite matrix of second partial derivatives. [math:lem-negative-semidefinite-hessian-at-an-interior-local-maximum](https://alphabetamath.cc/item/lem-negative-semidefinite-hessian-at-an-interior-local-maximum) The metric-dual gradient and coordinate identity $(\operatorname{Hess}_h f)_{ij}=\partial_i\partial_j f-\Gamma^k{}_{ij}\partial_k f$ are [math:prop-gradient-hessian-and-divergence-connection-formulas](https://alphabetamath.cc/item/prop-gradient-hessian-and-divergence-connection-formulas). The positive-trace convention is $\Delta_\Sigma f=\operatorname{tr}_h\operatorname{Hess}_h f$. [math:def-laplace-beltrami-operator-as-trace-of-the-hessian](https://alphabetamath.cc/item/def-laplace-beltrami-operator-as-trace-of-the-hessian)

[F4] Apply the scalar sum, product, quotient and chain rules in each coordinate. [math:lem-derivative-algebra-and-chain-rules](https://alphabetamath.cc/item/lem-derivative-algebra-and-chain-rules) For $s>0$, $(\log s)^{\prime}=1/s$ and $\log s=\int_1^s dt/t$, so the logarithm is smooth and strictly increasing there. [math:thm-logarithm-derivative-and-integral](https://alphabetamath.cc/item/thm-logarithm-derivative-and-integral)

[F5] For $a>0$ and $r\in\mathbb R$, define $a^r=\exp(r\log a)$ as in [math:def-real-power](https://alphabetamath.cc/item/def-real-power). The exponential maps $\mathbb R$ into $(0,\infty)$ and $\log(\exp s)=s$ for every real $s$, as recorded in [math:def-natural-logarithm](https://alphabetamath.cc/item/def-natural-logarithm); hence $a^r>0$ and $\log(a^r)=r\log a$. For $x,y>0$, $\log(xy)=\log x+\log y$ by [math:thm-natural-logarithm-laws](https://alphabetamath.cc/item/thm-natural-logarithm-laws).

## Proof

**Given:** The displayed bounds and choice of $\mu$. **Goal:** Exclude an interior local maximum with $v>2$.

1.1 Suppose $p$ is an interior local maximum of $\tau^\mu v$ with $\tau(p)>0$ and $v(p)>2$. In a neighborhood with these strict inequalities put $f=\log v+\mu\log\tau$. By [F5], $\tau^\mu>0$ and $f=\log(\tau^\mu v)$ there. By [F4], $f$ is smooth and has a local maximum at $p$. Apply the Euclidean extremum test in [F3] to its coordinate representation in an interior chart: $df(p)=0$ and the matrix $(\partial_i\partial_j f)(p)$ is negative semidefinite. The connection term in the coordinate Hessian formula vanishes because $df(p)=0$. Thus $\operatorname{Hess}_h f(p)$ is negative semidefinite, $\nabla_\Sigma f(p)=0$, and $\Delta_\Sigma f(p)=\sum_{a=1}^3\operatorname{Hess}_h f(e_a,e_a)\le0$ for an $h_p$-orthonormal basis $(e_a)$. [F2, F3, F4, F5, given, algebra]

2.1 By the coordinate scalar rules and the Hessian and trace formulas in [F3] and [F4], $\nabla_\Sigma\log\tau=\nabla_\Sigma\tau/\tau$ and $\Delta_\Sigma\log\tau=\Delta_\Sigma\tau/\tau-|\nabla_\Sigma\tau|^2/\tau^2$. At $p$, step 1.1 therefore gives $\nabla_\Sigma\log v=-\mu\nabla_\Sigma\tau/\tau$. Substituting this into the assumed inequalities gives $0\ge\Delta_\Sigma f\ge(\mu^2/4-\mu)|\nabla_\Sigma\tau|^2/\tau^2-Cv^2(1+\mu/\tau)$. [F2, F3, F4, step 1.1, given, algebra]

3.1 Multiply by $\tau^2>0$ and use [F1]. Put $A=T^2+\mu T>0$. The lower bound from step 2.1 is at least $2CA(v^2-1)-C(\tau^2+\mu\tau)v^2\ge CA(v^2-2)>0$, since $0<\tau\le T$ and $v>2$. This contradicts $\Delta f\le0$. Such a $\mu$ exists because the left side of its required inequality is quadratic in $\mu$ and the right side is affine. [F1, F2, step 1.1, step 2.1, algebra] ∎
