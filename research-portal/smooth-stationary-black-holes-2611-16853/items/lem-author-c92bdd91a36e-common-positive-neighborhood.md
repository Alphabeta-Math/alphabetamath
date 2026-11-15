---
id: lem-author-c92bdd91a36e-common-positive-neighborhood
title: A common positive Harrison domain across the compact sphere
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-complex-self-dual-two-form-data
  - math:def-axiom-of-choice
  - lem-author-7a3c9628f105-denominator-positivity
  - lem-author-7a3c9628f105-primitive-parameter-lift
  - math:def-embedded-submanifold-and-slice-chart
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-c-r-and-smooth-maps-between-smooth-manifolds
  - math:def-continuous-map-top
  - math:def-exterior-derivative-by-the-invariant-vector-field-formula
  - math:def-lie-derivative-of-a-differential-form
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-complex-self-dual-two-form-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  lem-author-7a3c9628f105-denominator-positivity: mathematical-premise
  lem-author-7a3c9628f105-primitive-parameter-lift: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  math:def-complex-conjugate-real-imaginary-part-and-modulus: mathematical-premise
  math:def-c-r-and-smooth-maps-between-smooth-manifolds: mathematical-premise
  math:def-continuous-map-top: mathematical-premise
  math:def-exterior-derivative-by-the-invariant-vector-field-formula: mathematical-premise
  math:def-lie-derivative-of-a-differential-form: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references: []
dependency_level: 3
---

## Statement

Let $S$ be a compact embedded smooth two-dimensional submanifold of stationary Lorentzian data, with positive-definite induced metric, with $T$ tangent to $S$, and with a supplied zero $p\in S$ of $T$. On an open neighborhood $U$ of $S$, suppose $\sigma=f+i\psi$ with $\psi:U\to\mathbb R$, and suppose a smooth stationary one-form $W_0$ is given (stationary means $\mathcal L_TW_0=0$), with $f=-g(T,T)$, $F=\tfrac12\mathrm dT^\flat$, $\mathrm dW_0=4((f-1)F+\psi\star_gF)$ and $W_0(T)=D_0(p)-D_0$, where $D_0=|1-\sigma|^2$. Set $D_q=|1+q-(1-q)\sigma|^2$ and $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. There is a common open neighborhood $O\subseteq U$ of $S$ with $D_q>0$ and $D_q+W_q(T)=d_q>0$ for every $q\in[0,1]$, where $d_q=D_q(p)$. On $O$, the polynomial curl and contraction identities are $\mathrm dW_q=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$ and $W_q(T)=d_q-D_q$.

## Facts & Assumptions

[F1] The metric, forms and ZFC convention are [[def-stationary-lorentzian-data]], [[def-complex-self-dual-two-form-data]] and [[math:def-axiom-of-choice]]. Stationarity of the one-form $W_0$ means $\mathcal L_TW_0=0$, with the Lie derivative of a differential form defined in [[math:def-lie-derivative-of-a-differential-form]].

[F2] The denominator calculation is recorded in [[lem-author-7a3c9628f105-denominator-positivity]]. Its needed algebra and neighborhood construction are repeated below; the supplier's additional smoothness and stationarity assumptions on $\sigma$ are not assumed here or used to invoke its full statement.

[F3] The polynomial one-form calculation is recorded in [[lem-author-7a3c9628f105-primitive-parameter-lift]]. Its contraction and curl calculations are repeated below directly from the assumed identities for $W_0$, without differentiating $\psi$ or invoking the supplier under unverified scalar hypotheses.

[F4] The surface is an embedded two-dimensional smooth submanifold with its inherited topology, as in [[math:def-embedded-submanifold-and-slice-chart]]. Positive-definiteness of its induced metric is the explicit spacelike assumption in the Statement.

[F5] For real $a,b$, $|a+ib|^2=a^2+b^2$, with the real and imaginary coordinates and modulus of [[math:def-complex-conjugate-real-imaginary-part-and-modulus]].

[F6] Smooth scalar maps include continuity in [[math:def-c-r-and-smooth-maps-between-smooth-manifolds]]. The open-neighborhood criterion for continuity is [[math:def-continuous-map-top]].

[F7] The exterior derivative is defined by [[math:def-exterior-derivative-by-the-invariant-vector-field-formula]]. Its defining sums are linear in the form, so $\mathrm d(a\alpha+b\beta)=a\,\mathrm d\alpha+b\,\mathrm d\beta$ for spacetime-constant real $a,b$ and smooth forms $\alpha,\beta$.

## Proof

**Given:** The hypotheses in the Statement and the mathematical conventions in [F1]–[F7].

**Goal:** Prove the common positivity and the polynomial identities without additional hypotheses on the scalar $\psi$.

1.1 By the induced-metric hypothesis and tangency, $g(T,T)\ge0$ on $S$, so $f\le0$ there. In coordinates $f=-g_{ab}T^aT^b$ is a finite sum of products of smooth functions, hence is smooth and continuous. Define $O=\{x\in U:f(x)<\tfrac12\}$. The open-neighborhood criterion in [F6], applied to $(-\infty,\tfrac12)$, makes $O$ open in $U$ and hence in the ambient manifold. It contains $S$ and is independent of $q$. This gives the neighborhood construction in [F2] using only the regularity of $f$. [given, F1, F2, F4, F6]

2.1 For $x\in O$ and $q\in[0,1]$, put $a_q=1+q-(1-q)f=2q+(1-q)(1-f)$. Since $1-f>\tfrac12$, $a_q\ge\tfrac12$ (also at $q=1$). By [F5], $D_q=a_q^2+(1-q)^2\psi^2\ge\tfrac14>0$. At $p$, $T(p)=0$ gives $f(p)=0$, so $d_q=(1+q)^2+(1-q)^2\psi(p)^2\ge1$. Neither estimate requires continuity or stationarity of $\psi$. [given, F1, F2, F5, algebra, step 1.1]

3.1 Repeating the pointwise calculation of [F2], subtract $(1-q)^2D_0$ from $D_q$ using [F5]. The $\psi^2$ terms cancel, leaving $(1+q-(1-q)f)^2-(1-q)^2(1-f)^2=4q(1-(1-q)f)$. Thus $D_q=(1-q)^2D_0+4q(1-(1-q)f)$, and $d_q=(1-q)^2D_0(p)+4q$. For the contraction calculation of [F3], $T^\flat(T)=-f$ gives $W_q(T)=(1-q)^2(D_0(p)-D_0)+4q(1-q)f=d_q-D_q$. Consequently $D_q+W_q(T)=d_q\ge1$ on the same $O$. These are pointwise algebraic identities with no scalar regularity premise. [given, F1, F2, F3, F5, algebra, step 2.1]

4.1 For the curl calculation of [F3], hold $q$ fixed and use [F7] and $\mathrm dT^\flat=2F$ to obtain $\mathrm dW_q=4(1-q)^2((f-1)F+\psi\star_gF)-8q(1-q)F=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$. No derivative of $\psi$ is taken. The defining expression for $W_q$ is polynomial in $q$ with smooth spacetime coefficients. Also $D_0=D_0(p)-W_0(T)$ is smooth by the assumed contraction identity, and the formula in step 3.1 makes $D_q$ smooth jointly in spacetime and $q$. The curl's displayed right-hand side equals the smooth form $\mathrm dW_q$ by the assumed curl identity and the calculation just given. Hence these are smooth local identities on all of $O$, including either side of any horizon lying in $O$; no restriction to an exterior is used. [given, F1, F3, F7, algebra, step 3.1] ∎
