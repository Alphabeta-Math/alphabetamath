---
id: lem-author-d20d145f998f-stationary-product-cauchy-time
title: Stationary product time is a Cauchy temporal coordinate
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-killing-field
  - physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets
  - math:def-local-and-global-flow
  - physics:def-gr-causal-curves-and-reachability
  - physics:lem-gr-causal-curve-calculus
  - math:def-countable-choice
  - math:def-dependent-choice
  - math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions
  - math:thm-nonnegative-integral-zero-iff-zero-almost-everywhere
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-killing-field: mathematical-premise
  physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets: mathematical-premise
  math:def-local-and-global-flow: mathematical-premise
  physics:def-gr-causal-curves-and-reachability: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-dependent-choice: mathematical-premise
  math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions: mathematical-premise
  math:thm-nonnegative-integral-zero-iff-zero-almost-everywhere: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Assume the Axioms of Countable Choice and Dependent Choice for the causal-curve calculus and Lebesgue fundamental theorem used below.

Let $E$ be a connected time-oriented Lorentzian spacetime and $C\subset E$ a smooth spacelike Cauchy hypersurface. Suppose a complete smooth Killing field $T$ has flow $\phi$ and the map $\Psi:\mathbb R\times C\to E$, $\Psi(t,p)=\phi_t(p)$, is a diffeomorphism. Suppose also $-g(T,n)>0$ along $C$, where $n$ is its future unit normal. Define $s(\Psi(t,p))=t$. Then $s$ is a smooth Cauchy temporal function: its gradient is past timelike and every level is a spacelike Cauchy hypersurface. In particular $s$ tends to $+\infty$ and $-\infty$ at the two ends of every inextendible future causal curve. This lemma assumes the displayed global product; it does not construct that product from orbit completeness alone.

## Statement references

[[physics:def-gr-smooth-lorentzian-objects]]

[[physics:def-gr-killing-field]]

[[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]]

[[math:def-local-and-global-flow]]

[[physics:def-gr-causal-curves-and-reachability]]

[[math:def-countable-choice]]

[[math:def-dependent-choice]]

## Facts & Assumptions

[F1] Lorentzian time orientation, the Killing field, spacelike Cauchy hypersurfaces and the global-flow laws have their named mathematical meanings. [[physics:def-gr-smooth-lorentzian-objects]] [[physics:def-gr-killing-field]] [[physics:def-gr-spacelike-hypersurfaces-and-cauchy-sets]] [[math:def-local-and-global-flow]]

[A1] Countable Choice and Dependent Choice are assumed to meet the hypotheses of [F3] and [F4]; no claim that these principles are necessary for the geometric conclusion is made. [[math:def-countable-choice]] [[math:def-dependent-choice]]

[F2] A future causal curve is continuous and locally absolutely continuous in charts, with nonzero future causal velocity almost everywhere. Future and past inextendibility mean absence of a limit in $E$ as the parameter tends to its respective end. [[physics:def-gr-causal-curves-and-reachability]]

[F3] Under [A1], smooth composition preserves local absolute continuity and obeys the almost-everywhere chain rule; every compact parameter interval admits a finite subdivision into absolutely continuous chart representatives. We use clauses (a) and (b) of the causal-curve calculus, with smooth maps $\phi_t$ and $s$ on all of $E$. [[physics:lem-gr-causal-curve-calculus]]

[F4] Under [A1], an absolutely continuous real function $h$ on $[a,b]$ has an integrable almost-everywhere derivative and satisfies $h(b)-h(a)=\int_a^b h\prime(r)\,dr$. [[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions]]

[F5] On any measure space a nonnegative measurable function has integral zero if and only if it vanishes almost everywhere. We apply this on a nondegenerate compact interval with Lebesgue measure. [[math:thm-nonnegative-integral-zero-iff-zero-almost-everywhere]]

## Proof

**Given:** The hypotheses in the Statement, including [A1].

**Goal:** Prove that $s$ is smooth with past timelike gradient and spacelike Cauchy levels, and establish both endpoint limits.

