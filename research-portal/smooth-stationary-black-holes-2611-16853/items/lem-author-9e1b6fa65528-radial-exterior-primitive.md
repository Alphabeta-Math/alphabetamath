---
id: lem-author-9e1b6fa65528-radial-exterior-primitive
title: Radial primitive and five differentiated decay bounds
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-asymptotic-decay-data
  - physics:def-cm-finite-regularity-canonical-calculus
  - math:def-improper-integral-at-infinity
  - math:thm-differentiation-under-dominated-improper-multiple-integrals
  - math:thm-extreme-value-metric
  - math:thm-heine-cantor-metric
  - math:thm-newton-leibniz-with-interior-derivative
  - math:thm-comparison-test-for-improper-integrals
  - math:lem-derivative-algebra-and-chain-rules
  - math:thm-continuous-partial-derivatives-imply-total-differentiability
  - math:thm-chain-rule-for-total-derivatives
dependency_roles:
  def-stationary-asymptotic-decay-data: mathematical-premise
  physics:def-cm-finite-regularity-canonical-calculus: mathematical-premise
  math:def-improper-integral-at-infinity: mathematical-premise
  math:thm-differentiation-under-dominated-improper-multiple-integrals: mathematical-premise
  math:thm-extreme-value-metric: mathematical-premise
  math:thm-heine-cantor-metric: mathematical-premise
  math:thm-newton-leibniz-with-interior-derivative: mathematical-premise
  math:thm-comparison-test-for-improper-integrals: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
  math:thm-continuous-partial-derivatives-imply-total-differentiability: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Let $B=\tfrac12B_{ij}\,dx^i\wedge dx^j$ be a closed $C^5$ two-form on $\{|x|>R\}\subset\mathbb R^3$, with $R>0$ and $B_{ij}=O_5(r^{-4})$, $r=|x|$, in the differentiated convention. Define $A_i(x)=-\int_1^\infty sx^jB_{ji}(sx)\,ds$ and $A=A_i\,dx^i$, with repeated spatial indices summed. Then $A$ is $C^5$, $dA=B$, $x^iA_i=0$, and $A_i=O_5(r^{-3})$. If the same differentiated estimates hold at every finite order, the same formula is smooth. The finite-order hypothesis alone is used only for the $C^5$ conclusion.

## Statement references

[[def-stationary-asymptotic-decay-data]]

[[physics:def-cm-finite-regularity-canonical-calculus]]

[[math:def-improper-integral-at-infinity]]

## Facts & Assumptions

[F1] The differentiated convention $B_{ij}=O_5(r^{-4})$ supplies a radius $R_1>R$ and constants $C_\beta$ such that $|\partial^\beta B_{ij}(y)|\leq C_\beta|y|^{-4-|\beta|}$ for $|\beta|\leq5$ and $|y|\geq R_1$. It imposes no bound as $|y|$ decreases to $R$. [[def-stationary-asymptotic-decay-data]]

[F2] A $C^k$ coordinate form has $C^k$ alternating coefficient functions; the exterior derivative is defined by differentiating coefficients and wedging the corresponding coordinate covector. Here closed means $dB=0$, equivalently $\partial_iB_{jk}+\partial_jB_{ki}+\partial_kB_{ij}=0$. These conventions apply on any open Euclidean set, including this three-dimensional exterior. [[physics:def-cm-finite-regularity-canonical-calculus]]

[F3] Every integral from $1$ to $\infty$ below denotes the limit of its proper integrals from $1$ to $L$ as $L\to\infty$, when that limit is finite. [[math:def-improper-integral-at-infinity]]

[F4] For an open integration domain and one real parameter in an open interval, a continuous integrand with a continuous parameter derivative, an absolutely integrable base slice, and an integrable bound for the derivative uniform on each compact parameter interval has a continuously differentiable integral, with derivative equal to the derivative integral. [[math:thm-differentiation-under-dominated-improper-multiple-integrals]]

[F5] Continuous real functions on nonempty compact metric spaces are bounded; continuous maps on compact metric spaces are uniformly continuous. [[math:thm-extreme-value-metric]] [[math:thm-heine-cantor-metric]]

[F6] For a function continuous on a closed interval and differentiable inside, a Riemann-integrable extension of its derivative integrates to its endpoint difference. [[math:thm-newton-leibniz-with-interior-derivative]]

[F7] A locally Riemann-integrable function dominated in absolute value eventually by a function with a convergent improper integral is absolutely improperly integrable. [[math:thm-comparison-test-for-improper-integrals]]

[F8] For real functions differentiable at a point, sums and products are differentiable there with the sum and product rules. A composition is differentiable when the inner function is differentiable there and the outer function is differentiable at its value, with derivative given by the chain rule. For integers $m\geq1$, $(t^m)'=mt^{m-1}$. [[math:lem-derivative-algebra-and-chain-rules]]

