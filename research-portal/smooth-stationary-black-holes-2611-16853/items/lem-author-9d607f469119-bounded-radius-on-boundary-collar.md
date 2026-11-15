---
id: lem-author-9d607f469119-bounded-radius-on-boundary-collar
title: The radius of a graph section is bounded on a compact boundary collar
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - math:thm-collar-neighborhood-theorem
  - math:def-axiom-of-choice
  - math:def-riemannian-distance-on-a-connected-manifold
  - math:thm-the-riemannian-distance-topology-is-the-manifold-topology
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds
  - math:def-differential-of-a-smooth-real-valued-function
  - math:def-the-standard-smooth-step-function
  - math:thm-chain-rule-for-differentials-of-smooth-maps
  - math:def-riemannian-speed-and-length
  - math:lem-continuous-functions-riemann-integrable
  - math:lem-riemann-integral-linearity
  - math:thm-newton-leibniz-with-interior-derivative
  - math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary
  - math:def-smooth-collar-of-a-manifold-boundary
dependency_roles:
  math:thm-collar-neighborhood-theorem: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:def-riemannian-distance-on-a-connected-manifold: mathematical-premise
  math:thm-the-riemannian-distance-topology-is-the-manifold-topology: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds: mathematical-premise
  math:def-differential-of-a-smooth-real-valued-function: mathematical-premise
  math:def-the-standard-smooth-step-function: mathematical-premise
  math:thm-chain-rule-for-differentials-of-smooth-maps: mathematical-premise
  math:def-riemannian-speed-and-length: mathematical-premise
  math:lem-continuous-functions-riemann-integrable: mathematical-premise
  math:lem-riemann-integral-linearity: mathematical-premise
  math:thm-newton-leibniz-with-interior-derivative: mathematical-premise
  math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary: mathematical-premise
  math:def-smooth-collar-of-a-manifold-boundary: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $\Sigma$ be a connected smooth Riemannian manifold with compact boundary $S$, with smooth positive metric $h$ up to $S$. Suppose a diffeomorphism $G:\{x\in\mathbb R^3:|x|>1\}\to\Sigma^\circ$ supplies the interior graph parameterization. Write $r(G(x))=|x|$. Assume $|dr|_h$ is bounded on $\{r\ge R_e\}$ for some $R_e>1$. Then every fixed compact smooth boundary collar $W\cong S\times[0,a]$ has bounded $r$ on $W\setminus S$. No continuous extension of the graph height or of $G^{-1}$ to $S$ is assumed.

## Facts & Assumptions

[F1] A smooth compact boundary admits a smooth collar; work in ZFC, hence with countable choice. [[math:thm-collar-neighborhood-theorem]] [[math:def-axiom-of-choice]] A compact boundary collar is a restriction of a smooth collar embedding to $S\times[0,a]$ within its parameter domain. [[math:def-smooth-collar-of-a-manifold-boundary]]

[F2] Riemannian distance is defined by lengths of piecewise smooth paths, and induces the manifold topology. [[math:def-riemannian-distance-on-a-connected-manifold]] [[math:thm-the-riemannian-distance-topology-is-the-manifold-topology]]

[F3] A Riemannian metric is a smooth positive-definite tensor, with boundaries allowed where stated; a diffeomorphism has a smooth inverse; and the differential of a smooth real-valued function satisfies $df_p(v)=v([f])$. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds]] [[math:def-differential-of-a-smooth-real-valued-function]] The smooth structure at the boundary is a maximal compatible atlas of half-space charts, with transition maps smooth in the local-extension sense. [[math:def-smooth-chart-atlas-and-structure-on-a-manifold-with-boundary]]

[F4] The standard smooth step function $\sigma:\mathbb R\to[0,1]$ is smooth, vanishes on $(-\infty,0]$, and equals one on $[1,\infty)$. [[math:def-the-standard-smooth-step-function]]

[F5] Differentials of smooth compositions obey the chain rule. For a covector $\alpha$, write $|\alpha|_h=\sup_{|v|_h=1}|\alpha(v)|$; thus $|\alpha(v)|\le|\alpha|_h|v|_h$. The Riemannian speed is $|\dot\gamma|_h=\sqrt{h(\dot\gamma,\dot\gamma)}$, and length is the sum of its integrals over the smooth pieces. [[math:thm-chain-rule-for-differentials-of-smooth-maps]] [[math:def-riemannian-speed-and-length]]

[F6] Continuous real functions on a compact interval are Riemann integrable; the integral is monotone, additive over intervals, and linear in continuous integrands. If a scalar function is continuous on the closed interval, differentiable inside, and its derivative has a Riemann-integrable extension, Newton–Leibniz identifies its endpoint difference with that integral. [[math:lem-continuous-functions-riemann-integrable]] [[math:lem-riemann-integral-linearity]] [[math:thm-newton-leibniz-with-interior-derivative]]

## Proof

**Given:**The hypotheses in the Statement.

**Goal:** Establish the stated conclusion.

1.1 With the standard step function of F4, put $\varphi(t)=R_e+(t-R_e)\sigma(t-R_e)$ and $f=\varphi\circ r$ on $\Sigma^\circ$. Then $\varphi$ is smooth, constant for $t\le R_e$, and equal to $t$ for $t\ge R_e+1$. Its derivative $\varphi'(t)=\sigma(t-R_e)+(t-R_e)\sigma'(t-R_e)$ is bounded, since $\sigma'$ vanishes outside $[0,1]$ and is continuous on that compact interval. By the chain rule, $df=\varphi'(r)dr$. Its norm is bounded on the far end by the hypothesis, zero near $r=1$, and bounded on the transition annulus because $G(\{R_e\le|x|\le R_e+1\})$ is compact in $\Sigma^\circ$ and $h$ is smooth and positive there. Thus $|df|_h\le L$ throughout $\Sigma^\circ$ for some finite $L\ge0$. [given, F3, F4, F5]

2.1 Let $\gamma$ be a piecewise smooth interior path from $y$ to $z$. On each smooth piece with parameter interval $[a,b]$, the chain rule and the covector norm give $|(f\circ\gamma)'(t)|=|df_{\gamma(t)}(\dot\gamma(t))|\le L|\dot\gamma(t)|_h$. Both derivative and speed are continuous on the closed piece, so F6 applies. Newton–Leibniz, monotonicity, and linearity give $-L\int_a^b|\dot\gamma|_h\,dt\le f(\gamma(b))-f(\gamma(a))\le L\int_a^b|\dot\gamma|_h\,dt$. Taking absolute values, summing the finitely many endpoint increments, and using the length definition yields $|f(y)-f(z)|\le L\operatorname{length}_h(\gamma)$. [F3, F5, F6, step 1.1]

3.1 On the fixed collar, smoothness and compactness bound the lengths of collar-coordinate segments from $(s,u)$ to $(s,a)$. On the compact connected outer collar face, paths from a fixed point to its other points have uniformly bounded lengths, using finitely many coordinate charts (for multiple boundary components use one fixed point on each, finitely many since $S$ is compact). Concatenating gives a uniform finite path-length bound to a finite collection of fixed interior points for every collar point with $u>0$. Step 2.1 then bounds $f$ there, and hence bounds $r$ since $f=r$ at large $r$. This uses only smooth collar geometry, not boundary extension of stationary graph coordinates. [F1, F2, F3, F5, step 2.1] ∎
