---
id: pthm-harrison-denominator-positive
title: Positivity of the Harrison denominator and horizon bound
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - post-stationary-vacuum-model
  - def-regular-stationary-vacuum-spacetime
  - def-stationary-lorentzian-data
  - def-harrison-normalization
  - def-harrison-one-form
  - def-harrison-electromagnetic-form
  - pthm-original-lapse-and-product
  - math:cor-transverse-intersection-theorem
dependency_roles:
  post-stationary-vacuum-model: physical-assumption
  def-regular-stationary-vacuum-spacetime: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-harrison-normalization: mathematical-premise
  def-harrison-one-form: mathematical-premise
  def-harrison-electromagnetic-form: mathematical-premise
  pthm-original-lapse-and-product: physical-result
  math:cor-transverse-intersection-theorem: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 8, Section 2.1, after equation (2.1) and final paragraph
      statement: The real part of the Harrison denominator is positive on the
        exterior; tangency of the stationary field to the bifurcation sphere
        gives the stated horizon bound and regularity of the formulas near the
        sphere.
      hypotheses: The article's mass-one regular stationary vacuum setting with
        maximal original section, q in [0,1], and the required smooth Harrison
        data near the sphere.
      reading_limits: Read the frozen article text at the cited passage. This
        reference attributes the article claim and is not used as its proof.
physical_scope: Conditional geometric consequences in the smooth stationary,
  asymptotically flat vacuum black-hole model; no measurement is asserted.
dependency_level: 7
---

## Statement

Assume the regular stationary vacuum model with the original outer section maximal and mass normalized to one. Let $\mathcal E$ be its open exterior, $S$ its bifurcation sphere, and $T$ its stationary Killing field. Suppose a smooth normalized Ernst potential $\sigma=f+i\psi$, with $f=-g(T,T)$ and real $\psi$, is supplied on an open set containing $\mathcal E\cup S$. For $q\in[0,1]$ put $B_q=q(1+\sigma)+(1-\sigma)$ and $D_q=|B_q|^2$. Then $\operatorname{Re}B_q=2q+(1-q)(1-f)>0$ on $\mathcal E$. On $S$, $f\le0$ and $D_q\ge(1+q)^2$. There is an open neighborhood of $S$, independent of $q\in[0,1]$, on which $B_q$ and $D_q$ are nonzero. Consequently the regular Harrison metric and electromagnetic formulas contain no division by $f$ and, for each fixed $q$, extend smoothly to such a neighborhood whenever the required Harrison one-form $W_q$ and the other displayed input fields are smooth there and satisfy their defining conditions.

## Statement references

[[post-stationary-vacuum-model]]

[[def-regular-stationary-vacuum-spacetime]]

[[def-stationary-lorentzian-data]]

[[def-harrison-normalization]]

[[def-harrison-one-form]]

[[def-harrison-electromagnetic-form]]

[[pthm-original-lapse-and-product]]

## Facts & Assumptions

[F1] In the regular stationary vacuum model, the two smooth horizon branches meet transversely in the spacelike sphere $S$, and $T$ is tangent to both branches. [[post-stationary-vacuum-model]] [[def-regular-stationary-vacuum-spacetime]]

[F2] Under the stated maximal-section hypotheses the original lapse and product result gives $f=-g(T,T)<1$ throughout $\mathcal E$. [[pthm-original-lapse-and-product]] [[def-stationary-lorentzian-data]]

[F3] For the normalization interface take $\Sigma_1=C=\Sigma_0\cap\mathcal E=\{r>1\}$. The original lapse and product result identifies this open outer hypersurface; it is smooth and spacelike as an open subset of $\Sigma_0$, maximal everywhere on $C$ by the outer-section assumption, and carries the same mass-one asymptotic end. No maximality of $\Sigma_0$ across $S$ is needed. With the supplied normalized Ernst potential, the normalization then defines $B_q=1+q-(1-q)\sigma$ and $D_q=B_q\overline{B_q}$. [[def-regular-stationary-vacuum-spacetime]] [[pthm-original-lapse-and-product]] [[def-harrison-normalization]]

[F4] The regular metric formula is $g_q=\tfrac14(D_qg+T^\flat\otimes W_q+W_q\otimes T^\flat-fD_q^{-1}W_q\otimes W_q)$. The electromagnetic formula is $\mathcal H_q=-\sqrt{1-q^2}(\overline{B_q}/B_q)(\mathcal F+W_q\wedge d\sigma/(2D_q))$, with $F_q=\operatorname{Re}\mathcal H_q$. Their definitions require the stated smooth input data and the relevant nonzero denominators. [[def-harrison-one-form]] [[def-harrison-electromagnetic-form]]

[F5] For transverse embedded submanifolds, the tangent space of their intersection equals the intersection of their tangent spaces. Applied to the two embedded horizon branches, this gives $T_pS=T_p\mathcal H^+\cap T_p\mathcal H^-$ for every $p\in S$. [[math:cor-transverse-intersection-theorem]]

## Proof

**Given:** The model and supplied smooth data in the Statement, with $0\le q\le1$.

**Goal:** Prove the exterior and horizon bounds and the conditional regularity near $S$.

1.1 Taking the real part in the definition of $B_q$ gives $\operatorname{Re}B_q=2q+(1-q)(1-f)$. On $\mathcal E$, $1-f>0$; if $q<1$ the second term is positive, while for $q=1$ the expression equals $2$. Thus $B_q\ne0$ and $D_q>0$ there. [given, F2, F3, algebra]

1.2 At each $p\in S$, the transverse-intersection theorem gives $T_pS=T_p\mathcal H^+\cap T_p\mathcal H^-$. Tangency of $T$ to both branches therefore gives $T_p\in T_pS$. Since $S$ is spacelike, $g(T,T)\ge0$, so $f\le0$. Hence $\operatorname{Re}B_q=1+q-(1-q)f\ge1+q$ and $D_q=(\operatorname{Re}B_q)^2+(\operatorname{Im}B_q)^2\ge(1+q)^2$. [given, F1, F3, F5, algebra]

2.1 In the supplied open domain $U$ of $\sigma$, smoothness of $f$ and $f\le0$ on $S$ give the open neighborhood $O=\{x\in U:f(x)<1/2\}$ of $S$. For every $q\in[0,1]$ there, $\operatorname{Re}B_q\ge2q+(1-q)/2\ge1/2>0$, so $B_q$ and $D_q$ are nonzero on the same $O$. The displayed metric and electromagnetic formulas divide only by $D_q$ or $B_q$, never by $f$. For each fixed $q$, their coefficients and tensor operations are therefore smooth on $O$ when the stated input fields and $W_q$ are smooth and satisfy the defining conditions there. This gives the asserted extensions; it does not assert existence of $W_q$. [given, F3, F4, step 1.2, algebra] ∎

## Source notes

The article passage attributes the denominator and horizon claims. The proof above uses the completed lapse result, the stated geometric definitions and the transverse-intersection theorem, not the article claim as a premise.
