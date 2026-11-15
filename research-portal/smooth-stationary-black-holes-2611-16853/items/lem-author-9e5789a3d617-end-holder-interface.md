---
id: lem-author-9e5789a3d617-end-holder-interface
title: Differentiated stationary end bounds imply the weighted Hölder interface
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-stationary-asymptotic-decay-data
  - math:thm-mean-value-inequality
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  math:thm-mean-value-inequality: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Fix a stationary chart with $X=\partial_t$ on $r=|x|>R$, metric components $g_{\mu\nu}=\eta_{\mu\nu}+O_{k+1}(r^{-\alpha})$, $k\geq2$, $0<\alpha\leq1$, and Minkowski matrix $\eta=\operatorname{diag}(-1,1,1,1)$. Here the asymptotic coefficient of $X$ means the constant $A$ in an expansion $X=(A+a)\partial_t+\sum_{i=1}^3 b^i\partial_{x^i}$ with $a,b^i=O_0(r^{-\alpha})$. Then after increasing $R$, $g_{00}<-1/2$, $g_{ij}v^iv^j\geq|v|^2/2$, $X$ is uniformly timelike and its asymptotic coefficient is $A=1$. Moreover for any $0<\lambda\leq1$, every order-$k$ coordinate derivative $q$ of a metric component satisfies $|q(t,x)-q(\tau,y)|\leq C r^{-\alpha-k-\lambda}(|t-\tau|^\lambda+|x-y|^\lambda)$ when $|x-y|\leq r/2$ and $|t-\tau|\leq1$, where $r=|x|$. These are the local quantitative end inequalities; end gluing and global causality remain separate conditions.

## Facts & Assumptions

[F1] Stationary fields, charts and metric components have the specified geometric meanings. [[def-stationary-lorentzian-data]]

[F2] Differentiated decay controls Cartesian derivatives uniformly in angle. [[def-stationary-asymptotic-decay-data]]

[F3] If $f:[a,b]\to\mathbb R$ is continuous on $[a,b]$, differentiable on $(a,b)$, $a<b$, and $|f'|\leq M$ there for a finite $M\geq0$, then $|f(b)-f(a)|\leq M(b-a)$. [[math:thm-mean-value-inequality]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated quantitative end inequalities and coefficient.

1.1 Fix a common radius $R_1$ beyond which the differentiated decay bounds hold, and increase the final $R$ so that $R>2R_1$ and every component of $g-\eta$ has absolute value at most $1/6$ for $r>R$. Then $g_{00}\leq-5/6<-1/2$ and $|\sum_{ij}(g_{ij}-\delta_{ij})v^iv^j|\leq\tfrac16(\sum_i|v^i|)^2\leq|v|^2/2$. Thus $g_{ij}v^iv^j\geq|v|^2/2$. Since $X=\partial_t$, its squared norm is $g_{00}$, so it is uniformly timelike. [given, F1, F2]

1.2 The local flow of $X=\partial_t$ translates $t$ and fixes $x$. Its preservation of $g$ makes the metric components independent of $t$; hence derivatives containing a time derivative vanish, and purely spatial derivatives are independent of $t$. The identity $X=\partial_t$ gives the defined expansion with $A=1$ and $a=b^i=0$. In any such expansion, its time component gives $1-A=a=O_0(r^{-\alpha})$; since $\alpha>0$, the right side tends to zero as $r\to\infty$, so the constant $A$ is uniquely $1$. [given, F1, F2]

2.1 Let $q$ be a purely spatial order-$k$ derivative of a metric component. Join $x$ to $y$ by changing their three coordinates one at a time. Every point $z$ on these coordinate segments satisfies $|z-x|\leq|y-x|\leq r/2$, so $|z|\geq r/2>R_1$. The next differentiated bound gives $|\partial_iq(z)|\leq C r^{-\alpha-k-1}$ on all three segments. On each nondegenerate coordinate interval the restriction of $q$ is $C^1$, and its one-variable derivative is the corresponding partial derivative. Apply [F3] on that interval; zero-length intervals contribute zero. Telescoping the three differences yields $|q(x)-q(y)|\leq C r^{-\alpha-k-1}\sum_{i=1}^3|y^i-x^i|\leq\sqrt3 C r^{-\alpha-k-1}|x-y|$. [given, F2, F3, step 1.1]

3.1 If $x\ne y$, then for $0<\lambda\leq1$ one has $|x-y|^{1-\lambda}\leq(r/2)^{1-\lambda}$, and the preceding bound is at most $C' r^{-\alpha-k-\lambda}|x-y|^\lambda$. For $x=y$ the difference is zero. Purely spatial derivatives have no time dependence, and derivatives containing a time derivative are zero. Adding the nonnegative term $C' r^{-\alpha-k-\lambda}|t-\tau|^\lambda$ therefore gives the claimed estimate for every order-$k$ coordinate derivative when $|t-\tau|\leq1$. [given, step 1.2, step 2.1] ∎
