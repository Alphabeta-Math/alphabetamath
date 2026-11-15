---
title: Stationary graph translation preserves source asymptotics
status: draft
research_item: lem-author-9e5789a3d617-graph-decay-translation
dependency_level: 1
---

## Prerequisites

- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:def-codimension-and-hypersurface](https://alphabetamath.cc/item/def-codimension-and-hypersurface)
- [math:thm-mean-value-inequality](https://alphabetamath.cc/item/thm-mean-value-inequality)
- [math:thm-logarithm-slower-than-every-positive-power](https://alphabetamath.cc/item/thm-logarithm-slower-than-every-positive-power)


## Statement

Let $k$ be a nonnegative integer, $R_0>0$, $E=\{x\in\mathbb R^3:r=|x|>R_0\}$, and $u\in C^{k+1}(E;\mathbb R)$. In a stationary end chart $V\subseteq\mathbb R\times E$, suppose $\Gamma_u=\{(u(x),x):x\in E\}\subseteq V$ is a hypersurface graph. Write $\mathcal D\subseteq\mathbb R\times M$ for the domain of the stationary flow $\phi$, with coordinate law $\phi_a(t,x)=(t+a,x)$ whenever the flow is defined and both points lie in $V$. Fix $s\in\mathbb R$ such that $(s,p)\in\mathcal D$ and $\phi_s(p)\in V$ for every $p\in\Gamma_u$. Then $\phi_s(\Gamma_u)$ is the graph $t=u(x)+s$ over the same $E$.

If $0<\alpha\leq1$ and $|u|+\sum_{j=1}^{k+1}r^j|\partial^j u|\leq Cw_\alpha(r)$ on $E$, where $C\geq0$ is finite, $w_\alpha(r)=(1+r)^{1-\alpha}$ for $\alpha<1$ and $w_1(r)=1+\log(1+r)$, then the fixed translate obeys the same bound with $C+|s|$ in place of $C$. Here $\partial^j u$ denotes the finite array of order-$j$ Cartesian derivatives, with its Euclidean norm. For $1\leq j\leq k+1$ and $0<\lambda\leq1$, any additionally imposed finite weighted Hölder bound on $\partial^j u$ is unchanged: on every annulus $A_R=\{R<|x|<2R\}\subseteq E$, the seminorm $[v]_{\lambda;A_R}=\sup_{x\ne y\in A_R}|v(x)-v(y)|/|x-y|^\lambda$ is identical for $v=\partial^j(u+s)$ and $v=\partial^j u$. Finiteness of the relevant Hölder seminorms is an additional hypothesis, not a consequence of the stated $C^{k+1}$ regularity. These source-type bounds do not force $u\to0$ or even convergence to a finite constant.

## Facts & Assumptions

[F1] Chart derivative bounds and weighted Hölder estimates have their fixed-coordinate meaning. The formula in the Statement also specifies the endpoint exponent $\lambda=1$. [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F2] A local flow has a domain $\mathcal D$; the translation law and the conditions that the chosen $s$ is defined on all of $\Gamma_u$ and its image remains in $V$ are explicit hypotheses here, not consequences of the flow definition. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F3] A hypersurface is an embedded submanifold of codimension one; $\Gamma_u$ is assumed to be such a hypersurface in the chart. [math:def-codimension-and-hypersurface](https://alphabetamath.cc/item/def-codimension-and-hypersurface)

[F4] If $f:[a,b]\to\mathbb R^m$ is continuous on $[a,b]$, differentiable on $(a,b)$, $a<b$, and $|f'(t)|\leq M$ there for a finite $M\geq0$, then $|f(b)-f(a)|\leq M(b-a)$. [math:thm-mean-value-inequality](https://alphabetamath.cc/item/thm-mean-value-inequality)

[F5] For every $\varepsilon>0$, $\log t/t^\varepsilon\to0$ as $t\to+\infty$. [math:thm-logarithm-slower-than-every-positive-power](https://alphabetamath.cc/item/thm-logarithm-slower-than-every-positive-power)

## Proof

**Given:** The chart, graph, flow-domain conditions, regularity and estimates in the Statement.

**Goal:** Establish graph translation, preservation of the estimates and the absence of forced finite limiting height.

1.1 For every $x\in E$, the domain and containment hypotheses permit use of the coordinate law at $(u(x),x)$, giving $\phi_s(u(x),x)=(u(x)+s,x)$. As $x$ ranges over $E$, these are exactly the points of the translated graph. All derivatives of positive order through $k+1$ remain the same, and $|u+s|\leq|u|+|s|$. Since $w_\alpha\geq1$, replacing $C$ by $C+|s|$ proves the claimed bound, while derivative Hölder differences, their seminorms and any fixed radius weights are identical. [F1, F2]

2.1 On $E=\{r>1\}$, the smooth function $u(x)=\log r$ is unbounded, but $r^j|\partial^j u|$ is bounded for every fixed $j\geq1$: the first derivatives are homogeneous of degree $-1$, further differentiation lowers that degree, and their angular factors are smooth on the unit sphere. Also $|u|\leq w_1(r)\leq C_\alpha w_\alpha(r)$ for $\alpha<1$: apply [F5] with $\varepsilon=1-\alpha>0$ and $t=1+r$. Choose $T\geq2$ so that $\log t\leq t^\varepsilon$ for $t\geq T$. There $1+\log t\leq2t^\varepsilon$; for $2<t\leq T$, $1+\log t\leq1+\log T\leq(1+\log T)t^\varepsilon$. Thus $C_\alpha=\max\{2,1+\log T\}$ suffices. For completeness, if $v=\partial^j u$ and $x,y\in A_R$ with $|x-y|\leq R/2$, the connecting segment stays at radius at least $R/2$. For distinct $x,y$, the finite derivative array $f(t)=v(x+t(y-x))$, $0\leq t\leq1$, is smooth and has $|f'(t)|\leq C_jR^{-j-1}|x-y|$ by the next-derivative bound. Applying [F4] on $[0,1]$ gives $|v(x)-v(y)|\leq C_jR^{-j-1}|x-y|$; for $x=y$ the inequality is immediate. If $|x-y|>R/2$, the individual derivative bounds give $|v(x)-v(y)|\leq C_jR^{-j}$. Consequently $[\partial^j u]_{\lambda;A_R}\leq C_{j,\lambda}R^{-j-\lambda}$ for $0<\lambda\leq1$ and $R\geq2$. This supplies the corresponding weighted Hölder control, including that at the highest derivative order. Thus the displayed growth class does not imply zero height or a finite limiting height; this is a statement about the estimate, not a spacetime counterexample. [F1, F4, F5, step 1.1] ∎