1.1 Smoothness of $s$ follows from the supplied inverse diffeomorphism. The flow laws give $\phi_t^{-1}=\phi_{-t}$ and $s\circ\phi_t=s+t$. The flow definition of the Lie derivative and the group law give $\frac{d}{dt}\phi_t^*g=\phi_t^*(\mathcal L_Tg)=0$, so each $\phi_t$ is an isometry. It preserves time orientation: the image of a future timelike vector varies continuously with $t$, stays timelike, and starts in the future cone, so it cannot change to the past cone. The isometry therefore preserves future causal cones as well. Thus the levels $s^{-1}(t)=\phi_t(C)$ are spacelike. [F1, given]

2.1 Fix $t\in\mathbb R$ and an inextendible future causal curve $\gamma:I\to E$. By [F3], $\eta=\phi_{-t}\circ\gamma$ is locally absolutely continuous with $\eta\prime=d\phi_{-t}(\gamma\prime)$ almost everywhere. The isometry has invertible differential and preserves future causal cones, so this velocity is nonzero future causal almost everywhere. If $\eta$ converged to $q\in E$ at either parameter end, continuity of $\phi_t$ would force $\gamma=\phi_t\circ\eta$ to converge to $\phi_t(q)$ there, contrary to [F2]. Thus $\eta$ is inextendible. Since $C$ is Cauchy, $\eta$ meets $C$ at exactly one parameter value; equivalently $\gamma$ meets $\phi_t(C)$ exactly once. For a past causal curve the same argument preserves its past causal velocity and gives exactly one crossing as well. Hence every level of $s$ is Cauchy. [A1, F1, F2, F3, step 1.1]

2.2 The covector $ds$ annihilates the spacelike tangent hyperplane of its level and satisfies $ds(T)=1$. At $\phi_t(p)$ let $n_t=d\phi_t(n_p)$ and $N=-g(T,n_t)$. Invariance of $T$ under its own isometric flow gives $N=-g(T,n_p)>0$. Write $T=Nn_t+X$ with $X$ tangent to the level. Then $1=ds(T)=Nds(n_t)$, so $ds(n_t)=1/N$ and the metric dual is $\nabla s=-n_t/N$. It is therefore past timelike. In a Lorentz orthonormal frame with future unit vector $n_t$, any nonzero future causal $v$ has positive time component, whence $ds(v)=-g(n_t,v)/N>0$. [F1, given, step 1.1]

3.1 For any future causal $\gamma:I\to E$, [F3] makes $h=s\circ\gamma$ locally absolutely continuous with $h\prime(r)=ds(\gamma\prime(r))>0$ almost everywhere by [F2] and step 2.2. On each compact $[a,b]\subseteq I$, finite subdivision from [F3] gives absolute continuity of $h$ on the whole interval: for a test family of disjoint intervals, split at the finitely many subdivision points and use each piece's absolute-continuity bound with tolerance divided by the number of pieces. For $a<b$, [F4] gives $h(b)-h(a)=\int_a^b h\prime(r)\,dr$. Choose the nonnegative measurable representative of $h\prime$ obtained by setting it to zero on its null exceptional set. It is positive almost everywhere on the positive-measure interval $[a,b]$, so [F5] makes its integral strictly positive. Consequently $h(b)>h(a)$ and $s$ increases strictly along every future causal curve. [A1, F2, F3, F4, F5, step 2.2]

4.1 For an inextendible future causal curve, step 2.1 gives exactly one meeting with each level $s^{-1}(R)$, for every $R\in\mathbb R$, so $s\circ\gamma$ has range $\mathbb R$. By strict increase from step 3.1, after the parameter where $s=R$ all values exceed $R$, and before it all values are below $R$. Since $R$ is arbitrary, the future and past endpoint limits are $+\infty$ and $-\infty$, respectively. Together with smoothness, the past timelike gradient and the spacelike Cauchy levels already proved, these are all the asserted conclusions. [F1, F2, step 1.1, step 2.1, step 2.2, step 3.1] ∎
