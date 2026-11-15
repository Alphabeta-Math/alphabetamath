---
title: A complete stationary flow preserves its compact tangent boundary
status: published
research_item: lem-author-9e5789a3d617-compact-boundary-flow
dependency_level: 1
---

## Prerequisites

- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart)
- [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)
- [math:def-integral-curve-of-a-vector-field](https://alphabetamath.cc/item/def-integral-curve-of-a-vector-field)
- [math:prop-a-vector-field-tangent-to-an-embedded-submanifold-restricts-to-a-vector-field](https://alphabetamath.cc/item/prop-a-vector-field-tangent-to-an-embedded-submanifold-restricts-to-a-vector-field)
- [math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves](https://alphabetamath.cc/item/thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves)
- [math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)


## Statement

Let $X$ have a complete smooth flow $\phi_t$ on $M$, and let $S\subset M$ be a compact embedded submanifold without boundary with $X_p\in T_pS$ for every $p\in S$. Then $\phi_t(S)=S$ for every real $t$. This requires tangency, not vanishing of $X$ on $S$, and does not assert that $S$ is a Killing bifurcation surface.

## Facts & Assumptions

[F1] A global flow has integral curves through each initial point and satisfies $\phi_0=\operatorname{id}$ and $\phi_t\circ\phi_s=\phi_{t+s}$; hence $\phi_{-t}$ is its inverse. An integral curve solves $\gamma\prime(t)=X_{\gamma(t)}$. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:def-integral-curve-of-a-vector-field](https://alphabetamath.cc/item/def-integral-curve-of-a-vector-field)

[F2] A stationary field is a smooth Killing field; its completeness is an additional hypothesis. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)

[F3] An embedded submanifold has slice charts and the subspace topology. Compactness of $S$ means that every cover by open subsets of $S$ has a finite subcover. [math:def-embedded-submanifold-and-slice-chart](https://alphabetamath.cc/item/def-embedded-submanifold-and-slice-chart) [math:def-compact-space](https://alphabetamath.cc/item/def-compact-space)

[F4] A smooth ambient vector field tangent to an embedded submanifold restricts to a smooth vector field on that submanifold. [math:prop-a-vector-field-tangent-to-an-embedded-submanifold-restricts-to-a-vector-field](https://alphabetamath.cc/item/prop-a-vector-field-tangent-to-an-embedded-submanifold-restricts-to-a-vector-field)

[F5] For a smooth vector field on a manifold, every point has an open neighborhood $U$ and a number $h>0$ with a smooth solution map on $(-h,h)\times U$, giving the unique integral curve for each initial point in $U$. [math:thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves](https://alphabetamath.cc/item/thm-local-existence-uniqueness-and-smooth-dependence-for-manifold-integral-curves)

[F6] Through each point of a manifold, a smooth vector field has a unique maximal integral curve. [math:thm-unique-maximal-integral-curve-through-each-point](https://alphabetamath.cc/item/thm-unique-maximal-integral-curve-through-each-point)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Prove $\phi_t(S)=S$ for every real $t$.

1.1 If $S$ is empty the conclusion holds immediately. Otherwise tangency and [F4] give a smooth vector field $Y=X|_S$ on the boundaryless manifold $S$. By [F5], the open subsets of $S$ admitting a solution map on some interval $(-h,h)$ form an open cover of $S$. Use intrinsic compactness in [F3] to take a finite subcover $U_1,\ldots,U_N$, with corresponding maps $\Psi_j:(-h_j,h_j)\times U_j\to S$ and $h_j>0$, and put $h=\min_j h_j>0$. Every point of $S$ therefore has a solution for $Y$ on $(-h,h)$. [given, F3, F4, F5]

2.1 Fix $p\in S$ and let $\gamma:(a,b)\to S$ be its maximal integral curve for $Y$, with $\gamma(0)=p$, supplied by [F6]. If $b<\infty$, choose $t_0\in(a,b)$ with $b-t_0<h$ and a $U_j$ containing $\gamma(t_0)$. The curve $t\mapsto\Psi_j(t-t_0,\gamma(t_0))$ is defined on $(t_0-h_j,t_0+h_j)$ and agrees with $\gamma$ on the overlap by uniqueness in [F5], applied at their common time $t_0$. Gluing extends $\gamma$ beyond $b$, contradicting maximality. If $a>-\infty$, choose $t_0$ with $t_0-a<h$ and use the same map for negative time to extend past $a$. Thus $a=-\infty$ and $b=\infty$. [F5, F6, step 1.1]

3.1 Viewed in $M$, each such restricted curve solves the ambient equation: in a slice chart its tangential derivatives are the components of $Y$, while its normal coordinates are zero, and tangency makes these derivatives exactly the components of $X$. It is therefore an ambient integral curve through $p$ by [F1]. Ambient uniqueness in [F5] and [F6] identifies it with $t\mapsto\phi_t(p)$ for every real $t$. Hence $\phi_t(S)\subseteq S$. Applying the same inclusion to $-t$ and using the inverse identity in [F1] gives $S\subseteq\phi_t(S)$, and consequently $\phi_t(S)=S$. [given, F1, F3, F4, F5, F6, step 2.1] ∎
