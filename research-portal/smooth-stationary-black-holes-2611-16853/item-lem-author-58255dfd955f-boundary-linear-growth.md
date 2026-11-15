---
title: Hopf positivity and uniform linear growth on a fixed compact collar
status: draft
research_item: lem-author-58255dfd955f-boundary-linear-growth
dependency_level: 3
---

## Prerequisites

- [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data)
- [lem-author-58255dfd955f-annular-hopf-barrier](item-lem-author-58255dfd955f-annular-hopf-barrier)
- [math:thm-collar-neighborhood-theorem](https://alphabetamath.cc/item/thm-collar-neighborhood-theorem)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps)
- [math:lem-closed-interval-compactness-from-completeness](https://alphabetamath.cc/item/lem-closed-interval-compactness-from-completeness)
- [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces)
- [math:lem-mean-value-theorem-on-closed-interval](https://alphabetamath.cc/item/lem-mean-value-theorem-on-closed-interval)
- [math:lem-continuous-functions-riemann-integrable](https://alphabetamath.cc/item/lem-continuous-functions-riemann-integrable)
- [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)


## Statement

Let $S$ be a nonempty compact smooth boundary of a smooth Riemannian exterior. Suppose $u\in C^2(\Sigma^\circ)\cap C^1_{\mathrm{loc}}(\Sigma)$ is positive inside, vanishes on $S$, and satisfies $(\Delta_h-V)u\le0$ with smooth $V\ge0$. Then $\partial_{\nu_{\mathrm{in}}}u>0$ at every point of $S$, where $\nu_{\mathrm{in}}$ is the metric unit inward normal. On some fixed compact collar, $u\ge c_0\rho$ with $c_0>0$, for the collar coordinate $\rho$ or the metric distance to $S$.

## Facts & Assumptions

[F1] Smooth boundary, the Riemannian metric and the Laplacian convention are those of [def-exterior-weighted-elliptic-data](item-def-exterior-weighted-elliptic-data). The inward unit normal is the vector orthogonal to $T_yS$, of $h$-norm one, pointing into $\Sigma$. The regularity $C^1_{\mathrm{loc}}(\Sigma)$ includes continuous first derivatives up to the boundary in boundary charts.

[F2] The tangent-ball derivative conclusion is supplied by [lem-author-58255dfd955f-annular-hopf-barrier](item-lem-author-58255dfd955f-annular-hopf-barrier). Smoothness of the metric and potential on a sufficiently small closed chart ball gives its coefficient bounds and uniform ellipticity.

[F3] Work in ZFC, including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) and the choice assumptions inherited through the barrier supplier. In particular the Countable Choice hypothesis of [math:thm-collar-neighborhood-theorem](https://alphabetamath.cc/item/thm-collar-neighborhood-theorem) holds. Fix its smooth collar $F:S\times[0,\epsilon)\to\Sigma$, a smooth embedding onto a relatively open neighbourhood of $S$ with $F(y,0)=y$. Its coordinate is $\rho(F(y,t))=t$. The vector $\partial_tF(y,0)$ is strictly inward and transverse, since $F$ is a collar embedding.

[F4] A continuous real function on a nonempty compact space attains its minimum and maximum, and a continuous image of a compact space is compact, by [math:thm-compactness-under-continuous-maps](https://alphabetamath.cc/item/thm-compactness-under-continuous-maps). The interval $[0,\delta]$ is compact for $\delta>0$ by [math:lem-closed-interval-compactness-from-completeness](https://alphabetamath.cc/item/lem-closed-interval-compactness-from-completeness), and its product with compact $S$ is compact by [math:thm-finite-products-of-compact-spaces](https://alphabetamath.cc/item/thm-finite-products-of-compact-spaces). Compactness also means that every open cover has a finite subcover; the common collar width will be obtained by that property directly.

[F5] The closed-interval mean value theorem [math:lem-mean-value-theorem-on-closed-interval](https://alphabetamath.cc/item/lem-mean-value-theorem-on-closed-interval) applies to a real function continuous on $[a,b]$ and differentiable on $(a,b)$. The supplier [math:lem-continuous-functions-riemann-integrable](https://alphabetamath.cc/item/lem-continuous-functions-riemann-integrable) defines the Riemann integral of continuous real functions on compact intervals, proves its interval additivity, and gives $m(b-a)\le\int_a^b g(s)\,ds\le M(b-a)$ whenever $m\le g\le M$ and $a<b$. These are used over the real numbers with the complete ordered-field structure of [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field).

[F6] For the distance formulation, curves are continuous maps $\gamma:[a,b]\to\Sigma$ that are $C^1$ on each piece of a finite subdivision $a=t_0<\cdots<t_N=b$, up to the piece endpoints in interior or boundary charts; endpoint derivatives are one-sided. They are allowed to lie on or meet $S$. Define $L_h(\gamma)=\sum_{j=1}^N\int_{t_{j-1}}^{t_j}\sqrt{h_{\gamma(s)}(\dot\gamma(s),\dot\gamma(s))}\,ds$. Each speed is continuous on its closed piece, so [F5] makes the length finite and nonnegative. At a subdivision point each adjacent piece uses its own one-sided derivative. Interval additivity gives invariance under refinement, and a common refinement gives independence of subdivision. For $a=b$, set $L_h(\gamma)=0$. Define $d_h(x,S)$ to be the infimum of $L_h(\gamma)$ over all these curves starting at any point of $S$ and ending at $x$, with $\inf\varnothing=+\infty$. A nonempty family of lengths has an infimum in $[0,\infty)$ by the completeness axiom in [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field), applied to the negatives of the nonnegative lengths. Thus this distance-to-subset construction applies to manifolds with boundary and disconnected exteriors, including components not joined to $S$; finiteness on the collar will follow from its explicit curves.

## Proof

**Given:** The hypotheses in the Statement and the data and suppliers in [F1]–[F6].

**Goal:** Establish the conclusions of the Statement.

**Proof technique:** direct.

1.1 In a boundary chart flatten the smooth boundary to a coordinate plane. A sufficiently small Euclidean ball in the half-space is tangent at the chosen boundary point and has closure in the chart. Apply [F2] to obtain a positive inward transverse derivative. All tangential derivatives vanish because $u|_S=0$. Its differential is therefore a positive multiple of the inward conormal, proving the strict positivity for the metric unit inward normal as well as for every smooth strictly inward transverse vector. [F1, F2, given]

2.1 Put $B(y,t)=\partial_t(u\circ F)(y,t)$ and $a(y)=B(y,0)$. These functions are continuous up to $t=0$, and $a(y)>0$ by step 1.1 and [F3]. Since $S$ is nonempty and compact, [F4] gives $a_*:=\min_Sa>0$. Fix $0<b<\epsilon$. For each $y\in S$, continuity of $B$ gives an open neighbourhood $U_y\subset S$ and a width $0<\eta_y<b$ such that $B(z,t)>a_*/2$ for $z\in U_y$ and $0\le t<\eta_y$. A finite subcover $U_{y_1},\ldots,U_{y_m}$ of $S$ exists by compactness. Choose $0<\delta<\min_i\eta_{y_i}$. Every $z\in S$ then lies in one of these sets, so $B(z,t)\ge a_*/2$ for all $0\le t\le\delta$. This proves the common width directly. [F3, F4, step 1.1, given, choose]

3.1 By [F4], $S\times[0,\delta]$ is compact and its continuous image $K_\delta:=F(S\times[0,\delta])$ is a compact collar. The speed $q(y,t):=\sqrt{h_{F(y,t)}(\partial_tF(y,t),\partial_tF(y,t))}$ is continuous there by smoothness of $h$ and $F$. Its maximum exists by [F4]; put $C:=\max(1,\max_{S\times[0,\delta]}q)$. Thus $0\le q\le C$ and $C\ge1$. [F1, F3, F4, step 2.1, construct]

3.2 For fixed $y$ and $0<t\le\delta$, the function $s\mapsto u(F(y,s))$ is continuous on $[0,t]$ and differentiable on $(0,t)$ with derivative $B(y,s)$. By [F5] there is $\theta\in(0,t)$ with $u(F(y,t))-u(F(y,0))=tB(y,\theta)\ge a_*t/2$. Since $u(F(y,0))=0$, this proves $u(F(y,t))\ge a_*t/2$; the same inequality holds at $t=0$. The closed-interval hypotheses include the boundary endpoint, so this argument uses exactly the stated regularity. [F3, F5, step 2.1, given]

4.1 For $x=F(y,t)$, $0\le t\le\delta$, the curve $s\mapsto F(y,s)$ on $[0,t]$ starts at $y\in S$, ends at $x$, and stays in $\Sigma$. Its length, as defined in [F6], is $\int_0^t q(y,s)\,ds\le Ct$ by [F5] and step 3.1. Hence $0\le d_h(x,S)\le Ct<\infty$. Combining this with step 3.2 yields $u(x)\ge (a_*/2C)d_h(x,S)$. With $c_0=a_*/(2C)>0$, the same constant also gives $u(x)\ge c_0\rho(x)$, since $C\ge1$ and $\rho(x)=t$. The constants depend on the actual solution and collar; no uniform family bound follows solely from pointwise Hopf positivity. [F3, F5, F6, step 3.1, step 3.2, algebra] ∎