[F9] A Euclidean map whose partial derivatives exist on a neighborhood and are continuous at a point is totally differentiable there with its Jacobian as derivative. For composable maps totally differentiable at the relevant points, $D(g\circ f)(a)=Dg(f(a))\circ Df(a)$. [[math:thm-continuous-partial-derivatives-imply-total-differentiability]] [[math:thm-chain-rule-for-total-derivatives]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated construction and identities.

1.1 Put $E=\{x:|x|>R\}$ and $h_i(s,x)=sx^jB_{ji}(sx)$. For fixed $s\geq1$, fixing the other two coordinates makes $x^\ell\mapsto B_{ji}(sx)$ a composition of the corresponding one-variable coordinate slice of $B_{ji}$ with $x^\ell\mapsto sx^\ell$. The slice is $C^5$ and the inner map is affine, so [F8] applies successively through five coordinate derivatives, with one factor $s$ per chain-rule differentiation. The product rule also differentiates the factor $x^j$ at most once. Thus, for $|\beta|=k\leq5$, these rules express $\partial_x^\beta h_i$ as a sum of terms of the forms $s^{k+1}x^j(\partial^\beta B_{ji})(sx)$ and, when $k\geq1$, constant multiples of $s^k(\partial^{\beta-e_\ell}B_{\ell i})(sx)$ with $\beta_\ell>0$. Thus, whenever $sr\geq R_1$, each sum is bounded by $C_k r^{-3-k}s^{-3}$. Let $K\subset E$ be nonempty and compact, let $a=\min_K|x|>R$, and choose $S>1$ with $Sa\geq R_1$. On $K\times[1,S]$ the same derivatives are continuous and hence bounded. Enlarging a constant to absorb this finite interval gives $|\partial_x^\beta h_i(s,x)|\leq C_{K,\beta}s^{-3}$ for all $s\geq1$ and $x\in K$. This is a local uniform majorant, not a bound uniform up to the inner boundary. [given, F1, F2, F5, F8]

2.1 Since $\int_1^L s^{-3}\,ds=(1-L^{-2})/2$, the majorant in step 1.1 is integrable. Comparison gives absolute convergence of every integral of $\partial_x^\beta h_i$ for $|\beta|\leq5$. These integrals are jointly continuous in $x$: on a compact neighborhood $K$ the tails beyond $L$ are bounded uniformly by $C_{K,\beta}/(2L^2)$, while the integral over $[1,L]$ is continuous by uniform continuity of its integrand on $K\times[1,L]$ and the estimate of an integral by interval length times the uniform bound. Choose an open rectangular neighborhood with compact closure $K\subset E$. For each $|\beta|\leq4$, fix the other two coordinates and apply [F4] to $\partial_x^\beta h_i$ with each remaining coordinate as the real parameter and integration domain $(1,\infty)$. The integrand and its parameter derivative are continuous, every base slice is absolutely integrable, and step 1.1 supplies an integrable derivative bound on every compact parameter interval. The endpoint $s=1$ is regular and has no effect on the integral. Successively applying this argument gives $\partial_x^\beta A_i(x)=-\int_1^\infty\partial_x^\beta h_i(s,x)\,ds$ for every $|\beta|\leq5$; their joint continuity proves $A\in C^5(E)$. [F3, F4, F5, F6, F7, step 1.1]

3.1 For $r\geq R_1$ the asymptotic estimate in step 1.1 holds for every $s\geq1$, so $|\partial_x^\beta A_i(x)|\leq C_k r^{-3-k}\int_1^\infty s^{-3}\,ds=(C_k/2)r^{-3-k}$. Hence $A_i=O_5(r^{-3})$ in exactly the convention of [F1]. If the hypotheses hold at every finite order, repeat steps 1.1 and 2.1 at each such order, with constants and radii allowed to depend on the order; this yields smoothness of the same integral without an all-order conclusion from the finite-order hypothesis alone. [F1, step 1.1, step 2.1]

4.1 Closedness and antisymmetry give $\partial_iB_{kj}-\partial_jB_{ki}=\partial_kB_{ij}$. The first derivative formula from step 2.1 therefore yields $\partial_iA_j-\partial_jA_i=-\int_1^\infty[2sB_{ij}(sx)+s^2x^k\partial_kB_{ij}(sx)]\,ds$. For fixed $x\in E$, the ray $\gamma_x(s)=sx$ lies in $E$ on the open interval $(R/r,\infty)$ containing $[1,L]$. Its derivative is the vector $x$. The $C^5$ coefficients of $B$ have continuous first partial derivatives, so [F9] makes them totally differentiable and gives $\frac{d}{ds}B_{ij}(sx)=x^k\partial_kB_{ij}(sx)$. The product and power rules in [F8] now identify the integrand as the continuous derivative of the $C^1$ function $s\mapsto s^2B_{ij}(sx)$. On $[1,L]$, [F6] evaluates its integral as $L^2B_{ij}(Lx)-B_{ij}(x)$. The first term tends to zero by [F1], since it is $O(L^{-2}r^{-4})$ as $L\to\infty$ for fixed $x$. Passing to the improper limit gives $\partial_iA_j-\partial_jA_i=B_{ij}(x)$, which is $dA=B$ by [F2]. Finally $x^iA_i=-\int_1^\infty s x^ix^jB_{ji}(sx)\,ds=0$ by antisymmetry and convergence. [F1, F2, F3, F6, F8, F9, step 2.1] ∎
